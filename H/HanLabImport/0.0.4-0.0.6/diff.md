# Comparing `tmp/HanLabImport-0.0.4.tar.gz` & `tmp/HanLabImport-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HanLabImport-0.0.4.tar", last modified: Wed May 31 19:31:51 2023, max compression
+gzip compressed data, was "HanLabImport-0.0.6.tar", last modified: Wed May 31 20:22:50 2023, max compression
```

## Comparing `HanLabImport-0.0.4.tar` & `HanLabImport-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:31:51.758771 HanLabImport-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:31:51.758771 HanLabImport-0.0.4/HanLabImport/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-31 19:31:41.000000 HanLabImport-0.0.4/HanLabImport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-31 19:31:41.000000 HanLabImport-0.0.4/HanLabImport/io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 19:31:41.000000 HanLabImport-0.0.4/HanLabImport/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:31:51.758771 HanLabImport-0.0.4/HanLabImport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-31 19:31:51.000000 HanLabImport-0.0.4/HanLabImport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-31 19:31:51.000000 HanLabImport-0.0.4/HanLabImport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:31:51.000000 HanLabImport-0.0.4/HanLabImport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 19:31:51.000000 HanLabImport-0.0.4/HanLabImport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 19:31:51.000000 HanLabImport-0.0.4/HanLabImport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 19:31:41.000000 HanLabImport-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-31 19:31:51.758771 HanLabImport-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-31 19:31:41.000000 HanLabImport-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 19:31:41.000000 HanLabImport-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:31:51.758771 HanLabImport-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-31 19:31:41.000000 HanLabImport-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:22:50.586124 HanLabImport-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:22:50.586124 HanLabImport-0.0.6/HanLabImport/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-31 20:22:39.000000 HanLabImport-0.0.6/HanLabImport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:22:50.586124 HanLabImport-0.0.6/HanLabImport/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-31 20:22:39.000000 HanLabImport-0.0.6/HanLabImport/config/HanLab.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-31 20:22:39.000000 HanLabImport-0.0.6/HanLabImport/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 20:22:39.000000 HanLabImport-0.0.6/HanLabImport/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:22:50.586124 HanLabImport-0.0.6/HanLabImport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 20:22:50.000000 HanLabImport-0.0.6/HanLabImport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 20:22:50.000000 HanLabImport-0.0.6/HanLabImport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:22:50.000000 HanLabImport-0.0.6/HanLabImport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 20:22:50.000000 HanLabImport-0.0.6/HanLabImport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 20:22:50.000000 HanLabImport-0.0.6/HanLabImport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 20:22:39.000000 HanLabImport-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 20:22:50.586124 HanLabImport-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-31 20:22:39.000000 HanLabImport-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 20:22:39.000000 HanLabImport-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:22:50.586124 HanLabImport-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-31 20:22:39.000000 HanLabImport-0.0.6/setup.py
```

### Comparing `HanLabImport-0.0.4/HanLabImport/io.py` & `HanLabImport-0.0.6/HanLabImport/io.py`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.4/HanLabImport.egg-info/PKG-INFO` & `HanLabImport-0.0.6/HanLabImport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: HanLabImport
-Version: 0.0.4
+Version: 0.0.6
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabImport
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabImport/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![http://dnplab.net](https://img.shields.io/pypi/v/dnplab)](https://pypi.org/project/dnplab/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dnplab)](https://www.python.org/downloads/)
 [![Downloads](https://pepy.tech/badge/dnplab/month)](https://pepy.tech/project/dnplab)
```

### Comparing `HanLabImport-0.0.4/LICENSE` & `HanLabImport-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.4/PKG-INFO` & `HanLabImport-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: HanLabImport
-Version: 0.0.4
+Version: 0.0.6
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabImport
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabImport/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![http://dnplab.net](https://img.shields.io/pypi/v/dnplab)](https://pypi.org/project/dnplab/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dnplab)](https://www.python.org/downloads/)
 [![Downloads](https://pepy.tech/badge/dnplab/month)](https://pepy.tech/project/dnplab)
```

### Comparing `HanLabImport-0.0.4/README.md` & `HanLabImport-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.4/setup.py` & `HanLabImport-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,17 +13,18 @@
     name="HanLabImport",
     version=__version__,
     description="Import tools for DNPLab specific to the Han Lab",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Thorsten Maly",
     author_email="tmaly@bridge12.com",
-    python_requires=">=3.9",
+    python_requires=">=3.10",
     install_requires=[
         "numpy>=1.24",
     ],
+    data_files=[('config', ['HanLabImport/config/HanLab.cfg'])],
     packages=setuptools.find_packages(),
     url="https://github.com/Bridge12Technologies/HanLabImport",
     project_urls={
         "Tracker": "https://github.com/Bridge12Technologies/HanLabImport/issues"
     },
 )
```

