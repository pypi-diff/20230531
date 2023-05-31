# Comparing `tmp/django-minio-storage-0.5.4.tar.gz` & `tmp/django-minio-storage-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-minio-storage-0.5.4.tar", last modified: Sun May 21 14:48:33 2023, max compression
+gzip compressed data, was "django-minio-storage-0.5.5.tar", last modified: Wed May 31 06:43:33 2023, max compression
```

## Comparing `django-minio-storage-0.5.4.tar` & `django-minio-storage-0.5.5.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.892261 django-minio-storage-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.flake8rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.884261 django-minio-storage-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-21 14:48:33.892261 django-minio-storage-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/django_minio_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/django_minio_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/licences.md
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/minio_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/minio_storage/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/minio_storage/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/management/commands/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/minio_storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 14:48:33.000000 django-minio-storage-0.5.4/minio_storage/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-21 14:48:33.892261 django-minio-storage-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/tests/django_minio_storage_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/django_minio_storage_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/django_minio_storage_tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/django_minio_storage_tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/django_minio_storage_tests/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.888261 django-minio-storage-0.5.4/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:33.892261 django-minio-storage-0.5.4/tests/test_app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/bucket_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/custom_storage_class_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/managementcommand_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/retrieve_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/upload_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/test_app/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tests/watermelon-cat.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-21 14:48:24.000000 django-minio-storage-0.5.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.814151 django-minio-storage-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.806151 django-minio-storage-0.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.806151 django-minio-storage-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-31 06:43:33.814151 django-minio-storage-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.806151 django-minio-storage-0.5.5/django_minio_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/licences.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/minio_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/minio_storage/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/minio_storage/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/management/commands/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/minio_storage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 06:43:33.814151 django-minio-storage-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/tests/django_minio_storage_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/django_minio_storage_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/django_minio_storage_tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/django_minio_storage_tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/django_minio_storage_tests/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.814151 django-minio-storage-0.5.5/tests/test_app/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/bucket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/custom_storage_class_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/managementcommand_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/retrieve_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/settings_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/upload_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/watermelon-cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tox.ini
```

### Comparing `django-minio-storage-0.5.4/.github/workflows/release.yml` & `django-minio-storage-0.5.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/.github/workflows/tox.yml` & `django-minio-storage-0.5.5/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/CHANGELOG.md` & `django-minio-storage-0.5.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/LICENSE` & `django-minio-storage-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/LICENSE-APACHE` & `django-minio-storage-0.5.5/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/PKG-INFO` & `django-minio-storage-0.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.4
+Version: 0.5.5
 Summary: Django file storage using the minio python client
 Author-email: Thomas Frössman <thomasf@jossystem.se>, Tom Houlé <tom@kafunsho.be>
 Maintainer-email: Thomas Frössman <thomasf@jossystem.se>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 The django-minio-storage developers
```

### Comparing `django-minio-storage-0.5.4/README.md` & `django-minio-storage-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/django_minio_storage.egg-info/PKG-INFO` & `django-minio-storage-0.5.5/django_minio_storage.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.4
+Version: 0.5.5
 Summary: Django file storage using the minio python client
 Author-email: Thomas Frössman <thomasf@jossystem.se>, Tom Houlé <tom@kafunsho.be>
 Maintainer-email: Thomas Frössman <thomasf@jossystem.se>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 The django-minio-storage developers
```

### Comparing `django-minio-storage-0.5.4/django_minio_storage.egg-info/SOURCES.txt` & `django-minio-storage-0.5.5/django_minio_storage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 .editorconfig
-.flake8rc
 .gitignore
-.isort.cfg
 .readthedocs.yaml
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 LICENSE-APACHE
 README.md
 dev-requirements.txt
@@ -49,9 +47,10 @@
 tests/test_app/__init__.py
 tests/test_app/tests/__init__.py
 tests/test_app/tests/bucket_tests.py
 tests/test_app/tests/custom_storage_class_tests.py
 tests/test_app/tests/delete_tests.py
 tests/test_app/tests/managementcommand_tests.py
 tests/test_app/tests/retrieve_tests.py
+tests/test_app/tests/settings_tests.py
 tests/test_app/tests/upload_tests.py
 tests/test_app/tests/utils.py
```

### Comparing `django-minio-storage-0.5.4/docs/development.md` & `django-minio-storage-0.5.5/docs/development.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/docs/index.md` & `django-minio-storage-0.5.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/docs/licences.md` & `django-minio-storage-0.5.5/docs/licences.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/docs/usage.md` & `django-minio-storage-0.5.5/docs/usage.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 The following settings are available:
 
 - `MINIO_STORAGE_ENDPOINT`: the access URL for the service (for example
   `minio.example.org:9000` (note that there is no scheme)).
 
 - `MINIO_STORAGE_ACCESS_KEY` and `MINIO_STORAGE_SECRET_KEY` (mandatory)
+  
+- `MINIO_STORAGE_REGION`: Allows you to specify the region. By setting this configuration option, an additional HTTP request to Minio for region checking can be prevented, resulting in improved performance and reduced latency for generating presigned URLs.
 
 - `MINIO_STORAGE_USE_HTTPS`: whether to use TLS or not (default: `True`). This
   affect both how how Django internally communicates with the Minio server AND
   controls if the generated the storage object URLs uses `http://` or
   `https://` schemes.
 
 - `MINIO_STORAGE_MEDIA_BUCKET_NAME`: the bucket that will act as `MEDIA` folder
```

### Comparing `django-minio-storage-0.5.4/minio_storage/files.py` & `django-minio-storage-0.5.5/minio_storage/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 obj = self._storage.client.get_object(
                     self._storage.bucket_name, self.name
                 )
                 self._file = obj
                 return self._file
             except merr.InvalidResponseError as error:
                 logger.warn(error)
-                raise OSError(f"File {self.name} does not exist")
+                raise OSError(f"File {self.name} does not exist") from error
             finally:
                 try:
                     if obj:
                         obj.release_conn()
                 except Exception as e:
                     logger.error(str(e))
         return self._file
@@ -130,15 +130,15 @@
                     max_size=self.max_memory_size
                 )
                 for d in obj.stream(amt=1024 * 1024):
                     self._file.write(d)
                 self._file.seek(0)
                 return self._file
             except merr.InvalidResponseError as error:
-                raise minio_error(f"File {self.name} does not exist", error)
+                raise minio_error(f"File {self.name} does not exist", error) from error
             finally:
                 try:
                     if obj:
                         obj.release_conn()
                 except Exception as e:
                     logger.error(str(e))
         return self._file
```

### Comparing `django-minio-storage-0.5.4/minio_storage/management/commands/minio.py` & `django-minio-storage-0.5.5/minio_storage/management/commands/minio.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,16 +125,16 @@
         class_name = {
             "media": "minio_storage.storage.MinioMediaStorage",
             "static": "minio_storage.storage.MinioStaticStorage",
         }.get(options["class"], options["class"])
 
         try:
             storage_class = import_string(class_name)
-        except ImportError:
-            raise CommandError(f"could not find storage class: {class_name}")
+        except ImportError as err:
+            raise CommandError(f"could not find storage class: {class_name}") from err
         if not issubclass(storage_class, MinioStorage):
             raise CommandError(f"{class_name} is not an sub class of MinioStorage.")
 
         # TODO: maybe another way
         with patch.object(storage_class, "_init_check", return_value=None):
             storage = storage_class()  # type: ignore
             return storage
@@ -207,29 +207,29 @@
         return
 
     def bucket_delete(self, storage, bucket_name):
         try:
             storage.client.remove_bucket(bucket_name)
         except minio.error.S3Error as err:
             if err.code == "BucketNotEmpty":
-                raise CommandError(f"bucket {bucket_name} is not empty")
+                raise CommandError(f"bucket {bucket_name} is not empty") from err
             elif err.code == "NoSuchBucket":
-                raise CommandError(f"bucket {bucket_name} does not exist")
+                raise CommandError(f"bucket {bucket_name} does not exist") from err
 
     def policy_get(self, storage, bucket_name):
         try:
             policy = storage.client.get_bucket_policy(bucket_name)
             policy = json.loads(policy)
             policy = json.dumps(policy, ensure_ascii=False, indent=2)
             return policy
         except minio.error.S3Error as err:
             if err.code == "NoSuchBucket":
-                raise CommandError(f"bucket {bucket_name} does not exist")
+                raise CommandError(f"bucket {bucket_name} does not exist") from err
             elif err.code == "NoSuchBucketPolicy":
-                raise CommandError(f"bucket {bucket_name} has no policy")
+                raise CommandError(f"bucket {bucket_name} has no policy") from err
 
     def policy_set(self, storage, bucket_name, policy: Policy):
         try:
             policy = Policy(policy)
             storage.client.set_bucket_policy(bucket_name, policy.bucket(bucket_name))
         except minio.error.S3Error as e:
             raise CommandError(e.message) from e
```

### Comparing `django-minio-storage-0.5.4/minio_storage/policy.py` & `django-minio-storage-0.5.5/minio_storage/policy.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/minio_storage/storage.py` & `django-minio-storage-0.5.5/minio_storage/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         sane_name = self._sanitize_path(name)
         return (content_size, content_type, sane_name)
 
     def _open(self, name, mode="rb"):
         try:
             f = self.file_class(self._sanitize_path(name), mode, self)
         except merr.MinioException as e:
-            raise minio_error(f"File {name} could not be saved: {str(e)}", e)
+            raise minio_error(f"File {name} could not be saved: {str(e)}", e) from e
         return f
 
     def _save(self, name: str, content: T.BinaryIO) -> str:
         try:
             if hasattr(content, "seek") and callable(content.seek):
                 content.seek(0)
             content_size, content_type, sane_name = self._examine_file(name, content)
@@ -158,61 +158,63 @@
                 content,
                 content_size,
                 content_type,
                 metadata=self.object_metadata,
             )
             return sane_name
         except merr.InvalidResponseError as error:
-            raise minio_error(f"File {name} could not be saved", error)
+            raise minio_error(f"File {name} could not be saved", error) from error
 
     def delete(self, name: str) -> None:
         if self.backup_format and self.backup_bucket:
             try:
                 obj = self.client.get_object(self.bucket_name, name)
             except merr.InvalidResponseError as error:
                 raise minio_error(
                     "Could not obtain file {} " "to make a copy of it".format(name),
                     error,
-                )
+                ) from error
 
             try:
                 content_length = int(obj.getheader("Content-Length"))
             except ValueError as error:
-                raise minio_error(f"Could not backup removed file {name}", error)
+                raise minio_error(
+                    f"Could not backup removed file {name}", error
+                ) from error
 
             # Creates the backup filename
             target_name = "{}{}".format(
                 timezone.now().strftime(self.backup_format), name
             )
             try:
                 self.client.put_object(
                     self.backup_bucket, target_name, obj, content_length
                 )
             except merr.InvalidResponseError as error:
                 raise minio_error(
                     "Could not make a copy of file "
                     "{} before removing it".format(name),
                     error,
-                )
+                ) from error
 
         try:
             self.client.remove_object(self.bucket_name, name)
         except merr.InvalidResponseError as error:
-            raise minio_error(f"Could not remove file {name}", error)
+            raise minio_error(f"Could not remove file {name}", error) from error
 
     def exists(self, name: str) -> bool:
         try:
             self.client.stat_object(self.bucket_name, self._sanitize_path(name))
             return True
         except merr.InvalidResponseError as error:
             # TODO - deprecate
             if error._code == "NoSuchKey":
                 return False
             else:
-                raise minio_error(f"Could not stat file {name}", error)
+                raise minio_error(f"Could not stat file {name}", error) from error
         except merr.S3Error:
             return False
         except Exception as error:
             logger.error(error)
         return False
 
     def listdir(self, path: str) -> T.Tuple[T.List, T.List]:
@@ -240,22 +242,24 @@
                     dirs.append(p)
                 else:
                     files.append(p)
             return dirs, files
         except merr.S3Error:
             raise
         except merr.InvalidResponseError as error:
-            raise minio_error(f"Could not list directory {path}", error)
+            raise minio_error(f"Could not list directory {path}", error) from error
 
     def size(self, name: str) -> int:
         try:
             info: Object = self.client.stat_object(self.bucket_name, name)
             return info.size  # type: ignore
         except merr.InvalidResponseError as error:
-            raise minio_error(f"Could not access file size for {name}", error)
+            raise minio_error(
+                f"Could not access file size for {name}", error
+            ) from error
 
     def _presigned_url(
         self, name: str, max_age: T.Optional[datetime.timedelta] = None
     ) -> T.Optional[str]:
         kwargs = {}
         if max_age is not None:
             kwargs["expires"] = max_age
@@ -266,15 +270,15 @@
         if self.base_url is not None:
             url_parts = urlsplit(url)
             base_url_parts = urlsplit(self.base_url)
 
             # It's assumed that self.base_url will contain bucket information,
             # which could be different, so remove the bucket_name component (with 1
             # extra character for the leading "/") from the generated URL
-            url_key_path = url_parts.path[len(self.bucket_name) + 1 :]
+            url_key_path = url_parts.path[len(self.bucket_name) + 1 :]  # noqa: E203
 
             # Prefix the URL with any path content from base_url
             new_url_path = base_url_parts.path + url_key_path
 
             # Reconstruct the URL with an updated path
             url = urlunsplit(
                 (
@@ -304,15 +308,15 @@
 
             def strip_end(path):
                 while path.endswith("/"):
                     path = path[:-1]
                 return path
 
             if self.base_url is not None:
-                url = "{}/{}".format(strip_end(self.base_url), quote(strip_beg(name)))
+                url = f"{strip_end(self.base_url)}/{quote(strip_beg(name))}"
             else:
                 url = "{}/{}/{}".format(
                     strip_end(self.endpoint_url),
                     self.bucket_name,
                     quote(strip_beg(name)),
                 )
         if url:
@@ -339,15 +343,15 @@
         try:
             info: Object = self.client.stat_object(self.bucket_name, name)
             if info.last_modified:
                 return info.last_modified  # type: ignore
         except merr.InvalidResponseError as error:
             raise minio_error(
                 f"Could not access modification time for file {name}", error
-            )
+            ) from error
         raise OSError(f"Could not access modification time for file {name}")
 
 
 _NoValue = object()
 
 
 def get_setting(name: str, default=_NoValue) -> T.Any:
@@ -355,29 +359,36 @@
     if result is _NoValue:
         # print("Attr {} : {}".format(name, getattr(settings, name, default)))
         raise ImproperlyConfigured
     else:
         return result
 
 
-def create_minio_client_from_settings(*, minio_kwargs=dict()):
+def create_minio_client_from_settings(*, minio_kwargs=None):
+    kwargs = {}
     endpoint = get_setting("MINIO_STORAGE_ENDPOINT")
     access_key = get_setting("MINIO_STORAGE_ACCESS_KEY")
     secret_key = get_setting("MINIO_STORAGE_SECRET_KEY")
     secure = get_setting("MINIO_STORAGE_USE_HTTPS", True)
+    region = get_setting("MINIO_STORAGE_REGION", None)
+    if region:
+        kwargs["region"] = region
+
+    if minio_kwargs:
+        kwargs.update(minio_kwargs)
     # Making this client deconstructible allows it to be passed directly as
     # an argument to MinioStorage, since Django needs to be able to
     # deconstruct all Storage constructor arguments for Storages referenced in
     # migrations (e.g. when using a custom storage on a FileField).
     client = deconstructible(minio.Minio)(
         endpoint,
         access_key=access_key,
         secret_key=secret_key,
         secure=secure,
-        **minio_kwargs,
+        **kwargs,
     )
     return client
 
 
 @deconstructible
 class MinioMediaStorage(MinioStorage):
     def __init__(self):
```

### Comparing `django-minio-storage-0.5.4/tests/django_minio_storage_tests/settings.py` & `django-minio-storage-0.5.5/tests/django_minio_storage_tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/tests/django_minio_storage_tests/urls.py` & `django-minio-storage-0.5.5/tests/django_minio_storage_tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/tests/test_app/tests/bucket_tests.py` & `django-minio-storage-0.5.5/tests/test_app/tests/bucket_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/tests/test_app/tests/custom_storage_class_tests.py` & `django-minio-storage-0.5.5/tests/test_app/tests/custom_storage_class_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/tests/test_app/tests/delete_tests.py` & `django-minio-storage-0.5.5/tests/test_app/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/tests/test_app/tests/managementcommand_tests.py` & `django-minio-storage-0.5.5/tests/test_app/tests/managementcommand_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/tests/test_app/tests/retrieve_tests.py` & `django-minio-storage-0.5.5/tests/test_app/tests/retrieve_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         existent = self.media_storage.save("existent.txt", ContentFile(b"meh"))
         self.assertTrue(self.media_storage.exists(existent))
 
     def test_file_exists_failure(self):
         self.assertFalse(self.media_storage.exists("nonexistent.txt"))
 
     def test_reading_non_existing_file_raises_exception(self):
-        with self.assertRaises(Exception):
+        with self.assertRaises(S3Error):
             f = self.media_storage.open("this does not exist")
             f.read()
 
     def test_file_names_are_properly_sanitized(self):
         self.media_storage.save("./meh22222.txt", io.BytesIO(b"stuff"))
 
     def test_url_max_age(self):
```

### Comparing `django-minio-storage-0.5.4/tests/test_app/tests/upload_tests.py` & `django-minio-storage-0.5.5/tests/test_app/tests/upload_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/tests/test_app/tests/utils.py` & `django-minio-storage-0.5.5/tests/test_app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/tests/watermelon-cat.jpg` & `django-minio-storage-0.5.5/tests/watermelon-cat.jpg`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.4/tox.ini` & `django-minio-storage-0.5.5/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -61,29 +61,27 @@
 
 
 [testenv:lint]
 setenv=
     PYTHONWARNINGS=ignore
 basepython = python3
 deps =
-        flake8==4.0.1
-        isort==5.10.1
+        ruff==0.0.270
         black==22.3.0
 commands =
-        flake8 --config .flake8rc
-        isort --check --diff .
+        ruff check .
         black --check --diff .
 
 [testenv:fmt]
 setenv=
     PYTHONWARNINGS=ignore
 basepython = python3
 deps =
         pyupgrade-directories
-        flake8==6.0.0
+        ruff==0.0.270
         isort==5.12.0
         black==23.3.0
 commands =
         pyup_dirs --exit-zero-even-if-changed --py36-plus minio_storage tests
         isort .
         black .
```

