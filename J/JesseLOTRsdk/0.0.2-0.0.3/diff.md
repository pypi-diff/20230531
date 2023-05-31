# Comparing `tmp/JesseLOTRsdk-0.0.2.tar.gz` & `tmp/JesseLOTRsdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JesseLOTRsdk-0.0.2.tar", last modified: Wed May 31 19:57:57 2023, max compression
+gzip compressed data, was "JesseLOTRsdk-0.0.3.tar", last modified: Wed May 31 20:02:52 2023, max compression
```

## Comparing `JesseLOTRsdk-0.0.2.tar` & `JesseLOTRsdk-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 19:57:57.822013 JesseLOTRsdk-0.0.2/
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 19:57:57.820773 JesseLOTRsdk-0.0.2/JesseLOTRsdk/
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       93 2023-05-31 19:14:01.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk/__init__.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     8270 2023-05-31 19:15:35.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk/sdk.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     5052 2023-05-31 18:23:20.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk/tests.py
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 19:57:57.821847 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/PKG-INFO
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      291 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/SOURCES.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        1 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/dependency_links.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       21 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/requires.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       13 2023-05-31 19:57:57.000000 JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/top_level.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     1081 2023-05-31 19:51:27.000000 JesseLOTRsdk-0.0.2/LICENSE.md
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 19:57:57.822070 JesseLOTRsdk-0.0.2/PKG-INFO
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      105 2023-05-31 19:11:52.000000 JesseLOTRsdk-0.0.2/README.md
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       96 2023-05-31 19:52:32.000000 JesseLOTRsdk-0.0.2/pyproject.toml
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      595 2023-05-31 19:57:57.822347 JesseLOTRsdk-0.0.2/setup.cfg
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:02:52.531979 JesseLOTRsdk-0.0.3/
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:02:52.530821 JesseLOTRsdk-0.0.3/JesseLOTRsdk/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       93 2023-05-31 19:14:01.000000 JesseLOTRsdk-0.0.3/JesseLOTRsdk/__init__.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     8270 2023-05-31 19:15:35.000000 JesseLOTRsdk-0.0.3/JesseLOTRsdk/sdk.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     5052 2023-05-31 18:23:20.000000 JesseLOTRsdk-0.0.3/JesseLOTRsdk/tests.py
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:02:52.531827 JesseLOTRsdk-0.0.3/JesseLOTRsdk.egg-info/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 20:02:52.000000 JesseLOTRsdk-0.0.3/JesseLOTRsdk.egg-info/PKG-INFO
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      291 2023-05-31 20:02:52.000000 JesseLOTRsdk-0.0.3/JesseLOTRsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        1 2023-05-31 20:02:52.000000 JesseLOTRsdk-0.0.3/JesseLOTRsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       28 2023-05-31 20:02:52.000000 JesseLOTRsdk-0.0.3/JesseLOTRsdk.egg-info/requires.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       13 2023-05-31 20:02:52.000000 JesseLOTRsdk-0.0.3/JesseLOTRsdk.egg-info/top_level.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     1081 2023-05-31 19:51:27.000000 JesseLOTRsdk-0.0.3/LICENSE.md
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 20:02:52.532049 JesseLOTRsdk-0.0.3/PKG-INFO
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      105 2023-05-31 19:11:52.000000 JesseLOTRsdk-0.0.3/README.md
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       96 2023-05-31 19:52:32.000000 JesseLOTRsdk-0.0.3/pyproject.toml
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      602 2023-05-31 20:02:52.532325 JesseLOTRsdk-0.0.3/setup.cfg
```

### Comparing `JesseLOTRsdk-0.0.2/JesseLOTRsdk/sdk.py` & `JesseLOTRsdk-0.0.3/JesseLOTRsdk/sdk.py`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.2/JesseLOTRsdk/tests.py` & `JesseLOTRsdk-0.0.3/JesseLOTRsdk/tests.py`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.2/JesseLOTRsdk.egg-info/PKG-INFO` & `JesseLOTRsdk-0.0.3/JesseLOTRsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JesseLOTRsdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: An SDK for the Lord of the Rings API. Created for a coding challenge.
 Home-page: https://github.com/vincjess
 Author: Jesse Vincent
 Author-email: vincenjes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `JesseLOTRsdk-0.0.2/LICENSE.md` & `JesseLOTRsdk-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.2/PKG-INFO` & `JesseLOTRsdk-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JesseLOTRsdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: An SDK for the Lord of the Rings API. Created for a coding challenge.
 Home-page: https://github.com/vincjess
 Author: Jesse Vincent
 Author-email: vincenjes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `JesseLOTRsdk-0.0.2/setup.cfg` & `JesseLOTRsdk-0.0.3/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = JesseLOTRsdk
-version = 0.0.2
+version = 0.0.3
 author = Jesse Vincent
 author_email = vincenjes@gmail.com
 description = An SDK for the Lord of the Rings API. Created for a coding challenge.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vincjess
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 install_requires = 
-	dotenv
+	python-dotenv
 	requests
 	json
 python_requires = >=3.9
 include_package_data = True
 
 [egg_info]
 tag_build =
```

