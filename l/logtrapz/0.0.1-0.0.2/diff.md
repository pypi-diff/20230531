# Comparing `tmp/logtrapz-0.0.1.tar.gz` & `tmp/logtrapz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logtrapz-0.0.1.tar", last modified: Wed May 31 15:55:08 2023, max compression
+gzip compressed data, was "logtrapz-0.0.2.tar", last modified: Wed May 31 16:07:04 2023, max compression
```

## Comparing `logtrapz-0.0.1.tar` & `logtrapz-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-31 15:55:08.113865 logtrapz-0.0.1/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1070 2023-05-31 15:31:17.000000 logtrapz-0.0.1/LICENSE
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      328 2023-05-31 15:55:08.113865 logtrapz-0.0.1/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       56 2023-05-31 15:32:05.000000 logtrapz-0.0.1/README.md
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-31 15:55:08.113865 logtrapz-0.0.1/logtrapz/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       30 2023-05-31 15:32:48.000000 logtrapz-0.0.1/logtrapz/__init__.py
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1837 2023-05-31 15:53:20.000000 logtrapz-0.0.1/logtrapz/logtrapz.py
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-31 15:55:08.113865 logtrapz-0.0.1/logtrapz.egg-info/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      328 2023-05-31 15:55:08.000000 logtrapz-0.0.1/logtrapz.egg-info/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      227 2023-05-31 15:55:08.000000 logtrapz-0.0.1/logtrapz.egg-info/SOURCES.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-05-31 15:55:08.000000 logtrapz-0.0.1/logtrapz.egg-info/dependency_links.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       12 2023-05-31 15:55:08.000000 logtrapz-0.0.1/logtrapz.egg-info/requires.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        9 2023-05-31 15:55:08.000000 logtrapz-0.0.1/logtrapz.egg-info/top_level.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-05-31 15:55:08.113865 logtrapz-0.0.1/setup.cfg
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      558 2023-05-31 15:54:52.000000 logtrapz-0.0.1/setup.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-31 16:07:04.214336 logtrapz-0.0.2/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1070 2023-05-31 15:31:17.000000 logtrapz-0.0.2/LICENSE
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      328 2023-05-31 16:07:04.210336 logtrapz-0.0.2/PKG-INFO
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       56 2023-05-31 15:32:05.000000 logtrapz-0.0.2/README.md
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-31 16:07:04.210336 logtrapz-0.0.2/logtrapz/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       31 2023-05-31 16:06:20.000000 logtrapz-0.0.2/logtrapz/__init__.py
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1837 2023-05-31 15:53:20.000000 logtrapz-0.0.2/logtrapz/logtrapz.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-31 16:07:04.210336 logtrapz-0.0.2/logtrapz.egg-info/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      328 2023-05-31 16:07:04.000000 logtrapz-0.0.2/logtrapz.egg-info/PKG-INFO
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      227 2023-05-31 16:07:04.000000 logtrapz-0.0.2/logtrapz.egg-info/SOURCES.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-05-31 16:07:04.000000 logtrapz-0.0.2/logtrapz.egg-info/dependency_links.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       12 2023-05-31 16:07:04.000000 logtrapz-0.0.2/logtrapz.egg-info/requires.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        9 2023-05-31 16:07:04.000000 logtrapz-0.0.2/logtrapz.egg-info/top_level.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-05-31 16:07:04.214336 logtrapz-0.0.2/setup.cfg
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      558 2023-05-31 16:06:40.000000 logtrapz-0.0.2/setup.py
```

### Comparing `logtrapz-0.0.1/LICENSE` & `logtrapz-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logtrapz-0.0.1/logtrapz/logtrapz.py` & `logtrapz-0.0.2/logtrapz/logtrapz.py`

 * *Files identical despite different names*

### Comparing `logtrapz-0.0.1/setup.py` & `logtrapz-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 name = 'logtrapz'
-version = '0.0.1'
+version = '0.0.2'
 
 with open('README.md' ,'r') as f:
     long_description = f.read().strip()
 
 setup(
     name=name,
     version=version,
```

