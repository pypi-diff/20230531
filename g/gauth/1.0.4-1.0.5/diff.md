# Comparing `tmp/gauth-1.0.4.tar.gz` & `tmp/gauth-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth-1.0.4.tar", last modified: Wed May 31 08:30:48 2023, max compression
+gzip compressed data, was "gauth-1.0.5.tar", last modified: Wed May 31 08:42:07 2023, max compression
```

## Comparing `gauth-1.0.4.tar` & `gauth-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 08:30:48.530413 gauth-1.0.4/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.4/LICENSE.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       62 2023-05-31 08:30:36.000000 gauth-1.0.4/MANIFEST.in
--rw-r--r--   0 damonyuan   (501) staff       (20)     1804 2023-05-31 08:30:48.530222 gauth-1.0.4/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)     1376 2023-05-31 07:07:42.000000 gauth-1.0.4/README.md
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 08:30:48.528316 gauth-1.0.4/gauth/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1921 2023-05-31 07:30:51.000000 gauth-1.0.4/gauth/main.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 08:30:48.529962 gauth-1.0.4/gauth.egg-info/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1804 2023-05-31 08:30:48.000000 gauth-1.0.4/gauth.egg-info/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)      249 2023-05-31 08:30:48.000000 gauth-1.0.4/gauth.egg-info/SOURCES.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 08:30:48.000000 gauth-1.0.4/gauth.egg-info/dependency_links.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 08:30:48.000000 gauth-1.0.4/gauth.egg-info/entry_points.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)      110 2023-05-31 08:30:48.000000 gauth-1.0.4/gauth.egg-info/requires.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 08:30:48.000000 gauth-1.0.4/gauth.egg-info/top_level.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)      110 2023-05-31 03:20:31.000000 gauth-1.0.4/requirements.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 08:30:48.530462 gauth-1.0.4/setup.cfg
--rw-r--r--   0 damonyuan   (501) staff       (20)      873 2023-05-31 08:30:36.000000 gauth-1.0.4/setup.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 08:42:07.227697 gauth-1.0.5/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.5/LICENSE.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       62 2023-05-31 08:30:36.000000 gauth-1.0.5/MANIFEST.in
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1804 2023-05-31 08:42:07.227466 gauth-1.0.5/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1376 2023-05-31 07:07:42.000000 gauth-1.0.5/README.md
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 08:42:07.225670 gauth-1.0.5/gauth/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1921 2023-05-31 07:30:51.000000 gauth-1.0.5/gauth/main.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 08:42:07.227168 gauth-1.0.5/gauth.egg-info/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1804 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)      221 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/SOURCES.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/dependency_links.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/entry_points.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 08:42:07.000000 gauth-1.0.5/gauth.egg-info/top_level.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)      110 2023-05-31 03:20:31.000000 gauth-1.0.5/requirements.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 08:42:07.227777 gauth-1.0.5/setup.cfg
+-rw-r--r--   0 damonyuan   (501) staff       (20)      863 2023-05-31 08:41:54.000000 gauth-1.0.5/setup.py
```

### Comparing `gauth-1.0.4/LICENSE.txt` & `gauth-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gauth-1.0.4/PKG-INFO` & `gauth-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gauth-1.0.4/README.md` & `gauth-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gauth-1.0.4/gauth/main.py` & `gauth-1.0.5/gauth/main.py`

 * *Files identical despite different names*

### Comparing `gauth-1.0.4/gauth.egg-info/PKG-INFO` & `gauth-1.0.5/gauth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gauth-1.0.4/setup.py` & `gauth-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 with open("requirements.txt", "r") as f:
     REQUIREMENTS = f.read().splitlines()
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gauth",
-    version="1.0.4",
+    version="1.0.5",
     license='MIT',
     description="Tool to help migrate Google Authenticator from phone to desktop",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Damon Yuan",
     author_email="damon.yuan.dev@gmail.com",
     url="https://github.com/damonYuan/gauth",
     packages=['gauth'],
     include_package_data=True,
     entry_points="""
     [console_scripts]
     gauth = gauth.main:main
     """,
-    install_requires=REQUIREMENTS,
+    install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires=">=3.6"
 )
```

