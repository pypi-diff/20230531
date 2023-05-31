# Comparing `tmp/crxcavatorpy-0.1.2.tar.gz` & `tmp/crxcavatorpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crxcavatorpy-0.1.2.tar", max compression
+gzip compressed data, was "crxcavatorpy-0.1.3.tar", max compression
```

## Comparing `crxcavatorpy-0.1.2.tar` & `crxcavatorpy-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      120 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/README.md
--rw-r--r--   0        0        0       51 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/crxcavator/__init__.py
--rw-r--r--   0        0        0     1643 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/crxcavator/__main__.py
--rw-r--r--   0        0        0      911 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/crxcavator/api.py
--rw-r--r--   0        0        0      729 2023-05-31 18:23:03.735989 crxcavatorpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 crxcavatorpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1178 2023-05-31 19:00:51.598354 crxcavatorpy-0.1.3/README.md
+-rw-r--r--   0        0        0       51 2023-05-31 19:00:51.598354 crxcavatorpy-0.1.3/crxcavator/__init__.py
+-rw-r--r--   0        0        0     1643 2023-05-31 19:00:51.598354 crxcavatorpy-0.1.3/crxcavator/__main__.py
+-rw-r--r--   0        0        0      911 2023-05-31 19:00:51.598354 crxcavatorpy-0.1.3/crxcavator/api.py
+-rw-r--r--   0        0        0      729 2023-05-31 19:00:51.602354 crxcavatorpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1716 1970-01-01 00:00:00.000000 crxcavatorpy-0.1.3/PKG-INFO
```

### Comparing `crxcavatorpy-0.1.2/crxcavator/__main__.py` & `crxcavatorpy-0.1.3/crxcavator/__main__.py`

 * *Files identical despite different names*

### Comparing `crxcavatorpy-0.1.2/crxcavator/api.py` & `crxcavatorpy-0.1.3/crxcavator/api.py`

 * *Files identical despite different names*

### Comparing `crxcavatorpy-0.1.2/pyproject.toml` & `crxcavatorpy-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crxcavatorpy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python module for interacting with the Crxcavator api"
 authors = ["Garrett Primm <garrett@alabamacloudsecurity.com>"]
 readme = "README.md"
 packages = [
     { include = "crxcavator" }
 ]
```

