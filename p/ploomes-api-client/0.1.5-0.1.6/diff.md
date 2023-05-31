# Comparing `tmp/ploomes-api-client-0.1.5.tar.gz` & `tmp/ploomes-api-client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomes-api-client-0.1.5.tar", last modified: Wed May 31 19:32:35 2023, max compression
+gzip compressed data, was "ploomes-api-client-0.1.6.tar", last modified: Wed May 31 19:43:53 2023, max compression
```

## Comparing `ploomes-api-client-0.1.5.tar` & `ploomes-api-client-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:32:35.965228 ploomes-api-client-0.1.5/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.5/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-31 19:32:35.965070 ploomes-api-client-0.1.5/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.5/README.md
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:32:35.964264 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:32:35.964498 ploomes-api-client-0.1.5/ploomes_client/
--rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.5/ploomes_client/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)    24681 2023-05-31 19:31:38.000000 ploomes-api-client-0.1.5/ploomes_client/ploomes_client.py
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-31 19:32:35.965283 ploomes-api-client-0.1.5/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-31 19:32:32.000000 ploomes-api-client-0.1.5/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:43:53.115454 ploomes-api-client-0.1.6/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.6/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-31 19:43:53.115316 ploomes-api-client-0.1.6/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.6/README.md
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:43:53.114442 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:43:53.114661 ploomes-api-client-0.1.6/ploomes_client/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.6/ploomes_client/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)    24697 2023-05-31 19:43:22.000000 ploomes-api-client-0.1.6/ploomes_client/ploomes_client.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-31 19:43:53.115505 ploomes-api-client-0.1.6/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-31 19:43:50.000000 ploomes-api-client-0.1.6/setup.py
```

### Comparing `ploomes-api-client-0.1.5/LICENSE` & `ploomes-api-client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.5/PKG-INFO` & `ploomes-api-client-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.5/README.md` & `ploomes-api-client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.5/ploomes_api_client.egg-info/PKG-INFO` & `ploomes-api-client-0.1.6/ploomes_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.5/ploomes_client/ploomes_client.py` & `ploomes-api-client-0.1.6/ploomes_client/ploomes_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import math
 import time
 import requests
 import json
 from ratelimit import limits, sleep_and_retry
 import pandas as pd
 import random
-from typing import Dict
+from typing import Dict, Optional, List
 
 """https://learn.microsoft.com/en-us/dynamics-nav/using-filter-expressions-in-odata-uris"""
 
 
 MAX_REQUESTS_PER_SECOND = 2
```

### Comparing `ploomes-api-client-0.1.5/setup.py` & `ploomes-api-client-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ploomes-api-client',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),   
     url='https://github.com/victorfigueredo/ploomes-api-client',
     author='Victor Figueredo',
     author_email='cto@filterfeed.com.br',
     description='Python client for the Ploomes API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

