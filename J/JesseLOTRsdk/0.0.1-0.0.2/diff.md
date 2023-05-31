# Comparing `tmp/JesseLOTRsdk-0.0.1.tar.gz` & `tmp/JesseLOTRsdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JesseLOTRsdk-0.0.1.tar", last modified: Wed May 31 19:55:38 2023, max compression
+gzip compressed data, was "JesseLOTRsdk-0.0.2.tar", last modified: Wed May 31 19:57:57 2023, max compression
```

## Comparing `JesseLOTRsdk-0.0.1.tar` & `JesseLOTRsdk-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 19:55:38.653093 JesseLOTRsdk-0.0.1/
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 19:55:38.651829 JesseLOTRsdk-0.0.1/JesseLOTRsdk/
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       93 2023-05-31 19:14:01.000000 JesseLOTRsdk-0.0.1/JesseLOTRsdk/__init__.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     8270 2023-05-31 19:15:35.000000 JesseLOTRsdk-0.0.1/JesseLOTRsdk/sdk.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     5052 2023-05-31 18:23:20.000000 JesseLOTRsdk-0.0.1/JesseLOTRsdk/tests.py
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 19:55:38.652920 JesseLOTRsdk-0.0.1/JesseLOTRsdk.egg-info/
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      464 2023-05-31 19:55:38.000000 JesseLOTRsdk-0.0.1/JesseLOTRsdk.egg-info/PKG-INFO
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      291 2023-05-31 19:55:38.000000 JesseLOTRsdk-0.0.1/JesseLOTRsdk.egg-info/SOURCES.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        1 2023-05-31 19:55:38.000000 JesseLOTRsdk-0.0.1/JesseLOTRsdk.egg-info/dependency_links.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       21 2023-05-31 19:55:38.000000 JesseLOTRsdk-0.0.1/JesseLOTRsdk.egg-info/requires.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       13 2023-05-31 19:55:38.000000 JesseLOTRsdk-0.0.1/JesseLOTRsdk.egg-info/top_level.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     1081 2023-05-31 19:51:27.000000 JesseLOTRsdk-0.0.1/LICENSE.md
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      464 2023-05-31 19:55:38.653156 JesseLOTRsdk-0.0.1/PKG-INFO
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      105 2023-05-31 19:11:52.000000 JesseLOTRsdk-0.0.1/README.md
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       96 2023-05-31 19:52:32.000000 JesseLOTRsdk-0.0.1/pyproject.toml
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      592 2023-05-31 19:55:38.653438 JesseLOTRsdk-0.0.1/setup.cfg
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 19:57:57.822013 JesseLOTRsdk-0.0.2/
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 19:57:57.820773 JesseLOTRsdk-0.0.2/JesseLOTRsdk/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       93 2023-05-31 19:14:01.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk/__init__.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     8270 2023-05-31 19:15:35.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk/sdk.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     5052 2023-05-31 18:23:20.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk/tests.py
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 19:57:57.821847 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/PKG-INFO
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      291 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        1 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       21 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/requires.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       13 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/top_level.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     1081 2023-05-31 19:51:27.000000 JesseLOTRsdk-0.0.2/LICENSE.md
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 19:57:57.822070 JesseLOTRsdk-0.0.2/PKG-INFO
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      105 2023-05-31 19:11:52.000000 JesseLOTRsdk-0.0.2/README.md
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       96 2023-05-31 19:52:32.000000 JesseLOTRsdk-0.0.2/pyproject.toml
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      595 2023-05-31 19:57:57.822347 JesseLOTRsdk-0.0.2/setup.cfg
```

### Comparing `JesseLOTRsdk-0.0.1/JesseLOTRsdk/sdk.py` & `JesseLOTRsdk-0.0.2/JesseLOTRsdk/sdk.py`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.1/JesseLOTRsdk/tests.py` & `JesseLOTRsdk-0.0.2/JesseLOTRsdk/tests.py`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.1/LICENSE.md` & `JesseLOTRsdk-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.1/setup.cfg` & `JesseLOTRsdk-0.0.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = JesseLOTRsdk
-version = 0.0.1
+version = 0.0.2
 author = Jesse Vincent
 author_email = vincenjes@gmail.com
 description = An SDK for the Lord of the Rings API. Created for a coding challenge.
-long_description = file: README
+long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vincjess
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

