# Comparing `tmp/django-virtual-models-0.1.5.tar.gz` & `tmp/django-virtual-models-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-virtual-models-0.1.5.tar", last modified: Mon May 29 19:31:39 2023, max compression
+gzip compressed data, was "django-virtual-models-0.1.6.tar", last modified: Wed May 31 20:55:05 2023, max compression
```

## Comparing `django-virtual-models-0.1.5.tar` & `django-virtual-models-0.1.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      503 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/.editorconfig
--rw-r--r--   0        0        0      165 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/.flake8
--rw-r--r--   0        0        0      234 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1848 2023-05-29 18:52:15.951093 django-virtual-models-0.1.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      978 2022-10-07 13:44:00.199208 django-virtual-models-0.1.5/.gitignore
--rw-r--r--   0        0        0     1352 2023-05-29 19:02:03.370944 django-virtual-models-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      287 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/AUTHORS.rst
--rw-r--r--   0        0        0      812 2023-05-29 19:24:01.679040 django-virtual-models-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0     5498 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3078 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1106 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/LICENSE
--rw-r--r--   0        0        0      287 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/MANIFEST.in
--rw-r--r--   0        0        0     6773 2022-10-20 23:29:19.957112 django-virtual-models-0.1.5/README.md
--rw-r--r--   0        0        0      365 2023-05-29 19:30:51.461765 django-virtual-models-0.1.5/django_virtual_models/__init__.py
--rw-r--r--   0        0        0      348 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/exceptions.py
--rw-r--r--   0        0        0    12337 2022-10-20 22:59:22.312626 django-virtual-models-0.1.5/django_virtual_models/fields.py
--rw-r--r--   0        0        0     1878 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/generic_views.py
--rw-r--r--   0        0        0        0 2022-10-11 23:33:37.024666 django-virtual-models-0.1.5/django_virtual_models/prefetch/__init__.py
--rw-r--r--   0        0        0      123 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/prefetch/exceptions.py
--rw-r--r--   0        0        0     4260 2022-10-11 23:37:09.682064 django-virtual-models-0.1.5/django_virtual_models/prefetch/hints.py
--rw-r--r--   0        0        0    19443 2022-10-20 22:25:31.135032 django-virtual-models-0.1.5/django_virtual_models/prefetch/serializer_optimization.py
--rw-r--r--   0        0        0       21 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/query_capture/__init__.py
--rw-r--r--   0        0        0     4463 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/query_capture/capture.py
--rw-r--r--   0        0        0     6027 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/query_capture/utils.py
--rw-r--r--   0        0        0     3628 2022-10-07 14:23:37.974878 django-virtual-models-0.1.5/django_virtual_models/serializers.py
--rw-r--r--   0        0        0     2586 2022-10-07 14:23:37.974878 django-virtual-models-0.1.5/django_virtual_models/utils.py
-lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/CHANGELOG.md -> ../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/LICENSE.md -> ../LICENSE
-lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/README.md -> ../README.md
--rw-r--r--   0        0        0     1992 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/img/4d-black.svg
--rw-r--r--   0        0        0     2656 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/img/4d-small.svg
--rw-r--r--   0        0        0     2004 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/img/4d-white.svg
--rw-r--r--   0        0        0     4286 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/img/favicon.ico
--rw-r--r--   0        0        0      537 2022-10-07 18:25:46.429082 django-virtual-models-0.1.5/docs/installation.md
--rw-r--r--   0        0        0    24190 2022-10-20 23:07:33.598593 django-virtual-models-0.1.5/docs/tutorial.md
--rw-r--r--   0        0        0      732 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/README.md
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/example/__init__.py
--rw-r--r--   0        0        0     3149 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/example/settings.py
--rw-r--r--   0        0        0      192 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/example/urls.py
--rw-r--r--   0        0        0      168 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/example/wsgi.py
--rwxr-xr-x   0        0        0      663 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/manage.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/__init__.py
--rw-r--r--   0        0        0      226 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/admin.py
--rw-r--r--   0        0        0      144 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/apps.py
--rw-r--r--   0        0        0     1574 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/fixtures/movies_initial.yaml
--rw-r--r--   0        0        0     2465 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/migrations/__init__.py
--rw-r--r--   0        0        0     1056 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/models.py
--rw-r--r--   0        0        0      796 2022-10-18 18:40:58.786984 django-virtual-models-0.1.5/example/movies/serializers.py
--rw-r--r--   0        0        0      149 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/urls.py
--rw-r--r--   0        0        0      234 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/views.py
--rw-r--r--   0        0        0      690 2022-10-20 23:06:37.427302 django-virtual-models-0.1.5/example/movies/virtual_models.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/tests/__init__.py
--rw-r--r--   0        0        0      865 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/tests/conftest.py
--rw-r--r--   0        0        0     2100 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/tests/test_views.py
--rw-r--r--   0        0        0      906 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/mkdocs.yml
--rwxr-xr-x   0        0        0     3698 2023-05-29 19:30:21.230066 django-virtual-models-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      773 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/optimization/__init__.py
--rw-r--r--   0        0        0    19025 2022-11-09 14:10:13.043069 django-virtual-models-0.1.5/tests/optimization/test_exceptions.py
--rw-r--r--   0        0        0    16704 2022-11-09 14:10:13.043069 django-virtual-models-0.1.5/tests/optimization/test_lookup_finder.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/query_capture/__init__.py
--rw-r--r--   0        0        0      896 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/query_capture/test_capture.py
--rw-r--r--   0        0        0      634 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/query_capture/test_utils.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/views/__init__.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/virtual_models/__init__.py
--rw-r--r--   0        0        0     1658 2023-05-15 19:48:28.523655 django-virtual-models-0.1.5/tests/virtual_models/db_utils.py
--rw-r--r--   0        0        0     7845 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/virtual_models/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/virtual_models/migrations/__init__.py
--rw-r--r--   0        0        0     4626 2022-11-09 14:10:13.043069 django-virtual-models-0.1.5/tests/virtual_models/models.py
--rw-r--r--   0        0        0     3436 2023-05-15 19:48:28.523655 django-virtual-models-0.1.5/tests/virtual_models/test_db_utils.py
--rw-r--r--   0        0        0     3757 2022-10-20 23:14:21.424762 django-virtual-models-0.1.5/tests/virtual_models/test_exceptions.py
--rw-r--r--   0        0        0      847 2022-10-07 13:42:04.430893 django-virtual-models-0.1.5/tests/virtual_models/test_utils.py
--rw-r--r--   0        0        0    17310 2022-10-20 23:10:23.647569 django-virtual-models-0.1.5/tests/virtual_models/test_virtual_models.py
--rw-r--r--   0        0        0     8710 1970-01-01 00:00:00.000000 django-virtual-models-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      503 2022-10-07 13:42:04.422893 django-virtual-models-0.1.6/.editorconfig
+-rw-r--r--   0        0        0      165 2022-10-07 13:42:04.422893 django-virtual-models-0.1.6/.flake8
+-rw-r--r--   0        0        0      234 2022-10-07 13:42:04.422893 django-virtual-models-0.1.6/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1848 2023-05-29 18:52:15.951093 django-virtual-models-0.1.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      978 2022-10-07 13:44:00.199208 django-virtual-models-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1352 2023-05-29 19:02:03.370944 django-virtual-models-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      287 2022-10-07 13:42:04.422893 django-virtual-models-0.1.6/AUTHORS.rst
+-rw-r--r--   0        0        0      931 2023-05-31 20:54:12.002515 django-virtual-models-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0     5498 2022-10-07 13:42:04.422893 django-virtual-models-0.1.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3078 2022-10-07 13:42:04.422893 django-virtual-models-0.1.6/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1106 2022-10-07 13:42:04.422893 django-virtual-models-0.1.6/LICENSE
+-rw-r--r--   0        0        0      287 2022-10-07 13:42:04.422893 django-virtual-models-0.1.6/MANIFEST.in
+-rw-r--r--   0        0        0     6773 2022-10-20 23:29:19.957112 django-virtual-models-0.1.6/README.md
+-rw-r--r--   0        0        0      365 2023-05-31 20:54:18.366305 django-virtual-models-0.1.6/django_virtual_models/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-30 20:05:03.403830 django-virtual-models-0.1.6/django_virtual_models/exceptions.py
+-rw-r--r--   0        0        0    12459 2023-05-31 17:34:16.758168 django-virtual-models-0.1.6/django_virtual_models/fields.py
+-rw-r--r--   0        0        0     1878 2022-10-07 14:23:37.970878 django-virtual-models-0.1.6/django_virtual_models/generic_views.py
+-rw-r--r--   0        0        0        0 2022-10-11 23:33:37.024666 django-virtual-models-0.1.6/django_virtual_models/prefetch/__init__.py
+-rw-r--r--   0        0        0      123 2022-10-07 14:23:37.970878 django-virtual-models-0.1.6/django_virtual_models/prefetch/exceptions.py
+-rw-r--r--   0        0        0     4260 2023-05-31 12:51:53.875261 django-virtual-models-0.1.6/django_virtual_models/prefetch/hints.py
+-rw-r--r--   0        0        0    19443 2023-05-31 12:51:53.875261 django-virtual-models-0.1.6/django_virtual_models/prefetch/serializer_optimization.py
+-rw-r--r--   0        0        0       21 2022-10-07 14:23:37.970878 django-virtual-models-0.1.6/django_virtual_models/query_capture/__init__.py
+-rw-r--r--   0        0        0     4463 2022-10-07 14:23:37.970878 django-virtual-models-0.1.6/django_virtual_models/query_capture/capture.py
+-rw-r--r--   0        0        0     6027 2022-10-07 14:23:37.970878 django-virtual-models-0.1.6/django_virtual_models/query_capture/utils.py
+-rw-r--r--   0        0        0     3628 2022-10-07 14:23:37.974878 django-virtual-models-0.1.6/django_virtual_models/serializers.py
+-rw-r--r--   0        0        0     2586 2022-10-07 14:23:37.974878 django-virtual-models-0.1.6/django_virtual_models/utils.py
+lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/docs/CHANGELOG.md -> ../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/docs/LICENSE.md -> ../LICENSE
+lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/docs/README.md -> ../README.md
+-rw-r--r--   0        0        0     1992 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/docs/img/4d-black.svg
+-rw-r--r--   0        0        0     2656 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/docs/img/4d-small.svg
+-rw-r--r--   0        0        0     2004 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/docs/img/4d-white.svg
+-rw-r--r--   0        0        0     4286 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/docs/img/favicon.ico
+-rw-r--r--   0        0        0      537 2022-10-07 18:25:46.429082 django-virtual-models-0.1.6/docs/installation.md
+-rw-r--r--   0        0        0    24190 2022-10-20 23:07:33.598593 django-virtual-models-0.1.6/docs/tutorial.md
+-rw-r--r--   0        0        0      732 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/README.md
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/example/__init__.py
+-rw-r--r--   0        0        0     3149 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/example/settings.py
+-rw-r--r--   0        0        0      192 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/example/urls.py
+-rw-r--r--   0        0        0      168 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/example/wsgi.py
+-rwxr-xr-x   0        0        0      663 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/manage.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/movies/__init__.py
+-rw-r--r--   0        0        0      226 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/movies/admin.py
+-rw-r--r--   0        0        0      144 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/movies/apps.py
+-rw-r--r--   0        0        0     1574 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/movies/fixtures/movies_initial.yaml
+-rw-r--r--   0        0        0     2465 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/movies/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/movies/migrations/__init__.py
+-rw-r--r--   0        0        0     1056 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/movies/models.py
+-rw-r--r--   0        0        0      796 2022-10-18 18:40:58.786984 django-virtual-models-0.1.6/example/movies/serializers.py
+-rw-r--r--   0        0        0      149 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/movies/urls.py
+-rw-r--r--   0        0        0      234 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/movies/views.py
+-rw-r--r--   0        0        0      690 2022-10-20 23:06:37.427302 django-virtual-models-0.1.6/example/movies/virtual_models.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/tests/__init__.py
+-rw-r--r--   0        0        0      865 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/tests/conftest.py
+-rw-r--r--   0        0        0     2100 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/example/tests/test_views.py
+-rw-r--r--   0        0        0      906 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/mkdocs.yml
+-rwxr-xr-x   0        0        0     3698 2023-05-29 19:30:21.230066 django-virtual-models-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0      773 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/optimization/__init__.py
+-rw-r--r--   0        0        0    19025 2022-11-09 14:10:13.043069 django-virtual-models-0.1.6/tests/optimization/test_exceptions.py
+-rw-r--r--   0        0        0    16704 2022-11-09 14:10:13.043069 django-virtual-models-0.1.6/tests/optimization/test_lookup_finder.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/query_capture/__init__.py
+-rw-r--r--   0        0        0      896 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/query_capture/test_capture.py
+-rw-r--r--   0        0        0      634 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/query_capture/test_utils.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/views/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/virtual_models/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-15 19:48:28.523655 django-virtual-models-0.1.6/tests/virtual_models/db_utils.py
+-rw-r--r--   0        0        0     7845 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/virtual_models/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.6/tests/virtual_models/migrations/__init__.py
+-rw-r--r--   0        0        0     4626 2022-11-09 14:10:13.043069 django-virtual-models-0.1.6/tests/virtual_models/models.py
+-rw-r--r--   0        0        0     3436 2023-05-15 19:48:28.523655 django-virtual-models-0.1.6/tests/virtual_models/test_db_utils.py
+-rw-r--r--   0        0        0     3757 2023-05-30 20:05:03.403830 django-virtual-models-0.1.6/tests/virtual_models/test_exceptions.py
+-rw-r--r--   0        0        0      847 2022-10-07 13:42:04.430893 django-virtual-models-0.1.6/tests/virtual_models/test_utils.py
+-rw-r--r--   0        0        0    17310 2022-10-20 23:10:23.647569 django-virtual-models-0.1.6/tests/virtual_models/test_virtual_models.py
+-rw-r--r--   0        0        0     8710 1970-01-01 00:00:00.000000 django-virtual-models-0.1.6/PKG-INFO
```

### Comparing `django-virtual-models-0.1.5/.github/workflows/tests.yml` & `django-virtual-models-0.1.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/.gitignore` & `django-virtual-models-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/.pre-commit-config.yaml` & `django-virtual-models-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/CHANGELOG.md` & `django-virtual-models-0.1.6/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.1.6]
+
+- Fix support for custom manager in VirtualModel
+- Separate method for _build_prefetch to allow overrides
+
 ## [0.1.5]
 
 - More robust `is_preloaded` check
 - Add Django 4.2 to tests.
 
 ## [0.1.4]
```

### Comparing `django-virtual-models-0.1.5/CODE_OF_CONDUCT.md` & `django-virtual-models-0.1.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/CONTRIBUTING.rst` & `django-virtual-models-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/LICENSE` & `django-virtual-models-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/README.md` & `django-virtual-models-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/django_virtual_models/fields.py` & `django-virtual-models-0.1.6/django_virtual_models/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -196,16 +196,20 @@
 
         if manager is None and (not hasattr(self.Meta, "model") or self.Meta.model is None):
             raise InvalidVirtualModelParams("Always provide a `manager` or `Meta.model`")
         if to_attr is not None and lookup is None:
             raise InvalidVirtualModelParams("Always provide a `lookup` when providing a `to_attr`")
 
         self.user = user
-        self.manager = manager or self.Meta.model._default_manager
-        self.model_cls = self.Meta.model or manager.model
+        if manager is None:
+            self.manager = self.Meta.model._default_manager
+            self.model_cls = self.Meta.model
+        else:
+            self.manager = manager
+            self.model_cls = manager.model
         self.lookup = lookup
         self.to_attr = to_attr  # can be `None`, but will receive `field_name` in `bind()`
         self.extra_kwargs = kwargs
 
     def get_fields(self) -> Dict[str, BaseVirtualField]:
         """
         Returns a dictionary of {field_name: field_instance}.
@@ -281,14 +285,20 @@
                 lookup_list=f_lookup_list,
                 user=user,
                 **kwargs,
             )
 
         return new_qs
 
+    def _build_prefetch(self, prefetch_queryset: QuerySet):
+        if self.lookup:
+            return Prefetch(self.lookup, queryset=prefetch_queryset, to_attr=self.to_attr)
+        else:
+            return Prefetch(self.field_name, queryset=prefetch_queryset)
+
     def hydrate_queryset(
         self,
         qs: QuerySet,
         lookup_list: List[str],
         user: Optional[Model] = None,
         **kwargs: Any,
     ) -> QuerySet:
@@ -317,23 +327,17 @@
         # defer fields on prefetch_queryset
         prefetch_queryset = _defer_fields(
             qs=prefetch_queryset,
             lookup_list=new_lookup_list,
             deferred_fields=self.deferred_fields,
         )
 
-        # build prefetch with lookups
-        if self.lookup:
-            prefetch = Prefetch(self.lookup, queryset=prefetch_queryset, to_attr=self.to_attr)
-        else:
-            prefetch = Prefetch(self.field_name, queryset=prefetch_queryset)
-
+        # build prefetch object, call prefetch_related
+        prefetch = self._build_prefetch(prefetch_queryset)
         new_qs = qs.prefetch_related(prefetch)
-        # prefeches don't need lookup
-        # (but their internal qs need, see prefetch_queryset above)
         return new_qs
 
     def get_optimized_queryset(
         self,
         qs: QuerySet,
         lookup_list: List[str],
         **kwargs: Any,
```

### Comparing `django-virtual-models-0.1.5/django_virtual_models/generic_views.py` & `django-virtual-models-0.1.6/django_virtual_models/generic_views.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/django_virtual_models/prefetch/hints.py` & `django-virtual-models-0.1.6/django_virtual_models/prefetch/hints.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/django_virtual_models/prefetch/serializer_optimization.py` & `django-virtual-models-0.1.6/django_virtual_models/prefetch/serializer_optimization.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/django_virtual_models/query_capture/capture.py` & `django-virtual-models-0.1.6/django_virtual_models/query_capture/capture.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/django_virtual_models/query_capture/utils.py` & `django-virtual-models-0.1.6/django_virtual_models/query_capture/utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/django_virtual_models/serializers.py` & `django-virtual-models-0.1.6/django_virtual_models/serializers.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/django_virtual_models/utils.py` & `django-virtual-models-0.1.6/django_virtual_models/utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/docs/img/4d-black.svg` & `django-virtual-models-0.1.6/docs/img/4d-black.svg`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/docs/img/4d-small.svg` & `django-virtual-models-0.1.6/docs/img/4d-small.svg`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/docs/img/4d-white.svg` & `django-virtual-models-0.1.6/docs/img/4d-white.svg`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/docs/img/favicon.ico` & `django-virtual-models-0.1.6/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/docs/installation.md` & `django-virtual-models-0.1.6/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/docs/tutorial.md` & `django-virtual-models-0.1.6/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/README.md` & `django-virtual-models-0.1.6/example/README.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/example/settings.py` & `django-virtual-models-0.1.6/example/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/manage.py` & `django-virtual-models-0.1.6/example/manage.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/movies/fixtures/movies_initial.yaml` & `django-virtual-models-0.1.6/example/movies/fixtures/movies_initial.yaml`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/movies/migrations/0001_initial.py` & `django-virtual-models-0.1.6/example/movies/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/movies/models.py` & `django-virtual-models-0.1.6/example/movies/models.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/movies/serializers.py` & `django-virtual-models-0.1.6/example/movies/serializers.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/movies/virtual_models.py` & `django-virtual-models-0.1.6/example/movies/virtual_models.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/tests/conftest.py` & `django-virtual-models-0.1.6/example/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/example/tests/test_views.py` & `django-virtual-models-0.1.6/example/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/mkdocs.yml` & `django-virtual-models-0.1.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/pyproject.toml` & `django-virtual-models-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/conftest.py` & `django-virtual-models-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/optimization/test_exceptions.py` & `django-virtual-models-0.1.6/tests/optimization/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/optimization/test_lookup_finder.py` & `django-virtual-models-0.1.6/tests/optimization/test_lookup_finder.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/query_capture/test_capture.py` & `django-virtual-models-0.1.6/tests/query_capture/test_capture.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/query_capture/test_utils.py` & `django-virtual-models-0.1.6/tests/query_capture/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/virtual_models/db_utils.py` & `django-virtual-models-0.1.6/tests/virtual_models/db_utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/virtual_models/migrations/0001_initial.py` & `django-virtual-models-0.1.6/tests/virtual_models/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/virtual_models/models.py` & `django-virtual-models-0.1.6/tests/virtual_models/models.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/virtual_models/test_db_utils.py` & `django-virtual-models-0.1.6/tests/virtual_models/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/virtual_models/test_exceptions.py` & `django-virtual-models-0.1.6/tests/virtual_models/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/virtual_models/test_utils.py` & `django-virtual-models-0.1.6/tests/virtual_models/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/tests/virtual_models/test_virtual_models.py` & `django-virtual-models-0.1.6/tests/virtual_models/test_virtual_models.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.5/PKG-INFO` & `django-virtual-models-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-virtual-models
-Version: 0.1.5
+Version: 0.1.6
 Summary: Improve performance and maintainability with a prefetching layer in your Django / Django REST Framework project
 Keywords: django,prefetch,performance,optimization
 Author-email: "Flávio Juvenal (Vinta Software)" <flavio@vinta.com.br>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

