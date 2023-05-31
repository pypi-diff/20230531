# Comparing `tmp/bp_data_grid-1.0.6.tar.gz` & `tmp/bp_data_grid-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_grid-1.0.6.tar", last modified: Wed May 31 03:41:17 2023, max compression
+gzip compressed data, was "bp_data_grid-1.0.7.tar", last modified: Wed May 31 03:58:00 2023, max compression
```

## Comparing `bp_data_grid-1.0.6.tar` & `bp_data_grid-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 03:41:17.511385 bp_data_grid-1.0.6/
--rw-rw-rw-   0        0        0     1082 2023-04-27 12:37:21.000000 bp_data_grid-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       45 2023-04-27 12:37:21.000000 bp_data_grid-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4018 2023-05-31 03:41:17.509414 bp_data_grid-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2907 2023-05-09 08:44:53.000000 bp_data_grid-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 03:41:17.475603 bp_data_grid-1.0.6/bp_data_grid.egg-info/
--rw-rw-rw-   0        0        0     4018 2023-05-31 03:41:17.000000 bp_data_grid-1.0.6/bp_data_grid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-31 03:41:17.000000 bp_data_grid-1.0.6/bp_data_grid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 03:41:17.000000 bp_data_grid-1.0.6/bp_data_grid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-31 03:41:17.000000 bp_data_grid-1.0.6/bp_data_grid.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-31 03:41:17.000000 bp_data_grid-1.0.6/bp_data_grid.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 03:41:17.498271 bp_data_grid-1.0.6/data_grid/
--rw-rw-rw-   0        0        0     2175 2023-04-27 12:37:21.000000 bp_data_grid-1.0.6/data_grid/__init__.py
--rw-rw-rw-   0        0        0     2206 2023-04-27 12:37:21.000000 bp_data_grid-1.0.6/data_grid/register.py
--rw-rw-rw-   0        0        0       42 2023-05-31 03:41:17.512463 bp_data_grid-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-05-31 03:40:56.000000 bp_data_grid-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 03:58:00.030973 bp_data_grid-1.0.7/
+-rw-rw-rw-   0        0        0     1082 2023-04-27 12:37:21.000000 bp_data_grid-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-04-27 12:37:21.000000 bp_data_grid-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4018 2023-05-31 03:58:00.026285 bp_data_grid-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2907 2023-05-09 08:44:53.000000 bp_data_grid-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 03:57:59.818725 bp_data_grid-1.0.7/bp_data_grid.egg-info/
+-rw-rw-rw-   0        0        0     4018 2023-05-31 03:57:59.000000 bp_data_grid-1.0.7/bp_data_grid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-05-31 03:57:59.000000 bp_data_grid-1.0.7/bp_data_grid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 03:57:59.000000 bp_data_grid-1.0.7/bp_data_grid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-31 03:57:59.000000 bp_data_grid-1.0.7/bp_data_grid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-31 03:57:59.000000 bp_data_grid-1.0.7/bp_data_grid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 03:57:59.851725 bp_data_grid-1.0.7/data_grid/
+-rw-rw-rw-   0        0        0     2175 2023-04-27 12:37:21.000000 bp_data_grid-1.0.7/data_grid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 03:57:59.722417 bp_data_grid-1.0.7/data_grid/frontend/
+drwxrwxrwx   0        0        0        0 2023-05-31 03:57:59.873764 bp_data_grid-1.0.7/data_grid/frontend/dist/
+drwxrwxrwx   0        0        0        0 2023-05-31 03:57:59.990907 bp_data_grid-1.0.7/data_grid/frontend/dist/assets/
+-rw-rw-rw-   0        0        0   202328 2023-05-31 03:56:35.000000 bp_data_grid-1.0.7/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js
+-rw-rw-rw-   0        0        0  1581973 2023-05-31 03:56:35.000000 bp_data_grid-1.0.7/data_grid/frontend/dist/assets/index-015db93e.js
+-rw-rw-rw-   0        0        0      300 2023-05-31 03:56:35.000000 bp_data_grid-1.0.7/data_grid/frontend/dist/assets/index-d081bea5.css
+-rw-rw-rw-   0        0        0   149944 2023-05-31 03:56:35.000000 bp_data_grid-1.0.7/data_grid/frontend/dist/assets/index.es-f2cb0452-6fcc3449.js
+-rw-rw-rw-   0        0        0    21573 2023-05-31 03:56:35.000000 bp_data_grid-1.0.7/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js
+-rw-rw-rw-   0        0        0      570 2023-05-31 03:56:35.000000 bp_data_grid-1.0.7/data_grid/frontend/dist/index.html
+-rw-rw-rw-   0        0        0     1497 2023-04-27 12:37:21.000000 bp_data_grid-1.0.7/data_grid/frontend/dist/vite.svg
+-rw-rw-rw-   0        0        0     2206 2023-04-27 12:37:21.000000 bp_data_grid-1.0.7/data_grid/register.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 03:58:00.034480 bp_data_grid-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-05-31 03:57:53.000000 bp_data_grid-1.0.7/setup.py
```

### Comparing `bp_data_grid-1.0.6/LICENSE` & `bp_data_grid-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.6/PKG-INFO` & `bp_data_grid-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp_data_grid
-Version: 1.0.6
+Version: 1.0.7
 Summary: Show data in data grid
 Home-page: UNKNOWN
 Author: Bluepineapple
 Author-email: avinash@bluepineapple.io
 License: UNKNOWN
 Description: # Data Grid
```

### Comparing `bp_data_grid-1.0.6/README.md` & `bp_data_grid-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.6/bp_data_grid.egg-info/PKG-INFO` & `bp_data_grid-1.0.7/bp_data_grid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp-data-grid
-Version: 1.0.6
+Version: 1.0.7
 Summary: Show data in data grid
 Home-page: UNKNOWN
 Author: Bluepineapple
 Author-email: avinash@bluepineapple.io
 License: UNKNOWN
 Description: # Data Grid
```

### Comparing `bp_data_grid-1.0.6/data_grid/__init__.py` & `bp_data_grid-1.0.7/data_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.6/data_grid/register.py` & `bp_data_grid-1.0.7/data_grid/register.py`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.6/setup.py` & `bp_data_grid-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp_data_grid",
-    version="1.0.6",
+    version="1.0.7",
     author="Bluepineapple",
     author_email="avinash@bluepineapple.io",
     description="Show data in data grid",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

