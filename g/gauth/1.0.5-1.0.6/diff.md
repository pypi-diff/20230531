# Comparing `tmp/gauth-1.0.5.tar.gz` & `tmp/gauth-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth-1.0.5.tar", last modified: Wed May 31 08:42:07 2023, max compression
+gzip compressed data, was "gauth-1.0.6.tar", last modified: Wed May 31 10:08:09 2023, max compression
```

## Comparing `gauth-1.0.5.tar` & `gauth-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 08:42:07.227697 gauth-1.0.5/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.5/LICENSE.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       62 2023-05-31 08:30:36.000000 gauth-1.0.5/MANIFEST.in
--rw-r--r--   0 damonyuan   (501) staff       (20)     1804 2023-05-31 08:42:07.227466 gauth-1.0.5/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)     1376 2023-05-31 07:07:42.000000 gauth-1.0.5/README.md
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 08:42:07.225670 gauth-1.0.5/gauth/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1921 2023-05-31 07:30:51.000000 gauth-1.0.5/gauth/main.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 08:42:07.227168 gauth-1.0.5/gauth.egg-info/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1804 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)      221 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/SOURCES.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/dependency_links.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/entry_points.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/top_level.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)      110 2023-05-31 03:20:31.000000 gauth-1.0.5/requirements.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 08:42:07.227777 gauth-1.0.5/setup.cfg
--rw-r--r--   0 damonyuan   (501) staff       (20)      863 2023-05-31 08:41:54.000000 gauth-1.0.5/setup.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.159083 gauth-1.0.6/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.6/LICENSE.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       24 2023-05-31 10:08:04.000000 gauth-1.0.6/MANIFEST.in
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1893 2023-05-31 10:08:09.158855 gauth-1.0.6/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1465 2023-05-31 09:47:37.000000 gauth-1.0.6/README.md
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.153974 gauth-1.0.6/gauth/
+-rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.6/gauth/__init__.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.157270 gauth-1.0.6/gauth/extract/
+-rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.6/gauth/extract/__init__.py
+-rw-r--r--   0 damonyuan   (501) staff       (20)    38669 2023-05-31 09:50:16.000000 gauth-1.0.6/gauth/extract/extract_otp_secrets.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.158362 gauth-1.0.6/gauth/extract/protobuf_generated_python/
+-rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.6/gauth/extract/protobuf_generated_python/__init__.py
+-rw-r--r--   0 damonyuan   (501) staff       (20)     2171 2023-05-31 09:14:07.000000 gauth-1.0.6/gauth/extract/protobuf_generated_python/google_auth_pb2.py
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1842 2023-05-31 09:48:48.000000 gauth-1.0.6/gauth/main.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:08:09.156453 gauth-1.0.6/gauth.egg-info/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1893 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)      441 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/SOURCES.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/dependency_links.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/entry_points.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)      263 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/requires.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 10:08:09.000000 gauth-1.0.6/gauth.egg-info/top_level.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)      274 2023-05-31 09:06:17.000000 gauth-1.0.6/requirements.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 10:08:09.159139 gauth-1.0.6/setup.cfg
+-rw-r--r--   0 damonyuan   (501) staff       (20)      933 2023-05-31 10:06:59.000000 gauth-1.0.6/setup.py
```

### Comparing `gauth-1.0.5/LICENSE.txt` & `gauth-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gauth-1.0.5/PKG-INFO` & `gauth-1.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,7 +58,11 @@
 
 ```
 pip install --upgrade twine
 python setup.py sdist
 twine upload dist/*
 ```
 
+# Reference
+
+[extract_otp_secrets v2.4.3](https://github.com/scito/extract_otp_secrets)
+
```

### Comparing `gauth-1.0.5/README.md` & `gauth-1.0.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -44,7 +44,11 @@
 
 ```
 pip install --upgrade twine
 python setup.py sdist
 twine upload dist/*
 ```
 
+# Reference
+
+[extract_otp_secrets v2.4.3](https://github.com/scito/extract_otp_secrets)
+
```

### Comparing `gauth-1.0.5/gauth/main.py` & `gauth-1.0.6/gauth/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 import os
 import argparse
 import pyotp
 import tempfile
 import json
-import logging
 from PIL import Image
 from contextlib import contextmanager
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), '../'))
 
 
 def check_img(filename):
     try:
@@ -34,28 +33,26 @@
             yield new_target
     finally:
         sys.stdout = old_target
         sys.stderr = old_stderr
 
 
 def main():
-    logging.basicConfig()
-    logging.getLogger().setLevel(logging.ERROR)
     parser = argparse.ArgumentParser(description='Tool to help migrate Google Authenticator from phone to desktop')
     parser.add_argument('-p', '--path', help='file path to the exported qr code or text file', required=True)
     args = parser.parse_args()
     if args.path:
         if check_img(args.path):
-            from extract_otp_secrets import main as eos_main
+            from gauth.extract import extract_otp_secrets
         else:
             with silence_stdout():
-                from extract_otp_secrets import main as eos_main
+                from gauth.extract import extract_otp_secrets
         with tempfile.NamedTemporaryFile() as tmp:
             params = [args.path, '--json', tmp.name, '--quiet', '--ignore']
-            eos_main(params)
+            extract_otp_secrets.main(params)
             otps(json.load(tmp))
 
 
 def otps(config):
     for e in config:
         otp(e['name'], e['issuer'], e['secret'].strip())
```

### Comparing `gauth-1.0.5/gauth.egg-info/PKG-INFO` & `gauth-1.0.6/gauth.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,7 +58,11 @@
 
 ```
 pip install --upgrade twine
 python setup.py sdist
 twine upload dist/*
 ```
 
+# Reference
+
+[extract_otp_secrets v2.4.3](https://github.com/scito/extract_otp_secrets)
+
```

