# Comparing `tmp/pylacus-1.4.2.tar.gz` & `tmp/pylacus-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylacus-1.4.2.tar", max compression
+gzip compressed data, was "pylacus-1.5.0.tar", max compression
```

## Comparing `pylacus-1.4.2.tar` & `pylacus-1.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1548 2022-09-21 08:51:05.297797 pylacus-1.4.2/LICENSE
--rw-r--r--   0        0        0     1246 2022-10-19 12:48:44.949008 pylacus-1.4.2/README.md
--rw-r--r--   0        0        0     1532 2022-09-22 10:52:07.800972 pylacus-1.4.2/pylacus/__init__.py
--rw-r--r--   0        0        0     8415 2022-11-01 13:48:16.210836 pylacus-1.4.2/pylacus/api.py
--rw-r--r--   0        0        0        0 2022-09-21 08:47:31.320167 pylacus-1.4.2/pylacus/py.typed
--rw-r--r--   0        0        0     1452 2023-05-23 13:26:00.992806 pylacus-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2720 1970-01-01 00:00:00.000000 pylacus-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1548 2022-09-21 08:51:05.297797 pylacus-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1246 2022-10-19 12:48:44.949008 pylacus-1.5.0/README.md
+-rw-r--r--   0        0        0     1532 2022-09-22 10:52:07.800972 pylacus-1.5.0/pylacus/__init__.py
+-rw-r--r--   0        0        0     8415 2022-11-01 13:48:16.210836 pylacus-1.5.0/pylacus/api.py
+-rw-r--r--   0        0        0        0 2022-09-21 08:47:31.320167 pylacus-1.5.0/pylacus/py.typed
+-rw-r--r--   0        0        0     1452 2023-05-31 14:22:28.750006 pylacus-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2720 1970-01-01 00:00:00.000000 pylacus-1.5.0/PKG-INFO
```

### Comparing `pylacus-1.4.2/LICENSE` & `pylacus-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylacus-1.4.2/README.md` & `pylacus-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pylacus-1.4.2/pylacus/__init__.py` & `pylacus-1.5.0/pylacus/__init__.py`

 * *Files identical despite different names*

### Comparing `pylacus-1.4.2/pylacus/api.py` & `pylacus-1.5.0/pylacus/api.py`

 * *Files identical despite different names*

### Comparing `pylacus-1.4.2/pyproject.toml` & `pylacus-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylacus"
-version = "1.4.2"
+version = "1.5.0"
 description = "Python CLI and module for lacus"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/PyLacus"
 documentation = "https://pylacus.readthedocs.io/en/latest/index.html"
 
 readme = "README.md"
@@ -34,15 +34,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 Sphinx = { version = "^7.0.1", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
-types-requests = "^2.31.0.0"
+types-requests = "^2.31.0.1"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.13.0", python = ">=3.9"}
 ]
 pytest = "^7.3.1"
 
 [tool.poetry.extras]
```

### Comparing `pylacus-1.4.2/PKG-INFO` & `pylacus-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylacus
-Version: 1.4.2
+Version: 1.5.0
 Summary: Python CLI and module for lacus
 Home-page: https://github.com/ail-project/PyLacus
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

