# Comparing `tmp/django-oauth-toolkit-2.2.0.tar.gz` & `tmp/django-oauth-toolkit-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oauth-toolkit-2.2.0.tar", last modified: Tue Oct 18 16:40:36 2022, max compression
+gzip compressed data, was "django-oauth-toolkit-2.3.0.tar", last modified: Wed May 31 21:01:09 2023, max compression
```

## Comparing `django-oauth-toolkit-2.2.0.tar` & `django-oauth-toolkit-2.3.0.tar`

### file list

```diff
@@ -1,76 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5737 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4655 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.777766 django-oauth-toolkit-2.2.0/django_oauth_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5737 2022-10-18 16:40:36.000000 django-oauth-toolkit-2.2.0/django_oauth_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-10-18 16:40:36.000000 django-oauth-toolkit-2.2.0/django_oauth_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 16:40:36.000000 django-oauth-toolkit-2.2.0/django_oauth_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 16:40:36.000000 django-oauth-toolkit-2.2.0/django_oauth_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-18 16:40:36.000000 django-oauth-toolkit-2.2.0/django_oauth_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-18 16:40:36.000000 django-oauth-toolkit-2.2.0/django_oauth_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/oauth2_provider/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/backends.py
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/oauth2_provider/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/oauth2_provider/contrib/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/contrib/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/contrib/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)     6587 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/contrib/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/generators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/http.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/oauth2_provider/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/oauth2_provider/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/management/commands/cleartokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     3857 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/management/commands/createapplication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/oauth2_provider/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     5872 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0002_auto_20190406_1805.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0003_auto_20201211_1314.py
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0004_auto_20200902_2022.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0005_auto_20211222_2352.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0006_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26184 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9459 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/oauth2_backends.py
--rw-r--r--   0 runner    (1001) docker     (121)    38268 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/oauth2_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/scopes.py
--rw-r--r--   0 runner    (1001) docker     (121)    11409 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.777766 django-oauth-toolkit-2.2.0/oauth2_provider/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/application_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/application_detail.html
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/application_form.html
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/application_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/application_registration_form.html
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/authorize.html
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/authorized-token-delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/authorized-tokens.html
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:40:36.781766 django-oauth-toolkit-2.2.0/oauth2_provider/views/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/views/application.py
--rw-r--r--   0 runner    (1001) docker     (121)    11959 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/views/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/views/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/views/introspect.py
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     5066 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/views/oidc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/oauth2_provider/views/token.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-10-18 16:40:36.785766 django-oauth-toolkit-2.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       62 2022-10-18 16:40:27.000000 django-oauth-toolkit-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.933997 django-oauth-toolkit-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-31 21:01:09.933997 django-oauth-toolkit-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.921996 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/cleartokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/createapplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.929997 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0002_auto_20190406_1805.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0003_auto_20201211_1314.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0004_auto_20200902_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0005_auto_20211222_2352.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0006_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0007_application_post_logout_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/oauth2_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38283 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/oauth2_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.921996 django-oauth-toolkit-2.3.0/oauth2_provider/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.929997 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_registration_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorize.html
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorized-token-delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorized-tokens.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/logout_confirm.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.929997 django-oauth-toolkit-2.3.0/oauth2_provider/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-31 21:01:09.937997 django-oauth-toolkit-2.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.933997 django-oauth-toolkit-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_application_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_auth_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73185 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_authorization_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_client_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57835 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_introspection_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_introspection_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_oauth2_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21967 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_oauth2_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27089 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_oidc_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_scopes_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_token_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_token_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_validators.py
```

### Comparing `django-oauth-toolkit-2.2.0/AUTHORS` & `django-oauth-toolkit-2.3.0/AUTHORS`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 Federico Frenguelli
 
 Contributors
 ------------
 
 Abhishek Patel
 Adam Johnson
+Adheeth P Praveen
 Alan Crosswell
 Alejandro Mantecon Guillen
 Aleksander Vaskevich
 Alessandro De Angelis
 Alex Szabó
 Allisson Azevedo
 Andrea Greco
 Andrej Zbín
 Andrew Chen Wang
+Antoine Laurent
 Anvesh Agarwal
 Aristóbulo Meneses
 Aryan Iyappan
 Ash Christopher
 Asif Saif Uddin
 Bart Merenda
 Bas van Oostveen
@@ -36,14 +38,15 @@
 Dawid Wolski
 Diego Garcia
 Dominik George
 Dulmandakh Sukhbaatar
 Dylan Giesler
 Dylan Tack
 Eduardo Oliveira
+Egor Poderiagin
 Emanuele Palazzetti
 Federico Dolce
 Frederico Vieira
 Hasan Ramezani
 Hiroki Kiyohara
 Hossein Shakiba
 Islam Kamel
@@ -52,19 +55,23 @@
 Jerome Leclanche
 Jesse Gibbs
 Jim Graham
 Jonas Nygaard Pedersen
 Jonathan Steffan
 Jordi Sanchez
 Joseph Abrahams
+Josh Thomas
 Jozef Knaperek
+Julian Mundhahs
 Julien Palard
 Jun Zhou
 Kaleb Porter
 Kristian Rune Larsen
+Ludwig Hähne
+Marcus Sonestedt
 Matias Seniquiel
 Michael Howitz
 Owen Gong
 Patrick Palacin
 Paul Dekkers
 Paul Oswald
 Pavel Tvrdík
@@ -74,14 +81,15 @@
 Rodney Richardson
 Rustem Saiargaliev
 Rustem Saiargaliev
 Sandro Rodrigues
 Shaheed Haque
 Shaun Stanworth
 Silvano Cerza
+Sora Yanai
 Spencer Carroll
 Stéphane Raimbault
 Tom Evans
 Vinay Karanam
 Víðir Valberg Guðmundsson
 Will Beaufoy
 pySilver
```

### Comparing `django-oauth-toolkit-2.2.0/LICENSE` & `django-oauth-toolkit-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/PKG-INFO` & `django-oauth-toolkit-2.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: django-oauth-toolkit
-Version: 2.2.0
+Version: 2.3.0
 Summary: OAuth2 Provider for Django
 Home-page: https://github.com/jazzband/django-oauth-toolkit
 Author: Federico Frenguelli, Massimiliano Pippi
 Author-email: synasius@gmail.com
 Keywords: django,oauth,oauth2,oauthlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Django OAuth Toolkit
 ====================
@@ -59,29 +61,24 @@
  * You need to implement an OAuth2 authorization server to provide tokens management for your infrastructure,
 
 Django OAuth Toolkit can help you providing out of the box all the endpoints, data and logic needed to add OAuth2
 capabilities to your Django projects. Django OAuth Toolkit makes extensive use of the excellent
 `OAuthLib <https://github.com/idan/oauthlib>`_, so that everything is
 `rfc-compliant <http://tools.ietf.org/html/rfc6749>`_.
 
-Note: If you have issues installing Django 4.0.0, it is because we only support
-Django 4.0.1+ due to a regression in Django 4.0.0. Besides 4.0.0, Django 2.2+ is supported.
-`Explanation <https://github.com/jazzband/django-oauth-toolkit/pull/1046#issuecomment-998015272>`_.
-
-
 Reporting security issues
 -------------------------
 
 Please report any security issues to the JazzBand security team at <security@jazzband.co>. Do not file an issue on the tracker.
 
 Requirements
 ------------
 
 * Python 3.7+
-* Django 2.2, 3.2, or >=4.0.1
+* Django 2.2, 3.2, 4.0 (4.0.1+ due to a regression), 4.1, or 4.2
 * oauthlib 3.1+
 
 Installation
 ------------
 
 Install with pip::
```

### Comparing `django-oauth-toolkit-2.2.0/README.rst` & `django-oauth-toolkit-2.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -31,29 +31,24 @@
  * You need to implement an OAuth2 authorization server to provide tokens management for your infrastructure,
 
 Django OAuth Toolkit can help you providing out of the box all the endpoints, data and logic needed to add OAuth2
 capabilities to your Django projects. Django OAuth Toolkit makes extensive use of the excellent
 `OAuthLib <https://github.com/idan/oauthlib>`_, so that everything is
 `rfc-compliant <http://tools.ietf.org/html/rfc6749>`_.
 
-Note: If you have issues installing Django 4.0.0, it is because we only support
-Django 4.0.1+ due to a regression in Django 4.0.0. Besides 4.0.0, Django 2.2+ is supported.
-`Explanation <https://github.com/jazzband/django-oauth-toolkit/pull/1046#issuecomment-998015272>`_.
-
-
 Reporting security issues
 -------------------------
 
 Please report any security issues to the JazzBand security team at <security@jazzband.co>. Do not file an issue on the tracker.
 
 Requirements
 ------------
 
 * Python 3.7+
-* Django 2.2, 3.2, or >=4.0.1
+* Django 2.2, 3.2, 4.0 (4.0.1+ due to a regression), 4.1, or 4.2
 * oauthlib 3.1+
 
 Installation
 ------------
 
 Install with pip::
```

### Comparing `django-oauth-toolkit-2.2.0/django_oauth_toolkit.egg-info/PKG-INFO` & `django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: django-oauth-toolkit
-Version: 2.2.0
+Version: 2.3.0
 Summary: OAuth2 Provider for Django
 Home-page: https://github.com/jazzband/django-oauth-toolkit
 Author: Federico Frenguelli, Massimiliano Pippi
 Author-email: synasius@gmail.com
 Keywords: django,oauth,oauth2,oauthlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Django OAuth Toolkit
 ====================
@@ -59,29 +61,24 @@
  * You need to implement an OAuth2 authorization server to provide tokens management for your infrastructure,
 
 Django OAuth Toolkit can help you providing out of the box all the endpoints, data and logic needed to add OAuth2
 capabilities to your Django projects. Django OAuth Toolkit makes extensive use of the excellent
 `OAuthLib <https://github.com/idan/oauthlib>`_, so that everything is
 `rfc-compliant <http://tools.ietf.org/html/rfc6749>`_.
 
-Note: If you have issues installing Django 4.0.0, it is because we only support
-Django 4.0.1+ due to a regression in Django 4.0.0. Besides 4.0.0, Django 2.2+ is supported.
-`Explanation <https://github.com/jazzband/django-oauth-toolkit/pull/1046#issuecomment-998015272>`_.
-
-
 Reporting security issues
 -------------------------
 
 Please report any security issues to the JazzBand security team at <security@jazzband.co>. Do not file an issue on the tracker.
 
 Requirements
 ------------
 
 * Python 3.7+
-* Django 2.2, 3.2, or >=4.0.1
+* Django 2.2, 3.2, 4.0 (4.0.1+ due to a regression), 4.1, or 4.2
 * oauthlib 3.1+
 
 Installation
 ------------
 
 Install with pip::
```

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/admin.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/admin.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/backends.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/backends.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/contrib/rest_framework/authentication.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/contrib/rest_framework/permissions.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/decorators.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/decorators.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/forms.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/forms.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,7 +8,21 @@
     nonce = forms.CharField(required=False, widget=forms.HiddenInput())
     client_id = forms.CharField(widget=forms.HiddenInput())
     state = forms.CharField(required=False, widget=forms.HiddenInput())
     response_type = forms.CharField(widget=forms.HiddenInput())
     code_challenge = forms.CharField(required=False, widget=forms.HiddenInput())
     code_challenge_method = forms.CharField(required=False, widget=forms.HiddenInput())
     claims = forms.CharField(required=False, widget=forms.HiddenInput())
+
+
+class ConfirmLogoutForm(forms.Form):
+    allow = forms.BooleanField(required=False)
+    id_token_hint = forms.CharField(required=False, widget=forms.HiddenInput())
+    logout_hint = forms.CharField(required=False, widget=forms.HiddenInput())
+    client_id = forms.CharField(required=False, widget=forms.HiddenInput())
+    post_logout_redirect_uri = forms.CharField(required=False, widget=forms.HiddenInput())
+    state = forms.CharField(required=False, widget=forms.HiddenInput())
+    ui_locales = forms.CharField(required=False, widget=forms.HiddenInput())
+
+    def __init__(self, *args, **kwargs):
+        self.request = kwargs.pop("request", None)
+        super(ConfirmLogoutForm, self).__init__(*args, **kwargs)
```

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/generators.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/generators.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/http.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/http.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/management/commands/createapplication.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/createapplication.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,20 @@
         )
         parser.add_argument(
             "--redirect-uris",
             type=str,
             help="The redirect URIs, this must be a space separated string e.g 'URI1 URI2'",
         )
         parser.add_argument(
+            "--post-logout-redirect-uris",
+            type=str,
+            help="The post logout redirect URIs, this must be a space separated string e.g 'URI1 URI2'",
+            default="",
+        )
+        parser.add_argument(
             "--client-secret",
             type=str,
             help="The secret for this application",
         )
         parser.add_argument(
             "--name",
             type=str,
```

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/middleware.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/middleware.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0001_initial.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0002_auto_20190406_1805.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0002_auto_20190406_1805.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0004_auto_20200902_2022.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0004_auto_20200902_2022.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0005_auto_20211222_2352.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0005_auto_20211222_2352.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/migrations/0006_alter_application_client_secret.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0006_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/models.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     Fields:
 
     * :attr:`client_id` The client identifier issued to the client during the
                         registration process as described in :rfc:`2.2`
     * :attr:`user` ref to a Django user
     * :attr:`redirect_uris` The list of allowed redirect uri. The string
                             consists of valid URLs separated by space
+    * :attr:`post_logout_redirect_uris` The list of allowed redirect uris after
+                                        an RP initiated logout. The string
+                                        consists of valid URLs separated by space
     * :attr:`client_type` Client type as described in :rfc:`2.1`
     * :attr:`authorization_grant_type` Authorization flows available to the
                                        Application
     * :attr:`client_secret` Confidential secret issued to the client during
                             the registration process as described in :rfc:`2.2`
     * :attr:`name` Friendly name for the Application
     """
@@ -99,14 +102,18 @@
         on_delete=models.CASCADE,
     )
 
     redirect_uris = models.TextField(
         blank=True,
         help_text=_("Allowed URIs list, space separated"),
     )
+    post_logout_redirect_uris = models.TextField(
+        blank=True,
+        help_text=_("Allowed Post Logout URIs list, space separated"),
+    )
     client_type = models.CharField(max_length=32, choices=CLIENT_TYPES)
     authorization_grant_type = models.CharField(max_length=32, choices=GRANT_TYPES)
     client_secret = ClientSecretField(
         max_length=255,
         blank=True,
         default=generate_client_secret,
         db_index=True,
@@ -146,14 +153,22 @@
         """
         Checks if given url is one of the items in :attr:`redirect_uris` string
 
         :param uri: Url to check
         """
         return redirect_to_uri_allowed(uri, self.redirect_uris.split())
 
+    def post_logout_redirect_uri_allowed(self, uri):
+        """
+        Checks if given URI is one of the items in :attr:`post_logout_redirect_uris` string
+
+        :param uri: URI to check
+        """
+        return redirect_to_uri_allowed(uri, self.post_logout_redirect_uris.split())
+
     def clean(self):
         from django.core.exceptions import ValidationError
 
         grant_types = (
             AbstractApplication.GRANT_AUTHORIZATION_CODE,
             AbstractApplication.GRANT_IMPLICIT,
             AbstractApplication.GRANT_OPENID_HYBRID,
@@ -659,14 +674,15 @@
         deleted = start_no - stop_no
         return deleted
 
     now = timezone.now()
     refresh_expire_at = None
     access_token_model = get_access_token_model()
     refresh_token_model = get_refresh_token_model()
+    id_token_model = get_id_token_model()
     grant_model = get_grant_model()
     REFRESH_TOKEN_EXPIRE_SECONDS = oauth2_settings.REFRESH_TOKEN_EXPIRE_SECONDS
 
     if REFRESH_TOKEN_EXPIRE_SECONDS:
         if not isinstance(REFRESH_TOKEN_EXPIRE_SECONDS, timedelta):
             try:
                 REFRESH_TOKEN_EXPIRE_SECONDS = timedelta(seconds=REFRESH_TOKEN_EXPIRE_SECONDS)
@@ -692,14 +708,20 @@
 
     access_token_query = models.Q(refresh_token__isnull=True, expires__lt=now)
     access_tokens = access_token_model.objects.filter(access_token_query)
 
     access_tokens_delete_no = batch_delete(access_tokens, access_token_query)
     logger.info("%s Expired access tokens deleted", access_tokens_delete_no)
 
+    id_token_query = models.Q(access_token__isnull=True, expires__lt=now)
+    id_tokens = id_token_model.objects.filter(id_token_query)
+
+    id_tokens_delete_no = batch_delete(id_tokens, id_token_query)
+    logger.info("%s Expired ID tokens deleted", id_tokens_delete_no)
+
     grants_query = models.Q(expires__lt=now)
     grants = grant_model.objects.filter(grants_query)
 
     grants_deleted_no = batch_delete(grants, grants_query)
     logger.info("%s Expired grant tokens deleted", grants_deleted_no)
 
 
@@ -738,13 +760,12 @@
             and parsed_allowed_uri.hostname == parsed_uri.hostname
             and parsed_allowed_uri.path == parsed_uri.path
         ) or (
             parsed_allowed_uri.scheme == parsed_uri.scheme
             and parsed_allowed_uri.netloc == parsed_uri.netloc
             and parsed_allowed_uri.path == parsed_uri.path
         ):
-
             aqs_set = set(parse_qsl(parsed_allowed_uri.query))
             if aqs_set.issubset(uqs_set):
                 return True
 
     return False
```

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/oauth2_backends.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/oauth2_backends.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/oauth2_validators.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/oauth2_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         Remember that this method is NOT RECOMMENDED and SHOULD be limited to
         clients unable to directly utilize the HTTP Basic authentication scheme.
         See rfc:`2.3.1` for more details.
         """
         # TODO: check if oauthlib has already unquoted client_id and client_secret
         try:
             client_id = request.client_id
-            client_secret = request.client_secret
+            client_secret = getattr(request, "client_secret", "")
         except AttributeError:
             return False
 
         if self._load_application(client_id, request) is None:
             log.debug("Failed body auth: Application %s does not exists" % client_id)
             return False
         elif not check_password(client_secret, request.client.client_secret):
@@ -568,15 +568,14 @@
 
             # If we are to reuse tokens, and we can: do so
             if (
                 not self.rotate_refresh_token(request)
                 and isinstance(refresh_token_instance, RefreshToken)
                 and refresh_token_instance.access_token
             ):
-
                 access_token = AccessToken.objects.select_for_update().get(
                     pk=refresh_token_instance.access_token.pk
                 )
                 access_token.user = request.user
                 access_token.scope = token["scope"]
                 access_token.expires = expires
                 access_token.token = token["access_token"]
```

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/scopes.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/scopes.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/settings.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,19 @@
         "code id_token token",
     ],
     "OIDC_SUBJECT_TYPES_SUPPORTED": ["public"],
     "OIDC_TOKEN_ENDPOINT_AUTH_METHODS_SUPPORTED": [
         "client_secret_post",
         "client_secret_basic",
     ],
+    "OIDC_RP_INITIATED_LOGOUT_ENABLED": False,
+    "OIDC_RP_INITIATED_LOGOUT_ALWAYS_PROMPT": True,
+    "OIDC_RP_INITIATED_LOGOUT_STRICT_REDIRECT_URIS": False,
+    "OIDC_RP_INITIATED_LOGOUT_ACCEPT_EXPIRED_TOKENS": True,
+    "OIDC_RP_INITIATED_LOGOUT_DELETE_TOKENS": True,
     # Special settings that will be evaluated at runtime
     "_SCOPES": [],
     "_DEFAULT_SCOPES": [],
     # Resource Server with Token Introspection
     "RESOURCE_SERVER_INTROSPECTION_URL": None,
     "RESOURCE_SERVER_AUTH_TOKEN": None,
     "RESOURCE_SERVER_INTROSPECTION_CREDENTIALS": None,
```

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/application_confirm_delete.html` & `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/application_detail.html` & `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_detail.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/application_form.html` & `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_form.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/application_list.html` & `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_list.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/authorize.html` & `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/authorized-tokens.html` & `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorized-tokens.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/templates/oauth2_provider/base.html` & `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/base.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/urls.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,11 +34,12 @@
     re_path(
         r"^\.well-known/openid-configuration/$",
         views.ConnectDiscoveryInfoView.as_view(),
         name="oidc-connect-discovery-info",
     ),
     re_path(r"^\.well-known/jwks.json$", views.JwksInfoView.as_view(), name="jwks-info"),
     re_path(r"^userinfo/$", views.UserInfoView.as_view(), name="user-info"),
+    re_path(r"^logout/$", views.RPInitiatedLogoutView.as_view(), name="rp-initiated-logout"),
 ]
 
 
 urlpatterns = base_urlpatterns + management_urlpatterns + oidc_urlpatterns
```

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/validators.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/validators.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/views/__init__.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/views/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     ClientProtectedResourceView,
     ClientProtectedScopedResourceView,
     ProtectedResourceView,
     ReadWriteScopedResourceView,
     ScopedProtectedResourceView,
 )
 from .introspect import IntrospectTokenView
-from .oidc import ConnectDiscoveryInfoView, JwksInfoView, UserInfoView
+from .oidc import ConnectDiscoveryInfoView, JwksInfoView, RPInitiatedLogoutView, UserInfoView
 from .token import AuthorizedTokenDeleteView, AuthorizedTokensListView
```

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/views/application.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/views/application.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/views/base.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/views/base.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/views/generic.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/views/generic.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/views/introspect.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/views/introspect.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/views/mixins.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/views/mixins.py`

 * *Files 12% similar despite different names*

```diff
@@ -322,7 +322,31 @@
     def dispatch(self, *args, **kwargs):
         if not oauth2_settings.OIDC_ENABLED:
             if settings.DEBUG:
                 raise ImproperlyConfigured(self.debug_error_message)
             log.warning(self.debug_error_message)
             return HttpResponseNotFound()
         return super().dispatch(*args, **kwargs)
+
+
+class OIDCLogoutOnlyMixin(OIDCOnlyMixin):
+    """
+    Mixin for views that should only be accessible when OIDC and OIDC RP-Initiated Logout are enabled.
+
+    If either is not enabled:
+
+    * if DEBUG is True, raises an ImproperlyConfigured exception explaining why
+    * otherwise, returns a 404 response, logging the same warning
+    """
+
+    debug_error_message = (
+        "The django-oauth-toolkit OIDC RP-Initiated Logout view is not enabled unless you "
+        "have configured OIDC_RP_INITIATED_LOGOUT_ENABLED in the settings"
+    )
+
+    def dispatch(self, *args, **kwargs):
+        if not oauth2_settings.OIDC_RP_INITIATED_LOGOUT_ENABLED:
+            if settings.DEBUG:
+                raise ImproperlyConfigured(self.debug_error_message)
+            log.warning(self.debug_error_message)
+            return HttpResponseNotFound()
+        return super().dispatch(*args, **kwargs)
```

### Comparing `django-oauth-toolkit-2.2.0/oauth2_provider/views/token.py` & `django-oauth-toolkit-2.3.0/oauth2_provider/views/token.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.2.0/setup.cfg` & `django-oauth-toolkit-2.3.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 2.2
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires =
```

