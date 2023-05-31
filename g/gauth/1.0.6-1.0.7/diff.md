# Comparing `tmp/gauth-1.0.6.tar.gz` & `tmp/gauth-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth-1.0.6.tar", last modified: Wed May 31 10:08:09 2023, max compression
+gzip compressed data, was "gauth-1.0.7.tar", last modified: Wed May 31 10:37:41 2023, max compression
```

## Comparing `gauth-1.0.6.tar` & `gauth-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.159083 gauth-1.0.6/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.6/LICENSE.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       24 2023-05-31 10:08:04.000000 gauth-1.0.6/MANIFEST.in
--rw-r--r--   0 damonyuan   (501) staff       (20)     1893 2023-05-31 10:08:09.158855 gauth-1.0.6/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)     1465 2023-05-31 09:47:37.000000 gauth-1.0.6/README.md
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.153974 gauth-1.0.6/gauth/
--rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.6/gauth/__init__.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.157270 gauth-1.0.6/gauth/extract/
--rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.6/gauth/extract/__init__.py
--rw-r--r--   0 damonyuan   (501) staff       (20)    38669 2023-05-31 09:50:16.000000 gauth-1.0.6/gauth/extract/extract_otp_secrets.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.158362 gauth-1.0.6/gauth/extract/protobuf_generated_python/
--rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.6/gauth/extract/protobuf_generated_python/__init__.py
--rw-r--r--   0 damonyuan   (501) staff       (20)     2171 2023-05-31 09:14:07.000000 gauth-1.0.6/gauth/extract/protobuf_generated_python/google_auth_pb2.py
--rw-r--r--   0 damonyuan   (501) staff       (20)     1842 2023-05-31 09:48:48.000000 gauth-1.0.6/gauth/main.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.156453 gauth-1.0.6/gauth.egg-info/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1893 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)      441 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/SOURCES.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/dependency_links.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/entry_points.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)      263 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/requires.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/top_level.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)      274 2023-05-31 09:06:17.000000 gauth-1.0.6/requirements.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 10:08:09.159139 gauth-1.0.6/setup.cfg
--rw-r--r--   0 damonyuan   (501) staff       (20)      933 2023-05-31 10:06:59.000000 gauth-1.0.6/setup.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.801763 gauth-1.0.7/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.7/LICENSE.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       24 2023-05-31 10:08:04.000000 gauth-1.0.7/MANIFEST.in
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1893 2023-05-31 10:37:41.801548 gauth-1.0.7/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1465 2023-05-31 09:47:37.000000 gauth-1.0.7/README.md
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.798003 gauth-1.0.7/gauth/
+-rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.7/gauth/__init__.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.800075 gauth-1.0.7/gauth/extract/
+-rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.7/gauth/extract/__init__.py
+-rw-r--r--   0 damonyuan   (501) staff       (20)    38669 2023-05-31 09:50:16.000000 gauth-1.0.7/gauth/extract/extract_otp_secrets.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.801129 gauth-1.0.7/gauth/extract/protobuf_generated_python/
+-rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.7/gauth/extract/protobuf_generated_python/__init__.py
+-rw-r--r--   0 damonyuan   (501) staff       (20)     2171 2023-05-31 09:14:07.000000 gauth-1.0.7/gauth/extract/protobuf_generated_python/google_auth_pb2.py
+-rw-r--r--   0 damonyuan   (501) staff       (20)     2075 2023-05-31 10:36:23.000000 gauth-1.0.7/gauth/main.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.799586 gauth-1.0.7/gauth.egg-info/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1893 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)      441 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/SOURCES.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/dependency_links.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/entry_points.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)      263 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/requires.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/top_level.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)      274 2023-05-31 09:06:17.000000 gauth-1.0.7/requirements.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 10:37:41.801815 gauth-1.0.7/setup.cfg
+-rw-r--r--   0 damonyuan   (501) staff       (20)      933 2023-05-31 10:36:54.000000 gauth-1.0.7/setup.py
```

### Comparing `gauth-1.0.6/LICENSE.txt` & `gauth-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gauth-1.0.6/PKG-INFO` & `gauth-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gauth-1.0.6/README.md` & `gauth-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gauth-1.0.6/gauth/extract/extract_otp_secrets.py` & `gauth-1.0.7/gauth/extract/extract_otp_secrets.py`

 * *Files identical despite different names*

### Comparing `gauth-1.0.6/gauth/extract/protobuf_generated_python/google_auth_pb2.py` & `gauth-1.0.7/gauth/extract/protobuf_generated_python/google_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `gauth-1.0.6/gauth.egg-info/PKG-INFO` & `gauth-1.0.7/gauth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gauth-1.0.6/setup.py` & `gauth-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 with open("requirements.txt", "r") as f:
     REQUIREMENTS = f.read().splitlines()
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gauth",
-    version="1.0.6",
+    version="1.0.7",
     license='MIT',
     description="Tool to help migrate Google Authenticator from phone to desktop",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Damon Yuan",
     author_email="damon.yuan.dev@gmail.com",
     url="https://github.com/damonYuan/gauth",
```

