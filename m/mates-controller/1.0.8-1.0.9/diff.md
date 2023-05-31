# Comparing `tmp/mates-controller-1.0.8.tar.gz` & `tmp/mates-controller-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mates-controller-1.0.8.tar", last modified: Thu Feb 23 17:07:45 2023, max compression
+gzip compressed data, was "mates-controller-1.0.9.tar", last modified: Wed May 31 07:32:45 2023, max compression
```

## Comparing `mates-controller-1.0.8.tar` & `mates-controller-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:45.743418 mates-controller-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-23 17:07:33.000000 mates-controller-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23441 2023-02-23 17:07:45.743418 mates-controller-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22815 2023-02-23 17:07:33.000000 mates-controller-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-23 17:07:33.000000 mates-controller-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-23 17:07:45.743418 mates-controller-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:45.739418 mates-controller-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:45.739418 mates-controller-1.0.8/src/mates/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-23 17:07:33.000000 mates-controller-1.0.8/src/mates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-02-23 17:07:33.000000 mates-controller-1.0.8/src/mates/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)   298263 2023-02-23 17:07:33.000000 mates-controller-1.0.8/src/mates/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    45874 2023-02-23 17:07:33.000000 mates-controller-1.0.8/src/mates/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-23 17:07:33.000000 mates-controller-1.0.8/src/mates/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:45.743418 mates-controller-1.0.8/src/mates_controller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23441 2023-02-23 17:07:45.000000 mates-controller-1.0.8/src/mates_controller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-23 17:07:45.000000 mates-controller-1.0.8/src/mates_controller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:07:45.000000 mates-controller-1.0.8/src/mates_controller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-23 17:07:45.000000 mates-controller-1.0.8/src/mates_controller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-23 17:07:45.000000 mates-controller-1.0.8/src/mates_controller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:32:45.618341 mates-controller-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 07:32:33.000000 mates-controller-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23441 2023-05-31 07:32:45.618341 mates-controller-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22815 2023-05-31 07:32:33.000000 mates-controller-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 07:32:33.000000 mates-controller-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-31 07:32:45.618341 mates-controller-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:32:45.614341 mates-controller-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:32:45.618341 mates-controller-1.0.9/src/mates/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 07:32:33.000000 mates-controller-1.0.9/src/mates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-31 07:32:33.000000 mates-controller-1.0.9/src/mates/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)   298263 2023-05-31 07:32:33.000000 mates-controller-1.0.9/src/mates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45892 2023-05-31 07:32:33.000000 mates-controller-1.0.9/src/mates/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-31 07:32:33.000000 mates-controller-1.0.9/src/mates/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:32:45.618341 mates-controller-1.0.9/src/mates_controller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23441 2023-05-31 07:32:45.000000 mates-controller-1.0.9/src/mates_controller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-31 07:32:45.000000 mates-controller-1.0.9/src/mates_controller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:32:45.000000 mates-controller-1.0.9/src/mates_controller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 07:32:45.000000 mates-controller-1.0.9/src/mates_controller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 07:32:45.000000 mates-controller-1.0.9/src/mates_controller.egg-info/top_level.txt
```

### Comparing `mates-controller-1.0.8/LICENSE` & `mates-controller-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mates-controller-1.0.8/PKG-INFO` & `mates-controller-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mates-controller
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python Library developed to be used with Mates Studio Commander and Architect Environments
 Home-page: https://github.com/BreadBoardMates/Python-Mates-Controller
 Author: Breadboard Mates
 Author-email: developers@breadboardmates.com
 Project-URL: Bug Tracker, https://github.com/BreadBoardMates/Python-Mates-Controller/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mates-controller-1.0.8/README.md` & `mates-controller-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mates-controller-1.0.8/setup.cfg` & `mates-controller-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mates-controller
-version = 1.0.8
+version = 1.0.9
 author = Breadboard Mates
 author_email = developers@breadboardmates.com
 description = A Python Library developed to be used with Mates Studio Commander and Architect Environments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BreadBoardMates/Python-Mates-Controller
 project_urls =
```

### Comparing `mates-controller-1.0.8/src/mates/commands.py` & `mates-controller-1.0.9/src/mates/commands.py`

 * *Files identical despite different names*

### Comparing `mates-controller-1.0.8/src/mates/constants.py` & `mates-controller-1.0.9/src/mates/constants.py`

 * *Files identical despite different names*

### Comparing `mates-controller-1.0.8/src/mates/controller.py` & `mates-controller-1.0.9/src/mates/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import typing
 import io
 import serial
 from time import time, sleep
 from typing import Tuple
 from PIL import Image
 
-from data import *
-from constants import *
-from commands import MatesCommand
+from mates.data import *
+from mates.constants import *
+from mates.commands import MatesCommand
 
 delay = lambda ms: sleep(ms/1000.0)
 delayMicroseconds = lambda us: sleep(us/1000000.0)
 
 
 class MatesController:
     """
```

### Comparing `mates-controller-1.0.8/src/mates/data.py` & `mates-controller-1.0.9/src/mates/data.py`

 * *Files identical despite different names*

### Comparing `mates-controller-1.0.8/src/mates_controller.egg-info/PKG-INFO` & `mates-controller-1.0.9/src/mates_controller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mates-controller
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python Library developed to be used with Mates Studio Commander and Architect Environments
 Home-page: https://github.com/BreadBoardMates/Python-Mates-Controller
 Author: Breadboard Mates
 Author-email: developers@breadboardmates.com
 Project-URL: Bug Tracker, https://github.com/BreadBoardMates/Python-Mates-Controller/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

