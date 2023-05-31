# Comparing `tmp/orbit_component_zerodocs-0.99.1.tar.gz` & `tmp/orbit_component_zerodocs-0.99.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_zerodocs-0.99.1.tar", max compression
+gzip compressed data, was "orbit_component_zerodocs-0.99.2.tar", max compression
```

## Comparing `orbit_component_zerodocs-0.99.1.tar` & `orbit_component_zerodocs-0.99.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1099 2023-05-26 16:08:47.603359 orbit_component_zerodocs-0.99.1/LICENSE.md
--rw-r--r--   0        0        0      220 2023-05-30 11:47:07.159067 orbit_component_zerodocs-0.99.1/README.md
--rw-r--r--   0        0        0       71 2023-05-26 17:04:09.643103 orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/__init__.py
--rwxr-xr-x   0        0        0    19748 2023-05-07 17:05:52.145221 orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/doc_python.py
--rw-r--r--   0        0        0     1599 2023-05-26 17:01:55.709849 orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/plugin.py
--rw-r--r--   0        0        0     2934 2023-05-26 16:22:26.974231 orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/schema/APIs.py
--rw-r--r--   0        0        0    10754 2023-05-26 17:02:42.840883 orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/schema/Cache.py
--rw-r--r--   0        0        0     1814 2023-05-26 16:23:55.004404 orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/schema/Project.py
--rw-r--r--   0        0        0     1345 2023-05-30 11:48:43.192926 orbit_component_zerodocs-0.99.1/pyproject.toml
--rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 orbit_component_zerodocs-0.99.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:37.980465 orbit_component_zerodocs-0.99.2/LICENSE.md
+-rw-r--r--   0        0        0      220 2023-05-30 20:41:27.418669 orbit_component_zerodocs-0.99.2/README.md
+-rw-r--r--   0        0        0       71 2023-05-30 15:19:37.980465 orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/__init__.py
+-rwxr-xr-x   0        0        0    19748 2023-05-30 15:19:37.980465 orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/doc_python.py
+-rw-r--r--   0        0        0     1599 2023-05-30 15:19:37.980465 orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/plugin.py
+-rw-r--r--   0        0        0     2934 2023-05-30 15:19:37.980465 orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/schema/APIs.py
+-rw-r--r--   0        0        0    10754 2023-05-30 15:19:37.980465 orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/schema/Cache.py
+-rw-r--r--   0        0        0     1814 2023-05-30 15:19:37.980465 orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/schema/Project.py
+-rw-r--r--   0        0        0     1345 2023-05-31 13:07:09.524317 orbit_component_zerodocs-0.99.2/pyproject.toml
+-rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 orbit_component_zerodocs-0.99.2/PKG-INFO
```

### Comparing `orbit_component_zerodocs-0.99.1/LICENSE.md` & `orbit_component_zerodocs-0.99.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/doc_python.py` & `orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/doc_python.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/plugin.py` & `orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/schema/APIs.py` & `orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/schema/APIs.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/schema/Cache.py` & `orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/schema/Cache.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-0.99.1/orbit_component_zerodocs/schema/Project.py` & `orbit_component_zerodocs-0.99.2/orbit_component_zerodocs/schema/Project.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-0.99.1/pyproject.toml` & `orbit_component_zerodocs-0.99.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-zerodocs"
-version = "0.99.1"
+version = "0.99.2"
 description = "Orbit Component for inline documentation"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 include = ['README.md', 'LICENSE.md']
 packages = [{include = "orbit_component_zerodocs"}]
 classifiers = [
```

### Comparing `orbit_component_zerodocs-0.99.1/PKG-INFO` & `orbit_component_zerodocs-0.99.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-zerodocs
-Version: 0.99.1
+Version: 0.99.2
 Summary: Orbit Component for inline documentation
 Home-page: https://gitlab.com/madpenguin/orbit-component-zerodocs
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

