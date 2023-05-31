# Comparing `tmp/lifetimefitting-0.0.21.tar.gz` & `tmp/lifetimefitting-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.21.tar", last modified: Wed May 31 01:00:00 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.22.tar", last modified: Wed May 31 01:04:28 2023, max compression
```

## Comparing `lifetimefitting-0.0.21.tar` & `lifetimefitting-0.0.22.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.214952 lifetimefitting-0.0.21/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.214952 lifetimefitting-0.0.21/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/app/lifetimefitting/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/funcs/expFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/funcs/fittingFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/funcs/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/app/lifetimefitting/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/funcs/expFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/funcs/fittingFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/funcs/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/setup.py
```

### Comparing `lifetimefitting-0.0.21/LICENSE.md` & `lifetimefitting-0.0.22/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.21/PKG-INFO` & `lifetimefitting-0.0.22/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.21
+Version: 0.0.22
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.21/README.md` & `lifetimefitting-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.21/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.22/app/lifetimefitting/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import matplotlib.pyplot as plt
 from PyQt6 import QtWidgets
 from PyQt6.QtWidgets import QFileDialog
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 from phdimporter import TRF
-from funcs.gui import Ui_Form
-from funcs.fittingFuncs import loadAndCull, fitFL
+from .funcs.gui import Ui_Form
+from .funcs.fittingFuncs import loadAndCull, fitFL
 import sys
 
 def plotFL():
     global csv
     plt.close('all')
     for i in ui.axList:
         i.remove()
```

### Comparing `lifetimefitting-0.0.21/app/lifetimefitting/funcs/expFuncs.py` & `lifetimefitting-0.0.22/app/lifetimefitting/funcs/expFuncs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.21/app/lifetimefitting/funcs/fittingFuncs.py` & `lifetimefitting-0.0.22/app/lifetimefitting/funcs/fittingFuncs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.21/app/lifetimefitting/funcs/gui.py` & `lifetimefitting-0.0.22/app/lifetimefitting/funcs/gui.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.21/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.22/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.21
+Version: 0.0.22
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.21/setup.py` & `lifetimefitting-0.0.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.21",
+    version = "0.0.22",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

