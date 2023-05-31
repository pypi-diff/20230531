# Comparing `tmp/fleet_sdk-0.5.2.tar.gz` & `tmp/fleet_sdk-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleet_sdk-0.5.2.tar", max compression
+gzip compressed data, was "fleet_sdk-0.5.3.tar", max compression
```

## Comparing `fleet_sdk-0.5.2.tar` & `fleet_sdk-0.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-05-28 23:24:11.000000 fleet_sdk-0.5.2/LICENSE
--rw-r--r--   0        0        0       39 2023-05-29 20:36:49.448172 fleet_sdk-0.5.2/README.md
--rw-r--r--   0        0        0      536 2023-05-30 17:38:57.099874 fleet_sdk-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-30 17:33:57.142994 fleet_sdk-0.5.2/src/fleet_sdk/.DS_Store
--rw-r--r--   0        0        0     5729 2023-05-30 17:33:53.922312 fleet_sdk-0.5.2/src/fleet_sdk/Tracker.py
--rw-r--r--   0        0        0       56 2023-05-29 21:37:45.269045 fleet_sdk-0.5.2/src/fleet_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 23:36:32.000000 fleet_sdk-0.5.2/src/fleet_sdk/adapters/__init__.py
--rw-r--r--   0        0        0     1243 2023-05-30 17:34:06.613851 fleet_sdk-0.5.2/src/fleet_sdk/adapters/base_adapter.py
--rw-r--r--   0        0        0     2138 2023-05-30 17:34:19.971392 fleet_sdk-0.5.2/src/fleet_sdk/adapters/fastapi_adapter.py
--rw-r--r--   0        0        0     1871 2023-05-30 17:34:57.215879 fleet_sdk-0.5.2/src/fleet_sdk/adapters/flask_adapter.py
--rw-r--r--   0        0        0     1987 2023-05-30 17:35:08.954831 fleet_sdk-0.5.2/src/fleet_sdk/adapters/quart_adapter.py
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 fleet_sdk-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-28 23:24:11.000000 fleet_sdk-0.5.3/LICENSE
+-rw-r--r--   0        0        0       39 2023-05-29 20:36:49.448172 fleet_sdk-0.5.3/README.md
+-rw-r--r--   0        0        0      536 2023-05-31 20:40:35.140960 fleet_sdk-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-30 17:33:57.142994 fleet_sdk-0.5.3/src/fleet_sdk/.DS_Store
+-rw-r--r--   0        0        0     5724 2023-05-31 20:40:01.146348 fleet_sdk-0.5.3/src/fleet_sdk/Tracker.py
+-rw-r--r--   0        0        0       56 2023-05-29 21:37:45.269045 fleet_sdk-0.5.3/src/fleet_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:36:32.000000 fleet_sdk-0.5.3/src/fleet_sdk/adapters/__init__.py
+-rw-r--r--   0        0        0     1243 2023-05-30 17:34:06.613851 fleet_sdk-0.5.3/src/fleet_sdk/adapters/base_adapter.py
+-rw-r--r--   0        0        0     2138 2023-05-30 17:34:19.971392 fleet_sdk-0.5.3/src/fleet_sdk/adapters/fastapi_adapter.py
+-rw-r--r--   0        0        0     1871 2023-05-30 17:34:57.215879 fleet_sdk-0.5.3/src/fleet_sdk/adapters/flask_adapter.py
+-rw-r--r--   0        0        0     1987 2023-05-30 17:35:08.954831 fleet_sdk-0.5.3/src/fleet_sdk/adapters/quart_adapter.py
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 fleet_sdk-0.5.3/PKG-INFO
```

### Comparing `fleet_sdk-0.5.2/LICENSE` & `fleet_sdk-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.2/pyproject.toml` & `fleet_sdk-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fleet-sdk"
-version = "0.5.2"
+version = "0.5.3"
 description = "Fleet SDK for building and managing chatGPT plugins"
 authors = ["fleet_team <fleet.ai.team@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 fastapi = "^0.95.0"
```

### Comparing `fleet_sdk-0.5.2/src/fleet_sdk/.DS_Store` & `fleet_sdk-0.5.3/src/fleet_sdk/.DS_Store`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.2/src/fleet_sdk/Tracker.py` & `fleet_sdk-0.5.3/src/fleet_sdk/Tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 sdk_dir = os.path.dirname(os.path.abspath(__file__))
 parent_dir = os.path.dirname(sdk_dir)
 if parent_dir not in sys.path:
   sys.path.insert(0, parent_dir)
 
 
 class Tracker:
-  DEFAULT_HOST = 'middleware.egdeltur.repl.co'
+  DEFAULT_HOST = 'middleware.usefleet.ai'
   DEFAULT_DEBUG = True
 
   def __init__(self, token, app, host=DEFAULT_HOST, debug=DEFAULT_DEBUG):
     """
         Initialize the Tracker with the provided token, host, and debug flag.
     """
     self.token = token
```

### Comparing `fleet_sdk-0.5.2/src/fleet_sdk/adapters/base_adapter.py` & `fleet_sdk-0.5.3/src/fleet_sdk/adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.2/src/fleet_sdk/adapters/fastapi_adapter.py` & `fleet_sdk-0.5.3/src/fleet_sdk/adapters/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.2/src/fleet_sdk/adapters/flask_adapter.py` & `fleet_sdk-0.5.3/src/fleet_sdk/adapters/flask_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.2/src/fleet_sdk/adapters/quart_adapter.py` & `fleet_sdk-0.5.3/src/fleet_sdk/adapters/quart_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.2/PKG-INFO` & `fleet_sdk-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleet-sdk
-Version: 0.5.2
+Version: 0.5.3
 Summary: Fleet SDK for building and managing chatGPT plugins
 Author: fleet_team
 Author-email: fleet.ai.team@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

