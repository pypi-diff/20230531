# Comparing `tmp/jupyter2pytest-0.3.1.tar.gz` & `tmp/jupyter2pytest-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter2pytest-0.3.1.tar", last modified: Wed May 31 20:03:29 2023, max compression
+gzip compressed data, was "jupyter2pytest-0.3.2.tar", max compression
```

## Comparing `jupyter2pytest-0.3.1.tar` & `jupyter2pytest-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,11 @@
-drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-31 20:03:29.866543 jupyter2pytest-0.3.1/
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     1079 2023-05-31 20:02:34.000000 jupyter2pytest-0.3.1/LICENSE
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     2897 2023-05-31 20:03:29.866543 jupyter2pytest-0.3.1/PKG-INFO
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      913 2023-05-31 20:02:34.000000 jupyter2pytest-0.3.1/README.md
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      763 2023-05-31 20:03:22.000000 jupyter2pytest-0.3.1/pyproject.toml
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)       38 2023-05-31 20:03:29.866543 jupyter2pytest-0.3.1/setup.cfg
-drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-31 20:03:29.865543 jupyter2pytest-0.3.1/src/
-drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-31 20:03:29.865543 jupyter2pytest-0.3.1/src/jupyter2pytest/
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-31 20:02:34.000000 jupyter2pytest-0.3.1/src/jupyter2pytest/__init__.py
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      489 2023-05-31 20:02:34.000000 jupyter2pytest-0.3.1/src/jupyter2pytest/__main__.py
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     2563 2023-05-31 20:02:34.000000 jupyter2pytest-0.3.1/src/jupyter2pytest/compiler.py
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     4371 2023-05-31 20:02:34.000000 jupyter2pytest-0.3.1/src/jupyter2pytest/extractor.py
-drwxr-xr-x   0 ddxtanx   (1000) ddxtanx   (1000)        0 2023-05-31 20:03:29.866543 jupyter2pytest-0.3.1/src/jupyter2pytest.egg-info/
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)     2897 2023-05-31 20:03:29.000000 jupyter2pytest-0.3.1/src/jupyter2pytest.egg-info/PKG-INFO
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)      366 2023-05-31 20:03:29.000000 jupyter2pytest-0.3.1/src/jupyter2pytest.egg-info/SOURCES.txt
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)        1 2023-05-31 20:03:29.000000 jupyter2pytest-0.3.1/src/jupyter2pytest.egg-info/dependency_links.txt
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)       15 2023-05-31 20:03:29.000000 jupyter2pytest-0.3.1/src/jupyter2pytest.egg-info/requires.txt
--rw-r--r--   0 ddxtanx   (1000) ddxtanx   (1000)       15 2023-05-31 20:03:29.000000 jupyter2pytest-0.3.1/src/jupyter2pytest.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1079 2023-05-31 20:02:34.128671 jupyter2pytest-0.3.2/LICENSE
+-rw-r--r--   0        0        0      913 2023-05-31 20:02:34.128671 jupyter2pytest-0.3.2/README.md
+-rw-r--r--   0        0        0      749 2023-05-31 20:18:23.961342 jupyter2pytest-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 20:02:34.128671 jupyter2pytest-0.3.2/src/jupyter2pytest/__init__.py
+-rw-r--r--   0        0        0      489 2023-05-31 20:02:34.128671 jupyter2pytest-0.3.2/src/jupyter2pytest/__main__.py
+-rw-r--r--   0        0        0     2563 2023-05-31 20:02:34.128671 jupyter2pytest-0.3.2/src/jupyter2pytest/compiler.py
+-rw-r--r--   0        0        0     4371 2023-05-31 20:02:34.129671 jupyter2pytest-0.3.2/src/jupyter2pytest/extractor.py
+-rw-r--r--   0        0        0      164 2023-05-31 20:02:34.129671 jupyter2pytest-0.3.2/src/jupyter2pytest/test_code_block_template.py.template
+-rw-r--r--   0        0        0     1020 2023-05-31 20:02:34.129671 jupyter2pytest-0.3.2/src/jupyter2pytest/test_file_template.py.template
+-rw-r--r--   0        0        0      318 2023-05-31 20:02:34.129671 jupyter2pytest-0.3.2/src/jupyter2pytest/test_function_template.py.template
+-rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 jupyter2pytest-0.3.2/PKG-INFO
```

### Comparing `jupyter2pytest-0.3.1/LICENSE` & `jupyter2pytest-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter2pytest-0.3.1/README.md` & `jupyter2pytest-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyter2pytest-0.3.1/src/jupyter2pytest/compiler.py` & `jupyter2pytest-0.3.2/src/jupyter2pytest/compiler.py`

 * *Files identical despite different names*

### Comparing `jupyter2pytest-0.3.1/src/jupyter2pytest/extractor.py` & `jupyter2pytest-0.3.2/src/jupyter2pytest/extractor.py`

 * *Files identical despite different names*

