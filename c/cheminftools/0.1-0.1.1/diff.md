# Comparing `tmp/cheminftools-0.1.tar.gz` & `tmp/cheminftools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheminftools-0.1.tar", last modified: Tue May 30 19:01:48 2023, max compression
+gzip compressed data, was "cheminftools-0.1.1.tar", last modified: Tue May 30 22:08:05 2023, max compression
```

## Comparing `cheminftools-0.1.tar` & `cheminftools-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:48.373197 cheminftools-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-05-30 19:01:48.373197 cheminftools-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-05-30 19:01:33.000000 cheminftools-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:48.373197 cheminftools-0.1/cheminftools/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 19:01:33.000000 cheminftools-0.1/cheminftools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:48.373197 cheminftools-0.1/cheminftools/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:33.000000 cheminftools-0.1/cheminftools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-30 19:01:33.000000 cheminftools-0.1/cheminftools/tools/featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-05-30 19:01:33.000000 cheminftools-0.1/cheminftools/tools/sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-30 19:01:33.000000 cheminftools-0.1/cheminftools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:48.373197 cheminftools-0.1/cheminftools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-05-30 19:01:48.000000 cheminftools-0.1/cheminftools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-30 19:01:48.000000 cheminftools-0.1/cheminftools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:01:48.000000 cheminftools-0.1/cheminftools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:01:48.000000 cheminftools-0.1/cheminftools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 19:01:48.000000 cheminftools-0.1/cheminftools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 19:01:48.000000 cheminftools-0.1/cheminftools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:01:48.373197 cheminftools-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-30 19:01:33.000000 cheminftools-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:05.921996 cheminftools-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-30 22:08:05.921996 cheminftools-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-30 22:07:44.000000 cheminftools-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:05.917996 cheminftools-0.1.1/cheminftools/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:05.921996 cheminftools-0.1.1/cheminftools/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/tools/featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/tools/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/tools/sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-30 22:07:44.000000 cheminftools-0.1.1/cheminftools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:08:05.917996 cheminftools-0.1.1/cheminftools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 22:08:05.000000 cheminftools-0.1.1/cheminftools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:08:05.921996 cheminftools-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-30 22:07:44.000000 cheminftools-0.1.1/setup.py
```

### Comparing `cheminftools-0.1/PKG-INFO` & `cheminftools-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheminftools
-Version: 0.1
+Version: 0.1.1
 Summary: A collection of tools for daily cheminformatics tasks.
 Home-page: https://github.com/marcossantanaioc/cheminftools
 Author: marcossantanaioc
 Author-email: marcosvssantana@gmail.com
 License: Apache Software License 2.0
 Keywords: cheminformatics computational chemistry rdkit
 Classifier: Development Status :: 4 - Beta
@@ -13,20 +13,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-chemtools
+cheminftools
 ================
 
 ## Installation
 
-pip install git+https://github.com/marcossantanaioc/chemtools.git
+> From GitHub repo:
+    ```pip install git+https://github.com/marcossantanaioc/cheminftools.git```
+
+> From PyPi:
+    ```pip install cheminftools```
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## How to use
 
 Chemtools offer a collection of cheminformatics scripts for daily tasks.
@@ -55,15 +59,15 @@
 ``` python
 data = pd.read_csv('../data/example_data.csv')
 ```
 
 # Sanitizing
 
 The
-[`MolCleaner`](https://marcossantanaioc.github.io/chemtools/sanitizer.html#molcleaner)
+[`MolCleaner`](https://marcossantanaioc.github.io/cheminftools/sanitizer.html#molcleaner)
 class performs sanitization tasks, including:
 
         1. Standardize unknown stereochemistry (Handled by the RDKit Mol file parser)
             i) Fix wiggly bonds on sp3 carbons - sets atoms and bonds marked as unknown stereo to no stereo
             ii) Fix wiggly bonds on double bonds – set double bond to crossed bond
         2. Clears S Group data from the mol file
         3. Kekulize the structure
```

### Comparing `cheminftools-0.1/README.md` & `cheminftools-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-chemtools
+cheminftools
 ================
 
 ## Installation
 
-pip install git+https://github.com/marcossantanaioc/chemtools.git
+> From GitHub repo:
+    ```pip install git+https://github.com/marcossantanaioc/cheminftools.git```
+
+> From PyPi:
+    ```pip install cheminftools```
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## How to use
 
 Chemtools offer a collection of cheminformatics scripts for daily tasks.
@@ -36,15 +40,15 @@
 ``` python
 data = pd.read_csv('../data/example_data.csv')
 ```
 
 # Sanitizing
 
 The
-[`MolCleaner`](https://marcossantanaioc.github.io/chemtools/sanitizer.html#molcleaner)
+[`MolCleaner`](https://marcossantanaioc.github.io/cheminftools/sanitizer.html#molcleaner)
 class performs sanitization tasks, including:
 
         1. Standardize unknown stereochemistry (Handled by the RDKit Mol file parser)
             i) Fix wiggly bonds on sp3 carbons - sets atoms and bonds marked as unknown stereo to no stereo
             ii) Fix wiggly bonds on double bonds – set double bond to crossed bond
         2. Clears S Group data from the mol file
         3. Kekulize the structure
```

### Comparing `cheminftools-0.1/cheminftools/tools/featurizer.py` & `cheminftools-0.1.1/cheminftools/tools/featurizer.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1/cheminftools/tools/sanitizer.py` & `cheminftools-0.1.1/cheminftools/tools/sanitizer.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1/cheminftools/utils.py` & `cheminftools-0.1.1/cheminftools/utils.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1/cheminftools.egg-info/PKG-INFO` & `cheminftools-0.1.1/cheminftools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheminftools
-Version: 0.1
+Version: 0.1.1
 Summary: A collection of tools for daily cheminformatics tasks.
 Home-page: https://github.com/marcossantanaioc/cheminftools
 Author: marcossantanaioc
 Author-email: marcosvssantana@gmail.com
 License: Apache Software License 2.0
 Keywords: cheminformatics computational chemistry rdkit
 Classifier: Development Status :: 4 - Beta
@@ -13,20 +13,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-chemtools
+cheminftools
 ================
 
 ## Installation
 
-pip install git+https://github.com/marcossantanaioc/chemtools.git
+> From GitHub repo:
+    ```pip install git+https://github.com/marcossantanaioc/cheminftools.git```
+
+> From PyPi:
+    ```pip install cheminftools```
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## How to use
 
 Chemtools offer a collection of cheminformatics scripts for daily tasks.
@@ -55,15 +59,15 @@
 ``` python
 data = pd.read_csv('../data/example_data.csv')
 ```
 
 # Sanitizing
 
 The
-[`MolCleaner`](https://marcossantanaioc.github.io/chemtools/sanitizer.html#molcleaner)
+[`MolCleaner`](https://marcossantanaioc.github.io/cheminftools/sanitizer.html#molcleaner)
 class performs sanitization tasks, including:
 
         1. Standardize unknown stereochemistry (Handled by the RDKit Mol file parser)
             i) Fix wiggly bonds on sp3 carbons - sets atoms and bonds marked as unknown stereo to no stereo
             ii) Fix wiggly bonds on double bonds – set double bond to crossed bond
         2. Clears S Group data from the mol file
         3. Kekulize the structure
```

### Comparing `cheminftools-0.1/setup.py` & `cheminftools-0.1.1/setup.py`

 * *Files identical despite different names*

