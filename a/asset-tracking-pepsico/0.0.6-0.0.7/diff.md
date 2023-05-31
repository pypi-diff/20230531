# Comparing `tmp/asset_tracking_pepsico-0.0.6.tar.gz` & `tmp/asset_tracking_pepsico-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-0.0.6.tar", last modified: Wed May 31 15:34:40 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-0.0.7.tar", last modified: Wed May 31 15:55:06 2023, max compression
```

## Comparing `asset_tracking_pepsico-0.0.6.tar` & `asset_tracking_pepsico-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:34:40.064689 asset_tracking_pepsico-0.0.6/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.6/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:34:40.064009 asset_tracking_pepsico-0.0.6/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-0.0.6/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:34:40.058457 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/asset_tracking_devicelogs.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     4834 2023-05-31 15:34:12.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/asset_tracking_ingest.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:34:40.062468 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     5772 2023-05-31 09:45:49.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/dto/PostgresSchema.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     3234 2023-05-31 14:40:13.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:34:40.061714 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 15:34:40.000000 asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 15:34:20.000000 asset_tracking_pepsico-0.0.6/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 15:34:40.064918 asset_tracking_pepsico-0.0.6/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:55:06.353675 asset_tracking_pepsico-0.0.7/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.7/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:55:06.353241 asset_tracking_pepsico-0.0.7/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-0.0.7/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:55:06.349198 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     4834 2023-05-31 15:34:12.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:55:06.352759 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6539 2023-05-31 15:54:17.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     3234 2023-05-31 14:40:13.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:55:06.352195 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 15:54:41.000000 asset_tracking_pepsico-0.0.7/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 15:55:06.353822 asset_tracking_pepsico-0.0.7/setup.cfg
```

### Comparing `asset_tracking_pepsico-0.0.6/LICENSE` & `asset_tracking_pepsico-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.6/PKG-INFO` & `asset_tracking_pepsico-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset_tracking_pepsico
-Version: 0.0.6
+Version: 0.0.7
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.6/README.md` & `asset_tracking_pepsico-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/asset_tracking_devicelogs.py` & `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/asset_tracking_devicelogs.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/asset_tracking_ingest.py` & `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/asset_tracking_ingest.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,31 @@
 from typing import Optional
+from pydantic import BaseModel
+
+
+class Item(BaseModel):
+    schema_version: Optional[float] = None
+    asset_type: Optional[str] = None
+    asset_id: Optional[str] = None
+    event_type: Optional[str] = None
+    location_description: Optional[str] = None
+    location_id: Optional[str] = None
+    asset_latitude: Optional[float] = None
+    asset_longitude: Optional[float] = None
+    lat_long_acc: Optional[float] = None
+    created_ts: Optional[str] = None
+    altitude: Optional[float] = None
+    heading: Optional[float] = None
+    speed: Optional[float] = None
+    speed_accuracy: Optional[float] = None
+    course: Optional[float] = None
+    course_accuracy: Optional[float] = None
+    datasource: Optional[str] = None
+    properties_dict: Optional[str] = None
+
 
 class PostgresSchemaDto:
     schema_version: Optional[float] = None
     asset_type: Optional[str] = None
     asset_id: Optional[str] = None
     event_type: Optional[str] = None
     location_description: Optional[str] = None
```

### Comparing `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico/utilities.py` & `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/utilities.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.6/asset_tracking_pepsico.egg-info/PKG-INFO` & `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset-tracking-pepsico
-Version: 0.0.6
+Version: 0.0.7
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.6/pyproject.toml` & `asset_tracking_pepsico-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
```

