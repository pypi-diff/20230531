# Comparing `tmp/visier-connector-0.9.5.tar.gz` & `tmp/visier-connector-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visier-connector-0.9.5.tar", last modified: Mon May 29 22:29:30 2023, max compression
+gzip compressed data, was "visier-connector-0.9.6.tar", last modified: Wed May 31 01:12:22 2023, max compression
```

## Comparing `visier-connector-0.9.5.tar` & `visier-connector-0.9.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.195076 visier-connector-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 22:29:19.000000 visier-connector-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-05-29 22:29:30.191076 visier-connector-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-29 22:29:19.000000 visier-connector-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-29 22:29:19.000000 visier-connector-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:29:30.195076 visier-connector-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.191076 visier-connector-0.9.5/visier/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.191076 visier-connector-0.9.5/visier/api/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/direct_intake.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.191076 visier-connector-0.9.5/visier/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/connector/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/connector/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/connector/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.191076 visier-connector-0.9.5/visier_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.963419 visier-connector-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 01:12:11.000000 visier-connector-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-05-31 01:12:22.963419 visier-connector-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-31 01:12:11.000000 visier-connector-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-31 01:12:11.000000 visier-connector-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:12:22.963419 visier-connector-0.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.959419 visier-connector-0.9.6/visier/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.963419 visier-connector-0.9.6/visier/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/direct_intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.963419 visier-connector-0.9.6/visier/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/connector/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/connector/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/connector/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.963419 visier-connector-0.9.6/visier_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/top_level.txt
```

### Comparing `visier-connector-0.9.5/LICENSE` & `visier-connector-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/PKG-INFO` & `visier-connector-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.5
+Version: 0.9.6
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `visier-connector-0.9.5/README.md` & `visier-connector-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/pyproject.toml` & `visier-connector-0.9.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 description = """Visier People Data connector"""
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["visier", "data", "query", "connector", "api"]
 license = {file = "LICENSE"}
 dynamic = ["version"]
 dependencies = [
-    "requests >= 2.28",
+    "requests >= 2.31",
     "deprecated",
 ]
 
 [tool.poetry]
 readme = "README.md"
 
 [tool.setuptools.dynamic]
```

### Comparing `visier-connector-0.9.5/visier/__init__.py` & `visier-connector-0.9.6/visier/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
-__version__ = "0.9.5"
+__version__ = "0.9.6"
```

### Comparing `visier-connector-0.9.5/visier/api/__init__.py` & `visier-connector-0.9.6/visier/api/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/visier/api/base.py` & `visier-connector-0.9.6/visier/api/base.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/visier/api/direct_intake.py` & `visier-connector-0.9.6/visier/api/direct_intake.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     def rollback_transaction(self, transaction_id: str) -> Response:
         """Roll-back a pending transaction and discard all uploaded data.
         
         Arguments:
         - transaction_id: The transaction id returned by start_transaction"""
         def call_impl(context: SessionContext) -> Response:
-            url = context.mk_url(f"{BASE_PATH}/transactions/{transaction_id}/")
+            url = context.mk_url(f"{BASE_PATH}/transactions/{transaction_id}")
             return context.session().delete(url)
         return self.run(call_impl)
 
     def commit_transaction(self, transaction_id: str) -> Response:
         """Commit the transaction and make the uploaded data available for use.
         
         Arguments:
```

### Comparing `visier-connector-0.9.5/visier/api/model.py` & `visier-connector-0.9.6/visier/api/model.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/visier/api/query.py` & `visier-connector-0.9.6/visier/api/query.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/visier/connector/__init__.py` & `visier-connector-0.9.6/visier/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/visier/connector/authentication.py` & `visier-connector-0.9.6/visier/connector/authentication.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/visier/connector/sessions.py` & `visier-connector-0.9.6/visier/connector/sessions.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/visier/connector/table.py` & `visier-connector-0.9.6/visier/connector/table.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.5/visier_connector.egg-info/PKG-INFO` & `visier-connector-0.9.6/visier_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.5
+Version: 0.9.6
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

