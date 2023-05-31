# Comparing `tmp/eodc-2023.5.2.tar.gz` & `tmp/eodc-2023.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.5.2.tar", max compression
+gzip compressed data, was "eodc-2023.5.3.tar", max compression
```

## Comparing `eodc-2023.5.2.tar` & `eodc-2023.5.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-05-30 19:27:13.728942 eodc-2023.5.2/README.md
--rw-r--r--   0        0        0      213 2023-05-30 19:27:13.728942 eodc-2023.5.2/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-05-30 19:27:13.728942 eodc-2023.5.2/eodc/dask.py
--rw-r--r--   0        0        0      590 2023-05-30 19:27:13.728942 eodc-2023.5.2/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-05-30 19:27:13.728942 eodc-2023.5.2/eodc/settings.py
--rw-r--r--   0        0        0     1114 2023-05-30 19:27:13.728942 eodc-2023.5.2/pyproject.toml
--rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 eodc-2023.5.2/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-05-31 06:57:59.894315 eodc-2023.5.3/README.md
+-rw-r--r--   0        0        0      213 2023-05-31 06:57:59.894315 eodc-2023.5.3/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-05-31 06:57:59.894315 eodc-2023.5.3/eodc/dask.py
+-rw-r--r--   0        0        0      757 2023-05-31 06:57:59.894315 eodc-2023.5.3/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-05-31 06:57:59.894315 eodc-2023.5.3/eodc/settings.py
+-rw-r--r--   0        0        0     1114 2023-05-31 06:57:59.894315 eodc-2023.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 eodc-2023.5.3/PKG-INFO
```

### Comparing `eodc-2023.5.2/README.md` & `eodc-2023.5.3/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.5.2/eodc/dask.py` & `eodc-2023.5.3/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.5.2/pyproject.toml` & `eodc-2023.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.5.2"
+version = "2023.5.3"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2023.5.2/PKG-INFO` & `eodc-2023.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.5.2
+Version: 2023.5.3
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

