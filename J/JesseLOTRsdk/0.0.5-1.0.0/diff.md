# Comparing `tmp/JesseLOTRsdk-0.0.5.tar.gz` & `tmp/JesseLOTRsdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JesseLOTRsdk-0.0.5.tar", last modified: Wed May 31 20:07:28 2023, max compression
+gzip compressed data, was "JesseLOTRsdk-1.0.0.tar", last modified: Wed May 31 20:52:19 2023, max compression
```

## Comparing `JesseLOTRsdk-0.0.5.tar` & `JesseLOTRsdk-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:28.179430 JesseLOTRsdk-0.0.5/
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:28.177435 JesseLOTRsdk-0.0.5/JesseLOTRsdk/
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       93 2023-05-31 19:14:01.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/__init__.py
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:28.179170 JesseLOTRsdk-0.0.5/JesseLOTRsdk/models/
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:06.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/models/__init__.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      663 2023-05-31 01:54:04.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/models/movie.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      346 2023-05-31 02:02:37.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/models/quote.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     8270 2023-05-31 19:15:35.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/sdk.py
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     5052 2023-05-31 18:23:20.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk/tests.py
-drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:28.178535 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/PKG-INFO
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      381 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/SOURCES.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        1 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/dependency_links.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       23 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/requires.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       13 2023-05-31 20:07:28.000000 JesseLOTRsdk-0.0.5/JesseLOTRsdk.egg-info/top_level.txt
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     1081 2023-05-31 19:51:27.000000 JesseLOTRsdk-0.0.5/LICENSE.md
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      570 2023-05-31 20:07:28.179495 JesseLOTRsdk-0.0.5/PKG-INFO
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      105 2023-05-31 19:11:52.000000 JesseLOTRsdk-0.0.5/README.md
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       96 2023-05-31 19:52:32.000000 JesseLOTRsdk-0.0.5/pyproject.toml
--rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      596 2023-05-31 20:07:28.179768 JesseLOTRsdk-0.0.5/setup.cfg
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:52:19.135933 JesseLOTRsdk-1.0.0/
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:52:19.133751 JesseLOTRsdk-1.0.0/JesseLOTRsdk/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       93 2023-05-31 19:14:01.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk/__init__.py
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:52:19.135587 JesseLOTRsdk-1.0.0/JesseLOTRsdk/models/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:07:06.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk/models/__init__.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      663 2023-05-31 01:54:04.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk/models/movie.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      346 2023-05-31 02:02:37.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk/models/quote.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     8274 2023-05-31 20:51:30.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk/sdk.py
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     5048 2023-05-31 20:16:10.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk/tests.py
+drwxr-xr-x   0 vincjess (430751568) BYU\Domain Users (1539093546)        0 2023-05-31 20:52:19.134855 JesseLOTRsdk-1.0.0/JesseLOTRsdk.egg-info/
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     4985 2023-05-31 20:52:19.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk.egg-info/PKG-INFO
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      381 2023-05-31 20:52:19.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)        1 2023-05-31 20:52:19.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       23 2023-05-31 20:52:19.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk.egg-info/requires.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       13 2023-05-31 20:52:19.000000 JesseLOTRsdk-1.0.0/JesseLOTRsdk.egg-info/top_level.txt
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     1081 2023-05-31 19:51:27.000000 JesseLOTRsdk-1.0.0/LICENSE.md
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     4985 2023-05-31 20:52:19.135991 JesseLOTRsdk-1.0.0/PKG-INFO
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)     4519 2023-05-31 20:50:07.000000 JesseLOTRsdk-1.0.0/README.md
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)       96 2023-05-31 19:52:32.000000 JesseLOTRsdk-1.0.0/pyproject.toml
+-rw-r--r--   0 vincjess (430751568) BYU\Domain Users (1539093546)      596 2023-05-31 20:52:19.136269 JesseLOTRsdk-1.0.0/setup.cfg
```

### Comparing `JesseLOTRsdk-0.0.5/JesseLOTRsdk/models/movie.py` & `JesseLOTRsdk-1.0.0/JesseLOTRsdk/models/movie.py`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.5/JesseLOTRsdk/sdk.py` & `JesseLOTRsdk-1.0.0/JesseLOTRsdk/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                 return f'{match_key}!=/{match_value}/i'
             elif 'compare' in filter_dict:
                 match_key, match_value = filter_dict['compare']
                 return f'{match_key}{match_value}'
         elif key == 'exist':
             return filter_dict['exist']
         elif key == 'not_exist':
-            return f'!{filter_dict["exist"]}'
+            return f'!{filter_dict["not_exist"]}'
         else:
             raise Exception(f'The filter key `{key}` does not exist.')
 
 
     def get_movies(self, **kwargs):
         """
         get_movies does a request for all the movies based on the pagination, sorting, and filtering criteria.
```

### Comparing `JesseLOTRsdk-0.0.5/JesseLOTRsdk/tests.py` & `JesseLOTRsdk-1.0.0/JesseLOTRsdk/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dotenv import load_dotenv
 import os
 import re
 from unittest import TestCase
-from ringSDK import LOTR
+from sdk import LOTR
 from models.movie import Movie
 from models.quote import Quote
 
 load_dotenv()
 TOKEN = os.getenv('TOKEN')
 
 class MountDoomTesting(TestCase):
```

### Comparing `JesseLOTRsdk-0.0.5/LICENSE.md` & `JesseLOTRsdk-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `JesseLOTRsdk-0.0.5/setup.cfg` & `JesseLOTRsdk-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = JesseLOTRsdk
-version = 0.0.5
+version = 1.0.0
 author = Jesse Vincent
 author_email = vincenjes@gmail.com
 description = An SDK for the Lord of the Rings API. Created for a coding challenge.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vincjess
 classifiers =
```

