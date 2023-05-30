# Comparing `tmp/webdns-0.0.8.tar.gz` & `tmp/webdns-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdns-0.0.8.tar", last modified: Mon May 29 19:46:37 2023, max compression
+gzip compressed data, was "webdns-0.0.9.tar", last modified: Tue May 30 23:09:55 2023, max compression
```

## Comparing `webdns-0.0.8.tar` & `webdns-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:46:37.869000 webdns-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      694 2023-05-29 19:46:37.869000 webdns-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 19:46:37.869000 webdns-0.0.8/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     4117 2023-05-29 19:45:40.000000 webdns-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:46:37.866000 webdns-0.0.8/webdns/
--rwxrwxr-x   0 root         (0) root         (0)       75 2023-05-25 13:50:57.000000 webdns-0.0.8/webdns/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)       98 2023-05-29 19:45:48.000000 webdns-0.0.8/webdns/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:46:37.868000 webdns-0.0.8/webdns/api/
--rwxrwxr-x   0 root         (0) root         (0)       24 2023-05-25 13:50:59.000000 webdns-0.0.8/webdns/api/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2083 2023-05-24 14:43:52.000000 webdns-0.0.8/webdns/api/api.py
--rwxrwxr-x   0 root         (0) root         (0)      826 2023-05-24 14:43:52.000000 webdns-0.0.8/webdns/api/utils.py
--rwxrwxr-x   0 root         (0) root         (0)     2896 2023-05-24 14:43:52.000000 webdns-0.0.8/webdns/app.py
--rwxrwxr-x   0 root         (0) root         (0)     3394 2023-05-24 20:14:17.000000 webdns-0.0.8/webdns/methods.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:46:37.868000 webdns-0.0.8/webdns.egg-info/
--rw-r--r--   0 root         (0) root         (0)      694 2023-05-29 19:46:37.000000 webdns-0.0.8/webdns.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      291 2023-05-29 19:46:37.000000 webdns-0.0.8/webdns.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 19:46:37.000000 webdns-0.0.8/webdns.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-29 19:46:37.000000 webdns-0.0.8/webdns.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-29 19:46:37.000000 webdns-0.0.8/webdns.egg-info/top_level.txt
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2023-05-30 23:09:55.900000 webdns-0.0.9/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     7632 2023-05-30 23:09:55.900000 webdns-0.0.9/PKG-INFO
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     6218 2023-05-12 01:14:27.000000 webdns-0.0.9/README.md
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       38 2023-05-30 23:09:55.900000 webdns-0.0.9/setup.cfg
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     3975 2023-05-12 05:45:00.000000 webdns-0.0.9/setup.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2023-05-30 23:09:55.900000 webdns-0.0.9/webdns/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2023-05-12 04:33:34.000000 webdns-0.0.9/webdns/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       98 2023-05-30 23:03:24.000000 webdns-0.0.9/webdns/__version__.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2023-05-30 23:09:55.900000 webdns-0.0.9/webdns/api/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2023-05-12 00:44:38.000000 webdns-0.0.9/webdns/api/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     2083 2023-05-24 01:14:00.000000 webdns-0.0.9/webdns/api/api.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      826 2023-05-24 01:14:00.000000 webdns-0.0.9/webdns/api/utils.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     2896 2023-05-24 00:37:40.000000 webdns-0.0.9/webdns/app.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     3394 2023-05-25 00:25:56.000000 webdns-0.0.9/webdns/methods.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2023-05-30 23:09:55.900000 webdns-0.0.9/webdns.egg-info/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     7632 2023-05-30 23:09:52.000000 webdns-0.0.9/webdns.egg-info/PKG-INFO
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      301 2023-05-30 23:09:53.000000 webdns-0.0.9/webdns.egg-info/SOURCES.txt
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        1 2023-05-30 23:09:52.000000 webdns-0.0.9/webdns.egg-info/dependency_links.txt
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       35 2023-05-30 23:09:52.000000 webdns-0.0.9/webdns.egg-info/requires.txt
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        7 2023-05-30 23:09:52.000000 webdns-0.0.9/webdns.egg-info/top_level.txt
```

### Comparing `webdns-0.0.8/setup.py` & `webdns-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'webdns'
-DESCRIPTION = 'DnsMasq utility to name IP addresses from Netbox NSOT.'
+DESCRIPTION = 'DnsMasq utiity to name IP addresses from Netbox NSOT.'
 URL = 'https://git.rnp.br/pop-rj/dns-conectividade'
 EMAIL = 'infra@pop-rj.rnp.br'
 AUTHOR = 'PoP-RJ/RNP - BR'
 REQUIRES_PYTHON = '>=3.8.0'
 VERSION = None # Available at NAME.__version__.py
 
 # What packages are required for this module to be executed?
 here = os.path.abspath(os.path.dirname(__file__))
 
-# with io.open(os.path.join(here, 'requirements.txt'), encoding='utf-8') as f:
-#     REQUIRED = f.readlines()
-# c=0
-# for item in REQUIRED:
-#     REQUIRED[c] = item.replace("\n", "")
-#     c+=1
+with io.open(os.path.join(here, 'requirements.txt'), encoding='utf-8') as f:
+    REQUIRED = f.readlines()
+c=0
+for item in REQUIRED:
+    REQUIRED[c] = item.replace("\n", "")
+    c+=1
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
@@ -109,24 +109,15 @@
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
-    
-    install_requires=[
-        'pynetbox',
-        'jsonschema ',
-        'flask',
-        'waitress',
-        'configparser',
-        'ipaddress'
-    ],
-
+    install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
```

### Comparing `webdns-0.0.8/webdns/api/api.py` & `webdns-0.0.9/webdns/api/api.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.8/webdns/api/utils.py` & `webdns-0.0.9/webdns/api/utils.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.8/webdns/app.py` & `webdns-0.0.9/webdns/app.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.8/webdns/methods.py` & `webdns-0.0.9/webdns/methods.py`

 * *Files identical despite different names*

