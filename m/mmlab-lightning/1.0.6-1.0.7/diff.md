# Comparing `tmp/mmlab-lightning-1.0.6.tar.gz` & `tmp/mmlab-lightning-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmlab-lightning-1.0.6.tar", last modified: Fri May 19 03:41:18 2023, max compression
+gzip compressed data, was "mmlab-lightning-1.0.7.tar", last modified: Wed May 31 04:05:36 2023, max compression
```

## Comparing `mmlab-lightning-1.0.6.tar` & `mmlab-lightning-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.900697 mmlab-lightning-1.0.6/mmlab_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/datasets/mmlab_dataset_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/models/mmlab_model_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning/tools/config/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/tools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/tools/config/get_mmconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/datasets/mmlab_dataset_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/models/mmlab_model_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/tools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/tools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/tools/config/get_mmconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/setup.py
```

### Comparing `mmlab-lightning-1.0.6/LICENSE` & `mmlab-lightning-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mmlab-lightning-1.0.6/PKG-INFO` & `mmlab-lightning-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab-lightning
-Version: 1.0.6
+Version: 1.0.7
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab-lightning-1.0.6/README.md` & `mmlab-lightning-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mmlab-lightning-1.0.6/mmlab_lightning/datasets/mmlab_dataset_adapter.py` & `mmlab-lightning-1.0.7/mmlab_lightning/datasets/mmlab_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mmlab-lightning-1.0.6/mmlab_lightning/models/mmlab_model_adapter.py` & `mmlab-lightning-1.0.7/mmlab_lightning/models/mmlab_model_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC
-from typing import Any, Optional
+from typing import Any
 
 from lightning_template.models import LightningModule
 from mmengine import MessageHub
 from mmengine.model import BaseModule
 
 
 class MMLabModelAdapter(LightningModule, BaseModule, ABC):
```

### Comparing `mmlab-lightning-1.0.6/mmlab_lightning.egg-info/PKG-INFO` & `mmlab-lightning-1.0.7/mmlab_lightning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab-lightning
-Version: 1.0.6
+Version: 1.0.7
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab-lightning-1.0.6/mmlab_lightning.egg-info/SOURCES.txt` & `mmlab-lightning-1.0.7/mmlab_lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmlab-lightning-1.0.6/setup.py` & `mmlab-lightning-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mmlab-lightning",
-    version="1.0.6",
+    version="1.0.7",
     description="A wrapper for mmlab repos to use in project_template.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/mmlab_lightning",
     project_urls={
```

