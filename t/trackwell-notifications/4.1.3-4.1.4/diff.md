# Comparing `tmp/trackwell-notifications-4.1.3.tar.gz` & `tmp/trackwell-notifications-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackwell-notifications-4.1.3.tar", last modified: Wed Jan 25 12:00:37 2023, max compression
+gzip compressed data, was "trackwell-notifications-4.1.4.tar", last modified: Wed May 31 11:32:27 2023, max compression
```

## Comparing `trackwell-notifications-4.1.3.tar` & `trackwell-notifications-4.1.4.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2928 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2243 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4973 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     7222 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/api/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/management/commands/update_notification_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3145 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/migrations/0002_add_image_field.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/migrations/0003_add_translations_and_url_filtering.py
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/migrations/0004_auto_20200915_1222.py
--rw-rw-rw-   0 root         (0) root         (0)     7366 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/migrations/0005_auto_20220701_1341.py
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/migrations/0006_remove_all_sns_push_notification_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     4940 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/migrations/0007_auto_20230113_1417.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/notifications/models/
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11390 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/models/notifications.py
--rw-rw-rw-   0 root         (0) root         (0)    16244 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/models/push.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/notifications/push/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/push/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4396 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/push/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/push/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/static/notifications/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/notifications/static/notifications/css/
--rw-rw-rw-   0 root         (0) root         (0)     4226 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/static/notifications/css/notifications.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/notifications/static/notifications/font/
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/static/notifications/font/notificationsfont.ttf
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/static/notifications/font/notificationsfont.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/notifications/static/notifications/js/
--rw-rw-rw-   0 root         (0) root         (0)    10371 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/static/notifications/js/NotificationsOnlyAPI.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.394791 trackwell-notifications-4.1.3/notifications/templates/admin/notifications/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/notifications/templates/admin/notifications/notification/
--rw-rw-rw-   0 root         (0) root         (0)     1464 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/templates/admin/notifications/notification/change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/notifications/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2629 2023-01-25 11:52:45.000000 trackwell-notifications-4.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1287 2023-01-25 12:00:36.000000 trackwell-notifications-4.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 12:00:37.398791 trackwell-notifications-4.1.3/trackwell_notifications.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2928 2023-01-25 12:00:37.000000 trackwell-notifications-4.1.3/trackwell_notifications.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1612 2023-01-25 12:00:37.000000 trackwell-notifications-4.1.3/trackwell_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 12:00:37.000000 trackwell-notifications-4.1.3/trackwell_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-01-25 12:00:37.000000 trackwell-notifications-4.1.3/trackwell_notifications.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-25 12:00:37.000000 trackwell-notifications-4.1.3/trackwell_notifications.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2243 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.794757 trackwell-notifications-4.1.4/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.794757 trackwell-notifications-4.1.4/notifications/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4399 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7128 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/api/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.794757 trackwell-notifications-4.1.4/notifications/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.794757 trackwell-notifications-4.1.4/notifications/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/management/commands/update_notification_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.794757 trackwell-notifications-4.1.4/notifications/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     3145 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/migrations/0002_add_image_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/migrations/0003_add_translations_and_url_filtering.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/migrations/0004_auto_20200915_1222.py
+-rw-rw-rw-   0 root         (0) root         (0)     7366 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/migrations/0005_auto_20220701_1341.py
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/migrations/0006_remove_all_sns_push_notification_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4940 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/migrations/0007_auto_20230113_1417.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/notifications/models/
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11424 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/models/notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)    16244 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/models/push.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/notifications/push/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/push/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4396 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/push/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/push/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.790758 trackwell-notifications-4.1.4/notifications/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.790758 trackwell-notifications-4.1.4/notifications/static/notifications/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/notifications/static/notifications/css/
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/static/notifications/css/notifications.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/notifications/static/notifications/font/
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/static/notifications/font/notificationsfont.ttf
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/static/notifications/font/notificationsfont.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/notifications/static/notifications/js/
+-rw-rw-rw-   0 root         (0) root         (0)    10371 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/static/notifications/js/NotificationsOnlyAPI.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.790758 trackwell-notifications-4.1.4/notifications/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.794757 trackwell-notifications-4.1.4/notifications/templates/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.794757 trackwell-notifications-4.1.4/notifications/templates/admin/notifications/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/notifications/templates/admin/notifications/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/templates/admin/notifications/notification/change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/notifications/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2629 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2023-05-31 11:32:26.000000 trackwell-notifications-4.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:32:27.798757 trackwell-notifications-4.1.4/trackwell_notifications.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-05-31 11:32:27.000000 trackwell-notifications-4.1.4/trackwell_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-05-31 11:32:27.000000 trackwell-notifications-4.1.4/trackwell_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 11:32:27.000000 trackwell-notifications-4.1.4/trackwell_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-31 11:32:27.000000 trackwell-notifications-4.1.4/trackwell_notifications.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-31 11:32:27.000000 trackwell-notifications-4.1.4/trackwell_notifications.egg-info/top_level.txt
```

### Comparing `trackwell-notifications-4.1.3/PKG-INFO` & `trackwell-notifications-4.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackwell-notifications
-Version: 4.1.3
+Version: 4.1.4
 Summary: A simple Django app to support Notifications.
 Home-page: UNKNOWN
 Author: trackwell
 Author-email: 
 License: NA
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trackwell-notifications Version: 4.1.3 Summary: A
+Metadata-Version: 2.1 Name: trackwell-notifications Version: 4.1.4 Summary: A
 simple Django app to support Notifications. Home-page: UNKNOWN Author:
 trackwell Author-email: License: NA Platform: UNKNOWN Classifier: Environment
 :: Web Environment Classifier: Framework :: Django Classifier: Framework ::
 Django :: 2.2 Classifier: Framework :: Django :: 3.2 Classifier: Intended
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
```

### Comparing `trackwell-notifications-4.1.3/README.rst` & `trackwell-notifications-4.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/admin.py` & `trackwell-notifications-4.1.4/notifications/admin.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/api/serializers.py` & `trackwell-notifications-4.1.4/notifications/api/serializers.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,27 +25,30 @@
     regex = serializers.CharField(source='display_only_if_url_path_matches_regex')
     class Meta:
         model = Notification
         fields = ('name', 'message', 'snooze_time', 'snooze_lock', 'look', 'image', 'regex',)
 
 
 class UserNotificationSerializer(serializers.HyperlinkedModelSerializer):
-    notification = NotificationSerializer()
-    user = UserSerializer()
+    notification = NotificationSerializer(read_only=True)
+    user = UserSerializer(read_only=True)
+    id = serializers.IntegerField(read_only=True)
+    seen = serializers.BooleanField(read_only=True)
+    answer_string = serializers.CharField(
+        max_length=255,
+        allow_null=True,
+        allow_blank=True,
+        required=False,
+        default=None,
+        write_only=True
+    )
 
     class Meta:
         model = UserNotification
-        fields = ('id', 'notification', 'user', 'seen', 'answer')
-
-
-class UserNotificationPutSerializer(serializers.HyperlinkedModelSerializer):
-
-    class Meta:
-        model = UserNotification
-        fields = ('answer', 'answer_string')
+        fields = ('id', 'notification', 'user', 'seen', 'answer', 'answer_string')
 
 
 class DeviceSerializer(ModelSerializer):
     # The origianl code for this serializer comes from the fcm-django module and is subject
     # to an MIT license. We may have modified the code from the original source to fit our needs.
     # For original source see: https://github.com/xtrinch/fcm-django
     class Meta:
```

### Comparing `trackwell-notifications-4.1.3/notifications/api/views.py` & `trackwell-notifications-4.1.4/notifications/api/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,75 +7,58 @@
     mixins,
     permissions,
     serializers,
     status,
     viewsets,
 )
 from rest_framework.decorators import action
+from rest_framework.generics import get_object_or_404
 from rest_framework.mixins import CreateModelMixin
 from rest_framework.response import Response
 from rest_framework.viewsets import GenericViewSet, ModelViewSet, ReadOnlyModelViewSet
 
 from django.db.models import Q, Count, BooleanField
 from django.db.models.functions import Cast
 from django_filters.rest_framework import DjangoFilterBackend
+from django.http import Http404
 
 from notifications.models import (
     UserDevice,
     UserNotification,
     Notification,
     Topic,
 )
 from notifications.push.settings import SETTINGS
 
 from .permissions import IsOwner
+from .filters import UserNotificationsFilter
 from .serializers import (
     DeviceSerializer,
     TopicSerializer,
     UserNotificationSerializer,
-    UserNotificationPutSerializer,
     NotificationSerializer,
 )
 
 
-class UserNotificationViewSet(mixins.RetrieveModelMixin, mixins.UpdateModelMixin, viewsets.GenericViewSet):
+class UserNotificationViewSet(
+    mixins.RetrieveModelMixin,
+    mixins.UpdateModelMixin,
+    mixins.ListModelMixin,
+    viewsets.GenericViewSet,
+):
     queryset = UserNotification.objects.all()
 
-    permission_classes = (permissions.IsAuthenticated,)
+    permission_classes = (permissions.IsAuthenticated, IsOwner, )
+    serializer_class = UserNotificationSerializer
 
-    filter_backends = (filters.SearchFilter, DjangoFilterBackend)
-
-    def get_serializer_class(self):
-        if self.request.method in ['PUT', 'PATCH']:
-            serializer_class = UserNotificationPutSerializer
-        else:
-            serializer_class = UserNotificationSerializer
-        return serializer_class
-
-    def list(self, request):
-        queryset = self.queryset.filter(
-            Q(user=self.request.user) &
-            (Q(next_display__isnull=True) | Q(next_display__lte=datetime.datetime.now())) &
-            (Q(notification__expires__isnull=True) | Q(notification__expires__gte=datetime.datetime.now())) &
-            (Q(notification__active_from__isnull=True) | Q(notification__active_from__lt=datetime.datetime.now()))
-        ).exclude(answer=True).select_related('notification', 'user').order_by('timestamp', 'id')
-        path = request.query_params.get('path', None)
-        if path is not None:
-            queryset = [
-                un for un in queryset
-                if re.match(un.notification.display_only_if_url_path_matches_regex, path) is not None
-            ]
-        serializer = self.get_serializer(queryset, many=True)
-        return Response(serializer.data)
+    filter_backends = (filters.SearchFilter, UserNotificationsFilter)
 
     def update(self, request, *args, **kwargs):
         partial = kwargs.pop('partial', False)
         instance = self.get_object()
-        if instance.user != request.user:
-            raise serializers.ValidationError('User can only change his own usernotifications')
         serializer = self.get_serializer(instance, data=request.data, partial=partial)
         serializer.is_valid(raise_exception=True)
         self.perform_update(serializer)
 
         if getattr(instance, '_prefetched_objects_cache', None):
             # If 'prefetch_related' has been applied to a queryset, we need to
             # forcibly invalidate the prefetch cache on the instance.
@@ -88,23 +71,18 @@
     queryset = Notification.objects.all()
 
     permission_classes = (permissions.IsAdminUser,)
     filter_backends = (filters.SearchFilter, DjangoFilterBackend)
 
     serializer_class = NotificationSerializer
 
-    def list(self, request):
-        queryset = Notification.objects.filter()
-        serializer = self.get_serializer(queryset, many=True)
-        return Response(serializer.data)
-
 
 # Mixins
 class DeviceViewSetMixin:
-    lookup_field = "registration_id"
+    lookup_field = "device_id"
 
     def create(self, request, *args, **kwargs):
         serializer = None
         is_update = False
         if (
             SETTINGS.get("UPDATE_ON_DUPLICATE_REG_ID")
             and "registration_id" in request.data
@@ -160,14 +138,45 @@
 
 
 # ViewSets
 class DeviceViewSet(DeviceViewSetMixin, ModelViewSet):
     queryset = UserDevice.objects.order_by("-id")
     serializer_class = DeviceSerializer
 
+    def get_object(self):
+        """
+        Returns the device requested by either device_id or registration_id.
+
+        Tries to fetch the device by device_id first, but if it fails
+        it will fallback to feth it via registration_id
+        """
+        queryset = self.filter_queryset(self.get_queryset())
+
+        # Perform the lookup filtering.
+        lookup_url_kwarg = self.lookup_url_kwarg or self.lookup_field
+
+        assert lookup_url_kwarg in self.kwargs, (
+            'Expected view %s to be called with a URL keyword argument '
+            'named "%s". Fix your URL conf, or set the `.lookup_field` '
+            'attribute on the view correctly.' %
+            (self.__class__.__name__, lookup_url_kwarg)
+        )
+
+        filter_kwargs = {self.lookup_field: self.kwargs[lookup_url_kwarg]}
+        try:
+            obj = get_object_or_404(queryset, **filter_kwargs)
+        except Http404:
+            filter_kwargs = {'registration_id': self.kwargs[lookup_url_kwarg]}
+            obj = get_object_or_404(queryset, **filter_kwargs)
+
+        # May raise a permission denied
+        self.check_object_permissions(self.request, obj)
+
+        return obj
+
 
 class DeviceCreateOnlyViewSet(DeviceViewSetMixin, CreateModelMixin, GenericViewSet):
     queryset = UserDevice.objects.all()
     serializer_class = DeviceSerializer
 
 
 class DeviceAuthorizedViewSet(AuthorizedMixin, DeviceViewSet):
```

### Comparing `trackwell-notifications-4.1.3/notifications/middleware.py` & `trackwell-notifications-4.1.4/notifications/middleware.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/migrations/0001_initial.py` & `trackwell-notifications-4.1.4/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/migrations/0002_add_image_field.py` & `trackwell-notifications-4.1.4/notifications/migrations/0002_add_image_field.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/migrations/0003_add_translations_and_url_filtering.py` & `trackwell-notifications-4.1.4/notifications/migrations/0003_add_translations_and_url_filtering.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/migrations/0004_auto_20200915_1222.py` & `trackwell-notifications-4.1.4/notifications/migrations/0004_auto_20200915_1222.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/migrations/0005_auto_20220701_1341.py` & `trackwell-notifications-4.1.4/notifications/migrations/0005_auto_20220701_1341.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/migrations/0006_remove_all_sns_push_notification_setup.py` & `trackwell-notifications-4.1.4/notifications/migrations/0006_remove_all_sns_push_notification_setup.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/migrations/0007_auto_20230113_1417.py` & `trackwell-notifications-4.1.4/notifications/migrations/0007_auto_20230113_1417.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/models/notifications.py` & `trackwell-notifications-4.1.4/notifications/models/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,24 +279,24 @@
             unseen[self.id] = datetime.datetime.now() - datetime.timedelta(minutes=10)
         if len(unseen) == 0:
             return cache.delete(Notification.notification_key(self.user))
         return cache.set(Notification.notification_key(self.user), unseen, timeout=None)
 
     def send_push_notification(self) -> None:
         """Send push notification for this notification"""
-        if not self.notification.is_push:
+        if not self.notification.is_push or not self.user.userdevice_set.exists():
             return
         default_language = get_default_language()
         profile = getattr(self.user, 'profile', None)
         prefs = getattr(profile, 'prefs', {})
         language = prefs.get('language', default_language)
         messages = self.notification.get_push_notification_messages()
         msg = messages.get(language, messages.get(default_language))
         if msg is not None:
-            Device.objects.filter(user=self.user).send_message(msg)
+            self.user.userdevice_set.all().send_message(msg)
 
     def save(self, *args, **kwargs) -> None:
         """Override save so it updates cache and does some snoozing"""
         if self.answer is not None:
             self.seen = True
         if self.seen and not self.answer:
             snooze_time = self.notification.snooze_time or 1
```

### Comparing `trackwell-notifications-4.1.3/notifications/models/push.py` & `trackwell-notifications-4.1.4/notifications/models/push.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/push/fields.py` & `trackwell-notifications-4.1.4/notifications/push/fields.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/push/settings.py` & `trackwell-notifications-4.1.4/notifications/push/settings.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/static/notifications/css/notifications.css` & `trackwell-notifications-4.1.4/notifications/static/notifications/css/notifications.css`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/static/notifications/font/notificationsfont.ttf` & `trackwell-notifications-4.1.4/notifications/static/notifications/font/notificationsfont.ttf`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/static/notifications/font/notificationsfont.woff` & `trackwell-notifications-4.1.4/notifications/static/notifications/font/notificationsfont.woff`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/static/notifications/js/NotificationsOnlyAPI.js` & `trackwell-notifications-4.1.4/notifications/static/notifications/js/NotificationsOnlyAPI.js`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/templates/admin/notifications/notification/change_form.html` & `trackwell-notifications-4.1.4/notifications/templates/admin/notifications/notification/change_form.html`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/notifications/utils.py` & `trackwell-notifications-4.1.4/notifications/utils.py`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/requirements.txt` & `trackwell-notifications-4.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `trackwell-notifications-4.1.3/setup.py` & `trackwell-notifications-4.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='trackwell-notifications',
-    version='4.1.3',
+    version='4.1.4',
     packages=find_packages(),
     include_package_data=True,
     license='NA',  # example license
     description='A simple Django app to support Notifications.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='',
```

### Comparing `trackwell-notifications-4.1.3/trackwell_notifications.egg-info/PKG-INFO` & `trackwell-notifications-4.1.4/trackwell_notifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackwell-notifications
-Version: 4.1.3
+Version: 4.1.4
 Summary: A simple Django app to support Notifications.
 Home-page: UNKNOWN
 Author: trackwell
 Author-email: 
 License: NA
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trackwell-notifications Version: 4.1.3 Summary: A
+Metadata-Version: 2.1 Name: trackwell-notifications Version: 4.1.4 Summary: A
 simple Django app to support Notifications. Home-page: UNKNOWN Author:
 trackwell Author-email: License: NA Platform: UNKNOWN Classifier: Environment
 :: Web Environment Classifier: Framework :: Django Classifier: Framework ::
 Django :: 2.2 Classifier: Framework :: Django :: 3.2 Classifier: Intended
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
```

### Comparing `trackwell-notifications-4.1.3/trackwell_notifications.egg-info/SOURCES.txt` & `trackwell-notifications-4.1.4/trackwell_notifications.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 notifications/__init__.py
 notifications/admin.py
 notifications/middleware.py
 notifications/translation.py
 notifications/utils.py
 notifications/api/__init__.py
+notifications/api/filters.py
 notifications/api/permissions.py
 notifications/api/serializers.py
 notifications/api/views.py
 notifications/management/__init__.py
 notifications/management/commands/__init__.py
 notifications/management/commands/update_notification_cache.py
 notifications/migrations/0001_initial.py
```

