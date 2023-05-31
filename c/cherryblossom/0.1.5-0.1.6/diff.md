# Comparing `tmp/cherryblossom-0.1.5.tar.gz` & `tmp/cherryblossom-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherryblossom-0.1.5.tar", last modified: Wed May 31 05:57:37 2023, max compression
+gzip compressed data, was "cherryblossom-0.1.6.tar", last modified: Wed May 31 06:03:41 2023, max compression
```

## Comparing `cherryblossom-0.1.5.tar` & `cherryblossom-0.1.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 05:57:37.664444 cherryblossom-0.1.5/
--rw-r--r--   0 arjun      (501) staff       (20)       32 2023-04-17 05:21:05.000000 cherryblossom-0.1.5/MANIFEST.in
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-05-31 05:57:37.664206 cherryblossom-0.1.5/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.1.5/README.md
--rw-r--r--   0 arjun      (501) staff       (20)     1570 2023-05-31 05:56:45.000000 cherryblossom-0.1.5/pyproject.toml
--rw-r--r--   0 arjun      (501) staff       (20)       38 2023-05-31 05:57:37.664496 cherryblossom-0.1.5/setup.cfg
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 05:57:37.653373 cherryblossom-0.1.5/src/
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 05:57:37.661139 cherryblossom-0.1.5/src/cherryblossom/
--rw-r--r--   0 arjun      (501) staff       (20)     4601 2023-04-16 02:36:30.000000 cherryblossom-0.1.5/src/cherryblossom/.key
--rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.1.5/src/cherryblossom/Analyzer.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.1.5/src/cherryblossom/Blossom.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.1.5/src/cherryblossom/Channels.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.1.5/src/cherryblossom/Chat.py
--rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.1.5/src/cherryblossom/DB.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.1.5/src/cherryblossom/Data.py
--rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.1.5/src/cherryblossom/Functions.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.1.5/src/cherryblossom/GPTModel.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.1.5/src/cherryblossom/Index.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.1.5/src/cherryblossom/Plots.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.1.5/src/cherryblossom/Timezone.py
--rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.1.5/src/cherryblossom/__init__.py
--rw-r--r--   0 arjun      (501) staff       (20)     1084 2023-05-31 05:54:45.000000 cherryblossom-0.1.5/src/cherryblossom/get_file.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.1.5/src/cherryblossom/imports.py
--rw-r--r--   0 arjun      (501) staff       (20)     1767 2023-05-31 05:55:10.000000 cherryblossom-0.1.5/src/cherryblossom/key.py
--rw-r--r--   0 arjun      (501) staff       (20)      586 2023-05-02 06:27:14.000000 cherryblossom-0.1.5/src/cherryblossom/main.py
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 05:57:37.662367 cherryblossom-0.1.5/src/cherryblossom.egg-info/
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 05:57:37.663811 cherryblossom-0.1.5/src/cherryblossom.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 arjun      (501) staff       (20)      713 2023-04-17 20:05:12.000000 cherryblossom-0.1.5/src/cherryblossom.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 20:05:12.000000 cherryblossom-0.1.5/src/cherryblossom.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 20:05:12.000000 cherryblossom-0.1.5/src/cherryblossom.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 20:05:12.000000 cherryblossom-0.1.5/src/cherryblossom.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-05-31 05:57:37.000000 cherryblossom-0.1.5/src/cherryblossom.egg-info/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)     1026 2023-05-31 05:57:37.000000 cherryblossom-0.1.5/src/cherryblossom.egg-info/SOURCES.txt
--rw-r--r--   0 arjun      (501) staff       (20)        1 2023-05-31 05:57:37.000000 cherryblossom-0.1.5/src/cherryblossom.egg-info/dependency_links.txt
--rw-r--r--   0 arjun      (501) staff       (20)       88 2023-05-31 05:57:37.000000 cherryblossom-0.1.5/src/cherryblossom.egg-info/requires.txt
--rw-r--r--   0 arjun      (501) staff       (20)       14 2023-05-31 05:57:37.000000 cherryblossom-0.1.5/src/cherryblossom.egg-info/top_level.txt
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 06:03:41.766646 cherryblossom-0.1.6/
+-rw-r--r--   0 arjun      (501) staff       (20)       32 2023-04-17 05:21:05.000000 cherryblossom-0.1.6/MANIFEST.in
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-05-31 06:03:41.766429 cherryblossom-0.1.6/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.1.6/README.md
+-rw-r--r--   0 arjun      (501) staff       (20)     1570 2023-05-31 06:03:15.000000 cherryblossom-0.1.6/pyproject.toml
+-rw-r--r--   0 arjun      (501) staff       (20)       38 2023-05-31 06:03:41.766698 cherryblossom-0.1.6/setup.cfg
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 06:03:41.755373 cherryblossom-0.1.6/src/
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 06:03:41.763698 cherryblossom-0.1.6/src/cherryblossom/
+-rw-r--r--   0 arjun      (501) staff       (20)     4601 2023-04-16 02:36:30.000000 cherryblossom-0.1.6/src/cherryblossom/.key
+-rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.1.6/src/cherryblossom/Analyzer.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.1.6/src/cherryblossom/Blossom.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.1.6/src/cherryblossom/Channels.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.1.6/src/cherryblossom/Chat.py
+-rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.1.6/src/cherryblossom/DB.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.1.6/src/cherryblossom/Data.py
+-rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.1.6/src/cherryblossom/Functions.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.1.6/src/cherryblossom/GPTModel.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.1.6/src/cherryblossom/Index.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.1.6/src/cherryblossom/Plots.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.1.6/src/cherryblossom/Timezone.py
+-rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.1.6/src/cherryblossom/__init__.py
+-rw-r--r--   0 arjun      (501) staff       (20)     1084 2023-05-31 06:01:39.000000 cherryblossom-0.1.6/src/cherryblossom/get_file.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.1.6/src/cherryblossom/imports.py
+-rw-r--r--   0 arjun      (501) staff       (20)     1767 2023-05-31 05:55:10.000000 cherryblossom-0.1.6/src/cherryblossom/key.py
+-rw-r--r--   0 arjun      (501) staff       (20)      586 2023-05-02 06:27:14.000000 cherryblossom-0.1.6/src/cherryblossom/main.py
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 06:03:41.764858 cherryblossom-0.1.6/src/cherryblossom.egg-info/
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-31 06:03:41.766081 cherryblossom-0.1.6/src/cherryblossom.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 arjun      (501) staff       (20)      713 2023-04-17 20:05:12.000000 cherryblossom-0.1.6/src/cherryblossom.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 20:05:12.000000 cherryblossom-0.1.6/src/cherryblossom.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 20:05:12.000000 cherryblossom-0.1.6/src/cherryblossom.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 20:05:12.000000 cherryblossom-0.1.6/src/cherryblossom.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-05-31 06:03:41.000000 cherryblossom-0.1.6/src/cherryblossom.egg-info/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)     1026 2023-05-31 06:03:41.000000 cherryblossom-0.1.6/src/cherryblossom.egg-info/SOURCES.txt
+-rw-r--r--   0 arjun      (501) staff       (20)        1 2023-05-31 06:03:41.000000 cherryblossom-0.1.6/src/cherryblossom.egg-info/dependency_links.txt
+-rw-r--r--   0 arjun      (501) staff       (20)       88 2023-05-31 06:03:41.000000 cherryblossom-0.1.6/src/cherryblossom.egg-info/requires.txt
+-rw-r--r--   0 arjun      (501) staff       (20)       14 2023-05-31 06:03:41.000000 cherryblossom-0.1.6/src/cherryblossom.egg-info/top_level.txt
```

### Comparing `cherryblossom-0.1.5/pyproject.toml` & `cherryblossom-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 cherryblossom = [".key", "src/cherryblossom/*.py", "src/cherryblossom/.key", "cherryblossom/.key"]
 
 [project]
 name = "cherryblossom"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Arjun Naik", email="arjunsatishnaik@gmail.com" },
 ]
 description = "CherryBlossom: an API for Nosedive AI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cherryblossom-0.1.5/src/cherryblossom/.key` & `cherryblossom-0.1.6/src/cherryblossom/.key`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.1.5/src/cherryblossom/get_file.py` & `cherryblossom-0.1.6/src/cherryblossom/get_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import paramiko
 from scp import SCPClient
 import io
 import shutil
 import os
 
-pkey = paramiko.RSAKey.from_private_key(io.StringIO(open('.key', 'r').read())
-
+pkey = paramiko.RSAKey.from_private_key(io.StringIO(open('.key', 'r').read()))
 server = 'vergil.u.washington.edu'
 username = 'arjunsn'
 directory = '~/cherryblossom/module'
 place_in = './.cherryblossom'
 
 def get_file1(filenames):
     ssh = paramiko.SSHClient()
```

### Comparing `cherryblossom-0.1.5/src/cherryblossom/key.py` & `cherryblossom-0.1.6/src/cherryblossom/key.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.1.5/src/cherryblossom/main.py` & `cherryblossom-0.1.6/src/cherryblossom/main.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.1.5/src/cherryblossom.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt` & `cherryblossom-0.1.6/src/cherryblossom.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.1.5/src/cherryblossom.egg-info/SOURCES.txt` & `cherryblossom-0.1.6/src/cherryblossom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

