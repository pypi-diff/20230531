# Comparing `tmp/asset_tracking_pepsico-0.0.2.tar.gz` & `tmp/asset_tracking_pepsico-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-0.0.2.tar", last modified: Tue May 30 12:40:01 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-0.0.3.tar", last modified: Wed May 31 09:51:42 2023, max compression
```

## Comparing `asset_tracking_pepsico-0.0.2.tar` & `asset_tracking_pepsico-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-30 12:40:01.499686 asset_tracking_pepsico-0.0.2/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.2/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-30 12:40:01.499060 asset_tracking_pepsico-0.0.2/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 asset_tracking_pepsico-0.0.2/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-30 12:40:01.493532 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     5247 2023-05-30 12:31:38.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/asset_tracking_devicelogs.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     4101 2023-05-30 12:29:56.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/asset_tracking_ingest.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-30 12:40:01.498158 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6630 2023-05-29 16:28:07.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/dto/PostgresSchema.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     3056 2023-05-30 12:33:32.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-30 12:40:01.497446 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-30 12:40:01.000000 asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-30 12:38:26.000000 asset_tracking_pepsico-0.0.2/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-30 12:40:01.500129 asset_tracking_pepsico-0.0.2/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 09:51:42.993161 asset_tracking_pepsico-0.0.3/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.3/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-31 09:51:42.992600 asset_tracking_pepsico-0.0.3/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 asset_tracking_pepsico-0.0.3/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 09:51:42.987335 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6723 2023-05-31 09:44:20.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     4792 2023-05-31 09:51:11.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 09:51:42.991835 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     5772 2023-05-31 09:45:49.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     3056 2023-05-30 12:33:32.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 09:51:42.990639 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 09:51:11.000000 asset_tracking_pepsico-0.0.3/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 09:51:42.993340 asset_tracking_pepsico-0.0.3/setup.cfg
```

### Comparing `asset_tracking_pepsico-0.0.2/LICENSE` & `asset_tracking_pepsico-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.2/PKG-INFO` & `asset_tracking_pepsico-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset_tracking_pepsico
-Version: 0.0.2
+Version: 0.0.3
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.2/README.md` & `asset_tracking_pepsico-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/asset_tracking_devicelogs.py` & `asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/asset_tracking_devicelogs.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,14 +15,54 @@
             offset_hours, offset_minutes = map(int, offset_string.split(':'))
             offset = timedelta(hours=offset_hours, minutes=offset_minutes)
             datetime_obj = datetime.strptime(date_string + ' ' + time_string, "%m/%d/%Y %H:%M:%S") + offset
             return datetime_obj, date
         except:
             traceback.print_exc()
 
+    # format the query to form an sql query
+    def format_query(self, query):
+        try:
+            start_pos = query.find("None, '{") + len("None, '{")
+            end_pos = query.find("}'")
+            substring = query[start_pos:end_pos]
+            new_substring = substring.replace("'", '"')
+            updated_query = query[:start_pos] + new_substring + query[end_pos:]
+            updated_query = updated_query.replace('None', 'NULL')
+            return updated_query
+        except:
+            traceback.print_exc()
+
+    # generate an insert query based on the table name and the columns
+    def generate_insert_query(self, table_name, schema, columns):
+        try:
+            print('-'*120 + "\ncreating query for SCHEMA === \n", type(schema), schema, "\n" + '-'*120)
+            query = f'''INSERT INTO {table_name} ({columns}) VALUES ({schema.__str__()})'''
+            query = self.format_query(query)
+            print("QUERY === ", query, type(query))
+            return query
+        except:
+            traceback.print_exc()
+
+    # write the data to postgres
+    def write_data(self, postgre_conn_str, table_name, schema_list, columns):
+        try:
+            rows_affected = []
+            cursor, conn = utilities.get_conn(postgre_conn_str)
+            for schema in schema_list:
+                print('-' * 100 + "\nwriting to postgres === ", schema.__str__() + "\n" + '-' * 100)
+                query = self.generate_insert_query(table_name, schema, columns)
+                cursor.execute(query)
+                rows_affected.append(cursor.rowcount)
+                conn.commit()
+            utilities.close_connection(conn)
+            return rows_affected
+        except:
+            traceback.print_exc()
+
     # read the data from postgres
     def read_data_from_db(self, postgre_conn_str):
         cursor, conn = utilities.get_conn(postgre_conn_str)
         sql1 = '''select * from rsrlocation_info limit 5;'''
         cursor.execute(sql1)
         for i in cursor.fetchall():
             print("result == ", i)
@@ -82,31 +122,27 @@
     # create the schema object in the form of dto defined in the PostgresSchemaDto class
     def create_schema_list(self, df, asset_type, gpid, data_source, schema_version):
         try:
             schema_list = []
             print(df.columns)
             for index, row in df.iterrows():
                 # print("creating schema for \n" + str(row) + "\n" + "-"*200)
-                event = {'event': row['event']}
-                if event['event'] == "OnLocationChanged":
+                event = row['event']
+                if event == "OnLocationChanged":
                     # print("Entered if condition for event === ", event)
                     speed = row['Speed']
-                    updated_ts = None
-                    store_id = None
+                    properties_dict = {}
                 else:
                     speed = None
-                    updated_ts = row['LastExitTime']
-                    store_id = row['cust_cis_id']
-                speed_acc = row['Accuracy']
+                    properties_dict = self.extract_extra_properties(row)
+                lat_long_acc = row['Accuracy']
                 ts = row['Timestamp']
-                _, dt = self.convert_datetime(row['Timestamp'])
                 lat, long = float(row['Latitude']), float(row['Longitude'])
-                properties_dict = self.extract_extra_properties(row)
 
-                schema = PostgresSchemaDto(schema_version=schema_version, asset_id=gpid, asset_type=asset_type, store_id=store_id,
+                schema = PostgresSchemaDto(schema_version=schema_version, asset_id=gpid, asset_type=asset_type,
                                            datasource=data_source, asset_latitude=lat, asset_longitude=long, speed=speed,
-                                           speed_accuracy=speed_acc, event=str(event), created_ts=ts, updated_ts=updated_ts,
-                                           created_dt=dt, properties_dict=properties_dict)
+                                           lat_long_acc=lat_long_acc, event_type=event, created_ts=ts,
+                                           properties_dict=str(properties_dict))
                 schema_list.append(schema)
             return schema_list
         except:
             traceback.print_exc()
```

### Comparing `asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,43 @@
+from typing import Optional
+
 class PostgresSchemaDto:
-    def __init__(self, schema_version=None, asset_type=None, asset_id=None, store_id=None, location_description=None, location_id=None,
-                 asset_latitude=None, asset_longitude=None, location_radius=None, location_latitude=None,
-                 location_longitude=None, asset=None, event=None, created_ts=None, created_dt=None, updated_ts=None,
-                 altitude=None, heading=None, speed=None, speed_accuracy=None, course=None, course_accuracy=None,
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
+    def __init__(self, schema_version=None, asset_type=None, asset_id=None, event_type=None, location_description=None, location_id=None,
+                 asset_latitude=None, asset_longitude=None, lat_long_acc=None, created_ts=None, altitude=None, heading=None,
+                 speed=None, speed_accuracy=None, course=None, course_accuracy=None,
                  datasource=None, properties_dict=None):
         self.schema_version = schema_version
         self.asset_type = asset_type
         self.asset_id = asset_id
-        self.store_id = store_id
+        self.event_type = event_type
         self.location_description = location_description
         self.location_id = location_id
         self.asset_latitude = asset_latitude
         self.asset_longitude = asset_longitude
-        self.location_radius = location_radius
-        self.location_latitude = location_latitude
-        self.location_longitude = location_longitude
-        self.asset = asset
-        self.event = event
-        self.created_dt = created_dt
+        self.lat_long_acc = lat_long_acc
         self.created_ts = created_ts
-        self.updated_ts = updated_ts
         self.altitude = altitude
         self.heading = heading
         self.speed = speed
         self.speed_accuracy = speed_accuracy
         self.course = course
         self.course_accuracy = course_accuracy
         self.datasource = datasource
@@ -35,53 +49,35 @@
 
     def get_asset_type(self):
         return self.asset_type
 
     def get_asset_id(self):
         return self.asset_id
 
-    def get_store_id(self):
-        return self.store_id
+    def get_event_type(self):
+        return self.event_type
 
     def get_location_description(self):
         return self.location_description
 
     def get_location_id(self):
         return self.location_id
 
     def get_asset_latitude(self):
         return self.asset_latitude
 
     def get_asset_longitude(self):
         return self.asset_longitude
 
-    def get_location_radius(self):
-        return self.location_radius
-
-    def get_location_latitude(self):
-        return self.location_latitude
-
-    def get_location_longitude(self):
-        return self.location_longitude
-
-    def get_asset(self):
-        return self.asset
-
-    def get_event(self):
-        return self.event
-
-    def get_created_dt(self):
-        return self.created_dt
+    def get_lat_long_acc(self):
+        return self.lat_long_acc
 
     def get_created_ts(self):
         return self.created_ts
 
-    def get_updated_ts(self):
-        return self.updated_ts
-
     def get_altitude(self):
         return self.altitude
 
     def get_heading(self):
         return self.heading
 
     def get_speed(self):
@@ -108,53 +104,35 @@
 
     def set_asset_type(self, value):
         self.asset_type = value
 
     def set_asset_id(self, value):
         self.asset_id = value
 
-    def set_store_id(self, value):
-        self.store_id = value
+    def set_event_type(self, value):
+        self.event_type = value
 
     def set_location_description(self, value):
         self.location_description = value
 
     def set_location_id(self, value):
         self.location_id = value
 
     def set_asset_latitude(self, value):
         self.asset_latitude = value
 
     def set_asset_longitude(self, value):
         self.asset_longitude = value
 
-    def set_location_radius(self, value):
-        self.location_radius = value
-
-    def set_location_latitude(self, value):
-        self.location_latitude = value
-
-    def set_location_longitude(self, value):
-        self.location_longitude = value
-
-    def set_asset(self, value):
-        self.asset = value
-
-    def set_event(self, value):
-        self.event = value
-
-    def set_created_dt(self, value):
-        self.created_dt = value
+    def set_lat_long_acc(self, value):
+        self.lat_long_acc = value
 
     def set_created_ts(self, value):
         self.created_ts = value
 
-    def set_updated_ts(self, value):
-        self.updated_ts = value
-
     def set_altitude(self, value):
         self.altitude = value
 
     def set_heading(self, value):
         self.heading = value
 
     def set_speed(self, value):
@@ -176,36 +154,29 @@
         self.properties_dict = value
 
     def __dict__(self):
         return {
             'schema_version': self.schema_version,
             'asset_type': self.asset_type,
             'asset_id': self.asset_id,
-            'store_id': self.store_id,
+            'event_type': self.event_type,
             'location_description': self.location_description,
             'location_id': self.location_id,
             'asset_latitude': self.asset_latitude,
             'asset_longitude': self.asset_longitude,
-            'location_radius': self.location_radius,
-            'location_latitude': self.location_latitude,
-            'location_longitude': self.location_longitude,
-            'asset': self.asset,
-            'event': self.event,
-            'created_dt': self.created_dt,
+            'lat_long_acc': self.lat_long_acc,
             'created_ts': self.created_ts,
-            'updated_ts': self.updated_ts,
             'altitude': self.altitude,
             'heading': self.heading,
             'speed': self.speed,
             'speed_accuracy': self.speed_accuracy,
             'course': self.course,
             'course_accuracy': self.course_accuracy,
             'datasource': self.datasource,
             'properties_dict': self.properties_dict
         }
 
     def __str__(self):
-        return f"{self.schema_version}, \'{self.asset_type}\', \'{self.asset_id}\', \'{self.store_id}\', \'{self.location_description}\', \'{self.location_id}\', " \
-               f"{self.asset_latitude}, {self.asset_longitude}, {self.location_radius}, {self.location_latitude}, " \
-               f"{self.location_longitude}, {self.asset}, \'{self.event}\', \'{self.created_dt}\', \'{self.created_ts}\', " \
-               f"\'{self.updated_ts}\', {self.altitude}, {self.heading}, {self.speed}, {self.speed_accuracy}, {self.course}," \
-               f" {self.course_accuracy}, \'{self.datasource}\', \'{self.properties_dict}\'"
+        return f"{self.schema_version}, \'{self.asset_type}\', \'{self.asset_id}\', \'{self.event_type}\', \'{self.location_description}\', " \
+               f"\'{self.location_id}\', {self.asset_latitude}, {self.asset_longitude}, {self.lat_long_acc}, \'{self.created_ts}\', " \
+               f"{self.altitude}, {self.heading}, {self.speed}, {self.speed_accuracy}, {self.course}, {self.course_accuracy}, " \
+               f"\'{self.datasource}\', \'{self.properties_dict}\'"
```

### Comparing `asset_tracking_pepsico-0.0.2/asset_tracking_pepsico/utilities.py` & `asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/utilities.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.2/asset_tracking_pepsico.egg-info/PKG-INFO` & `asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset-tracking-pepsico
-Version: 0.0.2
+Version: 0.0.3
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.2/pyproject.toml` & `asset_tracking_pepsico-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
```

