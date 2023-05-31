# Comparing `tmp/fnv-c-0.1.4.tar.gz` & `tmp/fnv-c-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fnv-c-0.1.4.tar", last modified: Tue May 30 15:55:23 2023, max compression
+gzip compressed data, was "dist/fnv-c-0.1.5.tar", last modified: Wed May 31 07:04:57 2023, max compression
```

## Comparing `fnv-c-0.1.4.tar` & `fnv-c-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:23.000000 fnv-c-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 15:55:09.000000 fnv-c-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 15:55:23.000000 fnv-c-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-30 15:55:09.000000 fnv-c-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/ext/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/ext/fnv.c
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/ext/fnv.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 15:55:09.000000 fnv-c-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:55:23.000000 fnv-c-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-30 15:55:21.000000 fnv-c-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:04:57.000000 fnv-c-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 07:04:43.000000 fnv-c-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-31 07:04:57.000000 fnv-c-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-31 07:04:43.000000 fnv-c-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:04:57.000000 fnv-c-0.1.5/fnv_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-31 07:04:43.000000 fnv-c-0.1.5/fnv_c/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:04:57.000000 fnv-c-0.1.5/fnv_c/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:04:43.000000 fnv-c-0.1.5/fnv_c/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-31 07:04:43.000000 fnv-c-0.1.5/fnv_c/ext/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 07:04:43.000000 fnv-c-0.1.5/fnv_c/ext/fnv.c
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-31 07:04:43.000000 fnv-c-0.1.5/fnv_c/ext/fnv.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:04:57.000000 fnv-c-0.1.5/fnv_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-31 07:04:56.000000 fnv-c-0.1.5/fnv_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 07:04:57.000000 fnv-c-0.1.5/fnv_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:04:56.000000 fnv-c-0.1.5/fnv_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 07:04:56.000000 fnv-c-0.1.5/fnv_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 07:04:56.000000 fnv-c-0.1.5/fnv_c.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-31 07:04:43.000000 fnv-c-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:04:57.000000 fnv-c-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-31 07:04:55.000000 fnv-c-0.1.5/setup.py
```

### Comparing `fnv-c-0.1.4/fnv_c/__init__.py` & `fnv-c-0.1.5/fnv_c/__init__.py`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.4/fnv_c/ext/fnv.c` & `fnv-c-0.1.5/fnv_c/ext/fnv.c`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.4/setup.py` & `fnv-c-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 
 DESCRIPTION = "Python 3.7+ FNV (fnv0, fnv1, fnv1a) non-cryptographic hash library implemented in C through libffi"
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 
 setup(
```

