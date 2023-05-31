# Comparing `tmp/rach_pack-0.3.0.tar.gz` & `tmp/rach_pack-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rach_pack-0.3.0.tar", last modified: Wed May 31 15:28:59 2023, max compression
+gzip compressed data, was "rach_pack-0.4.0.tar", last modified: Wed May 31 15:40:56 2023, max compression
```

## Comparing `rach_pack-0.3.0.tar` & `rach_pack-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 15:28:59.594110 rach_pack-0.3.0/
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      596 2023-05-31 15:28:59.594110 rach_pack-0.3.0/PKG-INFO
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      364 2023-05-31 13:04:04.000000 rach_pack-0.3.0/README.md
-drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 15:28:59.590110 rach_pack-0.3.0/rach_pack/
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       36 2023-05-31 15:22:35.000000 rach_pack-0.3.0/rach_pack/__init__.py
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       57 2023-05-31 14:54:04.000000 rach_pack-0.3.0/rach_pack/main.py
-drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 15:28:59.590110 rach_pack-0.3.0/rach_pack.egg-info/
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      596 2023-05-31 15:28:59.000000 rach_pack-0.3.0/rach_pack.egg-info/PKG-INFO
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      190 2023-05-31 15:28:59.000000 rach_pack-0.3.0/rach_pack.egg-info/SOURCES.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)        1 2023-05-31 15:28:59.000000 rach_pack-0.3.0/rach_pack.egg-info/dependency_links.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       10 2023-05-31 15:28:59.000000 rach_pack-0.3.0/rach_pack.egg-info/top_level.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       38 2023-05-31 15:28:59.594110 rach_pack-0.3.0/setup.cfg
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      663 2023-05-31 15:28:54.000000 rach_pack-0.3.0/setup.py
+drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 15:40:56.922683 rach_pack-0.4.0/
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      596 2023-05-31 15:40:56.922683 rach_pack-0.4.0/PKG-INFO
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      364 2023-05-31 13:04:04.000000 rach_pack-0.4.0/README.md
+drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 15:40:56.922683 rach_pack-0.4.0/rach_pack/
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       46 2023-05-31 15:40:47.000000 rach_pack-0.4.0/rach_pack/__init__.py
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       57 2023-05-31 14:54:04.000000 rach_pack-0.4.0/rach_pack/main.py
+drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 15:40:56.922683 rach_pack-0.4.0/rach_pack.egg-info/
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      596 2023-05-31 15:40:56.000000 rach_pack-0.4.0/rach_pack.egg-info/PKG-INFO
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      190 2023-05-31 15:40:56.000000 rach_pack-0.4.0/rach_pack.egg-info/SOURCES.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)        1 2023-05-31 15:40:56.000000 rach_pack-0.4.0/rach_pack.egg-info/dependency_links.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       10 2023-05-31 15:40:56.000000 rach_pack-0.4.0/rach_pack.egg-info/top_level.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       38 2023-05-31 15:40:56.922683 rach_pack-0.4.0/setup.cfg
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      663 2023-05-31 15:40:36.000000 rach_pack-0.4.0/setup.py
```

### Comparing `rach_pack-0.3.0/PKG-INFO` & `rach_pack-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rach_pack
-Version: 0.3.0
+Version: 0.4.0
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `rach_pack-0.3.0/rach_pack.egg-info/PKG-INFO` & `rach_pack-0.4.0/rach_pack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rach-pack
-Version: 0.3.0
+Version: 0.4.0
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `rach_pack-0.3.0/setup.py` & `rach_pack-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='rach_pack',
-    version='0.3.0',
+    version='0.4.0',
     description='A sample Python project for rach pack',
     author='Rac',
     author_email='rachitmahajan6399@gmail.com',
     url='https://github.com/r-mhjn/QuizCreator',
     packages=['rach_pack'],
     install_requires=[],
     classifiers=[
```

