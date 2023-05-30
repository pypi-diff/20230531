# Comparing `tmp/wicker-0.0.4b0.tar.gz` & `tmp/wicker-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicker-0.0.4b0.tar", last modified: Mon Mar  6 14:27:38 2023, max compression
+gzip compressed data, was "wicker-0.0.5a0.tar", last modified: Tue May 30 22:32:54 2023, max compression
```

## Comparing `wicker-0.0.4b0.tar` & `wicker-0.0.5a0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:38.648266 wicker-0.0.4b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-06 14:27:30.000000 wicker-0.0.4b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-06 14:27:30.000000 wicker-0.0.4b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-06 14:27:38.648266 wicker-0.0.4b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-06 14:27:30.000000 wicker-0.0.4b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 14:27:30.000000 wicker-0.0.4b0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-06 14:27:30.000000 wicker-0.0.4b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-06 14:27:38.648266 wicker-0.0.4b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-06 14:27:30.000000 wicker-0.0.4b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:38.648266 wicker-0.0.4b0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:38.644266 wicker-0.0.4b0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/core/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    21017 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/test_avro_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/test_column_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/test_filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/test_numpy_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/test_s3_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-03-06 14:27:30.000000 wicker-0.0.4b0/tests/test_wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:38.644266 wicker-0.0.4b0/wicker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:38.644266 wicker-0.0.4b0/wicker/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/column_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/persistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:38.644266 wicker-0.0.4b0/wicker/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/plugins/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/plugins/flyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/plugins/spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/plugins/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:38.648266 wicker-0.0.4b0/wicker/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/schema/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/schema/dataloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/schema/dataparsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/schema/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/schema/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:38.648266 wicker-0.0.4b0/wicker/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/testing/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-06 14:27:30.000000 wicker-0.0.4b0/wicker/testing/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:38.648266 wicker-0.0.4b0/wicker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-06 14:27:38.000000 wicker-0.0.4b0/wicker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-06 14:27:38.000000 wicker-0.0.4b0/wicker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:27:38.000000 wicker-0.0.4b0/wicker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-06 14:27:38.000000 wicker-0.0.4b0/wicker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-06 14:27:38.000000 wicker-0.0.4b0/wicker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.101565 wicker-0.0.5a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 22:32:46.000000 wicker-0.0.5a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 22:32:46.000000 wicker-0.0.5a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-30 22:32:54.101565 wicker-0.0.5a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-30 22:32:46.000000 wicker-0.0.5a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 22:32:46.000000 wicker-0.0.5a0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-30 22:32:46.000000 wicker-0.0.5a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-30 22:32:54.101565 wicker-0.0.5a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 22:32:46.000000 wicker-0.0.5a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.101565 wicker-0.0.5a0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/core/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21017 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_avro_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_column_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_numpy_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_s3_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/column_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/persistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/flyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/dataloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/dataparsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/testing/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/testing/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.101565 wicker-0.0.5a0/wicker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/top_level.txt
```

### Comparing `wicker-0.0.4b0/LICENSE` & `wicker-0.0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/PKG-INFO` & `wicker-0.0.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicker
-Version: 0.0.4b0
+Version: 0.0.5a0
 Summary: An open source framework for Machine Learning dataset storage and serving
 Home-page: https://github.com/woven-planet/Wicker
 Author: Jay Chia
 Author-email: jaychia94@gmail.com
 Project-URL: Bug Tracker, https://github.com/woven-planet/Wicker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `wicker-0.0.4b0/README.md` & `wicker-0.0.5a0/README.md`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/setup.cfg` & `wicker-0.0.5a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/tests/core/test_persistence.py` & `wicker-0.0.5a0/tests/core/test_persistence.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import copy
 import os
 import random
 import uuid
 from typing import Any, Dict, List, Tuple
 
+import pyarrow.fs as pafs
 import pyarrow.parquet as papq
 import pytest
 
 from wicker import schema
-from wicker.core.config import get_config
+from wicker.core.datasets import S3Dataset
 from wicker.core.persistance import BasicPersistor
 from wicker.core.storage import S3PathFactory
 from wicker.schema.schema import DatasetSchema
-from wicker.testing.storage import FakeS3DataStorage
+from wicker.testing.storage import LocalDataStorage
 
 DATASET_NAME = "dataset"
 DATASET_VERSION = "0.0.1"
 SCHEMA = schema.DatasetSchema(
     primary_keys=["bar", "foo"],
     fields=[
         schema.IntField("foo"),
@@ -37,23 +38,23 @@
 ]
 # Examples with a duplicated key
 EXAMPLES_DUPES = copy.deepcopy(EXAMPLES)
 
 
 @pytest.fixture
 def mock_basic_persistor(request, tmpdir) -> Tuple[BasicPersistor, str]:
-    storage = request.param.get("storage", FakeS3DataStorage(tmpdir=tmpdir))
-    path_factory = request.param.get("path_factory", S3PathFactory())
+    storage = request.param.get("storage", LocalDataStorage(root_path=tmpdir))
+    path_factory = request.param.get("path_factory", S3PathFactory(s3_root_path=os.path.join(tmpdir, "datasets")))
     return BasicPersistor(storage, path_factory), tmpdir
 
 
-def assert_written_correctness(tmpdir: str) -> None:
+def assert_written_correctness(persistor: BasicPersistor, data: List[Tuple[str, Dict[str, Any]]], tmpdir: str) -> None:
     """Asserts that all files are written as expected by the L5MLDatastore"""
     # Check that files are correctly written locally by Spark/Parquet with a _SUCCESS marker file
-    prefix = get_config().aws_s3_config.s3_datasets_path.replace("s3://", "")
+    prefix = persistor.s3_path_factory.root_path
     assert DATASET_NAME in os.listdir(os.path.join(tmpdir, prefix))
     assert DATASET_VERSION in os.listdir(os.path.join(tmpdir, prefix, DATASET_NAME))
     for partition in ["train", "test"]:
         print(os.listdir(os.path.join(tmpdir, prefix)))
         columns_path = os.path.join(tmpdir, prefix, "__COLUMN_CONCATENATED_FILES__")
         all_read_bytes = b""
         for filename in os.listdir(columns_path):
@@ -64,14 +65,30 @@
 
         # Load parquet file and assert ordering of primary_key
         assert f"{partition}.parquet" in os.listdir(os.path.join(tmpdir, prefix, DATASET_NAME, DATASET_VERSION))
         tbl = papq.read_table(os.path.join(tmpdir, prefix, DATASET_NAME, DATASET_VERSION, f"{partition}.parquet"))
         foobar = [(barval.as_py(), fooval.as_py()) for fooval, barval in zip(tbl["foo"], tbl["bar"])]
         assert foobar == sorted(foobar)
 
+        # Also load the data from the dataset and check it.
+        ds = S3Dataset(
+            DATASET_NAME,
+            DATASET_VERSION,
+            partition,
+            local_cache_path_prefix=tmpdir,
+            storage=persistor.s3_storage,
+            s3_path_factory=persistor.s3_path_factory,
+            pa_filesystem=pafs.LocalFileSystem(),
+        )
+
+        ds_values = [ds[idx] for idx in range(len(ds))]
+        # Sort the expected values by the primary keys.
+        expected_values = sorted([value for p, value in data if p == partition], key=lambda v: (v["bar"], v["foo"]))
+        assert ds_values == expected_values
+
 
 @pytest.mark.parametrize(
     "mock_basic_persistor, dataset_name, dataset_version, dataset_schema, dataset",
     [({}, DATASET_NAME, DATASET_VERSION, SCHEMA, copy.deepcopy(EXAMPLES_DUPES))],
     indirect=["mock_basic_persistor"],
 )
 def test_basic_persistor(
@@ -88,8 +105,8 @@
     and the ordering is correct.
     """
     # create the mock basic persistor
     mock_basic_persistor_obj, tempdir = mock_basic_persistor
     # persist the dataset
     mock_basic_persistor_obj.persist_wicker_dataset(dataset_name, dataset_version, dataset_schema, dataset)
     # assert the dataset is correctly written
-    assert_written_correctness(tempdir)
+    assert_written_correctness(persistor=mock_basic_persistor_obj, data=dataset, tmpdir=tempdir)
```

### Comparing `wicker-0.0.4b0/tests/test_avro_schema.py` & `wicker-0.0.5a0/tests/test_avro_schema.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/tests/test_column_files.py` & `wicker-0.0.5a0/tests/test_column_files.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/tests/test_datasets.py` & `wicker-0.0.5a0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/tests/test_filelock.py` & `wicker-0.0.5a0/tests/test_filelock.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/tests/test_numpy_codec.py` & `wicker-0.0.5a0/tests/test_numpy_codec.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/tests/test_s3_storage.py` & `wicker-0.0.5a0/tests/test_s3_storage.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/tests/test_shuffle.py` & `wicker-0.0.5a0/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/tests/test_spark.py` & `wicker-0.0.5a0/tests/test_spark.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/tests/test_wandb.py` & `wicker-0.0.5a0/tests/test_wandb.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/core/column_files.py` & `wicker-0.0.5a0/wicker/core/column_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
             self.byte_offset,
             self.data_size,
         )
 
     @classmethod
     def from_bytes(cls, b: bytes) -> ColumnBytesFileLocationV1:
         protocol_version = int.from_bytes(b[0:1], "little")
+        # non 1 version does not gurantee parsability in struct unpack
+        if protocol_version != 1:
+            raise ValueError(f"Unable to parse ColumnBytesFileLocation with protocol_version={protocol_version}")
         _, file_id, byte_offset, data_size = struct.unpack(ColumnBytesFileLocationV1.STRUCT_PACK_FMT, b)
         return cls(
             file_id=uuid.UUID(bytes=file_id),
             byte_offset=byte_offset,
             data_size=data_size,
         )
```

### Comparing `wicker-0.0.4b0/wicker/core/config.py` & `wicker-0.0.5a0/wicker/core/config.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/core/datasets.py` & `wicker-0.0.5a0/wicker/core/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,16 @@
     def _get_parquet_dir_size(self) -> int:
         """Get the arrow path and find all the files within, count their bytes
 
         Returns:
             int: bytes in parquet directory
         """
         # bytes size of arrow table not bytes in arrow table
+        # bytes in arrow table is a method of arrow table but it doesn't
+        # reflect the size of the file sizes stored on s3 just the loaded data
         arrow_path = self._s3_path_factory.get_dataset_partition_path(self._partition, s3_prefix=False)
         bucket, key = arrow_path.replace("s3://", "").split("/", 1)
 
         def get_folder_size(bucket, prefix):
             total_size = 0
             for obj in boto3.resource("s3").Bucket(bucket).objects.filter(Prefix=prefix):
                 total_size += obj.size
```

### Comparing `wicker-0.0.4b0/wicker/core/definitions.py` & `wicker-0.0.5a0/wicker/core/definitions.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/core/filelock.py` & `wicker-0.0.5a0/wicker/core/filelock.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/core/persistance.py` & `wicker-0.0.5a0/wicker/core/persistance.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from wicker import schema as schema_module
 from wicker.core.column_files import ColumnBytesFileWriter
 from wicker.core.definitions import DatasetID
 from wicker.core.shuffle import save_index
 from wicker.core.storage import S3DataStorage, S3PathFactory
 from wicker.schema import dataparsing, serialization
 
-PARTITION_SIZE = 256
 MAX_COL_FILE_NUMROW = 50  # TODO(isaak-willett): Magic number, we should derive this based on row size
 
 UnparsedExample = Dict[str, Any]
 ParsedExample = Dict[str, Any]
 PointerParsedExample = Dict[str, Any]
 
 
@@ -221,38 +220,24 @@
 
         # 3. Validate the rows and ensure data is well formed, sort while doing
         dataset_0 = [(row[0], self.parse_row(row[1], dataset_schema)) for row in dataset]
 
         # 4. Sort the dataset if not sorted
         sorted_dataset_0 = sorted(dataset_0, key=lambda tup: tup[0])
 
-        # 5. Partition the dataset into K partitions
-        partitions = []
-
-        def divide_chunks(list_to_divide):
-            # looping till length l
-            for i in range(0, len(list_to_divide), PARTITION_SIZE):
-                partitions.append(list_to_divide[i : i + PARTITION_SIZE])
-
-        divide_chunks(sorted_dataset_0)
-
         # 6. Persist the partitions to S3
-        for partition in partitions:
-            # build a persistence iterator for each parition
-            iterator = self.persist_wicker_partition(
-                partition, dataset_schema, self.s3_storage, self.s3_path_factory, MAX_COL_FILE_NUMROW
-            )
-            # make sure all yields get called
-            list(iterator)
+        metadata_iterator = self.persist_wicker_partition(
+            sorted_dataset_0, dataset_schema, self.s3_storage, self.s3_path_factory, MAX_COL_FILE_NUMROW
+        )
 
         # 7. Create the parition table, need to combine keys in a way we can form table
         # split into k dicts where k is partition number and the data is a list of values
         # for each key for all the dicts in the partition
         merged_dicts: Dict[str, Dict[str, List[Any]]] = {}
-        for partition_key, row in sorted_dataset_0:
+        for partition_key, row in metadata_iterator:
             current_dict: Dict[str, List[Any]] = merged_dicts.get(partition_key, {})
             for col in row.keys():
                 if col in current_dict:
                     current_dict[col].append(row[col])
                 else:
                     current_dict[col] = [row[col]]
             merged_dicts[partition_key] = current_dict
```

### Comparing `wicker-0.0.4b0/wicker/core/shuffle.py` & `wicker-0.0.5a0/wicker/core/shuffle.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/core/storage.py` & `wicker-0.0.5a0/wicker/core/storage.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/core/writer.py` & `wicker-0.0.5a0/wicker/core/writer.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/plugins/dynamodb.py` & `wicker-0.0.5a0/wicker/plugins/dynamodb.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/plugins/flyte.py` & `wicker-0.0.5a0/wicker/plugins/flyte.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/plugins/spark.py` & `wicker-0.0.5a0/wicker/plugins/spark.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/plugins/wandb.py` & `wicker-0.0.5a0/wicker/plugins/wandb.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/schema/codecs.py` & `wicker-0.0.5a0/wicker/schema/codecs.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/schema/dataloading.py` & `wicker-0.0.5a0/wicker/schema/dataloading.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/schema/dataparsing.py` & `wicker-0.0.5a0/wicker/schema/dataparsing.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/schema/schema.py` & `wicker-0.0.5a0/wicker/schema/schema.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/schema/serialization.py` & `wicker-0.0.5a0/wicker/schema/serialization.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/schema/validation.py` & `wicker-0.0.5a0/wicker/schema/validation.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker/testing/codecs.py` & `wicker-0.0.5a0/wicker/testing/codecs.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.4b0/wicker.egg-info/PKG-INFO` & `wicker-0.0.5a0/wicker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicker
-Version: 0.0.4b0
+Version: 0.0.5a0
 Summary: An open source framework for Machine Learning dataset storage and serving
 Home-page: https://github.com/woven-planet/Wicker
 Author: Jay Chia
 Author-email: jaychia94@gmail.com
 Project-URL: Bug Tracker, https://github.com/woven-planet/Wicker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `wicker-0.0.4b0/wicker.egg-info/SOURCES.txt` & `wicker-0.0.5a0/wicker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

