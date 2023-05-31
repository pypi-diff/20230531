# Comparing `tmp/jupyter2pytest-0.1.0.tar.gz` & `tmp/jupyter2pytest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter2pytest-0.1.0.tar", last modified: Fri May 26 19:15:48 2023, max compression
+gzip compressed data, was "jupyter2pytest-0.2.0.tar", last modified: Wed May 31 17:54:40 2023, max compression
```

## Comparing `jupyter2pytest-0.1.0.tar` & `jupyter2pytest-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-26 19:15:48.621498 jupyter2pytest-0.1.0/
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     1079 2023-05-26 15:14:26.000000 jupyter2pytest-0.1.0/LICENSE
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     2897 2023-05-26 19:15:48.621498 jupyter2pytest-0.1.0/PKG-INFO
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      913 2023-05-26 15:28:20.000000 jupyter2pytest-0.1.0/README.md
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      752 2023-05-26 15:14:57.000000 jupyter2pytest-0.1.0/pyproject.toml
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)       38 2023-05-26 19:15:48.621498 jupyter2pytest-0.1.0/setup.cfg
-drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-26 19:15:48.621498 jupyter2pytest-0.1.0/src/
-drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-26 19:15:48.621498 jupyter2pytest-0.1.0/src/jupyter2pytest/
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-25 18:18:40.000000 jupyter2pytest-0.1.0/src/jupyter2pytest/__init__.py
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      657 2023-05-26 02:58:02.000000 jupyter2pytest-0.1.0/src/jupyter2pytest/__main__.py
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     1609 2023-05-26 03:00:01.000000 jupyter2pytest-0.1.0/src/jupyter2pytest/compiler.py
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     2966 2023-05-25 18:45:32.000000 jupyter2pytest-0.1.0/src/jupyter2pytest/extractor.py
-drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-26 19:15:48.621498 jupyter2pytest-0.1.0/src/jupyter2pytest.egg-info/
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     2897 2023-05-26 19:15:48.000000 jupyter2pytest-0.1.0/src/jupyter2pytest.egg-info/PKG-INFO
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      366 2023-05-26 19:15:48.000000 jupyter2pytest-0.1.0/src/jupyter2pytest.egg-info/SOURCES.txt
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)        1 2023-05-26 19:15:48.000000 jupyter2pytest-0.1.0/src/jupyter2pytest.egg-info/dependency_links.txt
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)        9 2023-05-26 19:15:48.000000 jupyter2pytest-0.1.0/src/jupyter2pytest.egg-info/requires.txt
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)       15 2023-05-26 19:15:48.000000 jupyter2pytest-0.1.0/src/jupyter2pytest.egg-info/top_level.txt
+drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-31 17:54:40.584877 jupyter2pytest-0.2.0/
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     1079 2023-05-26 15:14:26.000000 jupyter2pytest-0.2.0/LICENSE
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     2897 2023-05-31 17:54:40.584877 jupyter2pytest-0.2.0/PKG-INFO
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      913 2023-05-26 15:28:20.000000 jupyter2pytest-0.2.0/README.md
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      752 2023-05-31 17:54:29.000000 jupyter2pytest-0.2.0/pyproject.toml
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)       38 2023-05-31 17:54:40.584877 jupyter2pytest-0.2.0/setup.cfg
+drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-31 17:54:40.581544 jupyter2pytest-0.2.0/src/
+drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-31 17:54:40.581544 jupyter2pytest-0.2.0/src/jupyter2pytest/
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-25 18:18:40.000000 jupyter2pytest-0.2.0/src/jupyter2pytest/__init__.py
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      489 2023-05-31 17:54:02.000000 jupyter2pytest-0.2.0/src/jupyter2pytest/__main__.py
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     3006 2023-05-31 17:54:02.000000 jupyter2pytest-0.2.0/src/jupyter2pytest/compiler.py
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     4371 2023-05-31 17:54:02.000000 jupyter2pytest-0.2.0/src/jupyter2pytest/extractor.py
+drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-31 17:54:40.584877 jupyter2pytest-0.2.0/src/jupyter2pytest.egg-info/
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     2897 2023-05-31 17:54:40.000000 jupyter2pytest-0.2.0/src/jupyter2pytest.egg-info/PKG-INFO
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      366 2023-05-31 17:54:40.000000 jupyter2pytest-0.2.0/src/jupyter2pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)        1 2023-05-31 17:54:40.000000 jupyter2pytest-0.2.0/src/jupyter2pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)        9 2023-05-31 17:54:40.000000 jupyter2pytest-0.2.0/src/jupyter2pytest.egg-info/requires.txt
+-rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)       15 2023-05-31 17:54:40.000000 jupyter2pytest-0.2.0/src/jupyter2pytest.egg-info/top_level.txt
```

### Comparing `jupyter2pytest-0.1.0/LICENSE` & `jupyter2pytest-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter2pytest-0.1.0/PKG-INFO` & `jupyter2pytest-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter2pytest
-Version: 0.1.0
+Version: 0.2.0
 Summary: Converts Jupyter notebooks into pytest capable test files.
 Author-email: Garrett Credi <garrettcredi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 University of Illinois
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jupyter2pytest-0.1.0/README.md` & `jupyter2pytest-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter2pytest-0.1.0/pyproject.toml` & `jupyter2pytest-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jupyter2pytest"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name = "Garrett Credi", email = "garrettcredi@gmail.com" }
 ]
 description = "Converts Jupyter notebooks into pytest capable test files."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `jupyter2pytest-0.1.0/src/jupyter2pytest.egg-info/PKG-INFO` & `jupyter2pytest-0.2.0/src/jupyter2pytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter2pytest
-Version: 0.1.0
+Version: 0.2.0
 Summary: Converts Jupyter notebooks into pytest capable test files.
 Author-email: Garrett Credi <garrettcredi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 University of Illinois
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

