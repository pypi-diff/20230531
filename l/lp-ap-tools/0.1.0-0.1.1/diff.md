# Comparing `tmp/lp_ap_tools-0.1.0.tar.gz` & `tmp/lp_ap_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lp_ap_tools-0.1.0.tar", last modified: Mon May 29 03:35:36 2023, max compression
+gzip compressed data, was "dist/lp_ap_tools-0.1.1.tar", last modified: Mon May 29 23:28:14 2023, max compression
```

## Comparing `lp_ap_tools-0.1.0.tar` & `lp_ap_tools-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-05-29 03:35:36.000000 lp_ap_tools-0.1.0/
--rw-r--r--   0 eller      (501) staff       (20)      406 2023-05-29 03:35:36.000000 lp_ap_tools-0.1.0/PKG-INFO
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-05-29 03:35:36.000000 lp_ap_tools-0.1.0/lp_ap_tools/
--rw-r--r--   0 eller      (501) staff       (20)       15 2023-05-29 02:44:23.000000 lp_ap_tools-0.1.0/lp_ap_tools/__init__.py
--rw-r--r--   0 eller      (501) staff       (20)     1018 2023-05-29 02:43:47.000000 lp_ap_tools-0.1.0/lp_ap_tools/lp_ap_tools.py
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-05-29 03:35:36.000000 lp_ap_tools-0.1.0/tests/
--rw-r--r--   0 eller      (501) staff       (20)        0 2023-05-29 02:51:18.000000 lp_ap_tools-0.1.0/tests/__init__.py
--rw-r--r--   0 eller      (501) staff       (20)      104 2023-05-29 03:34:42.000000 lp_ap_tools-0.1.0/tests/lp_ap_tools_test.py
--rw-r--r--   0 eller      (501) staff       (20)      114 2023-05-29 03:01:53.000000 lp_ap_tools-0.1.0/README.md
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-05-29 03:35:36.000000 lp_ap_tools-0.1.0/lp_ap_tools.egg-info/
--rw-r--r--   0 eller      (501) staff       (20)      406 2023-05-29 03:35:35.000000 lp_ap_tools-0.1.0/lp_ap_tools.egg-info/PKG-INFO
--rw-r--r--   0 eller      (501) staff       (20)      287 2023-05-29 03:35:35.000000 lp_ap_tools-0.1.0/lp_ap_tools.egg-info/SOURCES.txt
--rw-r--r--   0 eller      (501) staff       (20)        8 2023-05-29 03:35:35.000000 lp_ap_tools-0.1.0/lp_ap_tools.egg-info/requires.txt
--rw-r--r--   0 eller      (501) staff       (20)       18 2023-05-29 03:35:35.000000 lp_ap_tools-0.1.0/lp_ap_tools.egg-info/top_level.txt
--rw-r--r--   0 eller      (501) staff       (20)        1 2023-05-29 03:35:35.000000 lp_ap_tools-0.1.0/lp_ap_tools.egg-info/dependency_links.txt
--rw-r--r--   0 eller      (501) staff       (20)      630 2023-05-29 03:35:13.000000 lp_ap_tools-0.1.0/setup.py
--rw-r--r--   0 eller      (501) staff       (20)       38 2023-05-29 03:35:36.000000 lp_ap_tools-0.1.0/setup.cfg
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/
+-rw-r--r--   0 eller      (501) staff       (20)      406 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/PKG-INFO
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/lp_ap_tools/
+-rw-r--r--   0 eller      (501) staff       (20)       15 2023-05-29 02:44:23.000000 lp_ap_tools-0.1.1/lp_ap_tools/__init__.py
+-rw-r--r--   0 eller      (501) staff       (20)     1753 2023-05-29 23:26:16.000000 lp_ap_tools-0.1.1/lp_ap_tools/lp_ap_tools.py
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/tests/
+-rw-r--r--   0 eller      (501) staff       (20)        0 2023-05-29 02:51:18.000000 lp_ap_tools-0.1.1/tests/__init__.py
+-rw-r--r--   0 eller      (501) staff       (20)      104 2023-05-29 03:34:42.000000 lp_ap_tools-0.1.1/tests/lp_ap_tools_test.py
+-rw-r--r--   0 eller      (501) staff       (20)      114 2023-05-29 03:01:53.000000 lp_ap_tools-0.1.1/README.md
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/lp_ap_tools.egg-info/
+-rw-r--r--   0 eller      (501) staff       (20)      406 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/lp_ap_tools.egg-info/PKG-INFO
+-rw-r--r--   0 eller      (501) staff       (20)      287 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/lp_ap_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 eller      (501) staff       (20)       17 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/lp_ap_tools.egg-info/requires.txt
+-rw-r--r--   0 eller      (501) staff       (20)       18 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/lp_ap_tools.egg-info/top_level.txt
+-rw-r--r--   0 eller      (501) staff       (20)        1 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/lp_ap_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 eller      (501) staff       (20)      642 2023-05-29 23:28:08.000000 lp_ap_tools-0.1.1/setup.py
+-rw-r--r--   0 eller      (501) staff       (20)       38 2023-05-29 23:28:14.000000 lp_ap_tools-0.1.1/setup.cfg
```

### Comparing `lp_ap_tools-0.1.0/setup.py` & `lp_ap_tools-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import find_packages, setup
 
 setup(
     name='lp_ap_tools',
     packages=find_packages(),
-    version='0.1.0',
+    version='0.1.1',
     description='A python decorator for creating ActionProvider RO-crates within a Globus flow',
     author='Augustus Ellerm',
     license='MIT',
-    install_requires=['rocrate'],
+    install_requires=['rocrate', 'pydantic'],
     setup_requires=['pytest-runner'],
     test_requires=['pytest==4.4.1'],
     test_suite='tests',
     url='https://github.com/GusEllerm/lp_tools.git',
     classifiers=("Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent")
```

