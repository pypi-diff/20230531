# Comparing `tmp/ts2ml-0.0.1.tar.gz` & `tmp/ts2ml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts2ml-0.0.1.tar", last modified: Tue May 30 23:14:41 2023, max compression
+gzip compressed data, was "ts2ml-0.0.2.tar", last modified: Tue May 30 23:31:46 2023, max compression
```

## Comparing `ts2ml-0.0.1.tar` & `ts2ml-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-30 23:14:41.424625 ts2ml-0.0.1/
--rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ts2ml-0.0.1/LICENSE
--rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ts2ml-0.0.1/MANIFEST.in
--rw-r--r--   0 joaonogueira   (501) staff       (20)     3231 2023-05-30 23:14:41.424477 ts2ml-0.0.1/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)     2483 2023-05-30 22:47:57.000000 ts2ml-0.0.1/README.md
--rw-r--r--   0 joaonogueira   (501) staff       (20)     1013 2023-05-30 23:14:27.000000 ts2ml-0.0.1/settings.ini
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-30 23:14:41.424672 ts2ml-0.0.1/setup.cfg
--rw-rw-r--   0 joaonogueira   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ts2ml-0.0.1/setup.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-30 23:14:41.423873 ts2ml-0.0.1/ts2ml.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)     3231 2023-05-30 23:14:41.000000 ts2ml-0.0.1/ts2ml.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      301 2023-05-30 23:14:41.000000 ts2ml-0.0.1/ts2ml.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-30 23:14:41.000000 ts2ml-0.0.1/ts2ml.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       51 2023-05-30 23:14:41.000000 ts2ml-0.0.1/ts2ml.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-30 23:14:41.000000 ts2ml-0.0.1/ts2ml.egg-info/not-zip-safe
--rw-r--r--   0 joaonogueira   (501) staff       (20)       36 2023-05-30 23:14:41.000000 ts2ml-0.0.1/ts2ml.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        5 2023-05-30 23:14:41.000000 ts2ml-0.0.1/ts2ml.egg-info/top_level.txt
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-30 23:14:41.424275 ts2ml-0.0.1/tsml/
--rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-05-30 23:14:35.000000 ts2ml-0.0.1/tsml/__init__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      381 2023-05-30 23:14:35.000000 ts2ml-0.0.1/tsml/_modidx.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     2207 2023-05-30 23:14:35.000000 ts2ml-0.0.1/tsml/core.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-30 23:31:46.884358 ts2ml-0.0.2/
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ts2ml-0.0.2/LICENSE
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ts2ml-0.0.2/MANIFEST.in
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     3235 2023-05-30 23:31:46.884211 ts2ml-0.0.2/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     2486 2023-05-30 23:18:58.000000 ts2ml-0.0.2/README.md
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      911 2023-05-30 23:31:28.000000 ts2ml-0.0.2/settings.ini
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-30 23:31:46.884416 ts2ml-0.0.2/setup.cfg
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ts2ml-0.0.2/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-30 23:31:46.883091 ts2ml-0.0.2/ts2ml/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-05-30 23:27:47.000000 ts2ml-0.0.2/ts2ml/__init__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      387 2023-05-30 23:27:47.000000 ts2ml-0.0.2/ts2ml/_modidx.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     2207 2023-05-30 23:27:47.000000 ts2ml-0.0.2/ts2ml/core.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-30 23:31:46.884015 ts2ml-0.0.2/ts2ml.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     3235 2023-05-30 23:31:46.000000 ts2ml-0.0.2/ts2ml.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      304 2023-05-30 23:31:46.000000 ts2ml-0.0.2/ts2ml.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-30 23:31:46.000000 ts2ml-0.0.2/ts2ml.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       53 2023-05-30 23:31:46.000000 ts2ml-0.0.2/ts2ml.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-30 23:14:41.000000 ts2ml-0.0.2/ts2ml.egg-info/not-zip-safe
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       36 2023-05-30 23:31:46.000000 ts2ml-0.0.2/ts2ml.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        6 2023-05-30 23:31:46.000000 ts2ml-0.0.2/ts2ml.egg-info/top_level.txt
```

### Comparing `ts2ml-0.0.1/LICENSE` & `ts2ml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ts2ml-0.0.1/PKG-INFO` & `ts2ml-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ts2ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tools to Transform a Time Series into Features and Target a.k.a Supervised Learning
-Home-page: https://github.com/joaopcnogueira/tsml
+Home-page: https://github.com/joaopcnogueira/ts2ml
 Author: João Nogueira
 Author-email: joaopcnogueira@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,29 +15,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# tsml
+# ts2ml
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
 ``` sh
-pip install tsml
+pip install ts2ml
 ```
 
 ## How to use
 
 ``` python
 import pandas as pd
-from tsml.core import add_missing_slots
+from ts2ml.core import add_missing_slots
 ```
 
 ``` python
 df = pd.DataFrame({
     'pickup_hour': ['2022-01-01 00:00:00', '2022-01-01 01:00:00', '2022-01-01 03:00:00', '2022-01-01 01:00:00', '2022-01-01 02:00:00', '2022-01-01 05:00:00'],
     'pickup_location_id': [1, 1, 1, 2, 2, 2],
     'rides': [2, 3, 1, 1, 2, 1]
```

### Comparing `ts2ml-0.0.1/README.md` & `ts2ml-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# tsml
+# ts2ml
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
 ``` sh
-pip install tsml
+pip install ts2ml
 ```
 
 ## How to use
 
 ``` python
 import pandas as pd
-from tsml.core import add_missing_slots
+from ts2ml.core import add_missing_slots
 ```
 
 ``` python
 df = pd.DataFrame({
     'pickup_hour': ['2022-01-01 00:00:00', '2022-01-01 01:00:00', '2022-01-01 03:00:00', '2022-01-01 01:00:00', '2022-01-01 02:00:00', '2022-01-01 05:00:00'],
     'pickup_location_id': [1, 1, 1, 2, 2, 2],
     'rides': [2, 3, 1, 1, 2, 1]
```

### Comparing `ts2ml-0.0.1/setup.py` & `ts2ml-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `ts2ml-0.0.1/ts2ml.egg-info/PKG-INFO` & `ts2ml-0.0.2/ts2ml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ts2ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tools to Transform a Time Series into Features and Target a.k.a Supervised Learning
-Home-page: https://github.com/joaopcnogueira/tsml
+Home-page: https://github.com/joaopcnogueira/ts2ml
 Author: João Nogueira
 Author-email: joaopcnogueira@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,29 +15,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# tsml
+# ts2ml
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
 ``` sh
-pip install tsml
+pip install ts2ml
 ```
 
 ## How to use
 
 ``` python
 import pandas as pd
-from tsml.core import add_missing_slots
+from ts2ml.core import add_missing_slots
 ```
 
 ``` python
 df = pd.DataFrame({
     'pickup_hour': ['2022-01-01 00:00:00', '2022-01-01 01:00:00', '2022-01-01 03:00:00', '2022-01-01 01:00:00', '2022-01-01 02:00:00', '2022-01-01 05:00:00'],
     'pickup_location_id': [1, 1, 1, 2, 2, 2],
     'rides': [2, 3, 1, 1, 2, 1]
```

### Comparing `ts2ml-0.0.1/tsml/core.py` & `ts2ml-0.0.2/ts2ml/core.py`

 * *Files identical despite different names*

