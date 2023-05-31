# Comparing `tmp/django-yaaac-4.0.0.tar.gz` & `tmp/django-yaaac-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-yaaac-4.0.0.tar", last modified: Wed Feb 26 10:23:36 2020, max compression
+gzip compressed data, was "django-yaaac-4.1.0.tar", last modified: Wed May 31 11:32:25 2023, max compression
```

## Comparing `django-yaaac-4.0.0.tar` & `django-yaaac-4.1.0.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     8283 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/PKG-INFO
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     1800 2019-07-04 08:51:01.000000 django-yaaac-4.0.0/LICENSE
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/tests/
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/tests/autocomplete/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     2911 2020-02-25 16:17:06.000000 django-yaaac-4.0.0/tests/autocomplete/models.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2014-11-14 16:23:19.000000 django-yaaac-4.0.0/tests/autocomplete/__init__.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)      205 2020-02-25 15:46:00.000000 django-yaaac-4.0.0/tests/autocomplete/admin.py
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/tests/autocomplete/static/
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/tests/autocomplete/static/js/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)    86927 2019-07-04 08:51:01.000000 django-yaaac-4.0.0/tests/autocomplete/static/js/jquery.min.js
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/tests/autocomplete/fixtures/
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/tests/autocomplete/fixtures/autocomplete/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     2791 2014-11-14 16:23:19.000000 django-yaaac-4.0.0/tests/autocomplete/fixtures/autocomplete/initial.json
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)    13771 2020-02-26 10:17:50.000000 django-yaaac-4.0.0/tests/autocomplete/tests.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)      690 2020-02-25 16:16:11.000000 django-yaaac-4.0.0/tests/autocomplete/urls.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     4921 2020-02-26 10:17:45.000000 django-yaaac-4.0.0/tests/autocomplete/views.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)      389 2015-01-28 15:11:47.000000 django-yaaac-4.0.0/tests/test_sqlite_settings.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)      564 2020-02-25 15:46:00.000000 django-yaaac-4.0.0/tests/Makefile
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/tests/utils/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2014-11-14 16:23:19.000000 django-yaaac-4.0.0/tests/utils/__init__.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     1011 2014-11-14 16:23:19.000000 django-yaaac-4.0.0/tests/utils/tests.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)       28 2014-11-07 13:18:38.000000 django-yaaac-4.0.0/tests/coveragerc
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/tests/templates/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)      417 2020-02-26 10:16:05.000000 django-yaaac-4.0.0/tests/templates/base_form.html
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)       17 2014-11-14 16:23:19.000000 django-yaaac-4.0.0/tests/urls.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     5322 2020-02-25 16:14:54.000000 django-yaaac-4.0.0/tests/runtests.py
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac.egg-info/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     8283 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac.egg-info/PKG-INFO
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     1087 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac.egg-info/SOURCES.txt
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)       13 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac.egg-info/top_level.txt
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        1 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac.egg-info/dependency_links.txt
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)      196 2019-07-04 08:51:01.000000 django-yaaac-4.0.0/MANIFEST.in
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     1588 2020-02-26 10:20:27.000000 django-yaaac-4.0.0/setup.py
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac/
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac/forms/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     1773 2020-02-25 15:46:00.000000 django-yaaac-4.0.0/django_yaaac/forms/fields.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2013-09-23 15:32:30.000000 django-yaaac-4.0.0/django_yaaac/forms/__init__.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     6282 2020-02-25 16:32:58.000000 django-yaaac-4.0.0/django_yaaac/forms/widgets.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)       53 2019-07-04 08:51:01.000000 django-yaaac-4.0.0/django_yaaac/__init__.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)       91 2019-07-04 08:51:01.000000 django-yaaac-4.0.0/django_yaaac/apps.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)      531 2013-10-14 14:27:34.000000 django-yaaac-4.0.0/django_yaaac/utils.py
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac/static/
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac/static/django_yaaac/
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac/static/django_yaaac/css/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)      825 2013-10-03 13:49:30.000000 django-yaaac-4.0.0/django_yaaac/static/django_yaaac/css/autocomplete.css
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac/static/django_yaaac/js/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)       26 2013-12-23 12:27:05.000000 django-yaaac-4.0.0/django_yaaac/static/django_yaaac/js/yaaac_compat.js
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)    12958 2020-02-25 15:46:00.000000 django-yaaac-4.0.0/django_yaaac/static/django_yaaac/js/jquery.autocomplete.min.js
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     4424 2019-07-04 08:51:01.000000 django-yaaac-4.0.0/django_yaaac/static/django_yaaac/js/yaaac_autocomplete.js
-drwxr-xr-x   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)        0 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/django_yaaac/static/django_yaaac/img/
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)      552 2013-10-03 13:49:30.000000 django-yaaac-4.0.0/django_yaaac/static/django_yaaac/img/selector-search.gif
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     5192 2020-02-25 15:46:00.000000 django-yaaac-4.0.0/django_yaaac/manager.py
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)       38 2020-02-26 10:23:36.000000 django-yaaac-4.0.0/setup.cfg
--rw-r--r--   0 sguerra  (31307828) IO\Utilisa. du domaine (296225990)     6066 2020-02-25 15:46:00.000000 django-yaaac-4.0.0/README.rst
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1800 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/LICENSE
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      196 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/MANIFEST.in
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     8283 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6066 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/README.rst
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/django_yaaac/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       53 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       91 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/apps.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/django_yaaac/forms/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/forms/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1773 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/forms/fields.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6282 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/forms/widgets.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5195 2023-05-31 09:35:47.000000 django-yaaac-4.1.0/django_yaaac/manager.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/django_yaaac/static/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/django_yaaac/static/django_yaaac/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/django_yaaac/static/django_yaaac/css/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      825 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/static/django_yaaac/css/autocomplete.css
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/django_yaaac/static/django_yaaac/img/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      552 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/static/django_yaaac/img/selector-search.gif
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/django_yaaac/static/django_yaaac/js/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    12958 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/static/django_yaaac/js/jquery.autocomplete.min.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4424 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/static/django_yaaac/js/yaaac_autocomplete.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       26 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/static/django_yaaac/js/yaaac_compat.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      531 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/django_yaaac/utils.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/django_yaaac.egg-info/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     8283 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/django_yaaac.egg-info/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1195 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/django_yaaac.egg-info/SOURCES.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/django_yaaac.egg-info/dependency_links.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       13 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/django_yaaac.egg-info/top_level.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       38 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/setup.cfg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1588 2023-05-31 11:28:45.000000 django-yaaac-4.1.0/setup.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/tests/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    12288 2023-05-31 10:27:30.000000 django-yaaac-4.1.0/tests/.Makefile.swp
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    16384 2023-05-31 09:53:54.000000 django-yaaac-4.1.0/tests/.runtests.py.swp
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      548 2023-05-31 10:27:22.000000 django-yaaac-4.1.0/tests/Makefile
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/tests/autocomplete/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40960 2023-05-31 10:26:58.000000 django-yaaac-4.1.0/tests/autocomplete/.tests.py.swp
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    12288 2023-05-31 09:51:52.000000 django-yaaac-4.1.0/tests/autocomplete/.urls.py.swp
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/autocomplete/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      205 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/autocomplete/admin.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/tests/autocomplete/fixtures/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/tests/autocomplete/fixtures/autocomplete/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2791 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/autocomplete/fixtures/autocomplete/initial.json
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2911 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/autocomplete/models.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:24.000000 django-yaaac-4.1.0/tests/autocomplete/static/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/tests/autocomplete/static/js/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    86927 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/autocomplete/static/js/jquery.min.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    13763 2023-05-31 10:26:49.000000 django-yaaac-4.1.0/tests/autocomplete/tests.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      721 2023-05-31 09:51:44.000000 django-yaaac-4.1.0/tests/autocomplete/urls.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4921 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/autocomplete/views.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       28 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/coveragerc
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5322 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/runtests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/tests/templates/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      417 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/templates/base_form.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      389 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/test_sqlite_settings.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       17 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/urls.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 11:32:25.000000 django-yaaac-4.1.0/tests/utils/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/utils/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1011 2023-05-31 09:29:23.000000 django-yaaac-4.1.0/tests/utils/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-yaaac-4.0.0/PKG-INFO` & `django-yaaac-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: django-yaaac
-Version: 4.0.0
+Version: 4.1.0
 Summary: Django application providing Ajax search capabilities.
 Home-page: https://github.com/Starou/django-yaaac
 Author: Stanislas Guerra
 Author-email: stanislas.guerra@gmail.com
 License: BSD Licence
 Project-URL: Source Code, https://github.com/Starou/django-yaaac
 Project-URL: Issue Tracker, https://github.com/Starou/django-yaaac/issues
@@ -179,10 +179,10 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `django-yaaac-4.0.0/LICENSE` & `django-yaaac-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/tests/autocomplete/models.py` & `django-yaaac-4.1.0/tests/autocomplete/models.py`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/tests/autocomplete/static/js/jquery.min.js` & `django-yaaac-4.1.0/tests/autocomplete/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/tests/autocomplete/fixtures/autocomplete/initial.json` & `django-yaaac-4.1.0/tests/autocomplete/fixtures/autocomplete/initial.json`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/tests/autocomplete/tests.py` & `django-yaaac-4.1.0/tests/autocomplete/tests.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import time
 from django.contrib.admin.views.main import TO_FIELD_VAR
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.test import TestCase, LiveServerTestCase
 from django.test import override_settings
 from django.test.client import Client
 from . import models
 from selenium.webdriver.chrome.webdriver import WebDriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
@@ -24,50 +24,50 @@
 
     def setUp(self):
         super(AutocompleteTest, self).setUp()
         self.client = Client()
 
     def test_search(self):
         response = self.client.get("/yaaac/autocomplete/band/search/?%s=id&query=ge&search_fields=^name&suggest_by=name" % TO_FIELD_VAR)
-        self.assertEqual(json.loads(force_text(response.content)),
+        self.assertEqual(json.loads(force_str(response.content)),
                          {u'query': u'ge', u'suggestions': [{u'data': 1, u'value': u'Genesis'}]})
 
         response = self.client.get("/yaaac/autocomplete/band/search/?%s=id&query=ge&search_fields=name&suggest_by=get_full_info" % TO_FIELD_VAR)
-        self.assertEqual(json.loads(force_text(response.content)),
+        self.assertEqual(json.loads(force_str(response.content)),
                          {u'query': u'ge', u'suggestions': [
                              {u'data': 1, u'value': u'Genesis (Rock)'},
                              {u'data': 6, u'value': u'The Bee Gees (Cheese)'},
                          ]})
 
         response = self.client.get(
             "/yaaac/autocomplete/bandmember/search/?%s=id&query=ph&search_fields=first_name&suggest_by=get_full_name" % TO_FIELD_VAR)
-        self.assertEqual(json.loads(force_text(response.content)),
+        self.assertEqual(json.loads(force_str(response.content)),
                          {u'query': u'ph', u'suggestions': [
                              {u'data': 1, u'value': u'Phil Collins'},
                              {u'data': 4, u'value': u'Phil Spector'},
                          ]})
 
         response = self.client.get(
             "/yaaac/autocomplete/bandmember/search/?%s=id&query=ph&search_fields=first_name,last_name&suggest_by=get_full_name" % TO_FIELD_VAR)
-        self.assertEqual(json.loads(force_text(response.content)),
+        self.assertEqual(json.loads(force_str(response.content)),
                          {u'query': u'ph', u'suggestions': [
                              {u'data': 1, u'value': u'Phil Collins'},
                              {u'data': 4, u'value': u'Phil Spector'},
                          ]})
 
         response = self.client.get(
             "/yaaac/autocomplete/bandmember/search/?%s=id&query=ph col&search_fields=first_name,last_name&suggest_by=get_full_name" % TO_FIELD_VAR)
-        self.assertEqual(json.loads(force_text(response.content)),
+        self.assertEqual(json.loads(force_str(response.content)),
                          {u'query': u'ph col', u'suggestions': [
                              {u'data': 1, u'value': u'Phil Collins'},
                          ]})
 
     def test_search_with_pk(self):
         response = self.client.get("/yaaac/autocomplete/band/search/?pk=1")
-        self.assertEqual(json.loads(force_text(response.content)), {'value': 'Genesis', 'url': None})
+        self.assertEqual(json.loads(force_str(response.content)), {'value': 'Genesis', 'url': None})
 
     def test_search_not_found(self):
         response = self.client.get("/yaaac/auth/user/search/?%s=id&query=super&search_fields=^username&suggest_by=password" % TO_FIELD_VAR)
         self.assertEqual(response.status_code, 404)
         response = self.client.get("/yaaac/auth/user/search/?pk=1")
         self.assertEqual(response.status_code, 404)
 
@@ -111,155 +111,155 @@
         from selenium.webdriver.support import expected_conditions as EC
         WebDriverWait(self.selenium, 5).until(
             EC.presence_of_element_located((by, search))
         )
 
     def admin_login(self, username, password, login_url='/admin/'):
         self.selenium.get('%s%s' % (self.live_server_url, login_url))
-        username_input = self.selenium.find_element_by_name('username')
+        username_input = self.selenium.find_element("name", 'username')
         username_input.send_keys(username)
-        password_input = self.selenium.find_element_by_name('password')
+        password_input = self.selenium.find_element("name", 'password')
         password_input.send_keys(password)
         login_text = 'Log in'
-        self.selenium.find_element_by_xpath(
+        self.selenium.find_element("xpath",
             '//input[@value="%s"]' % login_text).click()
         self.wait_page_loaded(By.CLASS_NAME, "dashboard")
 
 
 @override_settings(ROOT_URLCONF="autocomplete.urls")
 class YaaacLiveServerTest(LiveServerTest):
     def test_foreign_key_autocomplete(self):
         mick = models.BandMember.objects.create(first_name="Mick", last_name="Jagger")
         self.selenium.get('%s/band-member-form/%d/' % (self.live_server_url, mick.pk))
 
-        band_search_elem = self.selenium.find_element_by_xpath('//input[@class="yaaac_search_input"]')
+        band_search_elem = self.selenium.find_element("xpath", '//input[@class="yaaac_search_input"]')
         self.assertTrue(band_search_elem.is_displayed())
         band_search_elem.send_keys("the ")
         self.wait_for_ajax()
-        suggestion_elems = self.selenium.find_elements_by_class_name('autocomplete-suggestion')
+        suggestion_elems = self.selenium.find_elements('class name', 'autocomplete-suggestion')
         self.assertEqual(len(suggestion_elems), 3)
         self.assertEqual([elem.text for elem in suggestion_elems],
                          [u"The Rolling Stones (Blues/Rock)", u"The Stone Roses (Rock)", "The Bee Gees (Cheese)"])
 
         suggestion_elems[0].click()
-        self.assertEqual(self.selenium.find_element_by_id('id_band').get_attribute("value"), "2")
+        self.assertEqual(self.selenium.find_element("id", 'id_band').get_attribute("value"), "2")
         WebDriverWait(self.selenium, 2).until(EC.invisibility_of_element_located((By.ID, "lookup_id_band")))
         self.assertFalse(band_search_elem.is_displayed())
 
-        band_value_container = self.selenium.find_element_by_class_name('yaaac_value_container')
+        band_value_container = self.selenium.find_element("class name", 'yaaac_value_container')
         self.assertTrue(band_value_container.is_displayed())
-        band_value_elem = self.selenium.find_element_by_class_name('yaaac_value')
+        band_value_elem = self.selenium.find_element("class name", 'yaaac_value')
         self.assertEqual(band_value_elem.text, "The Rolling Stones")
 
         # Clear the choice.
-        self.selenium.find_element_by_class_name('yaaac_clear_value').click()
-        self.assertEqual(self.selenium.find_element_by_id('id_band').get_attribute("value"), "")
+        self.selenium.find_element("class name", 'yaaac_clear_value').click()
+        self.assertEqual(self.selenium.find_element("id", 'id_band').get_attribute("value"), "")
         self.assertTrue(band_search_elem.is_displayed())
         self.assertFalse(band_value_container.is_displayed())
 
     def test_foreign_key_autocomplete_with_initial(self):
         mick = models.BandMember.objects.create(first_name="Mick", last_name="Jagger", band_id=2)
         self.selenium.get('%s/band-member-form/%d/' % (self.live_server_url, mick.pk))
 
         # The autocomplete field is not visible.
-        band_search_elem = self.selenium.find_element_by_xpath('//input[@class="yaaac_search_input"]')
+        band_search_elem = self.selenium.find_element("xpath", '//input[@class="yaaac_search_input"]')
         self.assertFalse(band_search_elem.is_displayed())
 
         # But the label is.
-        band_value_container = self.selenium.find_element_by_class_name('yaaac_value_container')
+        band_value_container = self.selenium.find_element("class name", 'yaaac_value_container')
         self.assertTrue(band_value_container.is_displayed())
-        band_value_elem = self.selenium.find_element_by_class_name('yaaac_value')
+        band_value_elem = self.selenium.find_element("class name", 'yaaac_value')
         self.assertEqual(band_value_elem.text, "The Rolling Stones")
 
     def test_foreign_key_related_lookup(self):
         self.admin_login("super", "secret", login_url='/admin/')
         mick = models.BandMember.objects.create(first_name="Mick", last_name="Jagger")
 
         self.selenium.get('%s/band-member-form/%d/' % (self.live_server_url, mick.pk))
         main_window = self.selenium.current_window_handle
-        self.selenium.find_element_by_class_name('yaaac_lookup').click()
+        self.selenium.find_element("class name", 'yaaac_lookup').click()
 
         self.wait_for_popup()
         self.selenium.switch_to.window(self.selenium.window_handles[1])
-        self.selenium.find_element_by_link_text("SuperHeavy").click()
+        self.selenium.find_element("link text", "SuperHeavy").click()
         self.selenium.switch_to.window(main_window)
-        self.assertEqual(self.selenium.find_element_by_id('id_band').get_attribute("value"), "4")
+        self.assertEqual(self.selenium.find_element("id", 'id_band').get_attribute("value"), "4")
 
         # The autocomplete field is now hidden.
-        band_search_elem = self.selenium.find_element_by_xpath('//input[@class="yaaac_search_input"]')
+        band_search_elem = self.selenium.find_element("xpath", '//input[@class="yaaac_search_input"]')
         WebDriverWait(self.selenium, 2).until(EC.invisibility_of_element_located(
             (By.XPATH, '//input[@class="yaaac_search_input"]')))
         self.assertFalse(band_search_elem.is_displayed())
 
         # And the label is shown.
-        band_value_container = self.selenium.find_element_by_class_name('yaaac_value_container')
+        band_value_container = self.selenium.find_element("class name", 'yaaac_value_container')
         self.assertTrue(band_value_container.is_displayed())
-        band_value_elem = self.selenium.find_element_by_class_name('yaaac_value')
+        band_value_elem = self.selenium.find_element("class name", 'yaaac_value')
         self.assertEqual(band_value_elem.text, "SuperHeavy")
 
     def test_foreign_key_limit_choices_autocomplete(self):
         mick = models.BandMember.objects.create(first_name="Mick", last_name="Jagger")
         self.selenium.get('%s/band-member-form/limit-choices/%d/' % (self.live_server_url, mick.pk))
 
-        band_search_elem = self.selenium.find_element_by_xpath('//input[@class="yaaac_search_input"]')
+        band_search_elem = self.selenium.find_element("xpath", '//input[@class="yaaac_search_input"]')
         self.assertTrue(band_search_elem.is_displayed())
         band_search_elem.send_keys("the ")
         self.wait_for_ajax()
-        suggestion_elems = self.selenium.find_elements_by_class_name('autocomplete-suggestion')
+        suggestion_elems = self.selenium.find_elements('class name', 'autocomplete-suggestion')
         self.assertEqual(len(suggestion_elems), 2)
         self.assertEqual([elem.text for elem in suggestion_elems],
                          [u"The Rolling Stones", u"The Stone Roses"])
 
         suggestion_elems[0].click()
-        self.assertEqual(self.selenium.find_element_by_id('id_band').get_attribute("value"), "2")
+        self.assertEqual(self.selenium.find_element("id", 'id_band').get_attribute("value"), "2")
         WebDriverWait(self.selenium, 2).until(EC.invisibility_of_element_located(
             (By.XPATH, '//input[@class="yaaac_search_input"]')))
         self.assertFalse(band_search_elem.is_displayed())
 
-        band_value_container = self.selenium.find_element_by_class_name('yaaac_value_container')
+        band_value_container = self.selenium.find_element("class name", 'yaaac_value_container')
         self.assertTrue(band_value_container.is_displayed())
-        band_value_elem = self.selenium.find_element_by_class_name('yaaac_value')
+        band_value_elem = self.selenium.find_element("class name", 'yaaac_value')
         self.assertEqual(band_value_elem.text, "The Rolling Stones")
 
         # Clear the choice.
-        self.selenium.find_element_by_class_name('yaaac_clear_value').click()
-        self.assertEqual(self.selenium.find_element_by_id('id_band').get_attribute("value"), "")
+        self.selenium.find_element("class name", 'yaaac_clear_value').click()
+        self.assertEqual(self.selenium.find_element("id", 'id_band').get_attribute("value"), "")
         self.assertTrue(band_search_elem.is_displayed())
         self.assertFalse(band_value_container.is_displayed())
 
     def test_foreign_key_limit_choices_related_lookup(self):
         self.admin_login("super", "secret", login_url='/admin/')
         mick = models.BandMember.objects.create(first_name="Mick", last_name="Jagger")
 
         self.selenium.get('%s/band-member-form/limit-choices/%d/' % (self.live_server_url, mick.pk))
         main_window = self.selenium.current_window_handle
-        self.selenium.find_element_by_class_name('yaaac_lookup').click()
+        self.selenium.find_element("class name", 'yaaac_lookup').click()
 
         self.wait_for_popup()
         self.selenium.switch_to.window(self.selenium.window_handles[1])
-        self.selenium.find_element_by_link_text("SuperHeavy").click()
+        self.selenium.find_element("link text", "SuperHeavy").click()
         self.selenium.switch_to.window(main_window)
-        self.assertEqual(self.selenium.find_element_by_id('id_band').get_attribute("value"), "4")
+        self.assertEqual(self.selenium.find_element("id", 'id_band').get_attribute("value"), "4")
 
         # The autocomplete field is now hidden.
-        band_search_elem = self.selenium.find_element_by_xpath('//input[@class="yaaac_search_input"]')
+        band_search_elem = self.selenium.find_element("xpath", '//input[@class="yaaac_search_input"]')
         WebDriverWait(self.selenium, 2).until(EC.invisibility_of_element_located(
             (By.XPATH, '//input[@class="yaaac_search_input"]')))
         self.assertFalse(band_search_elem.is_displayed())
 
         # And the label is shown.
-        band_value_container = self.selenium.find_element_by_class_name('yaaac_value_container')
+        band_value_container = self.selenium.find_element("class name", 'yaaac_value_container')
         self.assertTrue(band_value_container.is_displayed())
-        band_value_elem = self.selenium.find_element_by_class_name('yaaac_value')
+        band_value_elem = self.selenium.find_element("class name", 'yaaac_value')
         self.assertEqual(band_value_elem.text, "SuperHeavy")
 
     def test_extra_css(self):
         self.admin_login("super", "secret", login_url='/admin/')
         self.selenium.get('%s/band-member-form/extra-css/' % self.live_server_url)
-        container = self.selenium.find_element_by_class_name('yaaac_container')
+        container = self.selenium.find_element("class name", 'yaaac_container')
         self.assertEqual(container.get_attribute('class'), u'yaaac_container my_extra_class')
 
     def test_no_lookup(self):
         from selenium.common.exceptions import NoSuchElementException
         self.admin_login("super", "secret", login_url='/admin/')
         self.selenium.get('%s/band-member-form/no-lookup/' % self.live_server_url)
-        self.assertRaises(NoSuchElementException, self.selenium.find_element_by_class_name, 'yaaac_lookup')
+        self.assertRaises(NoSuchElementException, self.selenium.find_element, 'class name', 'yaaac_lookup')
```

### Comparing `django-yaaac-4.0.0/tests/autocomplete/urls.py` & `django-yaaac-4.1.0/tests/autocomplete/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django_yaaac.manager import autocomplete
-from django.conf.urls import url
+from django.urls import re_path
 from django.contrib import admin
 
 from autocomplete import views
 
 urlpatterns = [
-    url('^admin/', admin.site.urls),
-    url(r'^yaaac/', autocomplete.urls),
-    url(r'^band-member-form/$', views.band_member_form),
-    url(r'^band-member-form/(?P<member_id>\d+)/$', views.band_member_form),
-    url(r'^band-member-form/limit-choices/$', views.band_member_limit_form),
-    url(r'^band-member-form/limit-choices/(?P<member_id>\d+)/$', views.band_member_limit_form),
-    url(r'^band-member-form/extra-css/$', views.band_member_extra_css),
-    url(r'^band-member-form/no-lookup/$', views.band_member_no_lookup),
+    re_path('^admin/', admin.site.urls),
+    re_path(r'^yaaac/', autocomplete.urls),
+    re_path(r'^band-member-form/$', views.band_member_form),
+    re_path(r'^band-member-form/(?P<member_id>\d+)/$', views.band_member_form),
+    re_path(r'^band-member-form/limit-choices/$', views.band_member_limit_form),
+    re_path(r'^band-member-form/limit-choices/(?P<member_id>\d+)/$', views.band_member_limit_form),
+    re_path(r'^band-member-form/extra-css/$', views.band_member_extra_css),
+    re_path(r'^band-member-form/no-lookup/$', views.band_member_no_lookup),
 ]
```

### Comparing `django-yaaac-4.0.0/tests/autocomplete/views.py` & `django-yaaac-4.1.0/tests/autocomplete/views.py`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/tests/Makefile` & `django-yaaac-4.1.0/tests/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 tests:
 ifeq (${USER},vagrant)
-	@PATH=${PATH}:/usr/lib/chromium-browser/ DISPLAY=:99 PYTHONPATH=..:${PYTHONPATH} xvfb-run -n 99 python runtests.py
+	@PATH=${PATH}:/usr/lib/chromium/ DISPLAY=:99 PYTHONPATH=..:${PYTHONPATH} xvfb-run -n 99 python runtests.py
 else
 	@PYTHONPATH=..:${PYTHONPATH} python runtests.py
 endif
 
 coverage-report: coverage
 	@coverage report -m
 
 coverage-report-html: coverage
 	@coverage html
 
 coverage:
 ifeq (${USER},vagrant)
-	@PATH=${PATH}:/usr/lib/chromium-browser/ DISPLAY=:99 PYTHONPATH=..:${PYTHONPATH} xvfb-run -n 99 coverage run --rcfile=coveragerc runtests.py
+	@PATH=${PATH}:/usr/lib/chromium/ DISPLAY=:99 PYTHONPATH=..:${PYTHONPATH} xvfb-run -n 99 coverage run --rcfile=coveragerc runtests.py
 else
 	@PYTHONPATH=..:${PYTHONPATH} coverage run --rcfile=coveragerc runtests.py
 endif
```

### Comparing `django-yaaac-4.0.0/tests/utils/tests.py` & `django-yaaac-4.1.0/tests/utils/tests.py`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/tests/runtests.py` & `django-yaaac-4.1.0/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/django_yaaac.egg-info/PKG-INFO` & `django-yaaac-4.1.0/django_yaaac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: django-yaaac
-Version: 4.0.0
+Version: 4.1.0
 Summary: Django application providing Ajax search capabilities.
 Home-page: https://github.com/Starou/django-yaaac
 Author: Stanislas Guerra
 Author-email: stanislas.guerra@gmail.com
 License: BSD Licence
 Project-URL: Source Code, https://github.com/Starou/django-yaaac
 Project-URL: Issue Tracker, https://github.com/Starou/django-yaaac/issues
@@ -179,10 +179,10 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `django-yaaac-4.0.0/django_yaaac.egg-info/SOURCES.txt` & `django-yaaac-4.1.0/django_yaaac.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,23 @@
 django_yaaac/forms/fields.py
 django_yaaac/forms/widgets.py
 django_yaaac/static/django_yaaac/css/autocomplete.css
 django_yaaac/static/django_yaaac/img/selector-search.gif
 django_yaaac/static/django_yaaac/js/jquery.autocomplete.min.js
 django_yaaac/static/django_yaaac/js/yaaac_autocomplete.js
 django_yaaac/static/django_yaaac/js/yaaac_compat.js
+tests/.Makefile.swp
+tests/.runtests.py.swp
 tests/Makefile
 tests/coveragerc
 tests/runtests.py
 tests/test_sqlite_settings.py
 tests/urls.py
+tests/autocomplete/.tests.py.swp
+tests/autocomplete/.urls.py.swp
 tests/autocomplete/__init__.py
 tests/autocomplete/admin.py
 tests/autocomplete/models.py
 tests/autocomplete/tests.py
 tests/autocomplete/urls.py
 tests/autocomplete/views.py
 tests/autocomplete/fixtures/autocomplete/initial.json
```

### Comparing `django-yaaac-4.0.0/setup.py` & `django-yaaac-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = f.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-yaaac',
-    version='4.0.0',
+    version='4.1.0',
     license='BSD Licence',
     author='Stanislas Guerra',
     author_email='stanislas.guerra@gmail.com',
     description='Django application providing Ajax search capabilities.',
     long_description=README,
     url='https://github.com/Starou/django-yaaac',
     project_urls={
@@ -37,12 +37,12 @@
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
 )
```

### Comparing `django-yaaac-4.0.0/django_yaaac/forms/fields.py` & `django-yaaac-4.1.0/django_yaaac/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/django_yaaac/forms/widgets.py` & `django-yaaac-4.1.0/django_yaaac/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/django_yaaac/utils.py` & `django-yaaac-4.1.0/django_yaaac/utils.py`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/django_yaaac/static/django_yaaac/css/autocomplete.css` & `django-yaaac-4.1.0/django_yaaac/static/django_yaaac/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/django_yaaac/static/django_yaaac/js/jquery.autocomplete.min.js` & `django-yaaac-4.1.0/django_yaaac/static/django_yaaac/js/jquery.autocomplete.min.js`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/django_yaaac/static/django_yaaac/js/yaaac_autocomplete.js` & `django-yaaac-4.1.0/django_yaaac/static/django_yaaac/js/yaaac_autocomplete.js`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/django_yaaac/static/django_yaaac/img/selector-search.gif` & `django-yaaac-4.1.0/django_yaaac/static/django_yaaac/img/selector-search.gif`

 * *Files identical despite different names*

### Comparing `django-yaaac-4.0.0/django_yaaac/manager.py` & `django-yaaac-4.1.0/django_yaaac/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from builtins import str
 from builtins import object
 import operator
+from functools import reduce
 from django.contrib.admin.views.main import TO_FIELD_VAR
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.http import HttpResponseNotFound, HttpResponseForbidden, JsonResponse
+from django.urls import re_path
 from django_yaaac.utils import lookup_dict_from_url_params
-from functools import reduce
 
 
 def cache_model(f):
     def wrapper(manager, request, *args, **kwargs):
         app = kwargs["app"]
         model = kwargs["model"]
         kwargs["model"] = ContentType.objects.get(app_label=app,
@@ -43,19 +44,18 @@
 class AutocompleteManager(object):
     def __init__(self, name="yaaac", app_label="yaaac"):
         self.name = name
         self.app_label = app_label
         self.registered_querysets = {}
 
     def get_urls(self):
-        from django.conf.urls import url
         return [
-            url(r'^(?P<app>\w+)/(?P<model>\w+)/(?P<queryset_id>\d+)/search/$',
-                self.search, name='search_with_queryset_id'),
-            url(r'^(?P<app>\w+)/(?P<model>\w+)/search/$', self.search, name='search'),
+            re_path(r'^(?P<app>\w+)/(?P<model>\w+)/(?P<queryset_id>\d+)/search/$',
+                    self.search, name='search_with_queryset_id'),
+            re_path(r'^(?P<app>\w+)/(?P<model>\w+)/search/$', self.search, name='search'),
         ]
 
     @property
     def urls(self):
         return self.get_urls(), self.app_label, self.name
 
     @cache_model
```

### Comparing `django-yaaac-4.0.0/README.rst` & `django-yaaac-4.1.0/README.rst`

 * *Files identical despite different names*

