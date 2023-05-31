# Comparing `tmp/readlog-1.1.3.tar.gz` & `tmp/readlog-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readlog-1.1.3.tar", last modified: Tue May 30 16:27:25 2023, max compression
+gzip compressed data, was "readlog-1.1.4.tar", last modified: Wed May 31 05:43:01 2023, max compression
```

## Comparing `readlog-1.1.3.tar` & `readlog-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 16:27:25.271020 readlog-1.1.3/
--rw-rw-rw-   0        0        0      823 2023-05-30 16:27:25.269018 readlog-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-05-30 16:19:07.000000 readlog-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 16:27:25.271020 readlog-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      775 2023-05-30 16:27:13.000000 readlog-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:27:25.252026 readlog-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 16:27:25.266034 readlog-1.1.3/src/readlog.egg-info/
--rw-rw-rw-   0        0        0      823 2023-05-30 16:27:24.000000 readlog-1.1.3/src/readlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-30 16:27:25.000000 readlog-1.1.3/src/readlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 16:27:24.000000 readlog-1.1.3/src/readlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-30 16:27:24.000000 readlog-1.1.3/src/readlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 16:27:24.000000 readlog-1.1.3/src/readlog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3029 2023-05-30 13:09:29.000000 readlog-1.1.3/src/readlog.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.998133 readlog-1.1.4/
+-rw-rw-rw-   0        0        0      102 2023-05-31 05:41:04.000000 readlog-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      823 2023-05-31 05:43:00.997134 readlog-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-05-30 16:19:07.000000 readlog-1.1.4/README.md
+-rw-rw-rw-   0        0        0       49 2023-05-30 13:49:56.000000 readlog-1.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 05:43:00.998133 readlog-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-05-31 05:42:46.000000 readlog-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.985081 readlog-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.994133 readlog-1.1.4/src/readlog.egg-info/
+-rw-rw-rw-   0        0        0      823 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3029 2023-05-30 13:09:29.000000 readlog-1.1.4/src/readlog.py
```

### Comparing `readlog-1.1.3/PKG-INFO` & `readlog-1.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: readlog
-Version: 1.1.3
-Summary: Read themo info from lammps output file or log file
-Home-page: https://github.com/eastsheng/readlog
-Author: CHENDONGSHENG
-Author-email: eastsheng@hotmail.com
-Description-Content-Type: text/markdown
-
 ## ReadLog
 
 - A python code to read thermo info from lammps log file 
 
 ### Installation 
 
 ```bash
```

### Comparing `readlog-1.1.3/setup.py` & `readlog-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 # from distutils.core import setup
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-with open("src/readlog.egg-info/requires.txt","r") as f:
+with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'readlog',
-version      = '1.1.3',
+version      = '1.1.4',
 py_modules   = ['readlog'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/readlog',
```

### Comparing `readlog-1.1.3/src/readlog.py` & `readlog-1.1.4/src/readlog.py`

 * *Files identical despite different names*

