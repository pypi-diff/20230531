# Comparing `tmp/merlin-dataloader-23.4.0.tar.gz` & `tmp/merlin-dataloader-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-dataloader-23.4.0.tar", last modified: Wed Apr 26 19:02:30 2023, max compression
+gzip compressed data, was "merlin-dataloader-23.5.0.tar", last modified: Wed May 31 14:39:22 2023, max compression
```

## Comparing `merlin-dataloader-23.4.0.tar` & `merlin-dataloader-23.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/merlin/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/merlin/dataloader/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    29255 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/loader_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/dataloader/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/ops/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/ops/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/dataloader/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/dataloader/utils/tf/
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/utils/tf/tf_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/dataloader/utils/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/utils/torch/torch_trainer_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/loader/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/loader/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/loader/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/tensorflow.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/torch.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81931 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.920793 merlin-dataloader-23.5.0/merlin/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:22.920793 merlin-dataloader-23.5.0/merlin/dataloader/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29285 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/loader_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/dataloader/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/ops/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/ops/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/dataloader/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/dataloader/utils/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/utils/tf/tf_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/dataloader/utils/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/utils/torch/torch_trainer_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/loader/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/loader/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/loader/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/tensorflow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/torch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-31 14:39:22.920793 merlin-dataloader-23.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81931 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/versioneer.py
```

### Comparing `merlin-dataloader-23.4.0/LICENSE` & `merlin-dataloader-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/PKG-INFO` & `merlin-dataloader-23.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-dataloader
-Version: 23.4.0
+Version: 23.5.0
 Summary: Merlin Dataloader
 Home-page: https://github.com/NVIDIA-Merlin/dataloader
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-dataloader-23.4.0/README.md` & `merlin-dataloader-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/__init__.py` & `merlin-dataloader-23.5.0/merlin/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/jax.py` & `merlin-dataloader-23.5.0/merlin/dataloader/jax.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/loader_base.py` & `merlin-dataloader-23.5.0/merlin/dataloader/loader_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -662,15 +662,15 @@
             if col_spec.dtype not in self.dtype_reverse_map:
                 self.dtype_reverse_map[col_spec.dtype] = [col_name]
             else:
                 self.dtype_reverse_map[col_spec.dtype].append(col_name)
 
         if self._transform_graph is not None:
             self._transforms = self._transform_graph.construct_schema(
-                self._input_schema
+                self._input_schema.excluding_by_tag(Tags.TARGET)
             ).output_node
             self._output_schema = self._transforms.output_schema
         else:
             self._output_schema = self._input_schema
 
         if len(list(self.dtype_reverse_map.keys())) == 0:
             raise ValueError(
```

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/ops/__init__.py` & `merlin-dataloader-23.5.0/merlin/dataloader/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/ops/padding.py` & `merlin-dataloader-23.5.0/merlin/dataloader/ops/padding.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,31 +7,28 @@
 from merlin.dag import BaseOperator
 from merlin.dag.selector import ColumnSelector
 from merlin.schema import Schema
 from merlin.table import Device, TensorTable
 
 
 class Padding(BaseOperator):
-    """Create an operator that will apply a embedding table to supplied indices.
-    This operator allows the user to supply an id lookup table if the indices supplied
-    via the id_lookup_table.
+    """Create an operator that will apply right padding to a given sequence.
+    This operator pads the sequence with a specified padding value up to a specified padding size.
+    If the sequence is longer than the padding size,
+    it is truncated to the first `padding size` elements.
 
     Parameters
     ----------
-    embeddings : np.ndarray
-        numpy ndarray representing embedding values
-    lookup_key : str, optional
-        the name of the column that will be used as indices, by default "id"
-    embedding_name : str, optional
-        name of new column of embeddings, added to output, by default "embeddings"
-    id_lookup_table : np.array, optional
-        numpy array of values that represent embedding indices, by default None
+    padding_size : int
+        The target size for the padded sequence
+    padding_value : Union[int, float]
+        The value to be used for padding the sequence, by default 0
     """
 
-    def __init__(self, padding_size: int, padding_value: Union[int, float]):
+    def __init__(self, padding_size: int, padding_value: Union[int, float] = 0):
         self.padding_size = padding_size
         self.padding_value = padding_value
 
     def transform(
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
         to_pad = transformable[col_selector.names]
@@ -72,17 +69,18 @@
         return Schema(col_schemas)
 
 
 def pad_put_zeros(column, padding_size, padding_val):
     # account for zero prepend
     array_lib = cupy if column.device == Device.GPU else np
     num_rows = len(column.offsets) - 1
-    zeros = array_lib.zeros((num_rows, padding_size)).flatten()
+    zeros = array_lib.zeros((num_rows, padding_size)).flatten() + padding_val
     row_lengths = column.offsets[1:] - column.offsets[:-1]
     row_ranges = []
     starts = array_lib.arange(num_rows) * padding_size
     ends = starts + row_lengths
     for idx, offset in enumerate(column.offsets[:-1]):
         row_ranges.extend(array_lib.arange(int(starts[idx]), int(ends[idx])))
     array_lib.put(zeros, row_ranges, column.values)
     zeros = array_lib.reshape(zeros, (num_rows, padding_size))
+    zeros = zeros.astype(column.dtype.element_type.value)
     return zeros
```

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/tensorflow.py` & `merlin-dataloader-23.5.0/merlin/dataloader/tensorflow.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/tf_utils.py` & `merlin-dataloader-23.5.0/merlin/dataloader/tf_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/torch.py` & `merlin-dataloader-23.5.0/merlin/dataloader/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/utils/tf/tf_trainer.py` & `merlin-dataloader-23.5.0/merlin/dataloader/utils/tf/tf_trainer.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/dataloader/utils/torch/torch_trainer_dist.py` & `merlin-dataloader-23.5.0/merlin/dataloader/utils/torch/torch_trainer_dist.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/loader/__init__.py` & `merlin-dataloader-23.5.0/merlin/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/loader/jax.py` & `merlin-dataloader-23.5.0/merlin/loader/jax.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/loader/tensorflow.py` & `merlin-dataloader-23.5.0/merlin/loader/tensorflow.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin/loader/torch.py` & `merlin-dataloader-23.5.0/merlin/loader/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin_dataloader.egg-info/PKG-INFO` & `merlin-dataloader-23.5.0/merlin_dataloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-dataloader
-Version: 23.4.0
+Version: 23.5.0
 Summary: Merlin Dataloader
 Home-page: https://github.com/NVIDIA-Merlin/dataloader
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-dataloader-23.4.0/merlin_dataloader.egg-info/SOURCES.txt` & `merlin-dataloader-23.5.0/merlin_dataloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/merlin_dataloader.egg-info/requires.txt` & `merlin-dataloader-23.5.0/merlin_dataloader.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-merlin-core>=23.4.0
+merlin-core>=23.04.00
 
 [all]
-merlin-core>=23.4.0
+merlin-core>=23.04.00
 tensorflow>=2.3.0
 torch>=1.0
 torch>=1.0
 jax[cpu]
 scipy
 scikit-learn>=0.20
 npy_append_array
@@ -26,15 +26,15 @@
 sphinx_rtd_theme
 natsort<8.2
 myst-nb<0.14
 linkify-it-py<1.1
 markdown==3.3.7
 
 [base]
-merlin-core>=23.4.0
+merlin-core>=23.04.00
 
 [dev]
 scipy
 scikit-learn>=0.20
 npy_append_array
 ipython_genutils
 nbsphinx>=0.6
```

### Comparing `merlin-dataloader-23.4.0/pyproject.toml` & `merlin-dataloader-23.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/requirements/dev.txt` & `merlin-dataloader-23.5.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/setup.cfg` & `merlin-dataloader-23.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/setup.py` & `merlin-dataloader-23.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.4.0/versioneer.py` & `merlin-dataloader-23.5.0/versioneer.py`

 * *Files identical despite different names*

