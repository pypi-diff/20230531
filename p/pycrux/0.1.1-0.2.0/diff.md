# Comparing `tmp/pycrux-0.1.1.tar.gz` & `tmp/pycrux-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrux-0.1.1.tar", max compression
+gzip compressed data, was "pycrux-0.2.0.tar", max compression
```

## Comparing `pycrux-0.1.1.tar` & `pycrux-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-05-30 13:54:53.299492 pycrux-0.1.1/LICENSE
--rw-r--r--   0        0        0       85 2023-05-30 20:24:52.720158 pycrux-0.1.1/pycrux/__init__.py
--rw-r--r--   0        0        0     3494 2023-05-31 10:55:02.634701 pycrux-0.1.1/pycrux/crux.py
--rw-r--r--   0        0        0        0 2023-05-30 13:54:53.314684 pycrux-0.1.1/pycrux/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-30 13:54:53.314102 pycrux-0.1.1/pycrux/utils/config.py
--rw-r--r--   0        0        0      731 2023-05-30 14:16:53.108904 pycrux-0.1.1/pycrux/utils/logger.py
--rw-r--r--   0        0        0      925 2023-05-31 11:10:12.474853 pycrux-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 pycrux-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-30 13:54:53.299492 pycrux-0.2.0/LICENSE
+-rw-r--r--   0        0        0       85 2023-05-30 20:24:52.720158 pycrux-0.2.0/pycrux/__init__.py
+-rw-r--r--   0        0        0     3494 2023-05-31 10:55:02.634701 pycrux-0.2.0/pycrux/crux.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:54:53.314684 pycrux-0.2.0/pycrux/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-30 13:54:53.314102 pycrux-0.2.0/pycrux/utils/config.py
+-rw-r--r--   0        0        0      731 2023-05-30 14:16:53.108904 pycrux-0.2.0/pycrux/utils/logger.py
+-rw-r--r--   0        0        0      925 2023-05-31 11:12:08.018004 pycrux-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 pycrux-0.2.0/PKG-INFO
```

### Comparing `pycrux-0.1.1/LICENSE` & `pycrux-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrux-0.1.1/pycrux/crux.py` & `pycrux-0.2.0/pycrux/crux.py`

 * *Files identical despite different names*

### Comparing `pycrux-0.1.1/pycrux/utils/config.py` & `pycrux-0.2.0/pycrux/utils/config.py`

 * *Files identical despite different names*

### Comparing `pycrux-0.1.1/pycrux/utils/logger.py` & `pycrux-0.2.0/pycrux/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pycrux-0.1.1/pyproject.toml` & `pycrux-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycrux"
-version = "0.1.1"
+version = "0.2.0"
 description = "A python wrapper for crFitTool."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 homepage = "https://github.com/WahooFitness/pycrux"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 pandas = "^2.0.2"
```

