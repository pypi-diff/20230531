# Comparing `tmp/ohmytmp-destination-0.0.1.tar.gz` & `tmp/ohmytmp-destination-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmytmp-destination-0.0.1.tar", last modified: Sun May 28 14:56:24 2023, max compression
+gzip compressed data, was "ohmytmp-destination-0.0.2.tar", last modified: Wed May 31 08:34:30 2023, max compression
```

## Comparing `ohmytmp-destination-0.0.1.tar` & `ohmytmp-destination-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 14:56:24.623858 ohmytmp-destination-0.0.1/
--rw-rw-rw-   0        0        0     1064 2023-05-28 14:27:34.000000 ohmytmp-destination-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1911 2023-05-28 14:56:24.623858 ohmytmp-destination-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-05-28 14:27:34.000000 ohmytmp-destination-0.0.1/README.md
--rw-rw-rw-   0        0        0      897 2023-05-28 14:38:34.000000 ohmytmp-destination-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 14:56:24.624858 ohmytmp-destination-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 14:56:24.607859 ohmytmp-destination-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 14:56:24.620858 ohmytmp-destination-0.0.1/src/ohmytmp_destination.egg-info/
--rw-rw-rw-   0        0        0     1911 2023-05-28 14:56:24.000000 ohmytmp-destination-0.0.1/src/ohmytmp_destination.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-05-28 14:56:24.000000 ohmytmp-destination-0.0.1/src/ohmytmp_destination.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 14:56:24.000000 ohmytmp-destination-0.0.1/src/ohmytmp_destination.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 14:56:24.000000 ohmytmp-destination-0.0.1/src/ohmytmp_destination.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 14:56:24.000000 ohmytmp-destination-0.0.1/src/ohmytmp_destination.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 14:56:24.608858 ohmytmp-destination-0.0.1/src/ohmytmp_plugins/
-drwxrwxrwx   0        0        0        0 2023-05-28 14:56:24.622856 ohmytmp-destination-0.0.1/src/ohmytmp_plugins/destination/
--rw-rw-rw-   0        0        0       61 2023-05-28 14:39:28.000000 ohmytmp-destination-0.0.1/src/ohmytmp_plugins/destination/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-05-28 14:30:01.000000 ohmytmp-destination-0.0.1/src/ohmytmp_plugins/destination/dst.py
+drwxrwxrwx   0        0        0        0 2023-05-31 08:34:30.282787 ohmytmp-destination-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-05-28 14:27:34.000000 ohmytmp-destination-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2013 2023-05-31 08:34:30.281788 ohmytmp-destination-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-05-28 15:07:15.000000 ohmytmp-destination-0.0.2/README.md
+-rw-rw-rw-   0        0        0      904 2023-05-31 08:16:01.000000 ohmytmp-destination-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 08:34:30.282787 ohmytmp-destination-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 08:34:30.262787 ohmytmp-destination-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 08:34:30.278788 ohmytmp-destination-0.0.2/src/ohmytmp_destination.egg-info/
+-rw-rw-rw-   0        0        0     2013 2023-05-31 08:34:30.000000 ohmytmp-destination-0.0.2/src/ohmytmp_destination.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-05-31 08:34:30.000000 ohmytmp-destination-0.0.2/src/ohmytmp_destination.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 08:34:30.000000 ohmytmp-destination-0.0.2/src/ohmytmp_destination.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 08:34:30.000000 ohmytmp-destination-0.0.2/src/ohmytmp_destination.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-31 08:34:30.000000 ohmytmp-destination-0.0.2/src/ohmytmp_destination.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 08:34:30.262787 ohmytmp-destination-0.0.2/src/ohmytmp_plugins/
+drwxrwxrwx   0        0        0        0 2023-05-31 08:34:30.280788 ohmytmp-destination-0.0.2/src/ohmytmp_plugins/destination/
+-rw-rw-rw-   0        0        0       47 2023-05-31 08:03:30.000000 ohmytmp-destination-0.0.2/src/ohmytmp_plugins/destination/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-05-31 08:31:52.000000 ohmytmp-destination-0.0.2/src/ohmytmp_plugins/destination/dst.py
```

### Comparing `ohmytmp-destination-0.0.1/LICENSE` & `ohmytmp-destination-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmytmp-destination-0.0.1/PKG-INFO` & `ohmytmp-destination-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp-destination
-Version: 0.0.1
+Version: 0.0.2
 Summary: ohmytmp plugin destination
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
         
@@ -33,7 +33,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # plugin-destination
+
+```sh
+pip install ohmytmp-destination
+```
+
+```py
+from ohmytmp_plugins import destination
+```
```

### Comparing `ohmytmp-destination-0.0.1/pyproject.toml` & `ohmytmp-destination-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ohmytmp-destination"
-version = "0.0.1"
+version = "0.0.2"
 description = "ohmytmp plugin destination"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["ohmytmp"]
 
 authors = [
@@ -16,15 +16,15 @@
 
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3"
 ]
 
 dependencies = [
-  "ohmytmp",
+  "ohmytmp>=0.0.7",
 ]
 
 [tool.poetry]
 packages = [
     { include = "ohmytmp_plugins.destination" },
 ]
```

### Comparing `ohmytmp-destination-0.0.1/src/ohmytmp_destination.egg-info/PKG-INFO` & `ohmytmp-destination-0.0.2/src/ohmytmp_destination.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp-destination
-Version: 0.0.1
+Version: 0.0.2
 Summary: ohmytmp plugin destination
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
         
@@ -33,7 +33,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # plugin-destination
+
+```sh
+pip install ohmytmp-destination
+```
+
+```py
+from ohmytmp_plugins import destination
+```
```

