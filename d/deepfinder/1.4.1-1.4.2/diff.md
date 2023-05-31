# Comparing `tmp/deepfinder-1.4.1.tar.gz` & `tmp/deepfinder-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfinder-1.4.1.tar", last modified: Thu Jan 12 12:48:56 2023, max compression
+gzip compressed data, was "deepfinder-1.4.2.tar", last modified: Wed May 31 08:03:04 2023, max compression
```

## Comparing `deepfinder-1.4.1.tar` & `deepfinder-1.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:48:56.979330 deepfinder-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-12 12:48:40.000000 deepfinder-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-01-12 12:48:56.979330 deepfinder-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-01-12 12:48:40.000000 deepfinder-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:48:56.975329 deepfinder-1.4.1/deepfinder/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-12 12:48:40.000000 deepfinder-1.4.1/deepfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-01-12 12:48:40.000000 deepfinder-1.4.1/deepfinder/deep_find.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-12 12:48:40.000000 deepfinder-1.4.1/deepfinder/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:48:56.979330 deepfinder-1.4.1/deepfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-01-12 12:48:56.000000 deepfinder-1.4.1/deepfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-12 12:48:56.000000 deepfinder-1.4.1/deepfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 12:48:56.000000 deepfinder-1.4.1/deepfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-12 12:48:56.000000 deepfinder-1.4.1/deepfinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-12 12:48:40.000000 deepfinder-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-01-12 12:48:56.979330 deepfinder-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:03:04.279478 deepfinder-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 08:02:48.000000 deepfinder-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-31 08:03:04.279478 deepfinder-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-31 08:02:48.000000 deepfinder-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:03:04.279478 deepfinder-1.4.2/deepfinder/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-31 08:02:48.000000 deepfinder-1.4.2/deepfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-31 08:02:48.000000 deepfinder-1.4.2/deepfinder/deep_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-31 08:02:48.000000 deepfinder-1.4.2/deepfinder/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:03:04.279478 deepfinder-1.4.2/deepfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-31 08:03:04.000000 deepfinder-1.4.2/deepfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 08:03:04.000000 deepfinder-1.4.2/deepfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:03:04.000000 deepfinder-1.4.2/deepfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 08:03:04.000000 deepfinder-1.4.2/deepfinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-31 08:02:48.000000 deepfinder-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-31 08:03:04.283479 deepfinder-1.4.2/setup.cfg
```

### Comparing `deepfinder-1.4.1/LICENSE` & `deepfinder-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepfinder-1.4.1/PKG-INFO` & `deepfinder-1.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfinder
-Version: 1.4.1
+Version: 1.4.2
 Summary: Search attributes easily using dot paths. Within structures of type dictionary, list and embedded substructures with simple format 'dict.users.0.name'.
 Home-page: https://github.com/jparadadev/deepfinder.py
 Author: Javier Parada
 Author-email: javierparadadev@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jparadadev/deepfinder.py/issues
 Keywords: find,get,dictionary,list,array,deep,find,structure,nested,nested,data
@@ -16,21 +16,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Deepfinder
+<h1 align="center">🔍 Deepfinder </h1>
+
+<div align="center">
 
 ![](https://img.shields.io/badge/PRs-welcome-green.svg)
 [![GitHub](https://img.shields.io/github/license/jparadadev/deepfinder.py)](https://github.com/jparadadev/deepfinder.py/blob/main/LICENSE)
 [![Pypi](https://img.shields.io/pypi/v/deepfinder)](https://pypi.org/project/deepfinder/)
 [![Downloads](https://pepy.tech/badge/deepfinder)](https://pepy.tech/project/deepfinder)
 [![GA](https://github.com/jparadadev/deepfinder.py/workflows/Tests/badge.svg)](https://github.com/jparadadev/deepfinder.py/actions/workflows/test.yml)
+  
+</div>
+
+![](https://raw.githubusercontent.com/jparadadev/deepfinder.py/assets/assets/logo.png)
 
 Search attributes easily using dot paths. Within structures of type dictionary, list and embedded substructures with simple format 'dict.users.0.name'.
 
 ## Getting Started
 
 ### Installation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepfinder-1.4.1/README.md` & `deepfinder-1.4.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-# Deepfinder
+<h1 align="center">🔍 Deepfinder </h1>
+
+<div align="center">
 
 ![](https://img.shields.io/badge/PRs-welcome-green.svg)
 [![GitHub](https://img.shields.io/github/license/jparadadev/deepfinder.py)](https://github.com/jparadadev/deepfinder.py/blob/main/LICENSE)
 [![Pypi](https://img.shields.io/pypi/v/deepfinder)](https://pypi.org/project/deepfinder/)
 [![Downloads](https://pepy.tech/badge/deepfinder)](https://pepy.tech/project/deepfinder)
 [![GA](https://github.com/jparadadev/deepfinder.py/workflows/Tests/badge.svg)](https://github.com/jparadadev/deepfinder.py/actions/workflows/test.yml)
+  
+</div>
+
+![](https://raw.githubusercontent.com/jparadadev/deepfinder.py/assets/assets/logo.png)
 
 Search attributes easily using dot paths. Within structures of type dictionary, list and embedded substructures with simple format 'dict.users.0.name'.
 
 ## Getting Started
 
 ### Installation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepfinder-1.4.1/deepfinder/deep_find.py` & `deepfinder-1.4.2/deepfinder/deep_find.py`

 * *Files identical despite different names*

### Comparing `deepfinder-1.4.1/deepfinder.egg-info/PKG-INFO` & `deepfinder-1.4.2/deepfinder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfinder
-Version: 1.4.1
+Version: 1.4.2
 Summary: Search attributes easily using dot paths. Within structures of type dictionary, list and embedded substructures with simple format 'dict.users.0.name'.
 Home-page: https://github.com/jparadadev/deepfinder.py
 Author: Javier Parada
 Author-email: javierparadadev@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jparadadev/deepfinder.py/issues
 Keywords: find,get,dictionary,list,array,deep,find,structure,nested,nested,data
@@ -16,21 +16,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Deepfinder
+<h1 align="center">🔍 Deepfinder </h1>
+
+<div align="center">
 
 ![](https://img.shields.io/badge/PRs-welcome-green.svg)
 [![GitHub](https://img.shields.io/github/license/jparadadev/deepfinder.py)](https://github.com/jparadadev/deepfinder.py/blob/main/LICENSE)
 [![Pypi](https://img.shields.io/pypi/v/deepfinder)](https://pypi.org/project/deepfinder/)
 [![Downloads](https://pepy.tech/badge/deepfinder)](https://pepy.tech/project/deepfinder)
 [![GA](https://github.com/jparadadev/deepfinder.py/workflows/Tests/badge.svg)](https://github.com/jparadadev/deepfinder.py/actions/workflows/test.yml)
+  
+</div>
+
+![](https://raw.githubusercontent.com/jparadadev/deepfinder.py/assets/assets/logo.png)
 
 Search attributes easily using dot paths. Within structures of type dictionary, list and embedded substructures with simple format 'dict.users.0.name'.
 
 ## Getting Started
 
 ### Installation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepfinder-1.4.1/setup.cfg` & `deepfinder-1.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepfinder
-version = 1.4.1
+version = 1.4.2
 author = Javier Parada
 author_email = javierparadadev@gmail.com
 description = Search attributes easily using dot paths. Within structures of type dictionary, list and embedded substructures with simple format 'dict.users.0.name'.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 platform = any
```

