# Comparing `tmp/cheminftools-0.1.1.tar.gz` & `tmp/cheminftools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheminftools-0.1.1.tar", last modified: Tue May 30 22:08:05 2023, max compression
+gzip compressed data, was "cheminftools-0.1.2.tar", last modified: Tue May 30 22:14:57 2023, max compression
```

## Comparing `cheminftools-0.1.1.tar` & `cheminftools-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:05.921996 cheminftools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-30 22:08:05.921996 cheminftools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-30 22:07:44.000000 cheminftools-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:05.917996 cheminftools-0.1.1/cheminftools/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:05.921996 cheminftools-0.1.1/cheminftools/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/tools/featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/tools/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/tools/sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:05.917996 cheminftools-0.1.1/cheminftools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:08:05.921996 cheminftools-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-30 22:07:44.000000 cheminftools-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:57.882634 cheminftools-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-30 22:14:57.882634 cheminftools-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-30 22:14:40.000000 cheminftools-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:57.878634 cheminftools-0.1.2/cheminftools/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:57.882634 cheminftools-0.1.2/cheminftools/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/tools/featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/tools/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/tools/sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-30 22:14:40.000000 cheminftools-0.1.2/cheminftools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:14:57.882634 cheminftools-0.1.2/cheminftools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 22:14:57.000000 cheminftools-0.1.2/cheminftools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:14:57.882634 cheminftools-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-30 22:14:40.000000 cheminftools-0.1.2/setup.py
```

### Comparing `cheminftools-0.1.1/PKG-INFO` & `cheminftools-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheminftools
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of tools for daily cheminformatics tasks.
 Home-page: https://github.com/marcossantanaioc/cheminftools
 Author: marcossantanaioc
 Author-email: marcosvssantana@gmail.com
 License: Apache Software License 2.0
 Keywords: cheminformatics computational chemistry rdkit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cheminftools-0.1.1/README.md` & `cheminftools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1.1/cheminftools/tools/featurizer.py` & `cheminftools-0.1.2/cheminftools/tools/featurizer.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1.1/cheminftools/tools/filtering.py` & `cheminftools-0.1.2/cheminftools/tools/filtering.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1.1/cheminftools/tools/sanitizer.py` & `cheminftools-0.1.2/cheminftools/tools/sanitizer.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1.1/cheminftools/utils.py` & `cheminftools-0.1.2/cheminftools/utils.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1.1/cheminftools.egg-info/PKG-INFO` & `cheminftools-0.1.2/cheminftools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheminftools
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of tools for daily cheminformatics tasks.
 Home-page: https://github.com/marcossantanaioc/cheminftools
 Author: marcossantanaioc
 Author-email: marcosvssantana@gmail.com
 License: Apache Software License 2.0
 Keywords: cheminformatics computational chemistry rdkit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cheminftools-0.1.1/setup.py` & `cheminftools-0.1.2/setup.py`

 * *Files identical despite different names*

