# Comparing `tmp/asset_tracking_pepsico-0.0.1.tar.gz` & `tmp/asset_tracking_pepsico-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-0.0.1.tar", last modified: Tue May 23 13:09:46 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-0.0.2.tar", last modified: Tue May 30 12:40:01 2023, max compression
```

## Comparing `asset_tracking_pepsico-0.0.1.tar` & `asset_tracking_pepsico-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-23 13:09:46.014032 asset_tracking_pepsico-0.0.1/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.1/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1578 2023-05-23 13:09:46.013634 asset_tracking_pepsico-0.0.1/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 asset_tracking_pepsico-0.0.1/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-23 13:09:46.010524 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     7981 2023-05-23 13:08:44.000000 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico/asset_tracking_devicelogs.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-23 13:09:46.013109 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6040 2023-05-23 10:45:46.000000 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico/dto/PostgresSchema.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-23 13:09:46.012493 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1578 2023-05-23 13:09:45.000000 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      358 2023-05-23 13:09:46.000000 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-23 13:09:45.000000 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-23 13:09:45.000000 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-23 13:09:45.000000 asset_tracking_pepsico-0.0.1/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      788 2023-05-23 13:08:44.000000 asset_tracking_pepsico-0.0.1/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-23 13:09:46.014130 asset_tracking_pepsico-0.0.1/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-30 12:40:01.499686 asset_tracking_pepsico-0.0.2/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.2/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-30 12:40:01.499060 asset_tracking_pepsico-0.0.2/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 asset_tracking_pepsico-0.0.2/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-30 12:40:01.493532 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     5247 2023-05-30 12:31:38.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     4101 2023-05-30 12:29:56.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-30 12:40:01.498158 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6630 2023-05-29 16:28:07.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     3056 2023-05-30 12:33:32.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-30 12:40:01.497446 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-30 12:38:26.000000 asset_tracking_pepsico-0.0.2/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-30 12:40:01.500129 asset_tracking_pepsico-0.0.2/setup.cfg
```

### Comparing `asset_tracking_pepsico-0.0.1/LICENSE` & `asset_tracking_pepsico-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.1/PKG-INFO` & `asset_tracking_pepsico-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: asset_tracking_pepsico
-Version: 0.0.1
+Version: 0.0.2
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
-Keywords: asset,tracking,pepsico,location,latitude,longitude,store
+Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `asset_tracking_pepsico-0.0.1/README.md` & `asset_tracking_pepsico-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.1/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 class PostgresSchemaDto:
-    def __init__(self, asset_type=None, asset_id=None, store_id=None, location_description=None, location_id=None,
+    def __init__(self, schema_version=None, asset_type=None, asset_id=None, store_id=None, location_description=None, location_id=None,
                  asset_latitude=None, asset_longitude=None, location_radius=None, location_latitude=None,
                  location_longitude=None, asset=None, event=None, created_ts=None, created_dt=None, updated_ts=None,
                  altitude=None, heading=None, speed=None, speed_accuracy=None, course=None, course_accuracy=None,
-                 datasource=None):
+                 datasource=None, properties_dict=None):
+        self.schema_version = schema_version
         self.asset_type = asset_type
         self.asset_id = asset_id
         self.store_id = store_id
         self.location_description = location_description
         self.location_id = location_id
         self.asset_latitude = asset_latitude
         self.asset_longitude = asset_longitude
@@ -22,16 +23,20 @@
         self.altitude = altitude
         self.heading = heading
         self.speed = speed
         self.speed_accuracy = speed_accuracy
         self.course = course
         self.course_accuracy = course_accuracy
         self.datasource = datasource
+        self.properties_dict = properties_dict
 
     # Getter methods
+    def get_schema_version(self):
+        return self.schema_version
+
     def get_asset_type(self):
         return self.asset_type
 
     def get_asset_id(self):
         return self.asset_id
 
     def get_store_id(self):
@@ -90,15 +95,21 @@
 
     def get_course_accuracy(self):
         return self.course_accuracy
 
     def get_datasource(self):
         return self.datasource
 
+    def get_properties_dict(self):
+        return self.properties_dict
+
     # Setter methods
+    def set_schema_version(self, value):
+        self.schema_version = value
+
     def set_asset_type(self, value):
         self.asset_type = value
 
     def set_asset_id(self, value):
         self.asset_id = value
 
     def set_store_id(self, value):
@@ -157,16 +168,20 @@
 
     def set_course_accuracy(self, value):
         self.course_accuracy = value
 
     def set_datasource(self, value):
         self.datasource = value
 
+    def set_properties_dict(self, value):
+        self.properties_dict = value
+
     def __dict__(self):
         return {
+            'schema_version': self.schema_version,
             'asset_type': self.asset_type,
             'asset_id': self.asset_id,
             'store_id': self.store_id,
             'location_description': self.location_description,
             'location_id': self.location_id,
             'asset_latitude': self.asset_latitude,
             'asset_longitude': self.asset_longitude,
@@ -180,16 +195,17 @@
             'updated_ts': self.updated_ts,
             'altitude': self.altitude,
             'heading': self.heading,
             'speed': self.speed,
             'speed_accuracy': self.speed_accuracy,
             'course': self.course,
             'course_accuracy': self.course_accuracy,
-            'datasource': self.datasource
+            'datasource': self.datasource,
+            'properties_dict': self.properties_dict
         }
 
     def __str__(self):
-        return f"\'{self.asset_type}\', \'{self.asset_id}\', \'{self.store_id}\', \'{self.location_description}\', \'{self.location_id}\', " \
+        return f"{self.schema_version}, \'{self.asset_type}\', \'{self.asset_id}\', \'{self.store_id}\', \'{self.location_description}\', \'{self.location_id}\', " \
                f"{self.asset_latitude}, {self.asset_longitude}, {self.location_radius}, {self.location_latitude}, " \
                f"{self.location_longitude}, {self.asset}, \'{self.event}\', \'{self.created_dt}\', \'{self.created_ts}\', " \
                f"\'{self.updated_ts}\', {self.altitude}, {self.heading}, {self.speed}, {self.speed_accuracy}, {self.course}," \
-               f" {self.course_accuracy}, \'{self.datasource}\'"
+               f" {self.course_accuracy}, \'{self.datasource}\', \'{self.properties_dict}\'"
```

### Comparing `asset_tracking_pepsico-0.0.1/asset_tracking_pepsico.egg-info/PKG-INFO` & `asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: asset-tracking-pepsico
-Version: 0.0.1
+Version: 0.0.2
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
-Keywords: asset,tracking,pepsico,location,latitude,longitude,store
+Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `asset_tracking_pepsico-0.0.1/pyproject.toml` & `asset_tracking_pepsico-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
-keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store"]
+keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
 dependencies = [
   "azure-core",
   "azure-storage-blob",
   "requests",
   "requests-oauthlib",
   "toml",
   "psycopg2"
```

