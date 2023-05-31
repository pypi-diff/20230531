# Comparing `tmp/pytrino-0.0.1.tar.gz` & `tmp/pytrino-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrino-0.0.1.tar", last modified: Wed May 31 06:59:46 2023, max compression
+gzip compressed data, was "pytrino-0.0.2.tar", last modified: Wed May 31 07:32:31 2023, max compression
```

## Comparing `pytrino-0.0.1.tar` & `pytrino-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 06:59:46.064502 pytrino-0.0.1/
--rw-rw-rw-   0        0        0     2011 2023-05-31 06:59:46.063505 pytrino-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1438 2023-05-31 06:50:21.000000 pytrino-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 06:59:46.044509 pytrino-0.0.1/pytrino/
--rw-rw-rw-   0        0        0      147 2023-05-31 06:48:09.000000 pytrino-0.0.1/pytrino/__init__.py
--rw-rw-rw-   0        0        0    11382 2023-05-31 06:54:19.000000 pytrino-0.0.1/pytrino/oscprobs.py
--rw-rw-rw-   0        0        0      701 2023-05-16 05:03:51.000000 pytrino-0.0.1/pytrino/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:59:46.061504 pytrino-0.0.1/pytrino.egg-info/
--rw-rw-rw-   0        0        0     2011 2023-05-31 06:59:45.000000 pytrino-0.0.1/pytrino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-31 06:59:45.000000 pytrino-0.0.1/pytrino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 06:59:45.000000 pytrino-0.0.1/pytrino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-31 06:59:45.000000 pytrino-0.0.1/pytrino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 06:59:45.000000 pytrino-0.0.1/pytrino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 06:59:46.064502 pytrino-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-05-31 06:59:41.000000 pytrino-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:32:31.437487 pytrino-0.0.2/
+-rw-rw-rw-   0        0        0     2015 2023-05-31 07:32:31.436472 pytrino-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1442 2023-05-31 07:31:44.000000 pytrino-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 07:32:31.418478 pytrino-0.0.2/pytrino/
+-rw-rw-rw-   0        0        0      147 2023-05-31 06:48:09.000000 pytrino-0.0.2/pytrino/__init__.py
+-rw-rw-rw-   0        0        0    11382 2023-05-31 07:31:47.000000 pytrino-0.0.2/pytrino/oscprobs.py
+-rw-rw-rw-   0        0        0      701 2023-05-16 05:03:51.000000 pytrino-0.0.2/pytrino/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:32:31.434490 pytrino-0.0.2/pytrino.egg-info/
+-rw-rw-rw-   0        0        0     2015 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:32:31.437487 pytrino-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-05-31 07:32:22.000000 pytrino-0.0.2/setup.py
```

### Comparing `pytrino-0.0.1/PKG-INFO` & `pytrino-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pytrino
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pytrino: A new way to numerically compute neutrino oscillations
 Author: Baalateja Kataru
 Author-email: <kavesbteja@gmail.com>
 Keywords: probability,neutrino,oscillations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
-# Pytrino
+![](logo.png)
 
 We use the recently discovered Eigenvalue-Eigenvector and Adjugate Identities to compute oscillation probabilities with minimal algorithmic steps.
 
 # Usage
 
 
 ## Imports
```

### Comparing `pytrino-0.0.1/README.md` & `pytrino-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Pytrino
+![](logo.png)
 
 We use the recently discovered Eigenvalue-Eigenvector and Adjugate Identities to compute oscillation probabilities with minimal algorithmic steps.
 
 # Usage
 
 
 ## Imports
```

### Comparing `pytrino-0.0.1/pytrino/oscprobs.py` & `pytrino-0.0.2/pytrino/oscprobs.py`

 * *Files identical despite different names*

### Comparing `pytrino-0.0.1/pytrino/utils.py` & `pytrino-0.0.2/pytrino/utils.py`

 * *Files identical despite different names*

### Comparing `pytrino-0.0.1/pytrino.egg-info/PKG-INFO` & `pytrino-0.0.2/pytrino.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pytrino
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pytrino: A new way to numerically compute neutrino oscillations
 Author: Baalateja Kataru
 Author-email: <kavesbteja@gmail.com>
 Keywords: probability,neutrino,oscillations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
-# Pytrino
+![](logo.png)
 
 We use the recently discovered Eigenvalue-Eigenvector and Adjugate Identities to compute oscillation probabilities with minimal algorithmic steps.
 
 # Usage
 
 
 ## Imports
```

### Comparing `pytrino-0.0.1/setup.py` & `pytrino-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Pytrino: A new way to numerically compute neutrino oscillations'
 
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
         name="pytrino",
```

