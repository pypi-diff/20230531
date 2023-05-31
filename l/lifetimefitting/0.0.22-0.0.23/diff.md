# Comparing `tmp/lifetimefitting-0.0.22.tar.gz` & `tmp/lifetimefitting-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.22.tar", last modified: Wed May 31 01:04:28 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.23.tar", last modified: Wed May 31 05:25:42 2023, max compression
```

## Comparing `lifetimefitting-0.0.22.tar` & `lifetimefitting-0.0.23.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/app/lifetimefitting/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/funcs/expFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/funcs/fittingFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/app/lifetimefitting/funcs/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 01:04:28.000000 lifetimefitting-0.0.22/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:04:28.963254 lifetimefitting-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-31 01:04:18.000000 lifetimefitting-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.775295 lifetimefitting-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 05:25:42.775295 lifetimefitting-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.771295 lifetimefitting-0.0.23/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.771295 lifetimefitting-0.0.23/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.775295 lifetimefitting-0.0.23/app/lifetimefitting/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/funcs/expFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/funcs/fittingFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/funcs/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.771295 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 05:25:42.775295 lifetimefitting-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/setup.py
```

### Comparing `lifetimefitting-0.0.22/LICENSE.md` & `lifetimefitting-0.0.23/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.22/PKG-INFO` & `lifetimefitting-0.0.23/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.22
+Version: 0.0.23
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.22/README.md` & `lifetimefitting-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.22/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.23/app/lifetimefitting/__main__.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.22/app/lifetimefitting/funcs/expFuncs.py` & `lifetimefitting-0.0.23/app/lifetimefitting/funcs/expFuncs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.22/app/lifetimefitting/funcs/fittingFuncs.py` & `lifetimefitting-0.0.23/app/lifetimefitting/funcs/fittingFuncs.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 
 
 def loadAndCull(fc: QLineEdit, ui: Ui_Form):
     loaded = False
     x = y = []
 
     if fc.text() == '':
-        QMessageBox(icon=QMessageBox.Critical, text='TRF or IRF not loaded!').exec_()
+        QMessageBox(icon=QMessageBox.Icon.Critical, text='TRF or IRF not loaded!').exec()
     else:
         filename = fc.text().split("/")[-1].split("\\")[-1]
         try:
             trf = TRF(fc.text())
             y = trf.y
             x = trf.x
             ui.binSize_widg.setValue(trf.Resolution_int)
             loaded = True
         except struct.error:
-            QMessageBox(icon=QMessageBox.Critical, text=f'There was a problem reading {filename}').exec_()
+            QMessageBox(icon=QMessageBox.Icon.Critical, text=f'There was a problem reading {filename}').exec()
         except UnboundLocalError:
-            QMessageBox(icon=QMessageBox.Critical, text=f'There was a problem reading {filename}').exec_()
+            QMessageBox(icon=QMessageBox.Icon.Critical, text=f'There was a problem reading {filename}').exec()
 
     return x, y, loaded
 
 def fitLifetime(ui, x, y, maxIter):
     global FLFuncList
     global FLLinFuncList
     expCount = ui.expCount_widg.value()
@@ -122,15 +122,15 @@
     x_raw = np.subtract(x_raw, (x_start * binSize) / 1000)
     x = x_raw[x_start:]
     y = y_raw[x_start:]
 
     try:
         index = np.argmin(np.abs(np.array(x)-ui.maxTime_widg.value()))
     except ValueError:
-        QMessageBox(icon=QMessageBox.Critical, text=f'The chosen start offset of {ui.startOffset_widg.value()} was too large for the data').exec_()
+        QMessageBox(icon=QMessageBox.Icon.Critical, text=f'The chosen start offset of {ui.startOffset_widg.value()} was too large for the data').exec()
         return
 
     cutoff = x[index]
     x = x[:index]
     y = y[:index]
 
     if plot:
```

### Comparing `lifetimefitting-0.0.22/app/lifetimefitting/funcs/gui.py` & `lifetimefitting-0.0.23/app/lifetimefitting/funcs/gui.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.22/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.23/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.22
+Version: 0.0.23
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.22/setup.py` & `lifetimefitting-0.0.23/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.22",
+    version = "0.0.23",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

