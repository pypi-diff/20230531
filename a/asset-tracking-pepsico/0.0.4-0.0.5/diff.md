# Comparing `tmp/asset_tracking_pepsico-0.0.4.tar.gz` & `tmp/asset_tracking_pepsico-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-0.0.4.tar", last modified: Wed May 31 12:43:04 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-0.0.5.tar", last modified: Wed May 31 15:01:54 2023, max compression
```

## Comparing `asset_tracking_pepsico-0.0.4.tar` & `asset_tracking_pepsico-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 12:43:04.098533 asset_tracking_pepsico-0.0.4/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.4/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-31 12:43:04.097385 asset_tracking_pepsico-0.0.4/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 asset_tracking_pepsico-0.0.4/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 12:43:04.090556 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/asset_tracking_devicelogs.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     4815 2023-05-31 12:41:12.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/asset_tracking_ingest.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 12:43:04.095544 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     5772 2023-05-31 09:45:49.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/dto/PostgresSchema.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     3056 2023-05-30 12:33:32.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 12:43:04.094869 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 12:42:01.000000 asset_tracking_pepsico-0.0.4/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 12:43:04.098885 asset_tracking_pepsico-0.0.4/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:01:54.504204 asset_tracking_pepsico-0.0.5/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.5/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:01:54.503728 asset_tracking_pepsico-0.0.5/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-0.0.5/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:01:54.496201 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     4815 2023-05-31 14:27:22.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:01:54.502671 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     5772 2023-05-31 09:45:49.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     3234 2023-05-31 14:40:13.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:01:54.502107 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 15:01:54.000000 asset_tracking_pepsico-0.0.5/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 14:41:16.000000 asset_tracking_pepsico-0.0.5/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 15:01:54.504334 asset_tracking_pepsico-0.0.5/setup.cfg
```

### Comparing `asset_tracking_pepsico-0.0.4/LICENSE` & `asset_tracking_pepsico-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/asset_tracking_devicelogs.py` & `asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/asset_tracking_devicelogs.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/asset_tracking_ingest.py` & `asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/asset_tracking_ingest.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 elif i == '}' and len(ind) > 0:
                     ind.pop(-1)
                 if len(ind) == 0:
                     end = ix
                     sub_str = data[st:end + 1]
                     sub = json.loads(sub_str)
                     json_list.append(sub)
-                    st = end + 1
+                    st = end + 2
             return json_list
         except:
             traceback.print_exc()
 
     def extract_properties(self, properties):
         try:
             # print("properties === ", properties)
```

### Comparing `asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/utilities.py` & `asset_tracking_pepsico-0.0.5/asset_tracking_pepsico/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,22 @@
     try:
         str_list = [i.__str__() for i in schema_list]
         return str_list
     except:
         traceback.print_exc()
 
 
+def get_dict_from_schema_list(schema_list):
+    try:
+        dict_list = [i.__dict__() for i in schema_list]
+        return dict_list
+    except:
+        traceback.print_exc()
+
+
 # Get a connection to a new postgres server using the connection string.
 def get_conn(postgre_conn_str):
     try:
         conn = psycopg2.connect(postgre_conn_str)
         cursor = conn.cursor()
         return cursor, conn
     except:
```

### Comparing `asset_tracking_pepsico-0.0.4/pyproject.toml` & `asset_tracking_pepsico-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
```

