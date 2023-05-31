# Comparing `tmp/slim-trees-0.2.0.tar.gz` & `tmp/slim-trees-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slim-trees-0.2.0.tar", last modified: Fri Apr 14 10:59:07 2023, max compression
+gzip compressed data, was "slim-trees-0.2.1.tar", last modified: Wed May 31 09:39:37 2023, max compression
```

## Comparing `slim-trees-0.2.0.tar` & `slim-trees-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:59:07.655280 slim-trees-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-14 10:58:54.000000 slim-trees-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 10:58:54.000000 slim-trees-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-14 10:59:07.655280 slim-trees-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-14 10:58:54.000000 slim-trees-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-14 10:58:54.000000 slim-trees-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-14 10:59:07.655280 slim-trees-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:59:07.651280 slim-trees-0.2.0/slim_trees/
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/lgbm_booster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/sklearn_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:59:07.655280 slim-trees-0.2.0/slim_trees.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:39:36.996528 slim-trees-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-31 09:39:25.000000 slim-trees-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 09:39:25.000000 slim-trees-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-31 09:39:36.996528 slim-trees-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-31 09:39:25.000000 slim-trees-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 09:39:25.000000 slim-trees-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-31 09:39:36.996528 slim-trees-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:39:36.992528 slim-trees-0.2.1/slim_trees/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/lgbm_booster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/sklearn_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:39:36.996528 slim-trees-0.2.1/slim_trees.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/top_level.txt
```

### Comparing `slim-trees-0.2.0/LICENSE` & `slim-trees-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slim-trees-0.2.0/PKG-INFO` & `slim-trees-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,25 @@
-Metadata-Version: 2.1
-Name: slim-trees
-Version: 0.2.0
-Summary: A python package for efficient pickling of ML models.
-Home-page: https://github.com/pavelzw/slim-trees
-Author: Pavel Zwerschke
-Author-email: pavelzw@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: scikit-learn
-Provides-Extra: lightgbm
-License-File: LICENSE
-
 # Slim Trees
 
-[![CI](https://github.com/pavelzw/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/pavelzw/slim-trees/actions/workflows/ci.yml)
+[![CI](https://github.com/quantco/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/quantco/slim-trees/actions/workflows/ci.yml)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/slim-trees?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/slim-trees)
 [![pypi-version](https://img.shields.io/pypi/v/slim-trees.svg?logo=pypi&logoColor=white)](https://pypi.org/project/slim-trees)
 [![python-version](https://img.shields.io/pypi/pyversions/slim-trees?logoColor=white&logo=python)](https://pypi.org/project/slim-trees)
 
 `slim-trees` is a Python package for saving and loading compressed `sklearn` Tree-based and `lightgbm` models.
 The compression is performed by modifying how the model is pickled by Python's `pickle` module.
 
+We presented this library at PyData Berlin 2023, check out the [slides](.github/assets/slim-trees-presentation.pdf)!
+
 ## Installation
 
 ```bash
 pip install slim-trees
 # or
-mamba install slim-trees -c conda-forge
+micromamba install slim-trees -c conda-forge
 ```
 
 ## Usage
 
 Using `slim-trees` does not affect your training pipeline.
 Simply call `dump_sklearn_compressed` or `dump_lgbm_compressed` to save your model.
 
@@ -86,17 +70,31 @@
 model = load_compressed("model.pkl")
 
 # or alternatively with pickle.load
 with open("model.pkl", "rb") as f:
     model = pickle.load(f)
 ```
 
----
+### Save your model as `bytes`
+
+You can also save the model as `bytes` instead of in a file similar to the `pickle.dumps` method.
+
+```python
+from slim_trees import dumps_sklearn_compressed, loads_compressed
+
+X, y = ...
+model = RandomForestClassifier()
+model.fit(X, y)
+
+data = dumps_sklearn_compressed(model, compression="lzma")
+...
+model_loaded = loads_compressed(data, compression="lzma")
+```
 
-### drop-in replacement for pickle
+### Drop-in replacement for pickle
 
 You can also use the `slim_trees.sklearn_tree.dump` or `slim_trees.lgbm_booster.dump` functions as drop-in replacements for `pickle.dump`.
 
 ```python
 from slim_trees import sklearn_tree, lgbm_booster
 
 # for sklearn models
@@ -109,21 +107,20 @@
 ```
 
 ## Development Installation
 
 You can install the package in development mode using:
 
 ```bash
-git clone git@github.com:pavelzw/slim-trees.git
+git clone https://github.com/quantco/slim-trees.git
 cd slim-trees
 
 # create and activate a fresh environment named slim_trees
-# see environment.yml for details
-mamba env create
-conda activate slim_trees
+micromamba create -f environment.yml
+micromamba activate slim_trees
 
 pre-commit install
 pip install --no-build-isolation -e .
 ```
 
 ## Benchmark
```

### Comparing `slim-trees-0.2.0/README.md` & `slim-trees-0.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,43 @@
+Metadata-Version: 2.1
+Name: slim-trees
+Version: 0.2.1
+Summary: A python package for efficient pickling of ML models.
+Home-page: https://github.com/quantco/slim-trees
+Author: Pavel Zwerschke
+Author-email: pavel.zwerschke@quantco.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: scikit-learn
+Provides-Extra: lightgbm
+License-File: LICENSE
+
 # Slim Trees
 
-[![CI](https://github.com/pavelzw/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/pavelzw/slim-trees/actions/workflows/ci.yml)
+[![CI](https://github.com/quantco/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/quantco/slim-trees/actions/workflows/ci.yml)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/slim-trees?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/slim-trees)
 [![pypi-version](https://img.shields.io/pypi/v/slim-trees.svg?logo=pypi&logoColor=white)](https://pypi.org/project/slim-trees)
 [![python-version](https://img.shields.io/pypi/pyversions/slim-trees?logoColor=white&logo=python)](https://pypi.org/project/slim-trees)
 
 `slim-trees` is a Python package for saving and loading compressed `sklearn` Tree-based and `lightgbm` models.
 The compression is performed by modifying how the model is pickled by Python's `pickle` module.
 
+We presented this library at PyData Berlin 2023, check out the [slides](.github/assets/slim-trees-presentation.pdf)!
+
 ## Installation
 
 ```bash
 pip install slim-trees
 # or
-mamba install slim-trees -c conda-forge
+micromamba install slim-trees -c conda-forge
 ```
 
 ## Usage
 
 Using `slim-trees` does not affect your training pipeline.
 Simply call `dump_sklearn_compressed` or `dump_lgbm_compressed` to save your model.
 
@@ -68,17 +88,31 @@
 model = load_compressed("model.pkl")
 
 # or alternatively with pickle.load
 with open("model.pkl", "rb") as f:
     model = pickle.load(f)
 ```
 
----
+### Save your model as `bytes`
+
+You can also save the model as `bytes` instead of in a file similar to the `pickle.dumps` method.
+
+```python
+from slim_trees import dumps_sklearn_compressed, loads_compressed
+
+X, y = ...
+model = RandomForestClassifier()
+model.fit(X, y)
+
+data = dumps_sklearn_compressed(model, compression="lzma")
+...
+model_loaded = loads_compressed(data, compression="lzma")
+```
 
-### drop-in replacement for pickle
+### Drop-in replacement for pickle
 
 You can also use the `slim_trees.sklearn_tree.dump` or `slim_trees.lgbm_booster.dump` functions as drop-in replacements for `pickle.dump`.
 
 ```python
 from slim_trees import sklearn_tree, lgbm_booster
 
 # for sklearn models
@@ -91,21 +125,20 @@
 ```
 
 ## Development Installation
 
 You can install the package in development mode using:
 
 ```bash
-git clone git@github.com:pavelzw/slim-trees.git
+git clone https://github.com/quantco/slim-trees.git
 cd slim-trees
 
 # create and activate a fresh environment named slim_trees
-# see environment.yml for details
-mamba env create
-conda activate slim_trees
+micromamba create -f environment.yml
+micromamba activate slim_trees
 
 pre-commit install
 pip install --no-build-isolation -e .
 ```
 
 ## Benchmark
```

### Comparing `slim-trees-0.2.0/setup.cfg` & `slim-trees-0.2.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = slim-trees
 version = attr: slim_trees._version.__version__
 description = A python package for efficient pickling of ML models.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/pavelzw/slim-trees
+url = https://github.com/quantco/slim-trees
 author = Pavel Zwerschke
-author_email = pavelzw@gmail.com
+author_email = pavel.zwerschke@quantco.com
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
```

### Comparing `slim-trees-0.2.0/slim_trees/__init__.py` & `slim-trees-0.2.1/slim_trees/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,26 +11,35 @@
 """
 
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import pkg_resources
 
-from slim_trees.pickling import dump_compressed, load_compressed
+from slim_trees.pickling import (
+    dump_compressed,
+    dumps_compressed,
+    load_compressed,
+    loads_compressed,
+)
 
 try:
     __version__ = pkg_resources.get_distribution(__name__).version
 except Exception:
     __version__ = "unknown"
 
 __all__ = [
     "dump_compressed",
+    "dumps_compressed",
     "load_compressed",
+    "loads_compressed",
     "dump_sklearn_compressed",
+    "dumps_sklearn_compressed",
     "dump_lgbm_compressed",
+    "dumps_lgbm_compressed",
 ]
 
 
 def dump_sklearn_compressed(
     model: Any, path: Union[str, Path], compression: Optional[Union[str, dict]] = None
 ):
     """
@@ -45,14 +54,32 @@
                         Options: ["no", "lzma", "gzip", "bz2"]
     """
     from slim_trees.sklearn_tree import dump
 
     dump_compressed(model, path, compression, dump)
 
 
+def dumps_sklearn_compressed(
+    model: Any, compression: Optional[Union[str, dict]] = None
+) -> bytes:
+    """
+    Pickles a model and returns the saved object as bytes.
+
+    Saves the parameters of the model as int16 and float32 instead of int64 and float64.
+    :param model: the model to save
+    :param compression: the compression method used. Either a string or a dict with key 'method' set
+                        to the compression method and other key-value pairs are forwarded to `open`
+                        of the compression library.
+                        Options: ["no", "lzma", "gzip", "bz2"]
+    """
+    from slim_trees.sklearn_tree import dumps
+
+    return dumps_compressed(model, compression, dumps)
+
+
 def dump_lgbm_compressed(
     model: Any, path: Union[str, Path], compression: Optional[Union[str, dict]] = None
 ):
     """
     Pickles a model and saves a compressed version to the disk.
 
     Saves the parameters of the model as int16 and float32 instead of int64 and float64.
@@ -62,7 +89,25 @@
                         to the compression method and other key-value pairs are forwarded to `open`
                         of the compression library.
                         Options: ["no", "lzma", "gzip", "bz2"]
     """
     from slim_trees.lgbm_booster import dump
 
     dump_compressed(model, path, compression, dump)
+
+
+def dumps_lgbm_compressed(
+    model: Any, compression: Optional[Union[str, dict]] = None
+) -> bytes:
+    """
+    Pickles a model and returns the saved object as bytes.
+
+    Saves the parameters of the model as int16 and float32 instead of int64 and float64.
+    :param model: the model to save
+    :param compression: the compression method used. Either a string or a dict with key 'method' set
+                        to the compression method and other key-value pairs are forwarded to `open`
+                        of the compression library.
+                        Options: ["no", "lzma", "gzip", "bz2"]
+    """
+    from slim_trees.lgbm_booster import dumps
+
+    return dumps_compressed(model, compression, dumps)
```

### Comparing `slim-trees-0.2.0/slim_trees/compression_utils.py` & `slim-trees-0.2.1/slim_trees/compression_utils.py`

 * *Files identical despite different names*

### Comparing `slim-trees-0.2.0/slim_trees/pickling.py` & `slim-trees-0.2.1/slim_trees/pickling.py`

 * *Files 19% similar despite different names*

```diff
@@ -88,32 +88,76 @@
     compression_method, kwargs = _unpack_compression_args(compression, path)
     with _get_compression_library(compression_method).open(
         path, mode="wb", **kwargs
     ) as file:
         dump_function(obj, file)
 
 
+def dumps_compressed(
+    obj: Any,
+    compression: Optional[Union[str, dict]] = None,
+    dump_function: Optional[Callable] = None,
+) -> bytes:
+    """
+    Pickles a model and returns the pickled bytes. If compression is not specified, it won't use
+    any.
+    :param obj: the object to pickle
+    :param compression: the compression method used. Either a string or a dict with key 'method' set
+                        to the compression method and other key-value pairs are forwarded to open()
+                        of the compression library. Defaults to 'no' compression.
+                        Inspired by the pandas.to_csv interface.
+    :param dump_function: the function being called to dump the object, can be a custom pickler.
+                          Defaults to pickle.dumps()
+    """
+    if compression is None:
+        compression = "no"
+
+    if dump_function is None:
+        dump_function = pickle.dumps
+
+    compression_method, kwargs = _unpack_compression_args(compression, None)
+    data_uncompressed = dump_function(obj)
+    return _get_compression_library(compression_method).compress(data_uncompressed)
+
+
 def load_compressed(
     path: Union[str, pathlib.Path], compression: Optional[Union[str, dict]] = None
 ) -> Any:
     """
     Loads a compressed model.
     :param path: where to load the object from
-    :param compression: the compression method used. Either a string or a dict with key 'method' set
-                        to the compression method and other key-value pairs are forwarded to open()
-                        of the compression library.
+    :param compression: the compression method used. Either a string or a dict with key 'method'
+                        set to the compression method and other key-value pairs which are forwarded
+                        to open() of the compression library.
                         Inspired by the pandas.to_csv interface.
     """
     compression_method, kwargs = _unpack_compression_args(compression, path)
     with _get_compression_library(compression_method).open(
         path, mode="rb", **kwargs
     ) as file:
         return pickle.load(file)
 
 
+def loads_compressed(data: bytes, compression: Optional[Union[str, dict]] = None):
+    """
+    Loads a compressed model.
+    :param data: bytes containing the pickled object.
+    :param compression: the compression method used. Either a string or a dict with key 'method'
+                        set to the compression method and other key-value pairs which are forwarded
+                        to open() of the compression library. Defaults to 'no' compression.
+                        Inspired by the pandas.to_csv interface.
+    """
+    if compression is None:
+        compression = "no"
+
+    compression_method, kwargs = _unpack_compression_args(compression, None)
+    data_uncompressed = _get_compression_library(compression_method).decompress(data)
+    return pickle.loads(data_uncompressed)
+
+
 def get_pickled_size(
     obj: Any,
     compression: Union[str, dict] = "lzma",
     dump_function: Optional[Callable] = None,
 ) -> int:
     """
     Returns the size that an object would take on disk if pickled.
```

### Comparing `slim-trees-0.2.0/slim_trees/sklearn_tree.py` & `slim-trees-0.2.1/slim_trees/sklearn_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 import os
 import sys
 
 from slim_trees import __version__ as slim_trees_version
 from slim_trees.compression_utils import (
     compress_half_int_float_array,
     decompress_half_int_float_array,
@@ -25,14 +26,20 @@
 def dump(model: Any, file: BinaryIO):
     p = pickle.Pickler(file)
     p.dispatch_table = copyreg.dispatch_table.copy()
     p.dispatch_table[Tree] = _tree_pickle
     p.dump(model)
 
 
+def dumps(model: Any) -> bytes:
+    bytes_io = io.BytesIO()
+    dump(model, bytes_io)
+    return bytes_io.getvalue()
+
+
 def _tree_pickle(tree):
     assert isinstance(tree, Tree)
     reconstructor, args, state = tree.__reduce__()
     compressed_state = _compress_tree_state(state)
     return _tree_unpickle, (reconstructor, args, (slim_trees_version, compressed_state))
```

### Comparing `slim-trees-0.2.0/slim_trees.egg-info/PKG-INFO` & `slim-trees-0.2.1/slim_trees.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: slim-trees
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package for efficient pickling of ML models.
-Home-page: https://github.com/pavelzw/slim-trees
+Home-page: https://github.com/quantco/slim-trees
 Author: Pavel Zwerschke
-Author-email: pavelzw@gmail.com
+Author-email: pavel.zwerschke@quantco.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: scikit-learn
 Provides-Extra: lightgbm
 License-File: LICENSE
 
 # Slim Trees
 
-[![CI](https://github.com/pavelzw/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/pavelzw/slim-trees/actions/workflows/ci.yml)
+[![CI](https://github.com/quantco/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/quantco/slim-trees/actions/workflows/ci.yml)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/slim-trees?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/slim-trees)
 [![pypi-version](https://img.shields.io/pypi/v/slim-trees.svg?logo=pypi&logoColor=white)](https://pypi.org/project/slim-trees)
 [![python-version](https://img.shields.io/pypi/pyversions/slim-trees?logoColor=white&logo=python)](https://pypi.org/project/slim-trees)
 
 `slim-trees` is a Python package for saving and loading compressed `sklearn` Tree-based and `lightgbm` models.
 The compression is performed by modifying how the model is pickled by Python's `pickle` module.
 
+We presented this library at PyData Berlin 2023, check out the [slides](.github/assets/slim-trees-presentation.pdf)!
+
 ## Installation
 
 ```bash
 pip install slim-trees
 # or
-mamba install slim-trees -c conda-forge
+micromamba install slim-trees -c conda-forge
 ```
 
 ## Usage
 
 Using `slim-trees` does not affect your training pipeline.
 Simply call `dump_sklearn_compressed` or `dump_lgbm_compressed` to save your model.
 
@@ -86,17 +88,31 @@
 model = load_compressed("model.pkl")
 
 # or alternatively with pickle.load
 with open("model.pkl", "rb") as f:
     model = pickle.load(f)
 ```
 
----
+### Save your model as `bytes`
+
+You can also save the model as `bytes` instead of in a file similar to the `pickle.dumps` method.
+
+```python
+from slim_trees import dumps_sklearn_compressed, loads_compressed
+
+X, y = ...
+model = RandomForestClassifier()
+model.fit(X, y)
+
+data = dumps_sklearn_compressed(model, compression="lzma")
+...
+model_loaded = loads_compressed(data, compression="lzma")
+```
 
-### drop-in replacement for pickle
+### Drop-in replacement for pickle
 
 You can also use the `slim_trees.sklearn_tree.dump` or `slim_trees.lgbm_booster.dump` functions as drop-in replacements for `pickle.dump`.
 
 ```python
 from slim_trees import sklearn_tree, lgbm_booster
 
 # for sklearn models
@@ -109,21 +125,20 @@
 ```
 
 ## Development Installation
 
 You can install the package in development mode using:
 
 ```bash
-git clone git@github.com:pavelzw/slim-trees.git
+git clone https://github.com/quantco/slim-trees.git
 cd slim-trees
 
 # create and activate a fresh environment named slim_trees
-# see environment.yml for details
-mamba env create
-conda activate slim_trees
+micromamba create -f environment.yml
+micromamba activate slim_trees
 
 pre-commit install
 pip install --no-build-isolation -e .
 ```
 
 ## Benchmark
```

