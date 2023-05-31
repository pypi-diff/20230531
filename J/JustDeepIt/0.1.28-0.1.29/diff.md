# Comparing `tmp/JustDeepIt-0.1.28.tar.gz` & `tmp/JustDeepIt-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustDeepIt-0.1.28.tar", last modified: Fri Apr 21 02:33:07 2023, max compression
+gzip compressed data, was "JustDeepIt-0.1.29.tar", last modified: Wed May 31 04:20:12 2023, max compression
```

## Comparing `JustDeepIt-0.1.28.tar` & `JustDeepIt-0.1.29.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.964196 JustDeepIt-0.1.28/JustDeepIt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:33:07.000000 JustDeepIt-0.1.28/JustDeepIt.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.964196 JustDeepIt-0.1.28/justdeepit/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.964196 JustDeepIt-0.1.28/justdeepit/models/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13913 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/instance_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/object_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/salient_object_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.968196 JustDeepIt-0.1.28/justdeepit/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/detectron2base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/mmdetbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    36052 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/models/utils/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.960196 JustDeepIt-0.1.28/justdeepit/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.968196 JustDeepIt-0.1.28/justdeepit/src/font/
--rw-r--r--   0 runner    (1001) docker     (123)   555264 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/src/font/NotoSans-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/src/font/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    56340 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.972196 JustDeepIt-0.1.28/justdeepit/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/appbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/appis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/appod.py
--rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/appsod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/justdeepit/webapp/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/.Rhistory
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/jquery-3.6.0.min.map
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)    58702 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/tree.jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)   174878 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/tree.jquery.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    23347 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/static/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/justdeepit/webapp/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/templates/module.html
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/justdeepit/webapp/templates/shutdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 02:33:07.976196 JustDeepIt-0.1.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-21 02:30:46.000000 JustDeepIt-0.1.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.522696 JustDeepIt-0.1.29/JustDeepIt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:20:12.000000 JustDeepIt-0.1.29/JustDeepIt.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.522696 JustDeepIt-0.1.29/justdeepit/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.522696 JustDeepIt-0.1.29/justdeepit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13913 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/instance_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/object_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/salient_object_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.526696 JustDeepIt-0.1.29/justdeepit/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/detectron2base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/mmdetbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36052 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/models/utils/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.514696 JustDeepIt-0.1.29/justdeepit/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.526696 JustDeepIt-0.1.29/justdeepit/src/font/
+-rw-r--r--   0 runner    (1001) docker     (123)   555264 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/src/font/NotoSans-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/src/font/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    56382 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.530696 JustDeepIt-0.1.29/justdeepit/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/appbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/appis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/appod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/appsod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/justdeepit/webapp/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/.Rhistory
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/jquery-3.6.0.min.map
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58702 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/tree.jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)   174878 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/tree.jquery.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    23347 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/static/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/justdeepit/webapp/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/templates/module.html
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/justdeepit/webapp/templates/shutdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 04:20:12.534696 JustDeepIt-0.1.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-31 04:17:58.000000 JustDeepIt-0.1.29/setup.py
```

### Comparing `JustDeepIt-0.1.28/JustDeepIt.egg-info/PKG-INFO` & `JustDeepIt-0.1.29/JustDeepIt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.1.28
+Version: 0.1.29
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `JustDeepIt-0.1.28/JustDeepIt.egg-info/SOURCES.txt` & `JustDeepIt-0.1.29/JustDeepIt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/LICENSE` & `JustDeepIt-0.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/PKG-INFO` & `JustDeepIt-0.1.29/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.1.28
+Version: 0.1.29
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `JustDeepIt-0.1.28/README.md` & `JustDeepIt-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/models/instance_segment.py` & `JustDeepIt-0.1.29/justdeepit/models/instance_segment.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/models/object_detect.py` & `JustDeepIt-0.1.29/justdeepit/models/object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/models/salient_object_detect.py` & `JustDeepIt-0.1.29/justdeepit/models/salient_object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/models/utils/detectron2base.py` & `JustDeepIt-0.1.29/justdeepit/models/utils/detectron2base.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/models/utils/mmdetbase.py` & `JustDeepIt-0.1.29/justdeepit/models/utils/mmdetbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/models/utils/u2net.py` & `JustDeepIt-0.1.29/justdeepit/models/utils/u2net.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/models/utils/unet.py` & `JustDeepIt-0.1.29/justdeepit/models/utils/unet.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/src/font/NotoSans-Medium.ttf` & `JustDeepIt-0.1.29/justdeepit/src/font/NotoSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/src/font/OFL.txt` & `JustDeepIt-0.1.29/justdeepit/src/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/utils.py` & `JustDeepIt-0.1.29/justdeepit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,14 +607,15 @@
                 'image_id': image_id,
                 'category_id': cate2id[region['class']],
                 'bbox': [region['bbox'][0],
                          region['bbox'][1],
                          region['bbox'][2] - region['bbox'][0],
                          region['bbox'][3] - region['bbox'][1]],
                 'area': (region['bbox'][2] - region['bbox'][0]) * (region['bbox'][3] - region['bbox'][1]),
+                'score': region['score'],
                 'iscrowd': 0
             }
             if 'contour' in region and region['contour'] is not None:
                 ann['segmentation'] = [region['contour'].flatten(order='C').tolist()]
                 ann['area'] = self.__calc_area_from_polygon(region['contour'])
             
             tmpl['annotations'].append(ann)
```

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/app.py` & `JustDeepIt-0.1.29/justdeepit/webapp/app.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/appbase.py` & `JustDeepIt-0.1.29/justdeepit/webapp/appbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/appis.py` & `JustDeepIt-0.1.29/justdeepit/webapp/appis.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/appod.py` & `JustDeepIt-0.1.29/justdeepit/webapp/appod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/appsod.py` & `JustDeepIt-0.1.29/justdeepit/webapp/appsod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/static/jquery-3.6.0.min.js` & `JustDeepIt-0.1.29/justdeepit/webapp/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/static/jquery-3.6.0.min.map` & `JustDeepIt-0.1.29/justdeepit/webapp/static/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/static/styles.css` & `JustDeepIt-0.1.29/justdeepit/webapp/static/styles.css`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/static/tree.jquery.js` & `JustDeepIt-0.1.29/justdeepit/webapp/static/tree.jquery.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/static/tree.jquery.js.map` & `JustDeepIt-0.1.29/justdeepit/webapp/static/tree.jquery.js.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/static/utils.js` & `JustDeepIt-0.1.29/justdeepit/webapp/static/utils.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/templates/index.html` & `JustDeepIt-0.1.29/justdeepit/webapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/templates/module.html` & `JustDeepIt-0.1.29/justdeepit/webapp/templates/module.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/justdeepit/webapp/templates/shutdown.html` & `JustDeepIt-0.1.29/justdeepit/webapp/templates/shutdown.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.28/setup.py` & `JustDeepIt-0.1.29/setup.py`

 * *Files identical despite different names*

