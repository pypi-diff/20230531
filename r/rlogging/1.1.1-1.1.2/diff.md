# Comparing `tmp/rlogging-1.1.1.tar.gz` & `tmp/rlogging-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlogging-1.1.1.tar", max compression
+gzip compressed data, was "rlogging-1.1.2.tar", max compression
```

## Comparing `rlogging-1.1.1.tar` & `rlogging-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1393 2023-04-21 20:02:47.376896 rlogging-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      456 2023-04-21 20:02:47.376896 rlogging-1.1.1/readme.md
--rw-r--r--   0        0        0       65 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/__init__.py
--rw-r--r--   0        0        0     3208 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/adapters.py
--rw-r--r--   0        0        0      270 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/filters.py
--rw-r--r--   0        0        0     2339 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/formatters.py
--rw-r--r--   0        0        0      945 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/handlers.py
--rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/aiogram/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/django/__init__.py
--rw-r--r--   0        0        0      740 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/adapters.py
--rw-r--r--   0        0        0      125 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/admin.py
--rw-r--r--   0        0        0      267 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/apps.py
--rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/django/handlers.py
--rw-r--r--   0        0        0     1483 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/middleware.py
--rw-r--r--   0        0        0       72 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/models.py
--rw-r--r--   0        0        0     2019 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/signals.py
--rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/fastapi/__init__.py
--rw-r--r--   0        0        0       50 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/namespaces.py
--rw-r--r--   0        0        0     1509 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/utils.py
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 rlogging-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1393 2023-05-31 06:47:27.811892 rlogging-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      456 2023-05-31 06:47:27.811892 rlogging-1.1.2/readme.md
+-rw-r--r--   0        0        0       65 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/__init__.py
+-rw-r--r--   0        0        0     3208 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/adapters.py
+-rw-r--r--   0        0        0      270 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/filters.py
+-rw-r--r--   0        0        0     2339 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/formatters.py
+-rw-r--r--   0        0        0      945 2023-05-31 06:47:27.811892 rlogging-1.1.2/rlogging/handlers.py
+-rw-r--r--   0        0        0        0 2023-05-31 06:47:27.951892 rlogging-1.1.2/rlogging/integration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 06:47:27.959892 rlogging-1.1.2/rlogging/integration/aiogram/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 06:47:27.959892 rlogging-1.1.2/rlogging/integration/django/__init__.py
+-rw-r--r--   0        0        0      740 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/adapters.py
+-rw-r--r--   0        0        0      125 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/admin.py
+-rw-r--r--   0        0        0      271 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/apps.py
+-rw-r--r--   0        0        0        0 2023-05-31 06:47:27.959892 rlogging-1.1.2/rlogging/integration/django/handlers.py
+-rw-r--r--   0        0        0     1483 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/middleware.py
+-rw-r--r--   0        0        0       72 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/models.py
+-rw-r--r--   0        0        0     2019 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/integration/django/signals.py
+-rw-r--r--   0        0        0        0 2023-05-31 06:47:27.959892 rlogging-1.1.2/rlogging/integration/fastapi/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/namespaces.py
+-rw-r--r--   0        0        0     1509 2023-05-31 06:47:27.819892 rlogging-1.1.2/rlogging/utils.py
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 rlogging-1.1.2/PKG-INFO
```

### Comparing `rlogging-1.1.1/pyproject.toml` & `rlogging-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.1/rlogging/adapters.py` & `rlogging-1.1.2/rlogging/adapters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.1/rlogging/formatters.py` & `rlogging-1.1.2/rlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.1/rlogging/handlers.py` & `rlogging-1.1.2/rlogging/handlers.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.1/rlogging/integration/django/adapters.py` & `rlogging-1.1.2/rlogging/integration/django/adapters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.1/rlogging/integration/django/middleware.py` & `rlogging-1.1.2/rlogging/integration/django/middleware.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.1/rlogging/integration/django/signals.py` & `rlogging-1.1.2/rlogging/integration/django/signals.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.1/rlogging/utils.py` & `rlogging-1.1.2/rlogging/utils.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.1/PKG-INFO` & `rlogging-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlogging
-Version: 1.1.1
+Version: 1.1.2
 Summary: 
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

