# Comparing `tmp/bp_data_grid-1.0.4.tar.gz` & `tmp/bp_data_grid-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_grid-1.0.4.tar", last modified: Tue May 30 09:59:14 2023, max compression
+gzip compressed data, was "bp_data_grid-1.0.5.tar", last modified: Wed May 31 03:24:56 2023, max compression
```

## Comparing `bp_data_grid-1.0.4.tar` & `bp_data_grid-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:59:14.167108 bp_data_grid-1.0.4/
--rw-rw-rw-   0        0        0     1082 2023-04-27 12:37:21.000000 bp_data_grid-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       45 2023-04-27 12:37:21.000000 bp_data_grid-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4018 2023-05-30 09:59:14.159588 bp_data_grid-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2907 2023-05-09 08:44:53.000000 bp_data_grid-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 09:59:14.144593 bp_data_grid-1.0.4/bp_data_grid.egg-info/
--rw-rw-rw-   0        0        0     4018 2023-05-30 09:59:13.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-30 09:59:14.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:59:13.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-30 09:59:13.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 09:59:13.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 09:59:14.153971 bp_data_grid-1.0.4/data_grid/
--rw-rw-rw-   0        0        0     2175 2023-04-27 12:37:21.000000 bp_data_grid-1.0.4/data_grid/__init__.py
--rw-rw-rw-   0        0        0     2206 2023-04-27 12:37:21.000000 bp_data_grid-1.0.4/data_grid/register.py
--rw-rw-rw-   0        0        0       42 2023-05-30 09:59:14.169614 bp_data_grid-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-05-30 09:56:08.000000 bp_data_grid-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 03:24:56.398124 bp_data_grid-1.0.5/
+-rw-rw-rw-   0        0        0     1082 2023-04-27 12:37:21.000000 bp_data_grid-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-04-27 12:37:21.000000 bp_data_grid-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4018 2023-05-31 03:24:56.395377 bp_data_grid-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2907 2023-05-09 08:44:53.000000 bp_data_grid-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 03:24:56.348619 bp_data_grid-1.0.5/bp_data_grid.egg-info/
+-rw-rw-rw-   0        0        0     4018 2023-05-31 03:24:55.000000 bp_data_grid-1.0.5/bp_data_grid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-05-31 03:24:55.000000 bp_data_grid-1.0.5/bp_data_grid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 03:24:55.000000 bp_data_grid-1.0.5/bp_data_grid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-31 03:24:55.000000 bp_data_grid-1.0.5/bp_data_grid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-31 03:24:55.000000 bp_data_grid-1.0.5/bp_data_grid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 03:24:56.382036 bp_data_grid-1.0.5/data_grid/
+-rw-rw-rw-   0        0        0     2175 2023-04-27 12:37:21.000000 bp_data_grid-1.0.5/data_grid/__init__.py
+-rw-rw-rw-   0        0        0     2206 2023-04-27 12:37:21.000000 bp_data_grid-1.0.5/data_grid/register.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 03:24:56.399969 bp_data_grid-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-05-31 03:24:39.000000 bp_data_grid-1.0.5/setup.py
```

### Comparing `bp_data_grid-1.0.4/LICENSE` & `bp_data_grid-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.4/PKG-INFO` & `bp_data_grid-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp_data_grid
-Version: 1.0.4
+Version: 1.0.5
 Summary: Show data in data grid
 Home-page: UNKNOWN
 Author: Bluepineapple
 Author-email: avinash@bluepineapple.io
 License: UNKNOWN
 Description: # Data Grid
```

### Comparing `bp_data_grid-1.0.4/README.md` & `bp_data_grid-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.4/bp_data_grid.egg-info/PKG-INFO` & `bp_data_grid-1.0.5/bp_data_grid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp-data-grid
-Version: 1.0.4
+Version: 1.0.5
 Summary: Show data in data grid
 Home-page: UNKNOWN
 Author: Bluepineapple
 Author-email: avinash@bluepineapple.io
 License: UNKNOWN
 Description: # Data Grid
```

### Comparing `bp_data_grid-1.0.4/data_grid/__init__.py` & `bp_data_grid-1.0.5/data_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.4/data_grid/register.py` & `bp_data_grid-1.0.5/data_grid/register.py`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.4/setup.py` & `bp_data_grid-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp_data_grid",
-    version="1.0.4",
+    version="1.0.5",
     author="Bluepineapple",
     author_email="avinash@bluepineapple.io",
     description="Show data in data grid",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

