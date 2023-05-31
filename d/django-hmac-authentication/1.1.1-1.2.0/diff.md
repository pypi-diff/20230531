# Comparing `tmp/django_hmac_authentication-1.1.1.tar.gz` & `tmp/django_hmac_authentication-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hmac_authentication-1.1.1.tar", last modified: Wed May 10 01:30:26 2023, max compression
+gzip compressed data, was "django_hmac_authentication-1.2.0.tar", last modified: Wed May 31 05:31:00 2023, max compression
```

## Comparing `django_hmac_authentication-1.1.1.tar` & `django_hmac_authentication-1.2.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/
--rw-r--r--   0 topcat    (1000) topcat    (1000)    11358 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/LICENSE
--rw-r--r--   0 topcat    (1000) topcat    (1000)     4717 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/PKG-INFO
--rw-r--r--   0 topcat    (1000) topcat    (1000)     4179 2023-05-09 23:43:54.000000 django_hmac_authentication-1.1.1/README.md
--rw-r--r--   0 topcat    (1000) topcat    (1000)      722 2023-05-10 01:29:36.000000 django_hmac_authentication-1.1.1/pyproject.toml
--rw-r--r--   0 topcat    (1000) topcat    (1000)       38 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/setup.cfg
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.863941 django_hmac_authentication-1.1.1/src/
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication/
--rw-r--r--   0 topcat    (1000) topcat    (1000)       54 2023-05-10 01:29:36.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      752 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/admin.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      638 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/aes.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     3213 2023-05-10 01:25:49.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/authentication.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2817 2023-05-09 23:14:39.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/client_utils.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/__init__.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/commands/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/commands/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1282 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication/migrations/
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1776 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/migrations/0001_initial.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/migrations/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      969 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/models.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      192 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/padding.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      298 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/serializers.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1519 2023-05-09 22:12:50.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/server_utils.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      813 2023-05-08 07:07:48.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/views.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/
--rw-r--r--   0 topcat    (1000) topcat    (1000)     4717 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/PKG-INFO
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2089 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)        1 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/requires.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)       56 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/top_level.txt
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/example_django_project/
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/src/example_django_project/accounts/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/admin.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      148 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/apps.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/src/example_django_project/accounts/migrations/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/migrations/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       57 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/models.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       60 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/tests.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      266 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/urls.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      576 2023-05-09 23:14:39.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/views.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/asgi.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     3718 2023-05-09 13:02:58.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/settings.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1025 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/urls.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/wsgi.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1834 2023-05-10 01:27:46.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_python_client.py
--rwxr-xr-x   0 topcat    (1000) topcat    (1000)      678 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/src/example_django_project/manage.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/src/tests/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 05:37:24.000000 django_hmac_authentication-1.1.1/src/tests/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1427 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/tests/factories.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     7007 2023-05-10 01:25:49.000000 django_hmac_authentication-1.1.1/src/tests/test_authentication_api_key_secret.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1502 2023-05-10 01:25:49.000000 django_hmac_authentication-1.1.1/src/tests/test_hmac_authorization_header_parsing.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1510 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/tests/test_mgmt_cmd_create_hmac_for_user.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      563 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/tests/test_padding.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2747 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/tests/test_utils.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1836 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/tests/test_view_create_api_key_secret.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.319592 django_hmac_authentication-1.2.0/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)    11358 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/LICENSE
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     6060 2023-05-31 05:31:00.319592 django_hmac_authentication-1.2.0/PKG-INFO
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     5522 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/README.md
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      722 2023-05-31 05:30:36.000000 django_hmac_authentication-1.2.0/pyproject.toml
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       38 2023-05-31 05:31:00.319592 django_hmac_authentication-1.2.0/setup.cfg
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.299592 django_hmac_authentication-1.2.0/src/
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.307592 django_hmac_authentication-1.2.0/src/django_hmac_authentication/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       54 2023-05-31 05:30:36.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      752 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/admin.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      638 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/aes.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     4143 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/authentication.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     2817 2023-05-09 23:14:39.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/client_utils.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1248 2023-05-31 03:19:11.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/exceptions.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.307592 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/__init__.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.307592 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/commands/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/commands/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1282 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.311592 django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1776 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/0001_initial.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      494 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1111 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/models.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      192 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/padding.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      298 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/serializers.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1519 2023-05-09 22:12:50.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/server_utils.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      813 2023-05-08 07:07:48.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/views.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.307592 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     6060 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     2211 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        1 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/requires.txt
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       56 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.311592 django_hmac_authentication-1.2.0/src/example_django_project/
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.315592 django_hmac_authentication-1.2.0/src/example_django_project/accounts/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/admin.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      148 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/apps.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.315592 django_hmac_authentication-1.2.0/src/example_django_project/accounts/migrations/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/migrations/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       57 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/models.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       60 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/tests.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      266 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/urls.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      576 2023-05-09 23:14:39.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/views.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.315592 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/asgi.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     3718 2023-05-09 13:02:58.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/settings.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1025 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/urls.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/wsgi.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1834 2023-05-10 01:27:46.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_python_client.py
+-rwxr-xr-x   0 topcat    (1000) topcat    (1000)      678 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/src/example_django_project/manage.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.319592 django_hmac_authentication-1.2.0/src/tests/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 05:37:24.000000 django_hmac_authentication-1.2.0/src/tests/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1589 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/tests/factories.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)    13716 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/tests/test_authentication_api_key_secret.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1502 2023-05-10 01:25:49.000000 django_hmac_authentication-1.2.0/src/tests/test_hmac_authorization_header_parsing.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1510 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/tests/test_mgmt_cmd_create_hmac_for_user.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      563 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/tests/test_padding.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     2875 2023-05-19 01:52:32.000000 django_hmac_authentication-1.2.0/src/tests/test_utils.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1836 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/tests/test_view_create_api_key_secret.py
```

### Comparing `django_hmac_authentication-1.1.1/LICENSE` & `django_hmac_authentication-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/pyproject.toml` & `django_hmac_authentication-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_hmac_authentication"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
   { name="Harisankar Krishna Swamy", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django HMAC authentication using shared secret"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication/admin.py` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication/admin.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication/aes.py` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication/aes.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication/authentication.py` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication/authentication.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,18 +3,27 @@
 from datetime import timezone
 
 from django.conf import settings
 from rest_framework import authentication
 from rest_framework.exceptions import AuthenticationFailed
 
 from django_hmac_authentication.client_utils import prepare_string_to_sign, sign_string
+from django_hmac_authentication.exceptions import (
+    DateFormatException,
+    ExpiredRequestException,
+    KeyDoesNotExistException,
+    RevokedKeyException,
+    SignatureVerificationException,
+    UnsupportedHMACMethodException,
+)
 from django_hmac_authentication.models import ApiHMACKey
 from django_hmac_authentication.server_utils import aes_decrypt_hmac_secret
 
 auth_req_timeout = getattr(settings, 'HMAC_AUTH_REQUEST_TIMEOUT', 5)
+failed_attempts_threshold = getattr(settings, 'HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD', -1)
 
 
 class HMACAuthentication(authentication.BaseAuthentication):
     authentication_methods = {'HMAC-SHA512', 'HMAC-SHA384', 'HMAC-SHA256'}
 
     def parse_authorization_header(self, content):
         if not content:
@@ -52,34 +61,53 @@
         auth_method, key, signature, date_in = self.parse_authorization_header(auth_hdr)
 
         if not auth_method or not key or not signature or not date_in:
             return None
 
         # auth header structure is for hmac authentication
         if auth_method not in self.authentication_methods:
-            raise AuthenticationFailed(f'Unsupported HMAC method {auth_method}')
+            raise UnsupportedHMACMethodException(hmac_method=auth_method)
 
         utcnow = datetime.datetime.now(timezone.utc)
 
         try:
             req_utc = datetime.datetime.fromisoformat(date_in)
         except ValueError:
-            raise AuthenticationFailed('Invalid date format in Authorization header')
+            raise DateFormatException()
 
         delta = utcnow - req_utc
         if delta.total_seconds() > auth_req_timeout:
-            raise AuthenticationFailed('Request timed out')
+            raise ExpiredRequestException()
 
         hmac_key = ApiHMACKey.objects.filter(id=key).first()
-        if not hmac_key or hmac_key.revoked:
-            raise AuthenticationFailed('Invalid API Key')
+        if not hmac_key:
+            raise KeyDoesNotExistException()
+
+        if hmac_key.revoked:
+            raise RevokedKeyException()
 
         if not hmac_key.user.is_active:
             raise AuthenticationFailed('User is inactive')
 
         computed_signature = self.compute_request_signature(
             request, auth_method, date_in, hmac_key
         )
         if not computed_signature == signature:
-            raise AuthenticationFailed('Message verification failed')
+            if failed_attempts_threshold > 0:
+                self._revoke_key_on_failed_attempts(hmac_key)
+            raise SignatureVerificationException()
 
         return hmac_key.user, None
+
+    def _revoke_key_on_failed_attempts(self, hmac_key):
+        # check db field max value
+        failed_attempts = hmac_key.failed_attempts + 1
+        if failed_attempts < 32767:
+            hmac_key.failed_attempts = failed_attempts
+            hmac_key.save()
+
+        if hmac_key.failed_attempts >= failed_attempts_threshold:
+            hmac_key.revoked = True
+            hmac_key.save()
+            raise SignatureVerificationException(
+                'Signature verification failed. Too many failed attempts. Key revoked.'
+            )
```

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication/client_utils.py` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication/client_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication/migrations/0001_initial.py` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication/models.py` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     id = models.UUIDField(primary_key=True, default=uuid.uuid4)
     user = models.ForeignKey(
         user_model, on_delete=models.CASCADE, related_name='api_hmac_keys'
     )
     secret = models.CharField(_('Secret'), max_length=512, null=False, editable=False)
     salt = models.CharField(_('Salt'), max_length=80, null=False, editable=False)
     revoked = models.BooleanField(_('Revoked'), default=False)
+    failed_attempts = models.PositiveSmallIntegerField(
+        _('Failed authentication attempts'), default=0, null=False, blank=False
+    )
 
     def __str__(self):
         return f'{self.user}'
 
     class Meta:
         verbose_name = 'API HMAC Key'
         verbose_name_plural = 'API HMAC Keys'
```

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication/server_utils.py` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication/server_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication/views.py` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/SOURCES.txt` & `django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 README.md
 pyproject.toml
 src/django_hmac_authentication/__init__.py
 src/django_hmac_authentication/admin.py
 src/django_hmac_authentication/aes.py
 src/django_hmac_authentication/authentication.py
 src/django_hmac_authentication/client_utils.py
+src/django_hmac_authentication/exceptions.py
 src/django_hmac_authentication/models.py
 src/django_hmac_authentication/padding.py
 src/django_hmac_authentication/serializers.py
 src/django_hmac_authentication/server_utils.py
 src/django_hmac_authentication/views.py
 src/django_hmac_authentication.egg-info/PKG-INFO
 src/django_hmac_authentication.egg-info/SOURCES.txt
 src/django_hmac_authentication.egg-info/dependency_links.txt
 src/django_hmac_authentication.egg-info/requires.txt
 src/django_hmac_authentication.egg-info/top_level.txt
 src/django_hmac_authentication/management/__init__.py
 src/django_hmac_authentication/management/commands/__init__.py
 src/django_hmac_authentication/management/commands/create_hmac_for_user.py
 src/django_hmac_authentication/migrations/0001_initial.py
+src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
 src/django_hmac_authentication/migrations/__init__.py
 src/example_django_project/example_python_client.py
 src/example_django_project/manage.py
 src/example_django_project/accounts/__init__.py
 src/example_django_project/accounts/admin.py
 src/example_django_project/accounts/apps.py
 src/example_django_project/accounts/models.py
```

### Comparing `django_hmac_authentication-1.1.1/src/example_django_project/accounts/views.py` & `django_hmac_authentication-1.2.0/src/example_django_project/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/settings.py` & `django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/urls.py` & `django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/example_django_project/example_python_client.py` & `django_hmac_authentication-1.2.0/src/example_django_project/example_python_client.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/example_django_project/manage.py` & `django_hmac_authentication-1.2.0/src/example_django_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/tests/factories.py` & `django_hmac_authentication-1.2.0/src/tests/factories.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,7 +43,15 @@
     class Meta:
         model = ApiHMACKey
 
     user = factory.SubFactory(SuperUserFactory)
     salt = base64.b64encode(test_salt).decode('utf-8')
     secret = base64.b64encode(test_encrypted).decode('utf-8')
     revoked = False
+    failed_attempts = 0
+
+
+class ApiHMACKeyWithMaxFailedAttemptsFactory(ApiHMACKeyFactory):
+    class Meta:
+        model = ApiHMACKey
+
+    failed_attempts = 9999
```

### Comparing `django_hmac_authentication-1.1.1/src/tests/test_hmac_authorization_header_parsing.py` & `django_hmac_authentication-1.2.0/src/tests/test_hmac_authorization_header_parsing.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/tests/test_mgmt_cmd_create_hmac_for_user.py` & `django_hmac_authentication-1.2.0/src/tests/test_mgmt_cmd_create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/tests/test_padding.py` & `django_hmac_authentication-1.2.0/src/tests/test_padding.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.1/src/tests/test_utils.py` & `django_hmac_authentication-1.2.0/src/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 
     @data(
         (
             'HMAC-SHA512',
             'BsDXXZ895Ko1KhznDwBhRBS0+g+5X+KoZz1b3R7JUXhQ/5r0Q+pN+FfhlL88KRiL3ya2RNw6GETHbzolHcuXAw==',
         ),
         (
+            'HMAC-SHA384',
+            'd/bLM3PsSDS+/NxNqYwlqY9nNv/5OK9MJSd31uQ4cHB4DE9NIhG1cszPEgwJdu4+',
+        ),
+        (
             'HMAC-SHA256',
             'ZaIJF7XWibQHwbbgx6qd5AIh78SB/+WPJIXFHYIqzs4=',
         ),
     )
     @unpack
     def test_sign_string(
         self,
```

### Comparing `django_hmac_authentication-1.1.1/src/tests/test_view_create_api_key_secret.py` & `django_hmac_authentication-1.2.0/src/tests/test_view_create_api_key_secret.py`

 * *Files identical despite different names*

