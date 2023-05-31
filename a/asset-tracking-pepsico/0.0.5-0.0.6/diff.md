# Comparing `tmp/asset_tracking_pepsico-0.0.5.tar.gz` & `tmp/asset_tracking_pepsico-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-0.0.5.tar", last modified: Wed May 31 15:01:54 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-0.0.6.tar", last modified: Wed May 31 15:34:40 2023, max compression
```

## Comparing `asset_tracking_pepsico-0.0.5.tar` & `asset_tracking_pepsico-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:01:54.504204 asset_tracking_pepsico-0.0.5/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.5/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:01:54.503728 asset_tracking_pepsico-0.0.5/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-0.0.5/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:01:54.496201 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/asset_tracking_devicelogs.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     4815 2023-05-31 14:27:22.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/asset_tracking_ingest.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:01:54.502671 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     5772 2023-05-31 09:45:49.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/dto/PostgresSchema.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     3234 2023-05-31 14:40:13.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:01:54.502107 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 14:41:16.000000 asset_tracking_pepsico-0.0.5/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 15:01:54.504334 asset_tracking_pepsico-0.0.5/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:34:40.064689 asset_tracking_pepsico-0.0.6/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.6/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:34:40.064009 asset_tracking_pepsico-0.0.6/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-0.0.6/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:34:40.058457 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     4834 2023-05-31 15:34:12.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:34:40.062468 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     5772 2023-05-31 09:45:49.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     3234 2023-05-31 14:40:13.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:34:40.061714 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 15:34:20.000000 asset_tracking_pepsico-0.0.6/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 15:34:40.064918 asset_tracking_pepsico-0.0.6/setup.cfg
```

### Comparing `asset_tracking_pepsico-0.0.5/LICENSE` & `asset_tracking_pepsico-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.5/PKG-INFO` & `asset_tracking_pepsico-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset_tracking_pepsico
-Version: 0.0.5
+Version: 0.0.6
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.5/README.md` & `asset_tracking_pepsico-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/asset_tracking_devicelogs.py` & `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/asset_tracking_devicelogs.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/asset_tracking_ingest.py` & `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/asset_tracking_ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             traceback.print_exc()
 
     def extract_properties(self, properties):
         try:
             # print("properties === ", properties)
             emp_det = properties['Employee']
             loc_info = properties['UserLocationCoordinates']
-            asset_id, emp_name = [i.strip() for i in emp_det.split(',')]
+            asset_id, emp_name = emp_det[:emp_det.find(',')], emp_det[emp_det.find(',')+1:]
             lat, long, acc, _ = loc_info.split(',')
             lat, long, acc = float(lat.strip()), float(long.strip()), float(acc.strip())
             event_desc = properties['Description']
             try:
                 loc_desc = properties['LocationDescription']
             except KeyError:
                 loc_desc = None
```

### Comparing `asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/utilities.py` & `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/utilities.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/PKG-INFO` & `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset-tracking-pepsico
-Version: 0.0.5
+Version: 0.0.6
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.5/pyproject.toml` & `asset_tracking_pepsico-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
```

