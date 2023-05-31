# Comparing `tmp/drf-api-tracking-1.8.3.tar.gz` & `tmp/drf-api-tracking-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-api-tracking-1.8.3.tar", last modified: Tue May 23 19:20:38 2023, max compression
+gzip compressed data, was "drf-api-tracking-1.8.4.tar", last modified: Wed May 31 20:57:44 2023, max compression
```

## Comparing `drf-api-tracking-1.8.3.tar` & `drf-api-tracking-1.8.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-23 19:20:38.727967 drf-api-tracking-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/base_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/base_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/management/commands/clearapilogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0002_auto_20170118_1713.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0003_add_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0004_add_verbose_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0005_auto_20171219_1537.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0006_auto_20180315_1442.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0007_merge_20180419_1646.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0008_auto_20200201_2048.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0009_view_method_max_length_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0010_auto_20200609_1404.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0011_auto_20201117_2016.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0012_auto_20210930_0713.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/rest_framework_tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 19:20:38.727967 drf-api-tracking-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.456479 drf-api-tracking-1.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-31 20:57:44.456479 drf-api-tracking-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.452479 drf-api-tracking-1.8.4/drf_api_tracking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-31 20:57:44.000000 drf-api-tracking-1.8.4/drf_api_tracking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-31 20:57:44.000000 drf-api-tracking-1.8.4/drf_api_tracking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:57:44.000000 drf-api-tracking-1.8.4/drf_api_tracking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 20:57:44.000000 drf-api-tracking-1.8.4/drf_api_tracking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-31 20:57:44.000000 drf-api-tracking-1.8.4/drf_api_tracking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.452479 drf-api-tracking-1.8.4/rest_framework_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/base_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/base_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.448479 drf-api-tracking-1.8.4/rest_framework_tracking/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.452479 drf-api-tracking-1.8.4/rest_framework_tracking/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/management/commands/clearapilogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.456479 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0002_auto_20170118_1713.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0003_add_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0004_add_verbose_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0005_auto_20171219_1537.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0006_auto_20180315_1442.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0007_merge_20180419_1646.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0008_auto_20200201_2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0009_view_method_max_length_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0010_auto_20200609_1404.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0011_auto_20201117_2016.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0012_auto_20210930_0713.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0013_apirequestlog_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.448479 drf-api-tracking-1.8.4/rest_framework_tracking/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.448479 drf-api-tracking-1.8.4/rest_framework_tracking/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.448479 drf-api-tracking-1.8.4/rest_framework_tracking/templates/admin/rest_framework_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:57:44.456479 drf-api-tracking-1.8.4/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 20:57:44.456479 drf-api-tracking-1.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-31 20:57:31.000000 drf-api-tracking-1.8.4/setup.py
```

### Comparing `drf-api-tracking-1.8.3/LICENSE` & `drf-api-tracking-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/PKG-INFO` & `drf-api-tracking-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-api-tracking
-Version: 1.8.3
+Version: 1.8.4
 Summary: Utils to log Django Rest Framework requests to the database
 Home-page: https://github.com/lingster/drf-api-tracking
 Author: Anna Schneider
 Author-email: anna@WattTime.org
 License: BSD
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `drf-api-tracking-1.8.3/README.md` & `drf-api-tracking-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/drf_api_tracking.egg-info/PKG-INFO` & `drf-api-tracking-1.8.4/drf_api_tracking.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-api-tracking
-Version: 1.8.3
+Version: 1.8.4
 Summary: Utils to log Django Rest Framework requests to the database
 Home-page: https://github.com/lingster/drf-api-tracking
 Author: Anna Schneider
 Author-email: anna@WattTime.org
 License: BSD
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `drf-api-tracking-1.8.3/drf_api_tracking.egg-info/SOURCES.txt` & `drf-api-tracking-1.8.4/drf_api_tracking.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,9 +27,10 @@
 rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py
 rest_framework_tracking/migrations/0007_merge_20180419_1646.py
 rest_framework_tracking/migrations/0008_auto_20200201_2048.py
 rest_framework_tracking/migrations/0009_view_method_max_length_200.py
 rest_framework_tracking/migrations/0010_auto_20200609_1404.py
 rest_framework_tracking/migrations/0011_auto_20201117_2016.py
 rest_framework_tracking/migrations/0012_auto_20210930_0713.py
+rest_framework_tracking/migrations/0013_apirequestlog_user_agent.py
 rest_framework_tracking/migrations/__init__.py
 rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html
```

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/admin.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/admin.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/app_settings.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/app_settings.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/base_mixins.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/base_mixins.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/base_models.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/base_models.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/management/commands/clearapilogs.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/management/commands/clearapilogs.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0001_initial.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0002_auto_20170118_1713.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0002_auto_20170118_1713.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0005_auto_20171219_1537.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0005_auto_20171219_1537.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0006_auto_20180315_1442.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0006_auto_20180315_1442.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0008_auto_20200201_2048.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0008_auto_20200201_2048.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0009_view_method_max_length_200.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0009_view_method_max_length_200.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0010_auto_20200609_1404.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0010_auto_20200609_1404.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0012_auto_20210930_0713.py` & `drf-api-tracking-1.8.4/rest_framework_tracking/migrations/0012_auto_20210930_0713.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html` & `drf-api-tracking-1.8.4/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.3/setup.py` & `drf-api-tracking-1.8.4/setup.py`

 * *Files identical despite different names*

