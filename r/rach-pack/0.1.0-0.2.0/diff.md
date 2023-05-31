# Comparing `tmp/rach_pack-0.1.0.tar.gz` & `tmp/rach_pack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rach_pack-0.1.0.tar", last modified: Wed May 31 14:14:42 2023, max compression
+gzip compressed data, was "rach_pack-0.2.0.tar", last modified: Wed May 31 15:11:45 2023, max compression
```

## Comparing `rach_pack-0.1.0.tar` & `rach_pack-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 14:14:42.894094 rach_pack-0.1.0/
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      596 2023-05-31 14:14:42.894094 rach_pack-0.1.0/PKG-INFO
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      364 2023-05-31 13:04:04.000000 rach_pack-0.1.0/README.md
-drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 14:14:42.894094 rach_pack-0.1.0/rach_pack/
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       52 2023-05-31 13:02:32.000000 rach_pack-0.1.0/rach_pack/main.py
-drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 14:14:42.894094 rach_pack-0.1.0/rach_pack.egg-info/
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      596 2023-05-31 14:14:42.000000 rach_pack-0.1.0/rach_pack.egg-info/PKG-INFO
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      200 2023-05-31 14:14:42.000000 rach_pack-0.1.0/rach_pack.egg-info/SOURCES.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)        1 2023-05-31 14:14:42.000000 rach_pack-0.1.0/rach_pack.egg-info/dependency_links.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       24 2023-05-31 14:14:42.000000 rach_pack-0.1.0/rach_pack.egg-info/requires.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       10 2023-05-31 14:14:42.000000 rach_pack-0.1.0/rach_pack.egg-info/top_level.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       38 2023-05-31 14:14:42.894094 rach_pack-0.1.0/setup.cfg
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      753 2023-05-31 14:13:29.000000 rach_pack-0.1.0/setup.py
+drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 15:11:45.274780 rach_pack-0.2.0/
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      596 2023-05-31 15:11:45.274780 rach_pack-0.2.0/PKG-INFO
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      364 2023-05-31 13:04:04.000000 rach_pack-0.2.0/README.md
+drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 15:11:45.270780 rach_pack-0.2.0/rach_pack/
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       57 2023-05-31 14:54:04.000000 rach_pack-0.2.0/rach_pack/main.py
+drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-05-31 15:11:45.274780 rach_pack-0.2.0/rach_pack.egg-info/
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      596 2023-05-31 15:11:45.000000 rach_pack-0.2.0/rach_pack.egg-info/PKG-INFO
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      168 2023-05-31 15:11:45.000000 rach_pack-0.2.0/rach_pack.egg-info/SOURCES.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)        1 2023-05-31 15:11:45.000000 rach_pack-0.2.0/rach_pack.egg-info/dependency_links.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       10 2023-05-31 15:11:45.000000 rach_pack-0.2.0/rach_pack.egg-info/top_level.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       38 2023-05-31 15:11:45.274780 rach_pack-0.2.0/setup.cfg
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      663 2023-05-31 15:11:09.000000 rach_pack-0.2.0/setup.py
```

### Comparing `rach_pack-0.1.0/PKG-INFO` & `rach_pack-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rach_pack
-Version: 0.1.0
+Version: 0.2.0
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `rach_pack-0.1.0/rach_pack.egg-info/PKG-INFO` & `rach_pack-0.2.0/rach_pack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rach-pack
-Version: 0.1.0
+Version: 0.2.0
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `rach_pack-0.1.0/setup.py` & `rach_pack-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from setuptools import setup
 
 setup(
     name='rach_pack',
-    version='0.1.0',
+    version='0.2.0',
     description='A sample Python project for rach pack',
     author='Rac',
     author_email='rachitmahajan6399@gmail.com',
     url='https://github.com/r-mhjn/QuizCreator',
     packages=['rach_pack'],
-    install_requires=[
-        'dependency1',
-        'dependency2',
-        # List other dependencies here
-    ],
+    install_requires=[],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

