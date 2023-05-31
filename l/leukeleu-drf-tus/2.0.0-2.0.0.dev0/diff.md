# Comparing `tmp/leukeleu-drf-tus-2.0.0.tar.gz` & `tmp/leukeleu-drf-tus-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leukeleu-drf-tus-2.0.0.tar", last modified: Wed May 31 15:27:38 2023, max compression
+gzip compressed data, was "leukeleu-drf-tus-2.0.0.dev0.tar", last modified: Wed May 31 15:00:42 2023, max compression
```

## Comparing `leukeleu-drf-tus-2.0.0.tar` & `leukeleu-drf-tus-2.0.0.dev0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.474201 leukeleu-drf-tus-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-31 15:27:38.474201 leukeleu-drf-tus-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.470201 leukeleu-drf-tus-2.0.0/leukeleu_drf_tus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-31 15:27:38.000000 leukeleu-drf-tus-2.0.0/leukeleu_drf_tus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-31 15:27:38.000000 leukeleu-drf-tus-2.0.0/leukeleu_drf_tus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:27:38.000000 leukeleu-drf-tus-2.0.0/leukeleu_drf_tus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:27:38.000000 leukeleu-drf-tus-2.0.0/leukeleu_drf_tus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 15:27:38.000000 leukeleu-drf-tus-2.0.0/leukeleu_drf_tus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 15:27:38.000000 leukeleu-drf-tus-2.0.0/leukeleu_drf_tus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.470201 leukeleu-drf-tus-2.0.0/rest_framework_tus/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.474201 leukeleu-drf-tus-2.0.0/rest_framework_tus/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/migrations/0002_auto_20170406_0620.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/migrations/0003_auto_20170619_0358.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/migrations/0004_auto_20200317_1002.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/migrations/0005_alter_upload_upload_length.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.466201 leukeleu-drf-tus-2.0.0/rest_framework_tus/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.474201 leukeleu-drf-tus-2.0.0/rest_framework_tus/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/static/css/rest_framework_tus.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.474201 leukeleu-drf-tus-2.0.0/rest_framework_tus/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/static/js/rest_framework_tus.js
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.466201 leukeleu-drf-tus-2.0.0/rest_framework_tus/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.474201 leukeleu-drf-tus-2.0.0/rest_framework_tus/templates/rest_framework_tus/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/templates/rest_framework_tus/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/rest_framework_tus/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 15:27:38.474201 leukeleu-drf-tus-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:27:38.474201 leukeleu-drf-tus-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-31 15:27:26.000000 leukeleu-drf-tus-2.0.0/tests/test_settings.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.991886 leukeleu-drf-tus-2.0.0.dev0/
+-rw-r--r--   0 thomas     (501) staff       (20)     3206 2023-05-31 08:45:37.000000 leukeleu-drf-tus-2.0.0.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 thomas     (501) staff       (20)     2267 2023-05-31 08:45:37.000000 leukeleu-drf-tus-2.0.0.dev0/HISTORY.md
+-rw-r--r--   0 thomas     (501) staff       (20)     2136 2023-05-31 08:45:36.000000 leukeleu-drf-tus-2.0.0.dev0/LICENSE
+-rw-r--r--   0 thomas     (501) staff       (20)      164 2023-05-31 08:45:37.000000 leukeleu-drf-tus-2.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 thomas     (501) staff       (20)     4348 2023-05-31 15:00:42.991961 leukeleu-drf-tus-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     1234 2023-05-31 08:45:37.000000 leukeleu-drf-tus-2.0.0.dev0/README.md
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.986495 leukeleu-drf-tus-2.0.0.dev0/leukeleu_drf_tus.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)     4348 2023-05-31 15:00:42.000000 leukeleu-drf-tus-2.0.0.dev0/leukeleu_drf_tus.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     1337 2023-05-31 15:00:42.000000 leukeleu-drf-tus-2.0.0.dev0/leukeleu_drf_tus.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-05-31 15:00:42.000000 leukeleu-drf-tus-2.0.0.dev0/leukeleu_drf_tus.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-05-31 08:46:26.000000 leukeleu-drf-tus-2.0.0.dev0/leukeleu_drf_tus.egg-info/not-zip-safe
+-rw-r--r--   0 thomas     (501) staff       (20)       77 2023-05-31 15:00:42.000000 leukeleu-drf-tus-2.0.0.dev0/leukeleu_drf_tus.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       19 2023-05-31 15:00:42.000000 leukeleu-drf-tus-2.0.0.dev0/leukeleu_drf_tus.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.990173 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/
+-rw-r--r--   0 thomas     (501) staff       (20)      278 2023-05-31 08:45:36.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      177 2023-05-31 08:45:36.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/apps.py
+-rw-r--r--   0 thomas     (501) staff       (20)      293 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/constants.py
+-rw-r--r--   0 thomas     (501) staff       (20)      281 2022-10-13 14:18:33.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/exceptions.py
+-rw-r--r--   0 thomas     (501) staff       (20)     5096 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/middleware.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.991086 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/migrations/
+-rw-r--r--   0 thomas     (501) staff       (20)     1255 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/migrations/0001_initial.py
+-rw-r--r--   0 thomas     (501) staff       (20)      440 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/migrations/0002_auto_20170406_0620.py
+-rw-r--r--   0 thomas     (501) staff       (20)      570 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/migrations/0003_auto_20170619_0358.py
+-rw-r--r--   0 thomas     (501) staff       (20)      497 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/migrations/0004_auto_20200317_1002.py
+-rw-r--r--   0 thomas     (501) staff       (20)      407 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/migrations/0005_alter_upload_upload_length.py
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2022-10-13 14:15:02.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/migrations/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     4878 2022-10-13 14:18:37.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/models.py
+-rw-r--r--   0 thomas     (501) staff       (20)      280 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/parsers.py
+-rw-r--r--   0 thomas     (501) staff       (20)      802 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/receivers.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1827 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/routers.py
+-rw-r--r--   0 thomas     (501) staff       (20)      228 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/serializers.py
+-rw-r--r--   0 thomas     (501) staff       (20)      874 2023-05-31 08:45:36.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/settings.py
+-rw-r--r--   0 thomas     (501) staff       (20)      276 2022-10-13 14:17:59.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/signals.py
+-rw-r--r--   0 thomas     (501) staff       (20)       76 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/states.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.983815 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/static/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.991195 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/static/css/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2022-10-13 14:15:02.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/static/css/rest_framework_tus.css
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.991316 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/static/js/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2022-10-13 14:15:02.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/static/js/rest_framework_tus.js
+-rw-r--r--   0 thomas     (501) staff       (20)     1236 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/storage.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.983944 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/templates/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.991425 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/templates/rest_framework_tus/
+-rw-r--r--   0 thomas     (501) staff       (20)      661 2022-10-13 14:15:02.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/templates/rest_framework_tus/base.html
+-rw-r--r--   0 thomas     (501) staff       (20)      305 2022-10-18 13:44:51.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/urls.py
+-rw-r--r--   0 thomas     (501) staff       (20)     4567 2022-10-13 14:15:53.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/utils.py
+-rw-r--r--   0 thomas     (501) staff       (20)    12320 2023-05-31 08:45:36.000000 leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/views.py
+-rw-r--r--   0 thomas     (501) staff       (20)      478 2023-05-31 15:00:42.992343 leukeleu-drf-tus-2.0.0.dev0/setup.cfg
+-rwxr-xr-x   0 thomas     (501) staff       (20)     2359 2023-05-31 15:00:21.000000 leukeleu-drf-tus-2.0.0.dev0/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-31 15:00:42.991717 leukeleu-drf-tus-2.0.0.dev0/tests/
+-rw-r--r--   0 thomas     (501) staff       (20)      682 2023-05-31 08:45:36.000000 leukeleu-drf-tus-2.0.0.dev0/tests/test_settings.py
```

### Comparing `leukeleu-drf-tus-2.0.0/CONTRIBUTING.rst` & `leukeleu-drf-tus-2.0.0.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/HISTORY.md` & `leukeleu-drf-tus-2.0.0.dev0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # History
 
-## 2.0.0 (2023-05-31)
-
-* Release to PyPi
-
 ## 2.0.0.dev0 (2023-05-25)
 
 * Renamed package to leukeleu-drf-tus
 * Major refactoring
 
 ## 1.21.2 (2018-09-04)
```

### Comparing `leukeleu-drf-tus-2.0.0/LICENSE` & `leukeleu-drf-tus-2.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/PKG-INFO` & `leukeleu-drf-tus-2.0.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leukeleu-drf-tus
-Version: 2.0.0
+Version: 2.0.0.dev0
 Summary: A Tus (tus.io) library for Django Rest Framework
 Home-page: https://github.com/leukeleu/leukeleu-drf-tus
 Author: Leukeleu
 Author-email: info@leukeleu.nl
 License: MIT
 Keywords: drf-tus
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,18 +76,14 @@
 
 Does the code actually work?
 
     docker compose exec python make coveragetest
 
 # History
 
-## 2.0.0 (2023-05-31)
-
-* Release to PyPi
-
 ## 2.0.0.dev0 (2023-05-25)
 
 * Renamed package to leukeleu-drf-tus
 * Major refactoring
 
 ## 1.21.2 (2018-09-04)
```

### Comparing `leukeleu-drf-tus-2.0.0/README.md` & `leukeleu-drf-tus-2.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/leukeleu_drf_tus.egg-info/PKG-INFO` & `leukeleu-drf-tus-2.0.0.dev0/leukeleu_drf_tus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leukeleu-drf-tus
-Version: 2.0.0
+Version: 2.0.0.dev0
 Summary: A Tus (tus.io) library for Django Rest Framework
 Home-page: https://github.com/leukeleu/leukeleu-drf-tus
 Author: Leukeleu
 Author-email: info@leukeleu.nl
 License: MIT
 Keywords: drf-tus
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,18 +76,14 @@
 
 Does the code actually work?
 
     docker compose exec python make coveragetest
 
 # History
 
-## 2.0.0 (2023-05-31)
-
-* Release to PyPi
-
 ## 2.0.0.dev0 (2023-05-25)
 
 * Renamed package to leukeleu-drf-tus
 * Major refactoring
 
 ## 1.21.2 (2018-09-04)
```

### Comparing `leukeleu-drf-tus-2.0.0/leukeleu_drf_tus.egg-info/SOURCES.txt` & `leukeleu-drf-tus-2.0.0.dev0/leukeleu_drf_tus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/middleware.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/middleware.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/migrations/0001_initial.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/migrations/0003_auto_20170619_0358.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/migrations/0003_auto_20170619_0358.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/models.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/models.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/receivers.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/receivers.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/routers.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/routers.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/settings.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/settings.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/storage.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/storage.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/templates/rest_framework_tus/base.html` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/templates/rest_framework_tus/base.html`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/utils.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/utils.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/rest_framework_tus/views.py` & `leukeleu-drf-tus-2.0.0.dev0/rest_framework_tus/views.py`

 * *Files identical despite different names*

### Comparing `leukeleu-drf-tus-2.0.0/setup.py` & `leukeleu-drf-tus-2.0.0.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 history = (REPO_DIR / "HISTORY.md").read_text()
 
 setup(
     name="leukeleu-drf-tus",
     version=version,
     description="""A Tus (tus.io) library for Django Rest Framework""",
     long_description=f"{readme}\n{history}",
-    long_description_content_type="text/markdown",
+    long_description_content_type = "text/markdown",
     author="Leukeleu",
     author_email="info@leukeleu.nl",
     url="https://github.com/leukeleu/leukeleu-drf-tus",
     packages=[
         "rest_framework_tus",
     ],
     include_package_data=True,
```

### Comparing `leukeleu-drf-tus-2.0.0/tests/test_settings.py` & `leukeleu-drf-tus-2.0.0.dev0/tests/test_settings.py`

 * *Files identical despite different names*

