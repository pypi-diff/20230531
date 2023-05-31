# Comparing `tmp/pygeoweaver-0.6.6.tar.gz` & `tmp/pygeoweaver-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.6.6.tar", last modified: Thu May 25 18:50:39 2023, max compression
+gzip compressed data, was "pygeoweaver-0.6.7.tar", last modified: Wed May 31 17:41:58 2023, max compression
```

## Comparing `pygeoweaver-0.6.6.tar` & `pygeoweaver-0.6.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_resetpassword.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-25 18:50:39.000000 pygeoweaver-0.6.6/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-25 18:50:39.000000 pygeoweaver-0.6.6/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:50:39.000000 pygeoweaver-0.6.6/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 18:50:39.000000 pygeoweaver-0.6.6/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-25 18:50:39.015588 pygeoweaver-0.6.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:39.011588 pygeoweaver-0.6.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/test/test_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-25 18:50:28.000000 pygeoweaver-0.6.6/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_resetpassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-31 17:41:58.000000 pygeoweaver-0.6.7/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 17:41:58.000000 pygeoweaver-0.6.7/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:41:58.000000 pygeoweaver-0.6.7/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 17:41:58.000000 pygeoweaver-0.6.7/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/test/test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/test/test_server.py
```

### Comparing `pygeoweaver-0.6.6/LICENSE` & `pygeoweaver-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/PKG-INFO` & `pygeoweaver-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.6
+Version: 0.6.7
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.6/README.md` & `pygeoweaver-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/pygeoweaver/__main__.py` & `pygeoweaver-0.6.7/pygeoweaver/__main__.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/pygeoweaver/sc_detail.py` & `pygeoweaver-0.6.7/pygeoweaver/sc_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/pygeoweaver/sc_export.py` & `pygeoweaver-0.6.7/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/pygeoweaver/sc_help.py` & `pygeoweaver-0.6.7/pygeoweaver/sc_help.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/pygeoweaver/sc_import.py` & `pygeoweaver-0.6.7/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/pygeoweaver/sc_list.py` & `pygeoweaver-0.6.7/pygeoweaver/sc_list.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/pygeoweaver/sc_run.py` & `pygeoweaver-0.6.7/pygeoweaver/sc_run.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/pygeoweaver/server.py` & `pygeoweaver-0.6.7/pygeoweaver/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import subprocess
 import webbrowser
 from pygeoweaver.constants import GEOWEAVER_DEFAULT_ENDPOINT_URL
-from pygeoweaver.utils import checkIPython, checkOS, download_geoweaver_jar, get_logger, get_root_dir
+from pygeoweaver.utils import checkIPython, checkOS, download_geoweaver_jar, get_logger, get_module_absolute_path, get_root_dir
 
 """
 This module provides function to start and stop Geoweaver server.
 If it detects the current environment is Jupyter notebook, it will 
 open Geoweaver GUI in the output cell (if gui is not disabld.)
 
 """
@@ -14,23 +14,23 @@
 logger = get_logger(__name__)
 
 def start(force=False):
     download_geoweaver_jar(overwrite=force)
     if checkOS() == 3:
         raise RuntimeError("windows is not supported yet")
     else:
-        result = subprocess.run(['./start.sh'], cwd=f"{get_root_dir()}/")
+        result = subprocess.run([f'{get_module_absolute_path()}/start.sh'], cwd=f"{get_root_dir()}/")
     
 
 
 def stop():
     if checkOS() == 3:
         raise RuntimeError("Windows is not supported yet")
     else:
-        result = subprocess.run(['./stop.sh'], cwd=f"{get_root_dir()}/", shell=True)
+        result = subprocess.run([f'{get_module_absolute_path()}/stop.sh'], cwd=f"{get_root_dir()}/", shell=True)
     
 
 def show(geoweaver_url = GEOWEAVER_DEFAULT_ENDPOINT_URL):
     download_geoweaver_jar()  # check if geoweaver is initialized
     if checkIPython():
         logger.info("enter ipython block")
         from IPython.display import IFrame
```

### Comparing `pygeoweaver-0.6.6/pygeoweaver/utils.py` & `pygeoweaver-0.6.7/pygeoweaver/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     return os.path.expanduser('~')
 
 
 def get_root_dir():
     head, tail = os.path.split(__file__)
     return head
 
+def get_module_absolute_path():
+    module_path = os.path.abspath(__file__)
+    return os.path.dirname(module_path)
+
 
 def get_geoweaver_jar_path():
     return f"{get_home_dir()}/geoweaver.jar"
 
 
 def check_geoweaver_jar():
     return os.path.isfile(get_geoweaver_jar_path())
```

### Comparing `pygeoweaver-0.6.6/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.6.7/pygeoweaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.6
+Version: 0.6.7
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.6/pygeoweaver.egg-info/SOURCES.txt` & `pygeoweaver-0.6.7/pygeoweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/pyproject.toml` & `pygeoweaver-0.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "pytest-cov"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.6.6"
+version = "0.6.7"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,15 +18,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry]
 name = "pygeoweaver"
-version = "0.6.6"
+version = "0.6.7"
 description = "This is a wrapper package of the Geoweaver app."
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
```

### Comparing `pygeoweaver-0.6.6/test/test_detail.py` & `pygeoweaver-0.6.7/test/test_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.6/test/test_server.py` & `pygeoweaver-0.6.7/test/test_server.py`

 * *Files identical despite different names*

