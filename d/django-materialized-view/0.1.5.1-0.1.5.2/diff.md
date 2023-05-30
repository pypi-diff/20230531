# Comparing `tmp/django-materialized-view-0.1.5.1.tar.gz` & `tmp/django-materialized-view-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-materialized-view-0.1.5.1.tar", last modified: Tue May 30 22:21:10 2023, max compression
+gzip compressed data, was "django-materialized-view-0.1.5.2.tar", last modified: Tue May 30 22:40:49 2023, max compression
```

## Comparing `django-materialized-view-0.1.5.1.tar` & `django-materialized-view-0.1.5.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.604225 django-materialized-view-0.1.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/management/commands/migrate_with_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/django_materialized_view/sql_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.608225 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 22:21:10.000000 django-materialized-view-0.1.5.1/django_materialized_view.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/migrations/0002_materializedviewfromqueryset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/models/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/materialized_view_from_queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/materialized_view_from_raw_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/sql_files/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/sql_files/materializedviewfromrawsql.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_app/models/my_test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/example_project/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/example_project/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/example_project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    44215 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/testproject/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/testproject/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/testproject/tests/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:10.612225 django-materialized-view-0.1.5.1/testproject/tests/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/management/commands/test_migrate_with_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/tests/test_base_mode_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:20:56.000000 django-materialized-view-0.1.5.1/testproject/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.670542 django-materialized-view-0.1.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/django_materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/django_materialized_view/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/django_materialized_view/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/management/commands/migrate_with_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/django_materialized_view/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/django_materialized_view/sql_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/django_materialized_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-30 22:40:49.000000 django-materialized-view-0.1.5.2/django_materialized_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-30 22:40:49.000000 django-materialized-view-0.1.5.2/django_materialized_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:40:49.000000 django-materialized-view-0.1.5.2/django_materialized_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 22:40:49.000000 django-materialized-view-0.1.5.2/django_materialized_view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 22:40:49.000000 django-materialized-view-0.1.5.2/django_materialized_view.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/example_project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/example_project/example_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/example_project/example_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/migrations/0002_materializedviewfromqueryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.674542 django-materialized-view-0.1.5.2/example_project/example_app/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/example_project/example_app/models/materialized_views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/models/materialized_views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/models/materialized_views/materialized_view_from_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/models/materialized_views/materialized_view_from_raw_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/example_project/example_app/models/materialized_views/sql_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/models/materialized_views/sql_files/materializedviewfromrawsql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_app/models/my_test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/example_project/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_project/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/example_project/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/example_project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    44215 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/testproject/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/testproject/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/tests/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/testproject/tests/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/tests/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:49.678542 django-materialized-view-0.1.5.2/testproject/tests/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/tests/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/tests/management/commands/test_migrate_with_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/tests/test_base_mode_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:40:35.000000 django-materialized-view-0.1.5.2/testproject/urls.py
```

### Comparing `django-materialized-view-0.1.5.1/.github/workflows/release.yml` & `django-materialized-view-0.1.5.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/.github/workflows/test.yml` & `django-materialized-view-0.1.5.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/.pre-commit-config.yaml` & `django-materialized-view-0.1.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/LICENSE` & `django-materialized-view-0.1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/PKG-INFO` & `django-materialized-view-0.1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-materialized-view
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: Plugin for django to support Materialized Views
 Home-page: https://github.com/muehlemann-popp/django-materialized-view
 Author: Farruh Sheripiov
 Author-email: farruh.sheripov@muehlemann-popp.ch
 Maintainer: Silvan Mühlemann
 Maintainer-email: silvan.muehlemann@muehlemann-popp.ch
 License: 'MIT'
```

### Comparing `django-materialized-view-0.1.5.1/README.md` & `django-materialized-view-0.1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/django_materialized_view/base_model.py` & `django-materialized-view-0.1.5.2/django_materialized_view/base_model.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/django_materialized_view/management/commands/migrate_with_views.py` & `django-materialized-view-0.1.5.2/django_materialized_view/management/commands/migrate_with_views.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/django_materialized_view/migrations/0001_initial.py` & `django-materialized-view-0.1.5.2/django_materialized_view/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/django_materialized_view/models.py` & `django-materialized-view-0.1.5.2/django_materialized_view/models.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/django_materialized_view/processor.py` & `django-materialized-view-0.1.5.2/django_materialized_view/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 elif "does not exist" in exc.args[0]:
                     return False
                 else:
                     raise exc
         logger.debug(f"View created: {view_name} ")
         logger.debug(f"Creating migration: {view_name}")
         app, model_view_name = self.__separate_app_name_and_view_name(view_name)
-        actual_view_definition_hash = self.__get_hash_from_string(view_definition)
+        actual_view_definition_hash = self.__get_hash_from_string(view_definition % args)
         migration = MaterializedViewMigrations(app=app, view_name=model_view_name, hash=actual_view_definition_hash)
         migration.save()
         logger.debug(f"Migration created: {view_name}. migration_id={migration.pk}")
         return True
 
     def _recreate_view(self, view_name: str, delete_cascade: bool) -> bool:
         logger.debug(f"Recreating view. {view_name}")
```

### Comparing `django-materialized-view-0.1.5.1/django_materialized_view.egg-info/PKG-INFO` & `django-materialized-view-0.1.5.2/django_materialized_view.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-materialized-view
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: Plugin for django to support Materialized Views
 Home-page: https://github.com/muehlemann-popp/django-materialized-view
 Author: Farruh Sheripiov
 Author-email: farruh.sheripov@muehlemann-popp.ch
 Maintainer: Silvan Mühlemann
 Maintainer-email: silvan.muehlemann@muehlemann-popp.ch
 License: 'MIT'
```

### Comparing `django-materialized-view-0.1.5.1/django_materialized_view.egg-info/SOURCES.txt` & `django-materialized-view-0.1.5.2/django_materialized_view.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/example_project/example_app/migrations/0001_initial.py` & `django-materialized-view-0.1.5.2/example_project/example_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/example_project/example_app/migrations/0002_materializedviewfromqueryset.py` & `django-materialized-view-0.1.5.2/example_project/example_app/migrations/0002_materializedviewfromqueryset.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/materialized_view_from_queryset.py` & `django-materialized-view-0.1.5.2/example_project/example_app/models/materialized_views/materialized_view_from_queryset.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/example_project/example_app/models/materialized_views/materialized_view_from_raw_sql.py` & `django-materialized-view-0.1.5.2/example_project/example_app/models/materialized_views/materialized_view_from_raw_sql.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/example_project/example_project/settings.py` & `django-materialized-view-0.1.5.2/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/example_project/example_project/urls.py` & `django-materialized-view-0.1.5.2/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/example_project/manage.py` & `django-materialized-view-0.1.5.2/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/poetry.lock` & `django-materialized-view-0.1.5.2/poetry.lock`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/pyproject.toml` & `django-materialized-view-0.1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/setup.cfg` & `django-materialized-view-0.1.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/testproject/manage.py` & `django-materialized-view-0.1.5.2/testproject/manage.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/testproject/settings.py` & `django-materialized-view-0.1.5.2/testproject/settings.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/testproject/tests/management/commands/test_migrate_with_views.py` & `django-materialized-view-0.1.5.2/testproject/tests/management/commands/test_migrate_with_views.py`

 * *Files identical despite different names*

### Comparing `django-materialized-view-0.1.5.1/testproject/tests/test_base_mode_tests.py` & `django-materialized-view-0.1.5.2/testproject/tests/test_base_mode_tests.py`

 * *Files identical despite different names*

