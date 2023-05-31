# Comparing `tmp/un_yaml-0.1.0.tar.gz` & `tmp/un_yaml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "un_yaml-0.1.0.tar", max compression
+gzip compressed data, was "un_yaml-0.1.1.tar", max compression
```

## Comparing `un_yaml-0.1.0.tar` & `un_yaml-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.1.0/LICENSE
--rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.1.0/README.md
--rw-r--r--   0        0        0      705 2023-05-31 12:54:36.389004 un_yaml-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      120 2023-05-31 12:54:36.392580 un_yaml-0.1.0/un_yaml/__init__.py
--rw-r--r--   0        0        0     3728 2023-05-31 12:54:36.393070 un_yaml-0.1.0/un_yaml/un_cli.py
--rw-r--r--   0        0        0     1420 2023-05-31 12:54:36.393499 un_yaml-0.1.0/un_yaml/un_uri.py
--rw-r--r--   0        0        0     2180 2023-05-31 12:54:36.393871 un_yaml-0.1.0/un_yaml/un_yaml.py
--rw-r--r--   0        0        0       23 2023-05-31 12:54:36.394198 un_yaml-0.1.0/un_yaml/wrapper.py
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 un_yaml-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.1.1/LICENSE
+-rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.1.1/README.md
+-rw-r--r--   0        0        0      652 2023-05-31 13:33:07.339502 un_yaml-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-05-31 13:33:07.341430 un_yaml-0.1.1/un_yaml/__init__.py
+-rw-r--r--   0        0        0     3728 2023-05-31 12:54:36.393070 un_yaml-0.1.1/un_yaml/un_cli.py
+-rw-r--r--   0        0        0     1420 2023-05-31 12:54:36.393499 un_yaml-0.1.1/un_yaml/un_uri.py
+-rw-r--r--   0        0        0     2180 2023-05-31 12:54:36.393871 un_yaml-0.1.1/un_yaml/un_yaml.py
+-rw-r--r--   0        0        0       24 2023-05-31 13:33:07.342331 un_yaml-0.1.1/un_yaml/wrapper.py
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 un_yaml-0.1.1/PKG-INFO
```

### Comparing `un_yaml-0.1.0/LICENSE` & `un_yaml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `un_yaml-0.1.0/pyproject.toml` & `un_yaml-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "un_yaml"
-version = "0.1.0"
+version = "0.1.1"
 description = "Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anyio = "^3.7.0"
@@ -17,13 +17,10 @@
 pytest-coverage = "^0.0"
 pytest-watcher = "^0.2.6"
 pytest-asyncio = "^0.21.0"
 pytest-trio = "^0.8.0"
 pytest-codeblocks = "^0.16.1"
 ipykernel = "^6.23.1"
 
-[tool.poetry.scripts]
-un-yaml = "un-yaml.main:main"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `un_yaml-0.1.0/un_yaml/un_cli.py` & `un_yaml-0.1.1/un_yaml/un_cli.py`

 * *Files identical despite different names*

### Comparing `un_yaml-0.1.0/un_yaml/un_uri.py` & `un_yaml-0.1.1/un_yaml/un_uri.py`

 * *Files identical despite different names*

### Comparing `un_yaml-0.1.0/un_yaml/un_yaml.py` & `un_yaml-0.1.1/un_yaml/un_yaml.py`

 * *Files identical despite different names*

### Comparing `un_yaml-0.1.0/PKG-INFO` & `un_yaml-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: un-yaml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

