# Comparing `tmp/orbit_component_vcheck-0.99.1.tar.gz` & `tmp/orbit_component_vcheck-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_vcheck-0.99.1.tar", max compression
+gzip compressed data, was "orbit_component_vcheck-1.0.1.tar", max compression
```

## Comparing `orbit_component_vcheck-0.99.1.tar` & `orbit_component_vcheck-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1099 2023-05-26 17:26:20.263090 orbit_component_vcheck-0.99.1/LICENSE.md
--rw-r--r--   0        0        0      332 2023-05-26 17:27:54.657112 orbit_component_vcheck-0.99.1/README.md
--rw-r--r--   0        0        0       81 2023-05-26 17:22:41.859681 orbit_component_vcheck-0.99.1/orbit_component_vcheck/__init__.py
--rw-r--r--   0        0        0     2749 2023-05-26 17:28:47.268010 orbit_component_vcheck-0.99.1/orbit_component_vcheck/plugin.py
--rw-r--r--   0        0        0      810 2023-05-26 20:01:44.781520 orbit_component_vcheck-0.99.1/orbit_component_vcheck/schema/Sessions.py
--rw-r--r--   0        0        0      554 2023-05-26 20:02:03.721114 orbit_component_vcheck-0.99.1/orbit_component_vcheck/schema/Users.py
--rw-r--r--   0        0        0     1841 2023-05-26 20:02:31.976533 orbit_component_vcheck-0.99.1/orbit_component_vcheck/schema/Versions.py
--rw-r--r--   0        0        0      206 2023-05-25 11:52:53.142169 orbit_component_vcheck-0.99.1/orbit_component_vcheck/src/cli_base.py
--rw-r--r--   0        0        0     1577 2023-05-26 17:28:47.268010 orbit_component_vcheck-0.99.1/orbit_component_vcheck/src/sessions.py
--rw-r--r--   0        0        0     2002 2023-05-26 17:29:52.994636 orbit_component_vcheck-0.99.1/orbit_component_vcheck/src/users.py
--rw-r--r--   0        0        0     1779 2023-05-26 17:30:18.286108 orbit_component_vcheck-0.99.1/orbit_component_vcheck/src/versions.py
--rw-r--r--   0        0        0     1160 2023-05-30 11:56:37.882336 orbit_component_vcheck-0.99.1/pyproject.toml
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 orbit_component_vcheck-0.99.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0      332 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/README.md
+-rw-r--r--   0        0        0       81 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/orbit_component_vcheck/__init__.py
+-rw-r--r--   0        0        0     2749 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/orbit_component_vcheck/plugin.py
+-rw-r--r--   0        0        0      810 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/orbit_component_vcheck/schema/Sessions.py
+-rw-r--r--   0        0        0      554 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/orbit_component_vcheck/schema/Users.py
+-rw-r--r--   0        0        0     1841 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/orbit_component_vcheck/schema/Versions.py
+-rw-r--r--   0        0        0      206 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/orbit_component_vcheck/src/cli_base.py
+-rw-r--r--   0        0        0     1577 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/orbit_component_vcheck/src/sessions.py
+-rw-r--r--   0        0        0     2002 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/orbit_component_vcheck/src/users.py
+-rw-r--r--   0        0        0     1779 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.1/orbit_component_vcheck/src/versions.py
+-rw-r--r--   0        0        0     1159 2023-05-31 10:02:21.474414 orbit_component_vcheck-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 orbit_component_vcheck-1.0.1/PKG-INFO
```

### Comparing `orbit_component_vcheck-0.99.1/LICENSE.md` & `orbit_component_vcheck-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-0.99.1/orbit_component_vcheck/plugin.py` & `orbit_component_vcheck-1.0.1/orbit_component_vcheck/plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-0.99.1/orbit_component_vcheck/schema/Sessions.py` & `orbit_component_vcheck-1.0.1/orbit_component_vcheck/schema/Sessions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-0.99.1/orbit_component_vcheck/schema/Users.py` & `orbit_component_vcheck-1.0.1/orbit_component_vcheck/schema/Users.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-0.99.1/orbit_component_vcheck/schema/Versions.py` & `orbit_component_vcheck-1.0.1/orbit_component_vcheck/schema/Versions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-0.99.1/orbit_component_vcheck/src/sessions.py` & `orbit_component_vcheck-1.0.1/orbit_component_vcheck/src/sessions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-0.99.1/orbit_component_vcheck/src/users.py` & `orbit_component_vcheck-1.0.1/orbit_component_vcheck/src/users.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-0.99.1/orbit_component_vcheck/src/versions.py` & `orbit_component_vcheck-1.0.1/orbit_component_vcheck/src/versions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-0.99.1/pyproject.toml` & `orbit_component_vcheck-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-vcheck"
-version = "0.99.1"
+version = "1.0.1"
 description = "Orbit Component to track product versions"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 include = ['README.md', 'LICENSE.md']
 packages = [{include = "orbit_component_vcheck"}]
 classifiers = [
```

### Comparing `orbit_component_vcheck-0.99.1/PKG-INFO` & `orbit_component_vcheck-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-vcheck
-Version: 0.99.1
+Version: 1.0.1
 Summary: Orbit Component to track product versions
 Home-page: https://gitlab.com/madpenguin/orbit-component-vcheck
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

