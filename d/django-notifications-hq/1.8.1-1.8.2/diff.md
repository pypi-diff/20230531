# Comparing `tmp/django-notifications-hq-1.8.1.tar.gz` & `tmp/django-notifications-hq-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-notifications-hq-1.8.1.tar", last modified: Tue May 30 23:44:30 2023, max compression
+gzip compressed data, was "django-notifications-hq-1.8.2.tar", last modified: Wed May 31 12:09:30 2023, max compression
```

## Comparing `django-notifications-hq-1.8.1.tar` & `django-notifications-hq-1.8.2.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.745783 django-notifications-hq-1.8.1/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1076 2023-05-30 00:35:00.000000 django-notifications-hq-1.8.1/AUTHORS.txt
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     6301 2023-05-30 00:50:48.000000 django-notifications-hq-1.8.1/CHANGELOG.md
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1563 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.1/LICENSE.txt
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      122 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/MANIFEST.in
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)    17791 2023-05-30 23:44:30.746069 django-notifications-hq-1.8.1/PKG-INFO
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)    16575 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/README.md
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.721054 django-notifications-hq-1.8.1/django_notifications_hq.egg-info/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)    17791 2023-05-30 23:44:30.000000 django-notifications-hq-1.8.1/django_notifications_hq.egg-info/PKG-INFO
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2089 2023-05-30 23:44:30.000000 django-notifications-hq-1.8.1/django_notifications_hq.egg-info/SOURCES.txt
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)        1 2023-05-30 23:44:30.000000 django-notifications-hq-1.8.1/django_notifications_hq.egg-info/dependency_links.txt
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)       68 2023-05-30 23:44:30.000000 django-notifications-hq-1.8.1/django_notifications_hq.egg-info/requires.txt
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)       14 2023-05-30 23:44:30.000000 django-notifications-hq-1.8.1/django_notifications_hq.egg-info/top_level.txt
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.725511 django-notifications-hq-1.8.1/notifications/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      406 2023-05-30 00:58:26.000000 django-notifications-hq-1.8.1/notifications/__init__.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1038 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/admin.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      499 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/apps.py
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.726585 django-notifications-hq-1.8.1/notifications/base/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.1/notifications/base/__init__.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      440 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/base/admin.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)    13483 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/base/models.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1416 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/helpers.py
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.712286 django-notifications-hq-1.8.1/notifications/locale/
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.712493 django-notifications-hq-1.8.1/notifications/locale/ru/
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.727027 django-notifications-hq-1.8.1/notifications/locale/ru/LC_MESSAGES/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     3489 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.731501 django-notifications-hq-1.8.1/notifications/migrations/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2201 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/migrations/0001_initial.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      595 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/migrations/0002_auto_20150224_1134.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      446 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/migrations/0003_notification_data.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      420 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/migrations/0004_auto_20150826_1508.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      532 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/migrations/0005_auto_20160504_1520.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      947 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/migrations/0006_indexes.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      458 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/migrations/0007_add_timestamp_index.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      469 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/migrations/0008_index_together_recipient_unread.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.1/notifications/migrations/__init__.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      826 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/models.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      427 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/settings.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      119 2023-05-27 21:33:35.000000 django-notifications-hq-1.8.1/notifications/signals.py
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.713006 django-notifications-hq-1.8.1/notifications/templates/
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.733700 django-notifications-hq-1.8.1/notifications/templates/notifications/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      130 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.1/notifications/templates/notifications/list.html
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      655 2023-05-27 21:34:32.000000 django-notifications-hq-1.8.1/notifications/templates/notifications/notice.html
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      220 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.1/notifications/templates/notifications/test_tags.html
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.735423 django-notifications-hq-1.8.1/notifications/templatetags/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.1/notifications/templatetags/__init__.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     4193 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/templatetags/notifications_tags.py
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.739307 django-notifications-hq-1.8.1/notifications/tests/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.1/notifications/tests/__init__.py
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.743036 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)       95 2023-05-27 21:34:30.000000 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/__init__.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      272 2023-05-27 21:34:27.000000 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/admin.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      204 2023-05-27 21:34:24.000000 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/apps.py
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.743916 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/migrations/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2720 2023-05-27 21:34:20.000000 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/migrations/0001_initial.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/migrations/__init__.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      270 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/models.py
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.744518 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/templatetags/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/templatetags/__init__.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)       67 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/templatetags/notifications_tags.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1791 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/tests/sample_notifications/tests.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2128 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/tests/settings.py
-drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-30 23:44:30.744958 django-notifications-hq-1.8.1/notifications/tests/templates/
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      507 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/tests/templates/test_live.html
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)    28778 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/tests/tests.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1821 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/tests/urls.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      909 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.1/notifications/tests/views.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1338 2023-05-27 21:33:35.000000 django-notifications-hq-1.8.1/notifications/urls.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)      267 2023-05-27 21:33:35.000000 django-notifications-hq-1.8.1/notifications/utils.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)     6142 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/notifications/views.py
--rw-r--r--   0 alvaro.mariano   (501) staff       (20)       67 2023-05-30 23:44:30.746716 django-notifications-hq-1.8.1/setup.cfg
--rwxr-xr-x   0 alvaro.mariano   (501) staff       (20)     2418 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.1/setup.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.735257 django-notifications-hq-1.8.2/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1076 2023-05-31 11:42:58.000000 django-notifications-hq-1.8.2/AUTHORS.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     6301 2023-05-31 12:06:28.000000 django-notifications-hq-1.8.2/CHANGELOG.md
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1563 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.2/LICENSE.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      122 2023-05-31 11:42:58.000000 django-notifications-hq-1.8.2/MANIFEST.in
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    17791 2023-05-31 12:09:30.735428 django-notifications-hq-1.8.2/PKG-INFO
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    16575 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/README.md
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.707378 django-notifications-hq-1.8.2/django_notifications_hq.egg-info/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    17791 2023-05-31 12:09:30.000000 django-notifications-hq-1.8.2/django_notifications_hq.egg-info/PKG-INFO
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2158 2023-05-31 12:09:30.000000 django-notifications-hq-1.8.2/django_notifications_hq.egg-info/SOURCES.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        1 2023-05-31 12:09:30.000000 django-notifications-hq-1.8.2/django_notifications_hq.egg-info/dependency_links.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       68 2023-05-31 12:09:30.000000 django-notifications-hq-1.8.2/django_notifications_hq.egg-info/requires.txt
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       14 2023-05-31 12:09:30.000000 django-notifications-hq-1.8.2/django_notifications_hq.egg-info/top_level.txt
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.713844 django-notifications-hq-1.8.2/notifications/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      406 2023-05-31 12:06:23.000000 django-notifications-hq-1.8.2/notifications/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1038 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/admin.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      499 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/apps.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.716007 django-notifications-hq-1.8.2/notifications/base/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.2/notifications/base/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      440 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/base/admin.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    13483 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/base/models.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1416 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/helpers.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.696869 django-notifications-hq-1.8.2/notifications/locale/
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.697137 django-notifications-hq-1.8.2/notifications/locale/ru/
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.716580 django-notifications-hq-1.8.2/notifications/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     3489 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.723058 django-notifications-hq-1.8.2/notifications/migrations/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2201 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/migrations/0001_initial.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      595 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/migrations/0002_auto_20150224_1134.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      446 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/migrations/0003_notification_data.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      420 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/migrations/0004_auto_20150826_1508.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      532 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/migrations/0005_auto_20160504_1520.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      947 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/migrations/0006_indexes.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      458 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/migrations/0007_add_timestamp_index.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      469 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/migrations/0008_index_together_recipient_unread.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     5448 2023-05-31 11:45:49.000000 django-notifications-hq-1.8.2/notifications/migrations/0009_alter_notification_options_and_more.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.2/notifications/migrations/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      826 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/models.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      427 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/settings.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      119 2023-05-27 21:33:35.000000 django-notifications-hq-1.8.2/notifications/signals.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.697866 django-notifications-hq-1.8.2/notifications/templates/
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.724639 django-notifications-hq-1.8.2/notifications/templates/notifications/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      130 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.2/notifications/templates/notifications/list.html
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      655 2023-05-27 21:34:32.000000 django-notifications-hq-1.8.2/notifications/templates/notifications/notice.html
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      220 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.2/notifications/templates/notifications/test_tags.html
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.725575 django-notifications-hq-1.8.2/notifications/templatetags/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.2/notifications/templatetags/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     4193 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/templatetags/notifications_tags.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.728548 django-notifications-hq-1.8.2/notifications/tests/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-04-29 22:21:11.000000 django-notifications-hq-1.8.2/notifications/tests/__init__.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.732371 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       95 2023-05-27 21:34:30.000000 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      272 2023-05-27 21:34:27.000000 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/admin.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      204 2023-05-27 21:34:24.000000 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/apps.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.733640 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/migrations/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2720 2023-05-27 21:34:20.000000 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/migrations/0001_initial.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/migrations/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      270 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/models.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.734250 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/templatetags/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)        0 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/templatetags/__init__.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       67 2023-05-24 00:18:10.000000 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/templatetags/notifications_tags.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1791 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/tests/sample_notifications/tests.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     2128 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/tests/settings.py
+drwxr-xr-x   0 alvaro.mariano   (501) staff       (20)        0 2023-05-31 12:09:30.734860 django-notifications-hq-1.8.2/notifications/tests/templates/
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      507 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/tests/templates/test_live.html
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)    28778 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/tests/tests.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1821 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/tests/urls.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      909 2023-05-27 21:32:18.000000 django-notifications-hq-1.8.2/notifications/tests/views.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     1338 2023-05-27 21:33:35.000000 django-notifications-hq-1.8.2/notifications/urls.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)      267 2023-05-27 21:33:35.000000 django-notifications-hq-1.8.2/notifications/utils.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)     6142 2023-05-30 00:49:08.000000 django-notifications-hq-1.8.2/notifications/views.py
+-rw-r--r--   0 alvaro.mariano   (501) staff       (20)       67 2023-05-31 12:09:30.736003 django-notifications-hq-1.8.2/setup.cfg
+-rwxr-xr-x   0 alvaro.mariano   (501) staff       (20)     2418 2023-05-31 11:42:58.000000 django-notifications-hq-1.8.2/setup.py
```

### Comparing `django-notifications-hq-1.8.1/AUTHORS.txt` & `django-notifications-hq-1.8.2/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/CHANGELOG.md` & `django-notifications-hq-1.8.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changelog
 
-## 1.8.1
+## 1.8.2
 
   - Added the migration for verbose_name changes
 
 ## 1.8.0
 
   - Added support for Django 4.1
   - Dropped support for Django < 3.2 and Python < 3.7
```

### Comparing `django-notifications-hq-1.8.1/LICENSE.txt` & `django-notifications-hq-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/PKG-INFO` & `django-notifications-hq-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-notifications-hq
-Version: 1.8.1
+Version: 1.8.2
 Summary: GitHub notifications alike app for Django.
 Home-page: http://github.com/django-notifications/django-notifications
 Author: django-notifications team
 Author-email: yang@yangyubo.com
 License: MIT
 Keywords: django notifications github action event stream
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-notifications-hq-1.8.1/README.md` & `django-notifications-hq-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/django_notifications_hq.egg-info/PKG-INFO` & `django-notifications-hq-1.8.2/django_notifications_hq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-notifications-hq
-Version: 1.8.1
+Version: 1.8.2
 Summary: GitHub notifications alike app for Django.
 Home-page: http://github.com/django-notifications/django-notifications
 Author: django-notifications team
 Author-email: yang@yangyubo.com
 License: MIT
 Keywords: django notifications github action event stream
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-notifications-hq-1.8.1/django_notifications_hq.egg-info/SOURCES.txt` & `django-notifications-hq-1.8.2/django_notifications_hq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 notifications/migrations/0002_auto_20150224_1134.py
 notifications/migrations/0003_notification_data.py
 notifications/migrations/0004_auto_20150826_1508.py
 notifications/migrations/0005_auto_20160504_1520.py
 notifications/migrations/0006_indexes.py
 notifications/migrations/0007_add_timestamp_index.py
 notifications/migrations/0008_index_together_recipient_unread.py
+notifications/migrations/0009_alter_notification_options_and_more.py
 notifications/migrations/__init__.py
 notifications/templates/notifications/list.html
 notifications/templates/notifications/notice.html
 notifications/templates/notifications/test_tags.html
 notifications/templatetags/__init__.py
 notifications/templatetags/notifications_tags.py
 notifications/tests/__init__.py
```

### Comparing `django-notifications-hq-1.8.1/notifications/admin.py` & `django-notifications-hq-1.8.2/notifications/admin.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/base/models.py` & `django-notifications-hq-1.8.2/notifications/base/models.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/helpers.py` & `django-notifications-hq-1.8.2/notifications/helpers.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/locale/ru/LC_MESSAGES/django.po` & `django-notifications-hq-1.8.2/notifications/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/migrations/0001_initial.py` & `django-notifications-hq-1.8.2/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/migrations/0002_auto_20150224_1134.py` & `django-notifications-hq-1.8.2/notifications/migrations/0002_auto_20150224_1134.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/migrations/0005_auto_20160504_1520.py` & `django-notifications-hq-1.8.2/notifications/migrations/0005_auto_20160504_1520.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/migrations/0006_indexes.py` & `django-notifications-hq-1.8.2/notifications/migrations/0006_indexes.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/models.py` & `django-notifications-hq-1.8.2/notifications/models.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/templates/notifications/notice.html` & `django-notifications-hq-1.8.2/notifications/templates/notifications/notice.html`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/templatetags/notifications_tags.py` & `django-notifications-hq-1.8.2/notifications/templatetags/notifications_tags.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/tests/sample_notifications/migrations/0001_initial.py` & `django-notifications-hq-1.8.2/notifications/tests/sample_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/tests/sample_notifications/tests.py` & `django-notifications-hq-1.8.2/notifications/tests/sample_notifications/tests.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/tests/settings.py` & `django-notifications-hq-1.8.2/notifications/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/tests/tests.py` & `django-notifications-hq-1.8.2/notifications/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/tests/urls.py` & `django-notifications-hq-1.8.2/notifications/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/tests/views.py` & `django-notifications-hq-1.8.2/notifications/tests/views.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/urls.py` & `django-notifications-hq-1.8.2/notifications/urls.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/notifications/views.py` & `django-notifications-hq-1.8.2/notifications/views.py`

 * *Files identical despite different names*

### Comparing `django-notifications-hq-1.8.1/setup.py` & `django-notifications-hq-1.8.2/setup.py`

 * *Files identical despite different names*

