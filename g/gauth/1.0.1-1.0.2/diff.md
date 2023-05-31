# Comparing `tmp/gauth-1.0.1.tar.gz` & `tmp/gauth-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth-1.0.1.tar", last modified: Wed May 31 07:27:01 2023, max compression
+gzip compressed data, was "gauth-1.0.2.tar", last modified: Wed May 31 07:31:01 2023, max compression
```

## Comparing `gauth-1.0.1.tar` & `gauth-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:27:01.700435 gauth-1.0.1/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.1/LICENSE.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)     1851 2023-05-31 07:27:01.700246 gauth-1.0.1/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)     1376 2023-05-31 07:07:42.000000 gauth-1.0.1/README.md
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:27:01.698163 gauth-1.0.1/gauth/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1919 2023-05-31 06:46:05.000000 gauth-1.0.1/gauth/main.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:27:01.700007 gauth-1.0.1/gauth.egg-info/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1851 2023-05-31 07:27:01.000000 gauth-1.0.1/gauth.egg-info/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)      220 2023-05-31 07:27:01.000000 gauth-1.0.1/gauth.egg-info/SOURCES.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 07:27:01.000000 gauth-1.0.1/gauth.egg-info/dependency_links.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 07:27:01.000000 gauth-1.0.1/gauth.egg-info/entry_points.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)      110 2023-05-31 07:27:01.000000 gauth-1.0.1/gauth.egg-info/requires.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 07:27:01.000000 gauth-1.0.1/gauth.egg-info/top_level.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 07:27:01.700477 gauth-1.0.1/setup.cfg
--rw-r--r--   0 damonyuan   (501) staff       (20)      879 2023-05-31 07:26:54.000000 gauth-1.0.1/setup.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:31:01.493200 gauth-1.0.2/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.2/LICENSE.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1851 2023-05-31 07:31:01.492805 gauth-1.0.2/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1376 2023-05-31 07:07:42.000000 gauth-1.0.2/README.md
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:31:01.490284 gauth-1.0.2/gauth/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1921 2023-05-31 07:30:51.000000 gauth-1.0.2/gauth/main.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:31:01.492545 gauth-1.0.2/gauth.egg-info/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1851 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)      220 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/SOURCES.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/dependency_links.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/entry_points.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)      110 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/requires.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/top_level.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 07:31:01.493254 gauth-1.0.2/setup.cfg
+-rw-r--r--   0 damonyuan   (501) staff       (20)      879 2023-05-31 07:30:51.000000 gauth-1.0.2/setup.py
```

### Comparing `gauth-1.0.1/LICENSE.txt` & `gauth-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gauth-1.0.1/PKG-INFO` & `gauth-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gauth-1.0.1/README.md` & `gauth-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gauth-1.0.1/gauth/main.py` & `gauth-1.0.2/gauth/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         sys.stderr = old_stderr
 
 
 def main():
     logging.basicConfig()
     logging.getLogger().setLevel(logging.ERROR)
     parser = argparse.ArgumentParser(description='Tool to help migrate Google Authenticator from phone to desktop')
-    parser.add_argument('-p', '--path', help='file path to the export qr code or text file', required=True)
+    parser.add_argument('-p', '--path', help='file path to the exported qr code or text file', required=True)
     args = parser.parse_args()
     if args.path:
         if check_img(args.path):
             from extract_otp_secrets import main as eos_main
         else:
             with silence_stdout():
                 from extract_otp_secrets import main as eos_main
```

### Comparing `gauth-1.0.1/gauth.egg-info/PKG-INFO` & `gauth-1.0.2/gauth.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gauth-1.0.1/setup.py` & `gauth-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gauth",
-    version="1.0.1",
+    version="1.0.2",
     license='MIT',
     description="Tool to help migrate Google Authenticator from phone to desktop",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Damon Yuan",
     author_email="damon.yuan.dev@gmail.com",
     url="https://github.com/damonYuan/gauth",
```

