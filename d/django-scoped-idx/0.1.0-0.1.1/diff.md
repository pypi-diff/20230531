# Comparing `tmp/django_scoped_idx-0.1.0.tar.gz` & `tmp/django_scoped_idx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_scoped_idx-0.1.0.tar", max compression
+gzip compressed data, was "django_scoped_idx-0.1.1.tar", max compression
```

## Comparing `django_scoped_idx-0.1.0.tar` & `django_scoped_idx-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-31 09:36:43.084939 django_scoped_idx-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 09:36:43.084939 django_scoped_idx-0.1.0/django_scoped_idx/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 09:37:59.914527 django_scoped_idx-0.1.0/django_scoped_idx/fields.py
--rw-r--r--   0        0        0      376 2023-05-31 09:42:47.848215 django_scoped_idx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 django_scoped_idx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-31 09:36:43.084939 django_scoped_idx-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 09:36:43.084939 django_scoped_idx-0.1.1/django_scoped_idx/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-31 10:06:58.883555 django_scoped_idx-0.1.1/django_scoped_idx/fields.py
+-rw-r--r--   0        0        0      376 2023-05-31 10:07:10.115503 django_scoped_idx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 django_scoped_idx-0.1.1/PKG-INFO
```

