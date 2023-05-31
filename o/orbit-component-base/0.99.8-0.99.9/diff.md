# Comparing `tmp/orbit_component_base-0.99.8.tar.gz` & `tmp/orbit_component_base-0.99.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_base-0.99.8.tar", max compression
+gzip compressed data, was "orbit_component_base-0.99.9.tar", max compression
```

## Comparing `orbit_component_base-0.99.8.tar` & `orbit_component_base-0.99.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/LICENSE.md
--rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/README.md
--rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/__init__.py
--rw-r--r--   0        0        0      698 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/plugin.py
--rw-r--r--   0        0        0     1020 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/schema/OrbitSessions.py
--rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/schema/OrbitUsers.py
--rwxr-xr-x   0        0        0     3506 2023-05-30 20:47:27.827498 orbit_component_base-0.99.8/orbit_component_base/src/orbit_app.py
--rw-r--r--   0        0        0     6315 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_auth.py
--rw-r--r--   0        0        0     6281 2023-05-30 16:47:54.685910 orbit_component_base-0.99.8/orbit_component_base/src/orbit_config.py
--rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_database.py
--rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_decorators.py
--rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_logger.py
--rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-0.99.8/orbit_component_base/src/orbit_make_ssl.py
--rw-r--r--   0        0        0     8612 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_nql.py
--rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_nql_buffer.py
--rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_nql_emitter.py
--rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_nql_session.py
--rw-r--r--   0        0        0     6409 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_orm.py
--rw-r--r--   0        0        0     2293 2023-05-30 15:19:20.188832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_plugin.py
--rw-r--r--   0        0        0     1243 2023-05-30 15:19:20.192832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_plugins.py
--rw-r--r--   0        0        0     2329 2023-05-30 21:39:29.016203 orbit_component_base-0.99.8/orbit_component_base/src/orbit_router.py
--rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_shared.py
--rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-0.99.8/orbit_component_base/src/orbit_version.py
--rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-0.99.8/orbit_component_base/tests/test_main.py
--rw-r--r--   0        0        0       23 2023-05-31 16:33:58.884250 orbit_component_base-0.99.8/orbit_component_base/version.py
--rw-r--r--   0        0        0     1395 2023-05-31 16:33:58.884250 orbit_component_base-0.99.8/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 orbit_component_base-0.99.8/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/LICENSE.md
+-rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/README.md
+-rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/plugin.py
+-rw-r--r--   0        0        0     1020 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/schema/OrbitSessions.py
+-rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/schema/OrbitUsers.py
+-rwxr-xr-x   0        0        0     3506 2023-05-30 20:47:27.827498 orbit_component_base-0.99.9/orbit_component_base/src/orbit_app.py
+-rw-r--r--   0        0        0     6315 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_auth.py
+-rw-r--r--   0        0        0     6281 2023-05-30 16:47:54.685910 orbit_component_base-0.99.9/orbit_component_base/src/orbit_config.py
+-rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_database.py
+-rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_decorators.py
+-rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_logger.py
+-rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-0.99.9/orbit_component_base/src/orbit_make_ssl.py
+-rw-r--r--   0        0        0     8612 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql.py
+-rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_buffer.py
+-rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_emitter.py
+-rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_session.py
+-rw-r--r--   0        0        0     6409 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_orm.py
+-rw-r--r--   0        0        0     2293 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_plugin.py
+-rw-r--r--   0        0        0     1243 2023-05-30 15:19:20.192832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_plugins.py
+-rw-r--r--   0        0        0     2329 2023-05-30 21:39:29.016203 orbit_component_base-0.99.9/orbit_component_base/src/orbit_router.py
+-rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_shared.py
+-rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_version.py
+-rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-0.99.9/orbit_component_base/tests/test_main.py
+-rw-r--r--   0        0        0       23 2023-05-31 19:03:52.281919 orbit_component_base-0.99.9/orbit_component_base/version.py
+-rw-r--r--   0        0        0     1395 2023-05-31 19:03:52.281919 orbit_component_base-0.99.9/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 orbit_component_base-0.99.9/PKG-INFO
```

### Comparing `orbit_component_base-0.99.8/LICENSE.md` & `orbit_component_base-0.99.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/plugin.py` & `orbit_component_base-0.99.9/orbit_component_base/plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/schema/OrbitSessions.py` & `orbit_component_base-0.99.9/orbit_component_base/schema/OrbitSessions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_app.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_app.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_auth.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_auth.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_config.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_config.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_database.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_database.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_decorators.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_make_ssl.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_make_ssl.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_nql.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_nql_buffer.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_buffer.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_nql_emitter.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_emitter.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_nql_session.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_session.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_orm.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_orm.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_plugin.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_plugins.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_plugins.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_router.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_router.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/orbit_component_base/src/orbit_shared.py` & `orbit_component_base-0.99.9/orbit_component_base/src/orbit_shared.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.8/pyproject.toml` & `orbit_component_base-0.99.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-base"
-version = "0.99.8"
+version = "0.99.9"
 description = "Orbit Framework - base component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "orbit_component_base"}]
 include = ['README.md', 'LICENSE.md']
 keywords = ['orbit-framework', 'orbit-component', 'orbit-database']
```

### Comparing `orbit_component_base-0.99.8/PKG-INFO` & `orbit_component_base-0.99.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-base
-Version: 0.99.8
+Version: 0.99.9
 Summary: Orbit Framework - base component
 Home-page: https://gitlab.com/madpenguin/orbit-component-base
 License: MIT
 Keywords: orbit-framework,orbit-component,orbit-database
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
```

