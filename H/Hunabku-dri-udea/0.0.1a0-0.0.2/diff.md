# Comparing `tmp/Hunabku_dri_udea-0.0.1a0.tar.gz` & `tmp/Hunabku_dri_udea-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_dri_udea-0.0.1a0.tar", last modified: Fri May 26 20:47:05 2023, max compression
+gzip compressed data, was "Hunabku_dri_udea-0.0.2.tar", last modified: Tue May 30 21:55:47 2023, max compression
```

## Comparing `Hunabku_dri_udea-0.0.1a0.tar` & `Hunabku_dri_udea-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:47:05.958524 Hunabku_dri_udea-0.0.1a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:47:05.958524 Hunabku_dri_udea-0.0.1a0/Hunabku_dri_udea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-26 20:47:05.000000 Hunabku_dri_udea-0.0.1a0/Hunabku_dri_udea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-26 20:47:05.000000 Hunabku_dri_udea-0.0.1a0/Hunabku_dri_udea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:47:05.000000 Hunabku_dri_udea-0.0.1a0/Hunabku_dri_udea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:47:05.000000 Hunabku_dri_udea-0.0.1a0/Hunabku_dri_udea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 20:47:05.000000 Hunabku_dri_udea-0.0.1a0/Hunabku_dri_udea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 20:46:52.000000 Hunabku_dri_udea-0.0.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-26 20:47:05.958524 Hunabku_dri_udea-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-26 20:46:52.000000 Hunabku_dri_udea-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:47:05.958524 Hunabku_dri_udea-0.0.1a0/hunabku_dri_udea/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:46:52.000000 Hunabku_dri_udea-0.0.1a0/hunabku_dri_udea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 20:46:52.000000 Hunabku_dri_udea-0.0.1a0/hunabku_dri_udea/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:47:05.958524 Hunabku_dri_udea-0.0.1a0/hunabku_dri_udea/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-26 20:46:52.000000 Hunabku_dri_udea-0.0.1a0/hunabku_dri_udea/endpoints/dri_udea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:47:05.958524 Hunabku_dri_udea-0.0.1a0/hunabku_dri_udea/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-26 20:46:52.000000 Hunabku_dri_udea-0.0.1a0/hunabku_dri_udea/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:47:05.958524 Hunabku_dri_udea-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-26 20:46:52.000000 Hunabku_dri_udea-0.0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/endpoints/dri_udea.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/setup.py
```

### Comparing `Hunabku_dri_udea-0.0.1a0/Hunabku_dri_udea.egg-info/PKG-INFO` & `Hunabku_dri_udea-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Hunabku-dri-udea
-Version: 0.0.1a0
+Name: Hunabku_dri_udea
+Version: 0.0.2
 Summary: Hunabku plugin from the International Affairs Office of the university of Antioquia
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_dri_udea-0.0.1a0/PKG-INFO` & `Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Hunabku_dri_udea
-Version: 0.0.1a0
+Name: Hunabku-dri-udea
+Version: 0.0.2
 Summary: Hunabku plugin from the International Affairs Office of the university of Antioquia
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_dri_udea-0.0.1a0/hunabku_dri_udea/endpoints/dri_udea.py` & `Hunabku_dri_udea-0.0.2/hunabku_dri_udea/endpoints/dri_udea.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from hunabku.HunabkuBase import HunabkuPluginBase, endpoint
-from hunabku_dri_udea.utils.encoder import JsonEncoder
 from hunabku.Config import Config, Param
 from pymongo import MongoClient
 from flask import Response, request
 import csv
 
 
 class International(HunabkuPluginBase):
@@ -52,15 +51,15 @@
             return self.get_agreements_json()
         else:
             return self.badrequest_error()
 
     def get_agreements_json(self):
         data = list(self.agreements_collection.find())
         response = self.app.response_class(
-            response=self.json.dumps(data, cls=JsonEncoder),
+            response=self.json.dumps(data, default=str, ensure_ascii=False),
             status=200,
             mimetype='application/json'
         )
         return response
 
     def get_agreements_csv(self):
         data = list(self.agreements_collection.find())
@@ -110,15 +109,15 @@
             return self.get_mobility_json()
         else:
             return self.badrequest_error()
 
     def get_mobility_json(self):
         data = list(self.mobility_collection.find())
         response = self.app.response_class(
-            response=self.json.dumps(data, cls=JsonEncoder),
+            response=self.json.dumps(data, default=str, ensure_ascii=False),
             status=200,
             mimetype='application/json'
         )
         return response
 
     def get_mobility_csv(self):
         data = list(self.mobility_collection.find())
```

### Comparing `Hunabku_dri_udea-0.0.1a0/setup.py` & `Hunabku_dri_udea-0.0.2/setup.py`

 * *Files identical despite different names*

