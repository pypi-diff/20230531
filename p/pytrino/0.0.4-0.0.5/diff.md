# Comparing `tmp/pytrino-0.0.4.tar.gz` & `tmp/pytrino-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrino-0.0.4.tar", last modified: Wed May 31 09:38:18 2023, max compression
+gzip compressed data, was "pytrino-0.0.5.tar", last modified: Wed May 31 09:43:53 2023, max compression
```

## Comparing `pytrino-0.0.4.tar` & `pytrino-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 09:38:18.081068 pytrino-0.0.4/
--rw-rw-rw-   0        0        0     2015 2023-05-31 09:38:18.080082 pytrino-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1442 2023-05-31 07:31:44.000000 pytrino-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 09:38:18.053095 pytrino-0.0.4/pytrino/
--rw-rw-rw-   0        0        0      147 2023-05-31 06:48:09.000000 pytrino-0.0.4/pytrino/__init__.py
--rw-rw-rw-   0        0        0     8097 2023-05-31 09:36:02.000000 pytrino-0.0.4/pytrino/oscprobs.py
--rw-rw-rw-   0        0        0      701 2023-05-16 05:03:51.000000 pytrino-0.0.4/pytrino/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:38:18.078086 pytrino-0.0.4/pytrino.egg-info/
--rw-rw-rw-   0        0        0     2015 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 09:38:18.082068 pytrino-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-05-31 09:37:04.000000 pytrino-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:43:53.475975 pytrino-0.0.5/
+-rw-rw-rw-   0        0        0     2015 2023-05-31 09:43:53.474976 pytrino-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1442 2023-05-31 07:31:44.000000 pytrino-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 09:43:53.457000 pytrino-0.0.5/pytrino/
+-rw-rw-rw-   0        0        0      147 2023-05-31 06:48:09.000000 pytrino-0.0.5/pytrino/__init__.py
+-rw-rw-rw-   0        0        0     8097 2023-05-31 09:43:32.000000 pytrino-0.0.5/pytrino/oscprobs.py
+-rw-rw-rw-   0        0        0      701 2023-05-16 05:03:51.000000 pytrino-0.0.5/pytrino/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:43:53.472976 pytrino-0.0.5/pytrino.egg-info/
+-rw-rw-rw-   0        0        0     2015 2023-05-31 09:43:53.000000 pytrino-0.0.5/pytrino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-31 09:43:53.000000 pytrino-0.0.5/pytrino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 09:43:53.000000 pytrino-0.0.5/pytrino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 09:43:53.000000 pytrino-0.0.5/pytrino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 09:43:53.000000 pytrino-0.0.5/pytrino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 09:43:53.475975 pytrino-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-05-31 09:43:35.000000 pytrino-0.0.5/setup.py
```

### Comparing `pytrino-0.0.4/PKG-INFO` & `pytrino-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrino
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pytrino: A new way to numerically compute neutrino oscillations
 Author: Baalateja Kataru
 Author-email: <kavesbteja@gmail.com>
 Keywords: probability,neutrino,oscillations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pytrino-0.0.4/README.md` & `pytrino-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pytrino-0.0.4/pytrino/oscprobs.py` & `pytrino-0.0.5/pytrino/oscprobs.py`

 * *Files identical despite different names*

### Comparing `pytrino-0.0.4/pytrino/utils.py` & `pytrino-0.0.5/pytrino/utils.py`

 * *Files identical despite different names*

### Comparing `pytrino-0.0.4/pytrino.egg-info/PKG-INFO` & `pytrino-0.0.5/pytrino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrino
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pytrino: A new way to numerically compute neutrino oscillations
 Author: Baalateja Kataru
 Author-email: <kavesbteja@gmail.com>
 Keywords: probability,neutrino,oscillations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pytrino-0.0.4/setup.py` & `pytrino-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Pytrino: A new way to numerically compute neutrino oscillations'
 
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
         name="pytrino",
```

