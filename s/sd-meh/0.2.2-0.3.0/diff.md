# Comparing `tmp/sd_meh-0.2.2.tar.gz` & `tmp/sd_meh-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.2.2.tar", max compression
+gzip compressed data, was "sd_meh-0.3.0.tar", max compression
```

## Comparing `sd_meh-0.2.2.tar` & `sd_meh-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-30 11:34:33.627424 sd_meh-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     1400 2023-05-30 11:34:33.627424 sd_meh-0.2.2/README.md
--rw-r--r--   0        0        0      390 2023-05-30 11:34:33.627424 sd_meh-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-30 11:34:33.627424 sd_meh-0.2.2/sd_meh/__init__.py
--rw-r--r--   0        0        0     5399 2023-05-30 11:34:33.627424 sd_meh-0.2.2/sd_meh/merge.py
--rw-r--r--   0        0        0     1588 2023-05-30 11:34:33.627424 sd_meh-0.2.2/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1465 2023-05-30 11:34:33.627424 sd_meh-0.2.2/sd_meh/model.py
--rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 sd_meh-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-31 08:17:05.600958 sd_meh-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1510 2023-05-31 08:17:05.600958 sd_meh-0.3.0/README.md
+-rw-r--r--   0        0        0      390 2023-05-31 08:17:05.600958 sd_meh-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-31 08:17:05.600958 sd_meh-0.3.0/sd_meh/__init__.py
+-rw-r--r--   0        0        0     5375 2023-05-31 08:17:05.604958 sd_meh-0.3.0/sd_meh/merge.py
+-rw-r--r--   0        0        0     2416 2023-05-31 08:17:05.604958 sd_meh-0.3.0/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1465 2023-05-31 08:17:05.604958 sd_meh-0.3.0/sd_meh/model.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 sd_meh-0.3.0/PKG-INFO
```

### Comparing `sd_meh-0.2.2/LICENSE.txt` & `sd_meh-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.2.2/README.md` & `sd_meh-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 Usage: merge_models.py [OPTIONS]
 
 Options:
   -a, --model_a TEXT
   -b, --model_b TEXT
   -c, --model_c TEXT
-  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum]
+  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|transmogrify_distribution]
   -wc, --weights_clip
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
@@ -43,9 +43,9 @@
 ```
 
 ## Features
 
 - weights clipping
 - registered pypi package
 - block merge
-- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`
+- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`
 - `fp16` and `fp32`
```

### Comparing `sd_meh-0.2.2/sd_meh/merge.py` & `sd_meh-0.3.0/sd_meh/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import re
-import sys
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
 import safetensors.torch
 import torch
 from tqdm import tqdm
 
@@ -142,16 +141,15 @@
 
             if weight_index >= 0:
                 current_bases = {k: w[weight_index] for k, w in weights.items()}
 
         try:
             merge_method = getattr(merge_methods, merge_mode)
         except AttributeError:
-            print(f"{merge_mode} not implemented, aborting merge!")
-            sys.exit(1)
+            raise ValueError(f"{merge_mode} not implemented, aborting merge!")
 
         merge_args = get_merge_method_args(current_bases, thetas, key)
         merged_key = merge_method(**merge_args)
 
         if weights_clip:
             t0 = thetas["model_a"][key]
             t1 = thetas["model_b"][key]
```

### Comparing `sd_meh-0.2.2/sd_meh/model.py` & `sd_meh-0.3.0/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.2.2/PKG-INFO` & `sd_meh-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.2.2
+Version: 0.3.0
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -42,15 +42,15 @@
 ```
 Usage: merge_models.py [OPTIONS]
 
 Options:
   -a, --model_a TEXT
   -b, --model_b TEXT
   -c, --model_c TEXT
-  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum]
+  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|transmogrify_distribution]
   -wc, --weights_clip
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
@@ -59,10 +59,10 @@
 ```
 
 ## Features
 
 - weights clipping
 - registered pypi package
 - block merge
-- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`
+- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`
 - `fp16` and `fp32`
```

