# Comparing `tmp/SunshineDB-1.3.tar.gz` & `tmp/SunshineDB-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SunshineDB-1.3.tar", last modified: Wed May 31 16:44:23 2023, max compression
+gzip compressed data, was "SunshineDB-1.4.tar", last modified: Wed May 31 20:48:36 2023, max compression
```

## Comparing `SunshineDB-1.3.tar` & `SunshineDB-1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kayra     (1000) kayra     (1000)        0 2023-05-31 16:44:23.367263 SunshineDB-1.3/
--rw-r--r--   0 kayra     (1000) kayra     (1000)     5083 2023-05-31 16:44:23.367263 SunshineDB-1.3/PKG-INFO
--rw-r--r--   0 kayra     (1000) kayra     (1000)     4730 2023-05-31 16:11:05.000000 SunshineDB-1.3/PyPi.md
--rw-r--r--   0 kayra     (1000) kayra     (1000)     5317 2023-05-31 14:30:33.000000 SunshineDB-1.3/README.md
-drwxr-xr-x   0 kayra     (1000) kayra     (1000)        0 2023-05-31 16:44:23.367263 SunshineDB-1.3/Sunshine/
--rw-r--r--   0 kayra     (1000) kayra     (1000)       95 2023-05-31 16:16:45.000000 SunshineDB-1.3/Sunshine/__init__.py
--rw-r--r--   0 kayra     (1000) kayra     (1000)      660 2023-05-31 12:52:34.000000 SunshineDB-1.3/Sunshine/messages.py
--rw-r--r--   0 kayra     (1000) kayra     (1000)     2941 2023-05-31 16:41:58.000000 SunshineDB-1.3/Sunshine/moonlight.py
--rw-r--r--   0 kayra     (1000) kayra     (1000)     7485 2023-05-31 16:37:43.000000 SunshineDB-1.3/Sunshine/sunshine.py
-drwxr-xr-x   0 kayra     (1000) kayra     (1000)        0 2023-05-31 16:44:23.367263 SunshineDB-1.3/SunshineDB.egg-info/
--rw-r--r--   0 kayra     (1000) kayra     (1000)     5083 2023-05-31 16:44:23.000000 SunshineDB-1.3/SunshineDB.egg-info/PKG-INFO
--rw-r--r--   0 kayra     (1000) kayra     (1000)      323 2023-05-31 16:44:23.000000 SunshineDB-1.3/SunshineDB.egg-info/SOURCES.txt
--rw-r--r--   0 kayra     (1000) kayra     (1000)        1 2023-05-31 16:44:23.000000 SunshineDB-1.3/SunshineDB.egg-info/dependency_links.txt
--rw-r--r--   0 kayra     (1000) kayra     (1000)        1 2023-05-31 16:44:23.000000 SunshineDB-1.3/SunshineDB.egg-info/not-zip-safe
--rw-r--r--   0 kayra     (1000) kayra     (1000)       18 2023-05-31 16:44:23.000000 SunshineDB-1.3/SunshineDB.egg-info/requires.txt
--rw-r--r--   0 kayra     (1000) kayra     (1000)        9 2023-05-31 16:44:23.000000 SunshineDB-1.3/SunshineDB.egg-info/top_level.txt
--rw-r--r--   0 kayra     (1000) kayra     (1000)      519 2023-05-31 16:44:23.371263 SunshineDB-1.3/setup.cfg
--rw-r--r--   0 kayra     (1000) kayra     (1000)       37 2023-05-31 13:05:49.000000 SunshineDB-1.3/setup.py
+drwxr-xr-x   0 kayra     (1000) kayra     (1000)        0 2023-05-31 20:48:36.699257 SunshineDB-1.4/
+-rw-r--r--   0 kayra     (1000) kayra     (1000)     5083 2023-05-31 20:48:36.699257 SunshineDB-1.4/PKG-INFO
+-rw-r--r--   0 kayra     (1000) kayra     (1000)     4730 2023-05-31 16:11:05.000000 SunshineDB-1.4/PyPi.md
+-rw-r--r--   0 kayra     (1000) kayra     (1000)     5317 2023-05-31 14:30:33.000000 SunshineDB-1.4/README.md
+drwxr-xr-x   0 kayra     (1000) kayra     (1000)        0 2023-05-31 20:48:36.699257 SunshineDB-1.4/Sunshine/
+-rw-r--r--   0 kayra     (1000) kayra     (1000)       95 2023-05-31 16:16:45.000000 SunshineDB-1.4/Sunshine/__init__.py
+-rw-r--r--   0 kayra     (1000) kayra     (1000)      660 2023-05-31 12:52:34.000000 SunshineDB-1.4/Sunshine/messages.py
+-rw-r--r--   0 kayra     (1000) kayra     (1000)     2941 2023-05-31 16:41:58.000000 SunshineDB-1.4/Sunshine/moonlight.py
+-rw-r--r--   0 kayra     (1000) kayra     (1000)     7505 2023-05-31 20:48:00.000000 SunshineDB-1.4/Sunshine/sunshine.py
+drwxr-xr-x   0 kayra     (1000) kayra     (1000)        0 2023-05-31 20:48:36.699257 SunshineDB-1.4/SunshineDB.egg-info/
+-rw-r--r--   0 kayra     (1000) kayra     (1000)     5083 2023-05-31 20:48:36.000000 SunshineDB-1.4/SunshineDB.egg-info/PKG-INFO
+-rw-r--r--   0 kayra     (1000) kayra     (1000)      323 2023-05-31 20:48:36.000000 SunshineDB-1.4/SunshineDB.egg-info/SOURCES.txt
+-rw-r--r--   0 kayra     (1000) kayra     (1000)        1 2023-05-31 20:48:36.000000 SunshineDB-1.4/SunshineDB.egg-info/dependency_links.txt
+-rw-r--r--   0 kayra     (1000) kayra     (1000)        1 2023-05-31 20:48:36.000000 SunshineDB-1.4/SunshineDB.egg-info/not-zip-safe
+-rw-r--r--   0 kayra     (1000) kayra     (1000)       18 2023-05-31 20:48:36.000000 SunshineDB-1.4/SunshineDB.egg-info/requires.txt
+-rw-r--r--   0 kayra     (1000) kayra     (1000)        9 2023-05-31 20:48:36.000000 SunshineDB-1.4/SunshineDB.egg-info/top_level.txt
+-rw-r--r--   0 kayra     (1000) kayra     (1000)      519 2023-05-31 20:48:36.699257 SunshineDB-1.4/setup.cfg
+-rw-r--r--   0 kayra     (1000) kayra     (1000)       37 2023-05-31 13:05:49.000000 SunshineDB-1.4/setup.py
```

### Comparing `SunshineDB-1.3/PKG-INFO` & `SunshineDB-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunshineDB
-Version: 1.3
+Version: 1.4
 Summary: Lightweight json-database library for Python
 Home-page: https://github.com/Sunshine-Database/Sunshine
 Author: de4oult
 Author-email: kayra.dist@email.com
 License: MIT License
 Keywords: sunshine,database,json,json-database,db,async
 Requires-Python: >=3
```

### Comparing `SunshineDB-1.3/PyPi.md` & `SunshineDB-1.4/PyPi.md`

 * *Files identical despite different names*

### Comparing `SunshineDB-1.3/README.md` & `SunshineDB-1.4/README.md`

 * *Files identical despite different names*

### Comparing `SunshineDB-1.3/Sunshine/messages.py` & `SunshineDB-1.4/Sunshine/messages.py`

 * *Files identical despite different names*

### Comparing `SunshineDB-1.3/Sunshine/moonlight.py` & `SunshineDB-1.4/Sunshine/moonlight.py`

 * *Files identical despite different names*

### Comparing `SunshineDB-1.3/Sunshine/sunshine.py` & `SunshineDB-1.4/Sunshine/sunshine.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 EMPTY: dict[str, list] = {
     'data' : []
 }
 
 def create_database(filename: str, create_file: bool = True) -> True:
     if filename.endswith('.json'):
         if create_file and not os.path.exists(filename):
-            with open(filename, 'w') as database_file:
+            with open(filename, 'w', encoding = 'utf-8') as database_file:
                 database_file.write(json.dumps(EMPTY, indent = 4))
     
 
 class Sunshine:
     """
     Class of json-database. 
     Has the following set of methods: push, all, get, update, contains, delete, drop, backup.
```

### Comparing `SunshineDB-1.3/SunshineDB.egg-info/PKG-INFO` & `SunshineDB-1.4/SunshineDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunshineDB
-Version: 1.3
+Version: 1.4
 Summary: Lightweight json-database library for Python
 Home-page: https://github.com/Sunshine-Database/Sunshine
 Author: de4oult
 Author-email: kayra.dist@email.com
 License: MIT License
 Keywords: sunshine,database,json,json-database,db,async
 Requires-Python: >=3
```

### Comparing `SunshineDB-1.3/setup.cfg` & `SunshineDB-1.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SunshineDB
-version = 1.3
+version = 1.4
 description = Lightweight json-database library for Python
 url = https://github.com/Sunshine-Database/Sunshine
 license = MIT License
 keywords = sunshine, database, json, json-database, db, async
 author = de4oult
 author_email = kayra.dist@email.com
 long_description = file: PyPi.md
```

