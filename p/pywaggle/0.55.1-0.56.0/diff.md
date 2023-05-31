# Comparing `tmp/pywaggle-0.55.1.tar.gz` & `tmp/pywaggle-0.56.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaggle-0.55.1.tar", last modified: Wed Apr  5 22:51:59 2023, max compression
+gzip compressed data, was "pywaggle-0.56.0.tar", last modified: Wed May 31 16:18:56 2023, max compression
```

## Comparing `pywaggle-0.55.1.tar` & `pywaggle-0.56.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:51:59.251536 pywaggle-0.55.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-05 22:51:49.000000 pywaggle-0.55.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-05 22:51:59.251536 pywaggle-0.55.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-05 22:51:49.000000 pywaggle-0.55.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-05 22:51:49.000000 pywaggle-0.55.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-05 22:51:59.251536 pywaggle-0.55.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:51:59.247536 pywaggle-0.55.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:51:59.251536 pywaggle-0.55.1/src/pywaggle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-05 22:51:59.000000 pywaggle-0.55.1/src/pywaggle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-05 22:51:59.000000 pywaggle-0.55.1/src/pywaggle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 22:51:59.000000 pywaggle-0.55.1/src/pywaggle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-05 22:51:59.000000 pywaggle-0.55.1/src/pywaggle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 22:51:59.000000 pywaggle-0.55.1/src/pywaggle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:51:59.251536 pywaggle-0.55.1/src/waggle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:51:59.251536 pywaggle-0.55.1/src/waggle/data/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/data/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/data/data_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/data/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/data/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/data/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:51:59.251536 pywaggle-0.55.1/src/waggle/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/plugin/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/plugin/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/plugin/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-05 22:51:49.000000 pywaggle-0.55.1/src/waggle/plugin/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:51:59.251536 pywaggle-0.55.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-05 22:51:49.000000 pywaggle-0.55.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-04-05 22:51:49.000000 pywaggle-0.55.1/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:18:56.844728 pywaggle-0.56.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-31 16:18:41.000000 pywaggle-0.56.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-31 16:18:56.844728 pywaggle-0.56.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-31 16:18:41.000000 pywaggle-0.56.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-31 16:18:41.000000 pywaggle-0.56.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-31 16:18:56.844728 pywaggle-0.56.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:18:56.836727 pywaggle-0.56.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:18:56.840728 pywaggle-0.56.0/src/pywaggle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-31 16:18:56.000000 pywaggle-0.56.0/src/pywaggle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 16:18:56.000000 pywaggle-0.56.0/src/pywaggle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:18:56.000000 pywaggle-0.56.0/src/pywaggle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 16:18:56.000000 pywaggle-0.56.0/src/pywaggle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 16:18:56.000000 pywaggle-0.56.0/src/pywaggle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:18:56.840728 pywaggle-0.56.0/src/waggle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:18:56.840728 pywaggle-0.56.0/src/waggle/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/data/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/data/data_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/data/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/data/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/data/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:18:56.844728 pywaggle-0.56.0/src/waggle/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/plugin/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/plugin/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/plugin/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-31 16:18:41.000000 pywaggle-0.56.0/src/waggle/plugin/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:18:56.844728 pywaggle-0.56.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-31 16:18:41.000000 pywaggle-0.56.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-05-31 16:18:41.000000 pywaggle-0.56.0/tests/test_plugin.py
```

### Comparing `pywaggle-0.55.1/LICENSE` & `pywaggle-0.56.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/PKG-INFO` & `pywaggle-0.56.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaggle
-Version: 0.55.1
+Version: 0.56.0
 Summary: Official Waggle Python module.
 Home-page: https://github.com/waggle-sensor/pywaggle
 Author: Sean Shahkarami
 Author-email: sean.shahkarami@gmail.com
 Project-URL: Bug Tracker, https://github.com/waggle-sensor/pywaggle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pywaggle-0.55.1/README.md` & `pywaggle-0.56.0/README.md`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/setup.cfg` & `pywaggle-0.56.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pywaggle
-version = 0.55.1
+version = 0.56.0
 author = Sean Shahkarami
 author_email = sean.shahkarami@gmail.com
 description = Official Waggle Python module.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/waggle-sensor/pywaggle
 project_urls =
```

### Comparing `pywaggle-0.55.1/src/pywaggle.egg-info/PKG-INFO` & `pywaggle-0.56.0/src/pywaggle.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaggle
-Version: 0.55.1
+Version: 0.56.0
 Summary: Official Waggle Python module.
 Home-page: https://github.com/waggle-sensor/pywaggle
 Author: Sean Shahkarami
 Author-email: sean.shahkarami@gmail.com
 Project-URL: Bug Tracker, https://github.com/waggle-sensor/pywaggle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pywaggle-0.55.1/src/pywaggle.egg-info/SOURCES.txt` & `pywaggle-0.56.0/src/pywaggle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/src/waggle/data/audio.py` & `pywaggle-0.56.0/src/waggle/data/audio.py`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/src/waggle/data/data_shim.py` & `pywaggle-0.56.0/src/waggle/data/data_shim.py`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/src/waggle/data/measurements.py` & `pywaggle-0.56.0/src/waggle/data/measurements.py`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/src/waggle/data/vision.py` & `pywaggle-0.56.0/src/waggle/data/vision.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,24 +140,30 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.context_depth -= 1
         if self.context_depth == 0:
             self.capture.release()
 
     def snapshot(self):
-        timestamp = get_timestamp()
-        ok, data = self.capture.read()
+        ok = self.capture.grab()
         if not ok:
             raise RuntimeError("failed to take snapshot")
+        timestamp = get_timestamp()
+        ok, data = self.capture.retrieve()
+        if not ok:
+            raise RuntimeError("failed to retrieve the taken snapshot")
         return ImageSample(data=data, timestamp=timestamp, format=self.format)
 
     def stream(self):
         while True:
+            ok = self.capture.grab()
+            if not ok:
+                break
             timestamp = get_timestamp()
-            ok, data = self.capture.read()
+            ok, data = self.capture.retrieve()
             if not ok:
                 break
             yield ImageSample(data=data, timestamp=timestamp, format=self.format)
 
 
 class ImageFolder:
     available_formats = {".jpg", ".jpeg", ".png"}
```

### Comparing `pywaggle-0.55.1/src/waggle/plugin/plugin.py` & `pywaggle-0.56.0/src/waggle/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/src/waggle/plugin/rabbitmq.py` & `pywaggle-0.56.0/src/waggle/plugin/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/src/waggle/plugin/time.py` & `pywaggle-0.56.0/src/waggle/plugin/time.py`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/src/waggle/plugin/uploader.py` & `pywaggle-0.56.0/src/waggle/plugin/uploader.py`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/tests/test_data.py` & `pywaggle-0.56.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pywaggle-0.55.1/tests/test_plugin.py` & `pywaggle-0.56.0/tests/test_plugin.py`

 * *Files identical despite different names*

