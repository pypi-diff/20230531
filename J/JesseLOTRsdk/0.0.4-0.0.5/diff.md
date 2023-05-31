# Comparing `tmp/JesseLOTRsdk-0.0.4.tar.gz` & `tmp/JesseLOTRsdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JesseLOTRsdk-0.0.4.tar", last modified: Wed May 31 20:03:39 2023, max compression
+gzip compressed data, was "JesseLOTRsdk-0.0.5.tar", last modified: Wed May 31 20:07:28 2023, max compression
```

## Comparing `JesseLOTRsdk-0.0.4.tar` & `JesseLOTRsdk-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:03:39.940854 JesseLOTRsdk-0.0.4/
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:03:39.939595 JesseLOTRsdk-0.0.4/JesseLOTRsdk/
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       93 2023-05-31 19:14:01.000000 JesseLOTRsdk-0.0.4/JesseLOTRsdk/__init__.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     8270 2023-05-31 19:15:35.000000 JesseLOTRsdk-0.0.4/JesseLOTRsdk/sdk.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     5052 2023-05-31 18:23:20.000000 JesseLOTRsdk-0.0.4/JesseLOTRsdk/tests.py
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:03:39.940687 JesseLOTRsdk-0.0.4/JesseLOTRsdk.egg-info/
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 20:03:39.000000 JesseLOTRsdk-0.0.4/JesseLOTRsdk.egg-info/PKG-INFO
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      291 2023-05-31 20:03:39.000000 JesseLOTRsdk-0.0.4/JesseLOTRsdk.egg-info/SOURCES.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        1 2023-05-31 20:03:39.000000 JesseLOTRsdk-0.0.4/JesseLOTRsdk.egg-info/dependency_links.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       23 2023-05-31 20:03:39.000000 JesseLOTRsdk-0.0.4/JesseLOTRsdk.egg-info/requires.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       13 2023-05-31 20:03:39.000000 JesseLOTRsdk-0.0.4/JesseLOTRsdk.egg-info/top_level.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     1081 2023-05-31 19:51:27.000000 JesseLOTRsdk-0.0.4/LICENSE.md
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 20:03:39.940909 JesseLOTRsdk-0.0.4/PKG-INFO
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      105 2023-05-31 19:11:52.000000 JesseLOTRsdk-0.0.4/README.md
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       96 2023-05-31 19:52:32.000000 JesseLOTRsdk-0.0.4/pyproject.toml
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      596 2023-05-31 20:03:39.941168 JesseLOTRsdk-0.0.4/setup.cfg
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:28.179430 JesseLOTRsdk-0.0.5/
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:28.177435 JesseLOTRsdk-0.0.5/JesseLOTRsdk/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       93 2023-05-31 19:14:01.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/__init__.py
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:28.179170 JesseLOTRsdk-0.0.5/JesseLOTRsdk/models/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:06.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/models/__init__.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      663 2023-05-31 01:54:04.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/models/movie.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      346 2023-05-31 02:02:37.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/models/quote.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     8270 2023-05-31 19:15:35.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/sdk.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     5052 2023-05-31 18:23:20.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/tests.py
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:28.178535 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/PKG-INFO
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      381 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        1 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       23 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/requires.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       13 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/top_level.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     1081 2023-05-31 19:51:27.000000 JesseLOTRsdk-0.0.5/LICENSE.md
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 20:07:28.179495 JesseLOTRsdk-0.0.5/PKG-INFO
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      105 2023-05-31 19:11:52.000000 JesseLOTRsdk-0.0.5/README.md
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       96 2023-05-31 19:52:32.000000 JesseLOTRsdk-0.0.5/pyproject.toml
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      596 2023-05-31 20:07:28.179768 JesseLOTRsdk-0.0.5/setup.cfg
```

### Comparing `JesseLOTRsdk-0.0.4/JesseLOTRsdk/sdk.py` & `JesseLOTRsdk-0.0.5/JesseLOTRsdk/sdk.py`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.4/JesseLOTRsdk/tests.py` & `JesseLOTRsdk-0.0.5/JesseLOTRsdk/tests.py`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.4/JesseLOTRsdk.egg-info/PKG-INFO` & `JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JesseLOTRsdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: An SDK for the Lord of the Rings API. Created for a coding challenge.
 Home-page: https://github.com/vincjess
 Author: Jesse Vincent
 Author-email: vincenjes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `JesseLOTRsdk-0.0.4/LICENSE.md` & `JesseLOTRsdk-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.4/PKG-INFO` & `JesseLOTRsdk-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JesseLOTRsdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: An SDK for the Lord of the Rings API. Created for a coding challenge.
 Home-page: https://github.com/vincjess
 Author: Jesse Vincent
 Author-email: vincenjes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `JesseLOTRsdk-0.0.4/setup.cfg` & `JesseLOTRsdk-0.0.5/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = JesseLOTRsdk
-version = 0.0.4
+version = 0.0.5
 author = Jesse Vincent
 author_email = vincenjes@gmail.com
 description = An SDK for the Lord of the Rings API. Created for a coding challenge.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vincjess
 classifiers =
```

