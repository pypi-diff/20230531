# Comparing `tmp/djlds-2023.5.11.tar.gz` & `tmp/djlds-2023.5.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\djlds-2023.5.11.tar", last modified: Thu May 11 06:31:54 2023, max compression
+gzip compressed data, was "dist\djlds-2023.5.31.tar", last modified: Wed May 31 11:14:10 2023, max compression
```

## Comparing `djlds-2023.5.11.tar` & `djlds-2023.5.31.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/
-drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/djlds/
--rw-rw-rw-   0        0        0    11686 2022-11-22 10:26:59.000000 djlds-2023.5.11/djlds/admin.py
--rw-rw-rw-   0        0        0    18794 2023-05-11 06:23:49.000000 djlds-2023.5.11/djlds/import_export.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/djlds/management/
-drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/djlds/management/commands/
--rw-rw-rw-   0        0        0    13971 2019-12-09 08:21:17.000000 djlds-2023.5.11/djlds/management/commands/admin_generator.py
--rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2023.5.11/djlds/management/commands/__init__.py
--rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2023.5.11/djlds/management/__init__.py
--rw-rw-rw-   0        0        0    22248 2022-10-14 11:21:38.000000 djlds-2023.5.11/djlds/model.py
--rw-rw-rw-   0        0        0      449 2022-05-18 10:49:19.000000 djlds-2023.5.11/djlds/timezone.py
--rw-rw-rw-   0        0        0     2367 2022-01-21 02:47:57.000000 djlds-2023.5.11/djlds/user.py
--rw-rw-rw-   0        0        0     2859 2020-07-01 04:00:38.000000 djlds-2023.5.11/djlds/util.py
--rw-rw-rw-   0        0        0     1240 2020-03-20 08:22:22.000000 djlds-2023.5.11/djlds/xlsx_util.py
--rw-rw-rw-   0        0        0      656 2019-12-09 05:46:20.000000 djlds-2023.5.11/djlds/__about__.py
--rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2023.5.11/djlds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/djlds.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-12-09 09:34:28.000000 djlds-2023.5.11/djlds.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1359 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/requires.txt
--rw-rw-rw-   0        0        0      469 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2019-12-09 06:34:14.000000 djlds-2023.5.11/MANIFEST.in
--rw-rw-rw-   0        0        0     1359 2023-05-11 06:31:54.000000 djlds-2023.5.11/PKG-INFO
--rw-rw-rw-   0        0        0      329 2019-12-09 06:31:13.000000 djlds-2023.5.11/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 06:31:54.000000 djlds-2023.5.11/setup.cfg
--rw-rw-rw-   0        0        0     2916 2023-05-11 06:23:49.000000 djlds-2023.5.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:14:10.000000 djlds-2023.5.31/
+drwxrwxrwx   0        0        0        0 2023-05-31 11:14:10.000000 djlds-2023.5.31/djlds/
+-rw-rw-rw-   0        0        0    12117 2023-05-31 11:14:05.000000 djlds-2023.5.31/djlds/admin.py
+-rw-rw-rw-   0        0        0    18794 2023-05-11 06:23:49.000000 djlds-2023.5.31/djlds/import_export.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:14:10.000000 djlds-2023.5.31/djlds/management/
+drwxrwxrwx   0        0        0        0 2023-05-31 11:14:10.000000 djlds-2023.5.31/djlds/management/commands/
+-rw-rw-rw-   0        0        0    13971 2019-12-09 08:21:17.000000 djlds-2023.5.31/djlds/management/commands/admin_generator.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2023.5.31/djlds/management/commands/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2023.5.31/djlds/management/__init__.py
+-rw-rw-rw-   0        0        0    22248 2022-10-14 11:21:38.000000 djlds-2023.5.31/djlds/model.py
+-rw-rw-rw-   0        0        0      449 2022-05-18 10:49:19.000000 djlds-2023.5.31/djlds/timezone.py
+-rw-rw-rw-   0        0        0     2367 2022-01-21 02:47:57.000000 djlds-2023.5.31/djlds/user.py
+-rw-rw-rw-   0        0        0     2859 2020-07-01 04:00:38.000000 djlds-2023.5.31/djlds/util.py
+-rw-rw-rw-   0        0        0     1240 2020-03-20 08:22:22.000000 djlds-2023.5.31/djlds/xlsx_util.py
+-rw-rw-rw-   0        0        0      656 2019-12-09 05:46:20.000000 djlds-2023.5.31/djlds/__about__.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2023.5.31/djlds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:14:10.000000 djlds-2023.5.31/djlds.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-31 11:14:08.000000 djlds-2023.5.31/djlds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-12-09 09:34:28.000000 djlds-2023.5.31/djlds.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     1359 2023-05-31 11:14:08.000000 djlds-2023.5.31/djlds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-31 11:14:08.000000 djlds-2023.5.31/djlds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      469 2023-05-31 11:14:09.000000 djlds-2023.5.31/djlds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 11:14:08.000000 djlds-2023.5.31/djlds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2019-12-09 06:34:14.000000 djlds-2023.5.31/MANIFEST.in
+-rw-rw-rw-   0        0        0     1359 2023-05-31 11:14:10.000000 djlds-2023.5.31/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2019-12-09 06:31:13.000000 djlds-2023.5.31/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 11:14:10.000000 djlds-2023.5.31/setup.cfg
+-rw-rw-rw-   0        0        0     2916 2023-05-31 11:14:05.000000 djlds-2023.5.31/setup.py
```

### Comparing `djlds-2023.5.11/djlds/admin.py` & `djlds-2023.5.31/djlds/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,7 +303,20 @@
         else:
             info = ''
         file_size = queryset.aggregate(**{field: Sum(field)})[field]
         # print(human_size(file_size))
         self.message_user(request, f'选择内容的文件大小：{human_size(file_size)}' + info, level=messages.INFO)
 
     action_calc_file_size.short_description = "计算选择内容的文件大小"
+
+
+class QuickDeleteQuerysetAction:
+    # actions = ['action_quick_delete']
+
+    def action_quick_delete(self, request, queryset):
+        """
+        直接删除选择的内容（不需要确认，谨慎操作）
+        """
+
+        self.message_user(request, f'{queryset.delete()}', level=messages.INFO)
+
+    action_quick_delete.short_description = "直接删除选择的内容（不需要确认，谨慎操作）"
```

### Comparing `djlds-2023.5.11/djlds/import_export.py` & `djlds-2023.5.31/djlds/import_export.py`

 * *Files identical despite different names*

### Comparing `djlds-2023.5.11/djlds/management/commands/admin_generator.py` & `djlds-2023.5.31/djlds/management/commands/admin_generator.py`

 * *Files identical despite different names*

### Comparing `djlds-2023.5.11/djlds/model.py` & `djlds-2023.5.31/djlds/model.py`

 * *Files identical despite different names*

### Comparing `djlds-2023.5.11/djlds/user.py` & `djlds-2023.5.31/djlds/user.py`

 * *Files identical despite different names*

### Comparing `djlds-2023.5.11/djlds/util.py` & `djlds-2023.5.31/djlds/util.py`

 * *Files identical despite different names*

### Comparing `djlds-2023.5.11/djlds/xlsx_util.py` & `djlds-2023.5.31/djlds/xlsx_util.py`

 * *Files identical despite different names*

### Comparing `djlds-2023.5.11/djlds/__about__.py` & `djlds-2023.5.31/djlds/__about__.py`

 * *Files identical despite different names*

### Comparing `djlds-2023.5.11/djlds.egg-info/PKG-INFO` & `djlds-2023.5.31/djlds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djlds
-Version: 2023.5.11
+Version: 2023.5.31
 Summary: 常用 Django 功能集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/django-utils-lds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/django-utils-lds
 Description: # django-utils-lds
```

### Comparing `djlds-2023.5.11/PKG-INFO` & `djlds-2023.5.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djlds
-Version: 2023.5.11
+Version: 2023.5.31
 Summary: 常用 Django 功能集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/django-utils-lds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/django-utils-lds
 Description: # django-utils-lds
```

### Comparing `djlds-2023.5.11/setup.py` & `djlds-2023.5.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿import os
 import sys
 
 from setuptools import setup, find_packages
 
-version = '2023.5.11'
+version = '2023.5.31'
 
 """
 pip install -U spider-utils
 pip --no-cache-dir install -U spider-utils
 
 # 检查错误
 # twine check dist/*
```

