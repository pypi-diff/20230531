# Comparing `tmp/django-materialized-view-0.1.5.tar.gz` & `tmp/django-materialized-view-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-materialized-view-0.1.5.tar", last modified: Thu Mar 16 10:18:24 2023, max compression
+gzip compressed data, was "django-materialized-view-0.1.5.1.tar", last modified: Tue May 30 22:21:10 2023, max compression
```

## Comparing `django-materialized-view-0.1.5.tar` & `django-materialized-view-0.1.5.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.996702 django-materialized-view-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.984702 django-materialized-view-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.988702 django-materialized-view-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-03-16 10:18:23.996702 django-materialized-view-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.988702 django-materialized-view-0.1.5/django_materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.988702 django-materialized-view-0.1.5/django_materialized_view/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.988702 django-materialized-view-0.1.5/django_materialized_view/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/management/commands/migrate_with_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.988702 django-materialized-view-0.1.5/django_materialized_view/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/django_materialized_view/sql_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.988702 django-materialized-view-0.1.5/django_materialized_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-03-16 10:18:23.000000 django-materialized-view-0.1.5/django_materialized_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-16 10:18:23.000000 django-materialized-view-0.1.5/django_materialized_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 10:18:23.000000 django-materialized-view-0.1.5/django_materialized_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 10:18:23.000000 django-materialized-view-0.1.5/django_materialized_view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-16 10:18:23.000000 django-materialized-view-0.1.5/django_materialized_view.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.988702 django-materialized-view-0.1.5/example_project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.992702 django-materialized-view-0.1.5/example_project/example_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.992702 django-materialized-view-0.1.5/example_project/example_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/migrations/0002_materializedviewfromqueryset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.992702 django-materialized-view-0.1.5/example_project/example_app/models/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.992702 django-materialized-view-0.1.5/example_project/example_app/models/materialized_views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/models/materialized_views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/models/materialized_views/materialized_view_from_queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/models/materialized_views/materialized_view_from_raw_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.992702 django-materialized-view-0.1.5/example_project/example_app/models/materialized_views/sql_files/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/models/materialized_views/sql_files/materializedviewfromrawsql.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_app/models/my_test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.992702 django-materialized-view-0.1.5/example_project/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_project/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_project/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/example_project/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/example_project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    44215 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-16 10:18:23.996702 django-materialized-view-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.992702 django-materialized-view-0.1.5/testproject/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.996702 django-materialized-view-0.1.5/testproject/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/tests/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.996702 django-materialized-view-0.1.5/testproject/tests/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/tests/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:23.996702 django-materialized-view-0.1.5/testproject/tests/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/tests/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/tests/management/commands/test_migrate_with_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/tests/test_base_mode_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:18:04.000000 django-materialized-view-0.1.5/testproject/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.604225 django-materialized-view-0.1.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/management/commands/migrate_with_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/sql_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/migrations/0002_materializedviewfromqueryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/materialized_view_from_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/materialized_view_from_raw_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/sql_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/sql_files/materializedviewfromrawsql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/my_test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    44215 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/testproject/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/testproject/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/testproject/tests/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/testproject/tests/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/management/commands/test_migrate_with_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/test_base_mode_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/urls.py
```

### Comparing `django-materialized-view-0.1.5/.github/workflows/release.yml` & `django-materialized-view-0.1.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/.github/workflows/test.yml` & `django-materialized-view-0.1.5.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/.pre-commit-config.yaml` & `django-materialized-view-0.1.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/LICENSE` & `django-materialized-view-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/PKG-INFO` & `django-materialized-view-0.1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-materialized-view
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Plugin for django to support Materialized Views
 Home-page: https://github.com/muehlemann-popp/django-materialized-view
 Author: Farruh Sheripiov
 Author-email: farruh.sheripov@muehlemann-popp.ch
 Maintainer: Silvan Mühlemann
 Maintainer-email: silvan.muehlemann@muehlemann-popp.ch
 License: 'MIT'
```

### Comparing `django-materialized-view-0.1.5/README.md` & `django-materialized-view-0.1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/django_materialized_view/base_model.py` & `django-materialized-view-0.1.5.1/django_materialized_view/base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import logging
 import time
-from typing import Callable, Dict, Optional, Union
+from typing import Callable, Dict, Optional, Union, Tuple
 
 from django.conf import settings
 from django.db import DEFAULT_DB_ALIAS, connections, models
 from django.db.models import QuerySet
 from django.db.models.base import ModelBase
 
 __all__ = [
@@ -110,15 +110,15 @@
             log.duration = datetime.timedelta(seconds=end_time - start_time)
         except Exception:  # noqa
             log.failed = True
             logging.exception(f"failed to refresh materialized view {cls.get_tablename()}")
         log.save()
 
     @classmethod
-    def view_definition(cls):
+    def view_definition(cls) -> Tuple[str, tuple]:
         return cls.__get_query()
 
     @classmethod
     def __create_index_for_primary_key(cls) -> str:
         try:
             if not cls.create_pkey_index:
                 return ""
@@ -146,26 +146,26 @@
         @staticmethod
         def get_query_from_queryset() -> QuerySet:
             return User.objects.all()
         """
         pass
 
     @classmethod
-    def __get_query(cls) -> str:
+    def __get_query(cls, *args) -> Tuple[str, tuple]:
         queryset = cls.get_query_from_queryset()
-
         if isinstance(queryset, QuerySet):
-            sql_query = f"{queryset.query}; {cls.__create_index_for_primary_key()}"
-            return sql_query
+            query, args = queryset.query.sql_with_params()
+            sql_query = f"{query}; {cls.__create_index_for_primary_key()}"
+            return sql_query, args
         try:
             with open(cls.__get_sql_file_path(), "r") as sql_file:
                 sql_query = f"{sql_file.read()}; {cls.__create_index_for_primary_key()}"
         except FileNotFoundError as exc:
             raise FileNotFoundError(f"{exc}, - please create SQL file and put it to this directory")
-        return sql_query
+        return sql_query, args
 
     @classmethod
     def __get_class_name(cls) -> str:
         return cls.__name__.casefold()
 
     @classmethod
     def __get_app_label(cls) -> str:
```

### Comparing `django-materialized-view-0.1.5/django_materialized_view/management/commands/migrate_with_views.py` & `django-materialized-view-0.1.5.1/django_materialized_view/management/commands/migrate_with_views.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/django_materialized_view/migrations/0001_initial.py` & `django-materialized-view-0.1.5.1/django_materialized_view/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/django_materialized_view/models.py` & `django-materialized-view-0.1.5.1/django_materialized_view/models.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/django_materialized_view/processor.py` & `django-materialized-view-0.1.5.1/django_materialized_view/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     def add_view_to_be_deleted(self, view_name: str) -> None:
         self.__views_to_be_deleted.add(view_name)
 
     def mark_to_be_applied_new_views(self) -> None:
         view_models = self.__get_current_view_models()
         for (app_label, model_name), view_model in view_models.items():
             view_name = self.__get_view_name(app_label, model_name)
-            actual_view_definition = self.__get_actual_view_definition(view_name)
-            actual_view_definition_hash = self.__get_hash_from_string(actual_view_definition)
+            actual_view_definition, args = self.__get_actual_view_definition(view_name)
+            actual_view_definition_hash = self.__get_hash_from_string(actual_view_definition % args)
 
             previous_view_definition_hash = self.__get_previous_view_definition_hash(app_label, model_name)
 
             if previous_view_definition_hash is None:
                 self.add_view_to_be_created(view_name)
             elif not self.__is_same_views(previous_view_definition_hash, actual_view_definition_hash):
                 self.add_view_to_be_recreated(view_name)
@@ -123,18 +123,18 @@
 
         sorted_views = OrderedDict(sorted(self.__recreation_priority.items(), key=lambda item: item[1], reverse=True))
         return sorted_views
 
     def _create_view(self, view_name: str) -> bool:
         logger.debug(f"Creating view: {view_name}")
 
-        view_definition = self.__get_actual_view_definition(view_name)
+        view_definition, args = self.__get_actual_view_definition(view_name)
         with connection.cursor() as cursor:
             try:
-                cursor.execute(self.CREATE_COMMAND_TEMPLATE % (view_name, view_definition))
+                cursor.execute(self.CREATE_COMMAND_TEMPLATE % (view_name, view_definition), args)
             except ProgrammingError as exc:
                 logger.debug(f"Unable to create view: {view_name}. Error: {exc.args}")
                 if "already exists" in exc.args[0]:
                     logger.debug(f"Marking to recreate view: {view_name}. Marking to recreate view. Error: {exc.args}")
                     self.add_view_to_be_recreated(view_name)
                     self.__remove_view_from_creation_list(view_name)
                     return False
@@ -220,19 +220,19 @@
             for view_obj in related_views
             if view_obj[self.REF_TABLE_FIELD_NAME] == view_name
         ]
 
     def __get_actual_view_definition(self, view_name: str) -> str:
         view_model = DBViewsRegistry[view_name]
         if callable(view_model.view_definition):
-            raw_view_definition = view_model.view_definition()
+            raw_view_definition, args = view_model.view_definition()
         else:
-            raw_view_definition = view_model.view_definition
+            raise ValueError("view_definition must be callable")
         view_definition = self.__get_cleaned_view_definition_value(raw_view_definition)
-        return view_definition
+        return view_definition, args
 
     def __prioritize_view(self, view: str, related_views: List[str], dependencies_story: set[str]) -> None:
         if related_views:
             dependencies_story.update(related_views)
             self.__recreation_priority[view] += 1
         else:
             self.__recreation_priority[view] += 0
@@ -273,15 +273,15 @@
             row = dictfetchall(cursor)
         return row
 
     @staticmethod
     def __get_cleaned_view_definition_value(view_definition: str) -> str:
         assert isinstance(
             view_definition, str
-        ), "View definition must be callable and return string or be itself a string."
+        ), "View definition must be callable and return Tuple[str, Optional[tuple]]."
         return view_definition.strip()
 
     @staticmethod
     def __get_hash_from_string(string: str) -> str:
         string = string.replace('"', "").replace(" ", "").replace("\n", "").replace("'", "").lower()
         return hashlib.md5(string.encode()).hexdigest()
```

### Comparing `django-materialized-view-0.1.5/django_materialized_view.egg-info/PKG-INFO` & `django-materialized-view-0.1.5.1/django_materialized_view.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-materialized-view
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Plugin for django to support Materialized Views
 Home-page: https://github.com/muehlemann-popp/django-materialized-view
 Author: Farruh Sheripiov
 Author-email: farruh.sheripov@muehlemann-popp.ch
 Maintainer: Silvan Mühlemann
 Maintainer-email: silvan.muehlemann@muehlemann-popp.ch
 License: 'MIT'
```

### Comparing `django-materialized-view-0.1.5/django_materialized_view.egg-info/SOURCES.txt` & `django-materialized-view-0.1.5.1/django_materialized_view.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/example_project/example_app/migrations/0001_initial.py` & `django-materialized-view-0.1.5.1/example_project/example_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/example_project/example_app/migrations/0002_materializedviewfromqueryset.py` & `django-materialized-view-0.1.5.1/example_project/example_app/migrations/0002_materializedviewfromqueryset.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/example_project/example_app/models/materialized_views/materialized_view_from_queryset.py` & `django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/materialized_view_from_queryset.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/example_project/example_app/models/materialized_views/materialized_view_from_raw_sql.py` & `django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/materialized_view_from_raw_sql.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/example_project/example_project/settings.py` & `django-materialized-view-0.1.5.1/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/example_project/example_project/urls.py` & `django-materialized-view-0.1.5.1/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/example_project/manage.py` & `django-materialized-view-0.1.5.1/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/poetry.lock` & `django-materialized-view-0.1.5.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/pyproject.toml` & `django-materialized-view-0.1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/setup.cfg` & `django-materialized-view-0.1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/testproject/manage.py` & `django-materialized-view-0.1.5.1/testproject/manage.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/testproject/settings.py` & `django-materialized-view-0.1.5.1/testproject/settings.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/testproject/tests/management/commands/test_migrate_with_views.py` & `django-materialized-view-0.1.5.1/testproject/tests/management/commands/test_migrate_with_views.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5/testproject/tests/test_base_mode_tests.py` & `django-materialized-view-0.1.5.1/testproject/tests/test_base_mode_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         string = "test_string"
         result = self.view_processor._MaterializedViewsProcessor__get_cleaned_view_definition_value(string)
         assert result == string
 
     def test__get_cleaned_view_definition_value__invalid(self):
         with pytest.raises(AssertionError) as exc:
             self.view_processor._MaterializedViewsProcessor__get_cleaned_view_definition_value(1)
-        assert exc.value.args == ("View definition must be callable and return string or be itself a string.",)
+        assert exc.value.args == ("View definition must be callable and return Tuple[str, Optional[tuple]].",)
 
     @pytest.mark.django_db
     def test__get_related_views__success(self):
         with assertNumQueries(1):
             result = self.view_processor._MaterializedViewsProcessor__get_related_views()
         assert set([i["materialized_view"] for i in result]) == set(DBViewsRegistry.keys())
 
@@ -126,39 +126,26 @@
         assert test_dependencies_story == {test_view_name, test_view_name_two, *test_related_views}
         assert self.view_processor._MaterializedViewsProcessor__recreation_priority == {test_view_name: 3}
 
     def test__get_actual_view_definition__success(self, mocker, subtests):
         test_view_definition = "test"
         with subtests.test(msg="view_definition callable"):
             test_view_mock = MagicMock()
+            test_view_mock.view_definition.return_value = ("test raw query", ())
             DBViewsRegistry[test_view_definition] = test_view_mock
             get_cleaned_view_mock = mocker.patch.object(
                 MaterializedViewsProcessor,
                 "_MaterializedViewsProcessor__get_cleaned_view_definition_value",
                 return_value=test_view_definition,
             )
 
             result = self.view_processor._MaterializedViewsProcessor__get_actual_view_definition("test")
 
-            get_cleaned_view_mock.assert_called_once_with(test_view_mock.view_definition())
-            assert result == test_view_definition
-
-        with subtests.test(msg="view_definition is str"):
-            test_view_mock = MagicMock()
-            test_view_mock.view_definition = "test"
-            DBViewsRegistry[test_view_definition] = test_view_mock
-            get_cleaned_view_mock = mocker.patch.object(
-                MaterializedViewsProcessor,
-                "_MaterializedViewsProcessor__get_cleaned_view_definition_value",
-                return_value=test_view_definition,
-            )
-
-            result = self.view_processor._MaterializedViewsProcessor__get_actual_view_definition("test")
-            get_cleaned_view_mock.assert_called_once_with(test_view_mock.view_definition)
-            assert result == test_view_definition
+            get_cleaned_view_mock.assert_called_once_with("test raw query")
+            assert result == (test_view_definition, ())
 
     def test__get_ref_views__success(self, mocker):
         ref_view_name = "test_ref_view"
         test_mt_view_name = "test_mt_view"
         test_ref_views = [
             {
                 self.view_processor.MATERIALIZED_VIEW_FIELD_NAME: test_mt_view_name,
@@ -321,15 +308,15 @@
 
     @pytest.mark.django_db
     def test__create_view__success(self, mocker, subtests):
         test_app_name = "app"
         test_view_name = "viewname"
         full_view_name = f"{test_app_name}_{test_view_name}"
 
-        view_definition = "SELECT * FROM pg_depend"
+        view_definition = "SELECT * FROM pg_depend", ()
         get_actual_view_definition_mock = mocker.patch.object(
             MaterializedViewsProcessor,
             "_MaterializedViewsProcessor__get_actual_view_definition",
             return_value=view_definition,
         )
 
         with assertNumQueries(3):
```

