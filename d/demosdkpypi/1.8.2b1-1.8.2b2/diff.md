# Comparing `tmp/demosdkpypi-1.8.2b1.tar.gz` & `tmp/demosdkpypi-1.8.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demosdkpypi-1.8.2b1.tar", last modified: Wed May 31 17:59:30 2023, max compression
+gzip compressed data, was "demosdkpypi-1.8.2b2.tar", last modified: Wed May 31 18:05:00 2023, max compression
```

## Comparing `demosdkpypi-1.8.2b1.tar` & `demosdkpypi-1.8.2b2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:30.427224 demosdkpypi-1.8.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 17:59:30.427224 demosdkpypi-1.8.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 17:59:12.000000 demosdkpypi-1.8.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:30.423224 demosdkpypi-1.8.2b1/demosdkpypi/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 17:59:12.000000 demosdkpypi-1.8.2b1/demosdkpypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 17:59:12.000000 demosdkpypi-1.8.2b1/demosdkpypi/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:30.427224 demosdkpypi-1.8.2b1/demosdkpypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 17:59:30.000000 demosdkpypi-1.8.2b1/demosdkpypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-31 17:59:30.000000 demosdkpypi-1.8.2b1/demosdkpypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:59:30.000000 demosdkpypi-1.8.2b1/demosdkpypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 17:59:30.000000 demosdkpypi-1.8.2b1/demosdkpypi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:59:30.427224 demosdkpypi-1.8.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-31 17:59:27.000000 demosdkpypi-1.8.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 18:04:49.000000 demosdkpypi-1.8.2b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/demosdkpypi/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 18:04:49.000000 demosdkpypi-1.8.2b2/demosdkpypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 18:04:49.000000 demosdkpypi-1.8.2b2/demosdkpypi/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 18:05:00.000000 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-31 18:05:00.000000 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:05:00.000000 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 18:05:00.000000 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-31 18:04:58.000000 demosdkpypi-1.8.2b2/setup.py
```

### Comparing `demosdkpypi-1.8.2b1/setup.py` & `demosdkpypi-1.8.2b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import sys
 
 if sys.version_info < (3, 7):
     raise RuntimeError("my demo requires Python 3.7+")
-current_version = '1.8.2beta1'
+current_version = '1.8.2beta2'
 
 setup(
     name='demosdkpypi',
     version=current_version,
     author='Bharti',
     author_email='bharti.sagar@skyflow.com',
     packages=find_packages(),
```

