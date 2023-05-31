# Comparing `tmp/cnert-0.6.0.tar.gz` & `tmp/cnert-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnert-0.6.0.tar", max compression
+gzip compressed data, was "cnert-0.7.0.tar", max compression
```

## Comparing `cnert-0.6.0.tar` & `cnert-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.6.0/LICENSE
--rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.6.0/LICENSE.apache2
--rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.6.0/LICENSE.mit
--rw-r--r--   0        0        0     7748 2023-05-10 14:30:59.900805 cnert-0.6.0/README.md
--rw-r--r--   0        0        0     3150 2023-05-14 10:48:27.274639 cnert-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    26063 2023-05-14 10:48:27.305032 cnert-0.6.0/src/cnert/__init__.py
--rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.6.0/src/cnert/py.typed
--rw-r--r--   0        0        0     9512 1970-01-01 00:00:00.000000 cnert-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.7.0/LICENSE
+-rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.7.0/LICENSE.apache2
+-rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.7.0/LICENSE.mit
+-rw-r--r--   0        0        0     7748 2023-05-10 14:30:59.900805 cnert-0.7.0/README.md
+-rw-r--r--   0        0        0     3150 2023-05-31 09:55:13.663823 cnert-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    26246 2023-05-31 09:55:13.694605 cnert-0.7.0/src/cnert/__init__.py
+-rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.7.0/src/cnert/py.typed
+-rw-r--r--   0        0        0     9512 1970-01-01 00:00:00.000000 cnert-0.7.0/PKG-INFO
```

### Comparing `cnert-0.6.0/LICENSE.apache2` & `cnert-0.7.0/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `cnert-0.6.0/LICENSE.mit` & `cnert-0.7.0/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `cnert-0.6.0/README.md` & `cnert-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cnert-0.6.0/pyproject.toml` & `cnert-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cnert"
-version = "0.6.0"
+version = "0.7.0"
 description = "Cnert is trying to be a simple API for creating TLS Certificates testing purposes."
 authors = ["Maarten <ikmaarten@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maartenq/cnert"
 repository = "https://github.com/maartenq/cnert"
 documentation = "https://cnert.readthedocs.io/en/latest/"
```

### Comparing `cnert-0.6.0/PKG-INFO` & `cnert-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnert
-Version: 0.6.0
+Version: 0.7.0
 Summary: Cnert is trying to be a simple API for creating TLS Certificates testing purposes.
 Home-page: https://github.com/maartenq/cnert
 License: MIT
 Keywords: certificate,X.509,TLS,cryptography,testing
 Author: Maarten
 Author-email: ikmaarten@gmail.com
 Requires-Python: >=3.9,<4.0
```

