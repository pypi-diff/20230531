# Comparing `tmp/sd_meh-0.3.0.tar.gz` & `tmp/sd_meh-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.3.0.tar", max compression
+gzip compressed data, was "sd_meh-0.4.0.tar", max compression
```

## Comparing `sd_meh-0.3.0.tar` & `sd_meh-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-31 08:17:05.600958 sd_meh-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1510 2023-05-31 08:17:05.600958 sd_meh-0.3.0/README.md
--rw-r--r--   0        0        0      390 2023-05-31 08:17:05.600958 sd_meh-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-31 08:17:05.600958 sd_meh-0.3.0/sd_meh/__init__.py
--rw-r--r--   0        0        0     5375 2023-05-31 08:17:05.604958 sd_meh-0.3.0/sd_meh/merge.py
--rw-r--r--   0        0        0     2416 2023-05-31 08:17:05.604958 sd_meh-0.3.0/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1465 2023-05-31 08:17:05.604958 sd_meh-0.3.0/sd_meh/model.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 sd_meh-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-31 15:54:41.675357 sd_meh-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1585 2023-05-31 15:54:41.675357 sd_meh-0.4.0/README.md
+-rw-r--r--   0        0        0      390 2023-05-31 15:54:41.675357 sd_meh-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/__init__.py
+-rw-r--r--   0        0        0     7957 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/merge.py
+-rw-r--r--   0        0        0     2416 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1465 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/model.py
+-rw-r--r--   0        0        0    83125 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/rebasin.py
+-rw-r--r--   0        0        0     2109 1970-01-01 00:00:00.000000 sd_meh-0.4.0/PKG-INFO
```

### Comparing `sd_meh-0.3.0/LICENSE.txt` & `sd_meh-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.3.0/README.md` & `sd_meh-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,17 +35,20 @@
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
   -bb, --base_beta FLOAT
+  -rb, --re_basin
+  -rbi, --re_basin_iterations INTEGER
   --help                          Show this message and exit.
 ```
 
 ## Features
 
+- weights matching
 - weights clipping
 - registered pypi package
 - block merge
 - merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`
 - `fp16` and `fp32`
```

### Comparing `sd_meh-0.3.0/sd_meh/merge.py` & `sd_meh-0.4.0/sd_meh/merge.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 
 import safetensors.torch
 import torch
 from tqdm import tqdm
 
 from sd_meh import merge_methods
 from sd_meh.model import SDModel
+from sd_meh.rebasin import (
+    SPECIAL_KEYS,
+    apply_permutation,
+    sdunet_permutation_spec,
+    step_weights_and_bases,
+    weight_matching,
+)
 
 MAX_TOKENS = 77
 NUM_INPUT_BLOCKS = 12
 NUM_MID_BLOCK = 1
 NUM_OUTPUT_BLOCKS = 12
 NUM_TOTAL_BLOCKS = NUM_INPUT_BLOCKS + NUM_MID_BLOCK + NUM_OUTPUT_BLOCKS
 
@@ -69,17 +76,49 @@
 def merge_models(
     models: Dict[str, os.PathLike | str],
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
     weights_clip: bool = False,
+    re_basin: bool = False,
+    iterations: int = 1,
 ) -> Dict:
     thetas = {k: load_sd_model(m) for k, m in models.items()}
 
+    if re_basin:
+        return rebasin_merge(
+            thetas,
+            weights,
+            bases,
+            merge_mode,
+            precision=precision,
+            weights_clip=weights_clip,
+            iterations=iterations,
+            device="cpu",
+        )
+    else:
+        return simple_merge(
+            thetas,
+            weights,
+            bases,
+            merge_mode,
+            precision=precision,
+            weights_clip=weights_clip,
+        )
+
+
+def simple_merge(
+    thetas: Dict[str, Dict],
+    weights: Dict,
+    bases: Dict,
+    merge_mode: str,
+    precision: int = 16,
+    weights_clip: bool = False,
+) -> Dict:
     for key in tqdm(thetas["model_a"].keys(), desc="stage 1"):
         if result := merge_key(
             key,
             thetas,
             weights,
             bases,
             merge_mode,
@@ -95,14 +134,73 @@
             thetas["model_a"].update({key: thetas["model_b"][key]})
             if precision == 16:
                 thetas["model_a"][key] = thetas["model_a"][key].half()
 
     return fix_model(thetas["model_a"])
 
 
+def rebasin_merge(
+    thetas: Dict[str, os.PathLike | str],
+    weights: Dict,
+    bases: Dict,
+    merge_mode: str,
+    precision: int = 16,
+    weights_clip: bool = False,
+    iterations: int = 1,
+    device="cpu",
+):
+    # WARNING: not sure how this does when 3 models are involved...
+
+    model_a = thetas["model_a"].copy()
+    perm_spec = sdunet_permutation_spec()
+
+    print("permuting")
+    for it in range(iterations):
+        print(it)
+        new_weights, new_bases = step_weights_and_bases(weights, bases, it, iterations)
+
+        # normal block merge we already know and love
+        thetas["model_a"] = simple_merge(
+            thetas, new_weights, new_bases, merge_mode, precision, weights_clip
+        )
+
+        # find permutations
+        perm_1, y = weight_matching(
+            perm_spec,
+            model_a,
+            thetas["model_a"],
+            max_iter=it,
+            init_perm=None,
+            usefp16=precision == 16,
+            device=device,
+        )
+        thetas["model_a"] = apply_permutation(perm_spec, perm_1, thetas["model_a"])
+        perm_2, z = weight_matching(
+            perm_spec,
+            thetas["model_b"],
+            thetas["model_a"],
+            max_iter=it,
+            init_perm=None,
+            usefp16=precision == 16,
+            device=device,
+        )
+        theta_3 = apply_permutation(perm_spec, perm_2, thetas["model_a"])
+
+        # is this correct for block merge?
+        new_alpha = torch.nn.functional.normalize(
+            torch.sigmoid(torch.Tensor([y, z])), p=1, dim=0
+        ).tolist()[0]
+        for key in SPECIAL_KEYS:
+            thetas["model_a"][key] = (1 - new_alpha) * (
+                thetas["model_a"][key]
+            ) + new_alpha * theta_3[key]
+
+    return thetas["model_a"]
+
+
 def merge_key(
     key: str,
     thetas: Dict,
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
@@ -140,16 +238,16 @@
                 raise ValueError(f"illegal block index {key}")
 
             if weight_index >= 0:
                 current_bases = {k: w[weight_index] for k, w in weights.items()}
 
         try:
             merge_method = getattr(merge_methods, merge_mode)
-        except AttributeError:
-            raise ValueError(f"{merge_mode} not implemented, aborting merge!")
+        except AttributeError as e:
+            raise ValueError(f"{merge_mode} not implemented, aborting merge!") from e
 
         merge_args = get_merge_method_args(current_bases, thetas, key)
         merged_key = merge_method(**merge_args)
 
         if weights_clip:
             t0 = thetas["model_a"][key]
             t1 = thetas["model_b"][key]
@@ -166,19 +264,15 @@
     merge_method_args = {
         "a": thetas["model_a"][key],
         "b": thetas["model_b"][key],
         **current_bases,
     }
 
     if "model_c" in thetas:
-        merge_method_args.update(
-            {
-                "c": thetas["model_c"][key],
-            }
-        )
+        merge_method_args["c"] = thetas["model_c"][key]
 
     return merge_method_args
 
 
 def save_model(model, output_file, file_format) -> None:
     if file_format == "safetensors":
         safetensors.torch.save_file(
```

### Comparing `sd_meh-0.3.0/sd_meh/merge_methods.py` & `sd_meh-0.4.0/sd_meh/merge_methods.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.3.0/sd_meh/model.py` & `sd_meh-0.4.0/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.3.0/PKG-INFO` & `sd_meh-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.3.0
+Version: 0.4.0
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -51,18 +51,21 @@
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
   -bb, --base_beta FLOAT
+  -rb, --re_basin
+  -rbi, --re_basin_iterations INTEGER
   --help                          Show this message and exit.
 ```
 
 ## Features
 
+- weights matching
 - weights clipping
 - registered pypi package
 - block merge
 - merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`
 - `fp16` and `fp32`
```

