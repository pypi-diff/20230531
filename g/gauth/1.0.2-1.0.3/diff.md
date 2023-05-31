# Comparing `tmp/gauth-1.0.2.tar.gz` & `tmp/gauth-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth-1.0.2.tar", last modified: Wed May 31 07:31:01 2023, max compression
+gzip compressed data, was "gauth-1.0.3.tar", last modified: Wed May 31 07:54:13 2023, max compression
```

## Comparing `gauth-1.0.2.tar` & `gauth-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:31:01.493200 gauth-1.0.2/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.2/LICENSE.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)     1851 2023-05-31 07:31:01.492805 gauth-1.0.2/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)     1376 2023-05-31 07:07:42.000000 gauth-1.0.2/README.md
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:31:01.490284 gauth-1.0.2/gauth/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1921 2023-05-31 07:30:51.000000 gauth-1.0.2/gauth/main.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:31:01.492545 gauth-1.0.2/gauth.egg-info/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1851 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)      220 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/SOURCES.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/dependency_links.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/entry_points.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)      110 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/requires.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 07:31:01.000000 gauth-1.0.2/gauth.egg-info/top_level.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 07:31:01.493254 gauth-1.0.2/setup.cfg
--rw-r--r--   0 damonyuan   (501) staff       (20)      879 2023-05-31 07:30:51.000000 gauth-1.0.2/setup.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:54:13.501760 gauth-1.0.3/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.3/LICENSE.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1804 2023-05-31 07:54:13.501570 gauth-1.0.3/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1376 2023-05-31 07:07:42.000000 gauth-1.0.3/README.md
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:54:13.499613 gauth-1.0.3/gauth/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1921 2023-05-31 07:30:51.000000 gauth-1.0.3/gauth/main.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 07:54:13.501225 gauth-1.0.3/gauth.egg-info/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1804 2023-05-31 07:54:13.000000 gauth-1.0.3/gauth.egg-info/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)      220 2023-05-31 07:54:13.000000 gauth-1.0.3/gauth.egg-info/SOURCES.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 07:54:13.000000 gauth-1.0.3/gauth.egg-info/dependency_links.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 07:54:13.000000 gauth-1.0.3/gauth.egg-info/entry_points.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)      110 2023-05-31 07:54:13.000000 gauth-1.0.3/gauth.egg-info/requires.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 07:54:13.000000 gauth-1.0.3/gauth.egg-info/top_level.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 07:54:13.501810 gauth-1.0.3/setup.cfg
+-rw-r--r--   0 damonyuan   (501) staff       (20)      925 2023-05-31 07:53:11.000000 gauth-1.0.3/setup.py
```

### Comparing `gauth-1.0.2/LICENSE.txt` & `gauth-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gauth-1.0.2/PKG-INFO` & `gauth-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 GAuth
 ====
```

### Comparing `gauth-1.0.2/README.md` & `gauth-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gauth-1.0.2/gauth/main.py` & `gauth-1.0.3/gauth/main.py`

 * *Files identical despite different names*

### Comparing `gauth-1.0.2/gauth.egg-info/PKG-INFO` & `gauth-1.0.3/gauth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 GAuth
 ====
```

### Comparing `gauth-1.0.2/setup.py` & `gauth-1.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from setuptools import setup
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gauth",
-    version="1.0.2",
+    version="1.0.3",
     license='MIT',
     description="Tool to help migrate Google Authenticator from phone to desktop",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Damon Yuan",
     author_email="damon.yuan.dev@gmail.com",
     url="https://github.com/damonYuan/gauth",
     packages=['gauth'],
+    package_data={
+        'gauth': ['README.md', 'LICENSE.txt', 'requirements.txt']
+    },
     entry_points="""
     [console_scripts]
     gauth = gauth.main:main
     """,
     install_requires=REQUIREMENTS,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
     ],
     python_requires=">=3.6"
 )
```

