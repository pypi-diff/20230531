# Comparing `tmp/crxcavatorpy-0.1.0.tar.gz` & `tmp/crxcavatorpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crxcavatorpy-0.1.0.tar", max compression
+gzip compressed data, was "crxcavatorpy-0.1.1.tar", max compression
```

## Comparing `crxcavatorpy-0.1.0.tar` & `crxcavatorpy-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      120 2023-05-31 17:48:49.679892 crxcavatorpy-0.1.0/README.md
--rw-r--r--   0        0        0       51 2023-05-31 17:48:49.679892 crxcavatorpy-0.1.0/crxcavator/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-31 17:48:49.679892 crxcavatorpy-0.1.0/crxcavator/__main__.py
--rw-r--r--   0        0        0      911 2023-05-31 17:48:49.679892 crxcavatorpy-0.1.0/crxcavator/api.py
--rw-r--r--   0        0        0      727 2023-05-31 17:48:49.679892 crxcavatorpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 crxcavatorpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      120 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/README.md
+-rw-r--r--   0        0        0       51 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/crxcavator/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/crxcavator/__main__.py
+-rw-r--r--   0        0        0      911 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/crxcavator/api.py
+-rw-r--r--   0        0        0      729 2023-05-31 18:02:24.934803 crxcavatorpy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 crxcavatorpy-0.1.1/PKG-INFO
```

### Comparing `crxcavatorpy-0.1.0/crxcavator/__main__.py` & `crxcavatorpy-0.1.1/crxcavator/__main__.py`

 * *Files identical despite different names*

### Comparing `crxcavatorpy-0.1.0/crxcavator/api.py` & `crxcavatorpy-0.1.1/crxcavator/api.py`

 * *Files identical despite different names*

### Comparing `crxcavatorpy-0.1.0/pyproject.toml` & `crxcavatorpy-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "crxcavatorpy"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python module for interacting with the Crxcavator api"
 authors = ["Garrett Primm <garrett@alabamacloudsecurity.com>"]
 readme = "README.md"
 packages = [
     { include = "crxcavator" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.8.1"
 requests = "^2.31.0"
 argparse = "^1.4.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
```

