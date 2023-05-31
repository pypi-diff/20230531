# Comparing `tmp/h-vialib-1.1.0.tar.gz` & `tmp/h-vialib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h-vialib-1.1.0.tar", last modified: Wed Jan 11 09:00:30 2023, max compression
+gzip compressed data, was "h-vialib-1.2.0.tar", last modified: Wed May 31 11:27:28 2023, max compression
```

## Comparing `h-vialib-1.1.0.tar` & `h-vialib-1.2.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.294783 h-vialib-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/.cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-01-11 09:00:22.000000 h-vialib-1.1.0/.cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.286783 h-vialib-1.1.0/.cookiecutter/includes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/.cookiecutter/includes/README/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-11 09:00:22.000000 h-vialib-1.1.0/.cookiecutter/includes/README/head.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/.cookiecutter/includes/setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-11 09:00:22.000000 h-vialib-1.1.0/.cookiecutter/includes/setuptools/install_requires
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/.cookiecutter/includes/tox/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-11 09:00:22.000000 h-vialib-1.1.0/.cookiecutter/includes/tox/deps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-11 09:00:22.000000 h-vialib-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-01-11 09:00:22.000000 h-vialib-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-11 09:00:22.000000 h-vialib-1.1.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-11 09:00:22.000000 h-vialib-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-11 09:00:22.000000 h-vialib-1.1.0/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-11 09:00:22.000000 h-vialib-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-01-11 09:00:22.000000 h-vialib-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-01-11 09:00:30.294783 h-vialib-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-01-11 09:00:22.000000 h-vialib-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-01-11 09:00:22.000000 h-vialib-1.1.0/bin/make_python
--rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-01-11 09:00:22.000000 h-vialib-1.1.0/bin/make_template
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-01-11 09:00:22.000000 h-vialib-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-01-11 09:00:30.294783 h-vialib-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.286783 h-vialib-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/src/h_vialib/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/_flat_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/src/h_vialib/secure/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/secure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/secure/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/secure/expiry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/secure/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-01-11 09:00:22.000000 h-vialib-1.1.0/src/h_vialib/secure/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/src/h_vialib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-01-11 09:00:30.000000 h-vialib-1.1.0/src/h_vialib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-01-11 09:00:30.000000 h-vialib-1.1.0/src/h_vialib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 09:00:30.000000 h-vialib-1.1.0/src/h_vialib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-11 09:00:30.000000 h-vialib-1.1.0/src/h_vialib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-11 09:00:30.000000 h-vialib-1.1.0/src/h_vialib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/functional/sanity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.290783 h-vialib-1.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.294783 h-vialib-1.1.0/tests/unit/h_vialib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/_flat_dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/_params_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/configuration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:30.294783 h-vialib-1.1.0/tests/unit/h_vialib/secure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/secure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/secure/encryption_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/secure/expiry_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/secure/token_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tests/unit/h_vialib/secure/url_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-01-11 09:00:22.000000 h-vialib-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.757838 h-vialib-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/includes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/includes/README/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.cookiecutter/includes/README/head.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/includes/setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.cookiecutter/includes/setuptools/install_requires
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/includes/tox/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.cookiecutter/includes/tox/deps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-31 11:27:20.000000 h-vialib-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-31 11:27:20.000000 h-vialib-1.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-31 11:27:28.757838 h-vialib-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-31 11:27:20.000000 h-vialib-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-05-31 11:27:20.000000 h-vialib-1.2.0/bin/make_python
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-05-31 11:27:20.000000 h-vialib-1.2.0/bin/make_template
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-31 11:27:20.000000 h-vialib-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 11:27:28.757838 h-vialib-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/src/h_vialib/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/_flat_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/src/h_vialib/secure/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/expiry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/src/h_vialib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/functional/sanity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/tests/unit/h_vialib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/_flat_dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/_params_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/configuration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.757838 h-vialib-1.2.0/tests/unit/h_vialib/secure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/encryption_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/expiry_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/token_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/url_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tox.ini
```

### Comparing `h-vialib-1.1.0/.cookiecutter/cookiecutter.json` & `h-vialib-1.2.0/.cookiecutter/cookiecutter.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9882352941176471%*

 * *Differences: {"'extra_context'": "{'__copyright_year': '2022', 'pypi': 'yes'}"}*

```diff
@@ -1,21 +1,23 @@
 {
     "checkout": null,
     "directory": "pypackage",
     "extra_context": {
+        "__copyright_year": "2022",
         "__entry_point": "h-vialib",
         "__github_url": "https://github.com/hypothesis/h-vialib",
         "__pypi_url": "https://pypi.org/project/h-vialib",
         "console_script": "no",
         "copyright_holder": "Hypothesis",
         "dependabot_pip_interval": "monthly",
         "devdata": "no",
         "github_owner": "hypothesis",
         "name": "h-vialib",
         "package_name": "h_vialib",
+        "pypi": "yes",
         "python_versions": "3.9.13,3.8.13",
         "services": "no",
         "short_description": "Library functions for use with Via.",
         "slug": "h-vialib",
         "visibility": "public"
     },
     "ignore": [
```

### Comparing `h-vialib-1.1.0/.github/workflows/ci.yml` & `h-vialib-1.2.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 name: CI
 on:
   push:
+    paths-ignore:
+      - '.cookiecutter/*'
+      - '.github/dependabot.yml'
+      - 'bin/make_python'
+      - 'bin/make_template'
+      - 'docs/*'
+      - '**/.gitignore'
+      - '.python-version'
+      - 'LICENSE'
+      - '*.md'
   workflow_dispatch:
   workflow_call:
   schedule:
   - cron: '0 1 * * *'
 jobs:
   Format:
     runs-on: ubuntu-latest
```

### Comparing `h-vialib-1.1.0/LICENSE` & `h-vialib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/Makefile` & `h-vialib-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/PKG-INFO` & `h-vialib-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: h-vialib
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library functions for use with Via.
 Home-page: https://github.com/hypothesis/h-vialib
 Project-URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues
 Project-URL: Changelog, https://github.com/hypothesis/h-vialib/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<a href="https://github.com/hypothesis/h-vialib/actions/workflows/ci.yml?query=branch%3Amain"><img src="https://img.shields.io/github/workflow/status/hypothesis/h-vialib/CI/main"></a>
+<a href="https://github.com/hypothesis/h-vialib/actions/workflows/ci.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/ci.yml?branch=main"></a>
 <a href="https://pypi.org/project/h-vialib"><img src="https://img.shields.io/pypi/v/h-vialib"></a>
 <a><img src="https://img.shields.io/badge/python-3.9 | 3.8-success"></a>
 <a href="https://github.com/hypothesis/h-vialib/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-BSD--2--Clause-success"></a>
 <a href="https://github.com/hypothesis/cookiecutters/tree/main/pypackage"><img src="https://img.shields.io/badge/cookiecutter-pypackage-success"></a>
 <a href="https://black.readthedocs.io/en/stable/"><img src="https://img.shields.io/badge/code%20style-black-000000"></a>
 
 # h-vialib
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: h-vialib Version: 1.1.0 Summary: Library functions
+Metadata-Version: 2.1 Name: h-vialib Version: 1.2.0 Summary: Library functions
 for use with Via. Home-page: https://github.com/hypothesis/h-vialib Project-
 URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues Project-URL:
 Changelog, https://github.com/hypothesis/h-vialib/releases Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Intended Audience :: Developers Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [https://
-img.shields.io/github/workflow/status/hypothesis/h-vialib/CI/main] [https://
-img.shields.io/pypi/v/h-vialib] [https://img.shields.io/badge/python-3.9 | 3.8-
-success] [https://img.shields.io/badge/license-BSD--2--Clause-success] [https:/
-/img.shields.io/badge/cookiecutter-pypackage-success] [https://img.shields.io/
-badge/code%20style-black-000000] # h-vialib Library functions for use with Via.
-Usage ----- This is an internal library, mostly of interest to maintainers of
-[Via](https://github.com/hypothesis/via) and related components. Some items of
-interest: * [Configuration](https://github.com/hypothesis/h-vialib/blob/main/
-src/h_vialib/configuration.py) - Configuration parameter management ## Setting
-up Your h-vialib Development Environment First you'll need to install: * [Git]
-(https://git-scm.com/). On Ubuntu: `sudo apt install git`, on macOS: `brew
-install git`. * [GNU Make](https://www.gnu.org/software/make/). This is
-probably already installed, run `make --version` to check. * [pyenv](https://
-github.com/pyenv/pyenv). Follow the instructions in pyenv's README to install
-it. The **Homebrew** method works best on macOS. The **Basic GitHub Checkout**
-method works best on Ubuntu. You _don't_ need to set up pyenv's shell
-integration ("shims"), you can [use pyenv without shims](https://github.com/
-pyenv/pyenv#using-pyenv-without-shims). Then to set up your development
-environment: ```terminal git clone https://github.com/hypothesis/h-vialib.git
-cd h-vialib make help ``` ## Releasing a New Version of the Project 1. First,
-to get PyPI publishing working you need to go to:
+img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/
+ci.yml?branch=main] [https://img.shields.io/pypi/v/h-vialib] [https://
+img.shields.io/badge/python-3.9 | 3.8-success] [https://img.shields.io/badge/
+license-BSD--2--Clause-success] [https://img.shields.io/badge/cookiecutter-
+pypackage-success] [https://img.shields.io/badge/code%20style-black-000000] #
+h-vialib Library functions for use with Via. Usage ----- This is an internal
+library, mostly of interest to maintainers of [Via](https://github.com/
+hypothesis/via) and related components. Some items of interest: *
+[Configuration](https://github.com/hypothesis/h-vialib/blob/main/src/h_vialib/
+configuration.py) - Configuration parameter management ## Setting up Your h-
+vialib Development Environment First you'll need to install: * [Git](https://
+git-scm.com/). On Ubuntu: `sudo apt install git`, on macOS: `brew install git`.
+* [GNU Make](https://www.gnu.org/software/make/). This is probably already
+installed, run `make --version` to check. * [pyenv](https://github.com/pyenv/
+pyenv). Follow the instructions in pyenv's README to install it. The
+**Homebrew** method works best on macOS. The **Basic GitHub Checkout** method
+works best on Ubuntu. You _don't_ need to set up pyenv's shell integration
+("shims"), you can [use pyenv without shims](https://github.com/pyenv/
+pyenv#using-pyenv-without-shims). Then to set up your development environment:
+```terminal git clone https://github.com/hypothesis/h-vialib.git cd h-vialib
+make help ``` ## Releasing a New Version of the Project 1. First, to get PyPI
+publishing working you need to go to:
 github.com/organizations/hypothesis/settings/secrets/actions/PYPI_TOKEN> and
 add h-vialib to the `PYPI_TOKEN` secret's selected repositories. 2. Now that
 the h-vialib project has access to the `PYPI_TOKEN` secret you can release a
 new version by just [creating a new GitHub release](https://docs.github.com/en/
 repositories/releasing-projects-on-github/managing-releases-in-a-repository).
 Publishing a new GitHub release will automatically trigger [a GitHub Actions
 workflow](.github/workflows/pypi.yml) that will build the new version of your
```

### Comparing `h-vialib-1.1.0/README.md` & `h-vialib-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<a href="https://github.com/hypothesis/h-vialib/actions/workflows/ci.yml?query=branch%3Amain"><img src="https://img.shields.io/github/workflow/status/hypothesis/h-vialib/CI/main"></a>
+<a href="https://github.com/hypothesis/h-vialib/actions/workflows/ci.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/ci.yml?branch=main"></a>
 <a href="https://pypi.org/project/h-vialib"><img src="https://img.shields.io/pypi/v/h-vialib"></a>
 <a><img src="https://img.shields.io/badge/python-3.9 | 3.8-success"></a>
 <a href="https://github.com/hypothesis/h-vialib/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-BSD--2--Clause-success"></a>
 <a href="https://github.com/hypothesis/cookiecutters/tree/main/pypackage"><img src="https://img.shields.io/badge/cookiecutter-pypackage-success"></a>
 <a href="https://black.readthedocs.io/en/stable/"><img src="https://img.shields.io/badge/code%20style-black-000000"></a>
 
 # h-vialib
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-[https://img.shields.io/github/workflow/status/hypothesis/h-vialib/CI/main]
-[https://img.shields.io/pypi/v/h-vialib] [https://img.shields.io/badge/python-
-3.9 | 3.8-success] [https://img.shields.io/badge/license-BSD--2--Clause-
-success] [https://img.shields.io/badge/cookiecutter-pypackage-success] [https:/
-/img.shields.io/badge/code%20style-black-000000] # h-vialib Library functions
-for use with Via. Usage ----- This is an internal library, mostly of interest
-to maintainers of [Via](https://github.com/hypothesis/via) and related
-components. Some items of interest: * [Configuration](https://github.com/
-hypothesis/h-vialib/blob/main/src/h_vialib/configuration.py) - Configuration
-parameter management ## Setting up Your h-vialib Development Environment First
-you'll need to install: * [Git](https://git-scm.com/). On Ubuntu: `sudo apt
-install git`, on macOS: `brew install git`. * [GNU Make](https://www.gnu.org/
-software/make/). This is probably already installed, run `make --version` to
-check. * [pyenv](https://github.com/pyenv/pyenv). Follow the instructions in
-pyenv's README to install it. The **Homebrew** method works best on macOS. The
-**Basic GitHub Checkout** method works best on Ubuntu. You _don't_ need to set
-up pyenv's shell integration ("shims"), you can [use pyenv without shims]
-(https://github.com/pyenv/pyenv#using-pyenv-without-shims). Then to set up your
-development environment: ```terminal git clone https://github.com/hypothesis/h-
-vialib.git cd h-vialib make help ``` ## Releasing a New Version of the Project
-1. First, to get PyPI publishing working you need to go to:
+[https://img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/
+ci.yml?branch=main] [https://img.shields.io/pypi/v/h-vialib] [https://
+img.shields.io/badge/python-3.9 | 3.8-success] [https://img.shields.io/badge/
+license-BSD--2--Clause-success] [https://img.shields.io/badge/cookiecutter-
+pypackage-success] [https://img.shields.io/badge/code%20style-black-000000] #
+h-vialib Library functions for use with Via. Usage ----- This is an internal
+library, mostly of interest to maintainers of [Via](https://github.com/
+hypothesis/via) and related components. Some items of interest: *
+[Configuration](https://github.com/hypothesis/h-vialib/blob/main/src/h_vialib/
+configuration.py) - Configuration parameter management ## Setting up Your h-
+vialib Development Environment First you'll need to install: * [Git](https://
+git-scm.com/). On Ubuntu: `sudo apt install git`, on macOS: `brew install git`.
+* [GNU Make](https://www.gnu.org/software/make/). This is probably already
+installed, run `make --version` to check. * [pyenv](https://github.com/pyenv/
+pyenv). Follow the instructions in pyenv's README to install it. The
+**Homebrew** method works best on macOS. The **Basic GitHub Checkout** method
+works best on Ubuntu. You _don't_ need to set up pyenv's shell integration
+("shims"), you can [use pyenv without shims](https://github.com/pyenv/
+pyenv#using-pyenv-without-shims). Then to set up your development environment:
+```terminal git clone https://github.com/hypothesis/h-vialib.git cd h-vialib
+make help ``` ## Releasing a New Version of the Project 1. First, to get PyPI
+publishing working you need to go to:
 github.com/organizations/hypothesis/settings/secrets/actions/PYPI_TOKEN> and
 add h-vialib to the `PYPI_TOKEN` secret's selected repositories. 2. Now that
 the h-vialib project has access to the `PYPI_TOKEN` secret you can release a
 new version by just [creating a new GitHub release](https://docs.github.com/en/
 repositories/releasing-projects-on-github/managing-releases-in-a-repository).
 Publishing a new GitHub release will automatically trigger [a GitHub Actions
 workflow](.github/workflows/pypi.yml) that will build the new version of your
```

### Comparing `h-vialib-1.1.0/bin/make_python` & `h-vialib-1.2.0/bin/make_python`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/bin/make_template` & `h-vialib-1.2.0/bin/make_template`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/pyproject.toml` & `h-vialib-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 [tool.pytest.ini_options]
 addopts = "-q"
 filterwarnings = [
     "error", # Fail the tests if there are any warnings.
     "ignore:^find_module\\(\\) is deprecated and slated for removal in Python 3.12; use find_spec\\(\\) instead$:DeprecationWarning:importlib",
     "ignore:^FileFinder.find_loader\\(\\) is deprecated and slated for removal in Python 3.12; use find_spec\\(\\) instead$:DeprecationWarning:importlib",
+    "ignore:^pkg_resources is deprecated as an API:DeprecationWarning:pkg_resources",
+    "ignore:^Deprecated call to .pkg_resources\\.declare_namespace\\('.*'\\).\\.:DeprecationWarning:pkg_resources",
 ]
 
 [tool.pydocstyle]
 ignore = [
     # Missing docstrings.
     "D100","D101","D102","D103","D104","D105","D106","D107",
```

### Comparing `h-vialib-1.1.0/setup.cfg` & `h-vialib-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/src/h_vialib/_flat_dict.py` & `h-vialib-1.2.0/src/h_vialib/_flat_dict.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/src/h_vialib/_params.py` & `h-vialib-1.2.0/src/h_vialib/_params.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/src/h_vialib/client.py` & `h-vialib-1.2.0/src/h_vialib/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 """Helper classes for clients using Via proxying."""
 
 import re
+from enum import Enum
+from typing import Optional
 from urllib.parse import parse_qsl, urlencode, urlparse
 
 from webob.multidict import MultiDict
 
 from h_vialib.secure import Encryption, ViaSecureURL
 
 
+class ContentType(str, Enum):
+    PDF = "pdf"
+    HTML = "html"
+    VIDEO = "video"
+
+
 class ViaDoc:
     """A doc we want to proxy with content type."""
 
     _GOOGLE_DRIVE_REGEX = re.compile(
         r"^https://drive.google.com/uc\?id=(.*)&export=download$", re.IGNORECASE
     )
 
     def __init__(self, url, content_type=None):
         """Initialize a new doc with it's url and content_type if known."""
         self.url = url
 
         if content_type is None and self._GOOGLE_DRIVE_REGEX.match(url):
-            content_type = "pdf"
+            content_type = ContentType.PDF
 
-        self._content_type = content_type
-
-    @property
-    def is_html(self):
-        """Check if document is known to be a HTML."""
-        return self._content_type == "html"
-
-    @property
-    def is_pdf(self):
-        """Check if document is known to be a pdf."""
-        return self._content_type == "pdf"
+        self.content_type = content_type
 
 
 class ViaClient:  # pylint: disable=too-few-public-methods
     """A small wrapper to make calling Via easier."""
 
     def __init__(self, secret, service_url=None, html_service_url=None):
         """Initialize a ViaClient pointing to a `via_url` via server.
@@ -55,15 +53,20 @@
             "via.client.ignoreOtherConfiguration": "1",
             "via.client.openSidebar": "1",
             "via.external_link_mode": "new-tab",
         }
 
     # pylint:disable=too-many-arguments
     def url_for(
-        self, url, content_type=None, options=None, blocked_for=None, headers=None
+        self,
+        url,
+        content_type: Optional[ContentType] = None,
+        options=None,
+        blocked_for=None,
+        headers=None,
     ):
         """Generate a Via URL to display a given URL.
 
         If provided, the options will be merged with default Via options.
 
         :param url: URL to proxy thru Via
         :param content_type: content type, if known, of the document ("pdf"
@@ -84,28 +87,32 @@
 
         if headers:
             query["via.secret.headers"] = self._secure_secrets.encrypt_dict(headers)
 
         if blocked_for:
             query["via.blocked_for"] = blocked_for
 
-        if doc.is_html:
+        if doc.content_type == ContentType.HTML:
             # Optimisation to skip routing for documents we know are HTML
             via_url = self._url_for_html(doc.url, query)
         else:
             via_url = self._secure_url.create(self._url_for(doc, query))
 
         return via_url
 
     def _url_for(self, doc, query):
         if self._service_url is None:
             raise ValueError("Cannot rewrite URLs without a service URL")
 
-        # Optimisation to skip routing for documents we know are PDFs
-        path = "/pdf" if doc.is_pdf else "/route"
+        # Optimisation to skip routing for documents we know the type of
+        content_type_paths = {
+            ContentType.PDF: "/pdf",
+            ContentType.VIDEO: "/video",
+        }
+        path = content_type_paths.get(doc.content_type, "/route")
 
         query["url"] = doc.url
 
         return self._service_url._replace(path=path, query=urlencode(query)).geturl()
 
     def _url_for_html(self, url, query):
         if self._html_service_url is None:
```

### Comparing `h-vialib-1.1.0/src/h_vialib/configuration.py` & `h-vialib-1.2.0/src/h_vialib/configuration.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/src/h_vialib/secure/encryption.py` & `h-vialib-1.2.0/src/h_vialib/secure/encryption.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/src/h_vialib/secure/expiry.py` & `h-vialib-1.2.0/src/h_vialib/secure/expiry.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/src/h_vialib/secure/token.py` & `h-vialib-1.2.0/src/h_vialib/secure/token.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/src/h_vialib/secure/url.py` & `h-vialib-1.2.0/src/h_vialib/secure/url.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/src/h_vialib.egg-info/PKG-INFO` & `h-vialib-1.2.0/src/h_vialib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: h-vialib
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library functions for use with Via.
 Home-page: https://github.com/hypothesis/h-vialib
 Project-URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues
 Project-URL: Changelog, https://github.com/hypothesis/h-vialib/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<a href="https://github.com/hypothesis/h-vialib/actions/workflows/ci.yml?query=branch%3Amain"><img src="https://img.shields.io/github/workflow/status/hypothesis/h-vialib/CI/main"></a>
+<a href="https://github.com/hypothesis/h-vialib/actions/workflows/ci.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/ci.yml?branch=main"></a>
 <a href="https://pypi.org/project/h-vialib"><img src="https://img.shields.io/pypi/v/h-vialib"></a>
 <a><img src="https://img.shields.io/badge/python-3.9 | 3.8-success"></a>
 <a href="https://github.com/hypothesis/h-vialib/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-BSD--2--Clause-success"></a>
 <a href="https://github.com/hypothesis/cookiecutters/tree/main/pypackage"><img src="https://img.shields.io/badge/cookiecutter-pypackage-success"></a>
 <a href="https://black.readthedocs.io/en/stable/"><img src="https://img.shields.io/badge/code%20style-black-000000"></a>
 
 # h-vialib
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: h-vialib Version: 1.1.0 Summary: Library functions
+Metadata-Version: 2.1 Name: h-vialib Version: 1.2.0 Summary: Library functions
 for use with Via. Home-page: https://github.com/hypothesis/h-vialib Project-
 URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues Project-URL:
 Changelog, https://github.com/hypothesis/h-vialib/releases Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Intended Audience :: Developers Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [https://
-img.shields.io/github/workflow/status/hypothesis/h-vialib/CI/main] [https://
-img.shields.io/pypi/v/h-vialib] [https://img.shields.io/badge/python-3.9 | 3.8-
-success] [https://img.shields.io/badge/license-BSD--2--Clause-success] [https:/
-/img.shields.io/badge/cookiecutter-pypackage-success] [https://img.shields.io/
-badge/code%20style-black-000000] # h-vialib Library functions for use with Via.
-Usage ----- This is an internal library, mostly of interest to maintainers of
-[Via](https://github.com/hypothesis/via) and related components. Some items of
-interest: * [Configuration](https://github.com/hypothesis/h-vialib/blob/main/
-src/h_vialib/configuration.py) - Configuration parameter management ## Setting
-up Your h-vialib Development Environment First you'll need to install: * [Git]
-(https://git-scm.com/). On Ubuntu: `sudo apt install git`, on macOS: `brew
-install git`. * [GNU Make](https://www.gnu.org/software/make/). This is
-probably already installed, run `make --version` to check. * [pyenv](https://
-github.com/pyenv/pyenv). Follow the instructions in pyenv's README to install
-it. The **Homebrew** method works best on macOS. The **Basic GitHub Checkout**
-method works best on Ubuntu. You _don't_ need to set up pyenv's shell
-integration ("shims"), you can [use pyenv without shims](https://github.com/
-pyenv/pyenv#using-pyenv-without-shims). Then to set up your development
-environment: ```terminal git clone https://github.com/hypothesis/h-vialib.git
-cd h-vialib make help ``` ## Releasing a New Version of the Project 1. First,
-to get PyPI publishing working you need to go to:
+img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/
+ci.yml?branch=main] [https://img.shields.io/pypi/v/h-vialib] [https://
+img.shields.io/badge/python-3.9 | 3.8-success] [https://img.shields.io/badge/
+license-BSD--2--Clause-success] [https://img.shields.io/badge/cookiecutter-
+pypackage-success] [https://img.shields.io/badge/code%20style-black-000000] #
+h-vialib Library functions for use with Via. Usage ----- This is an internal
+library, mostly of interest to maintainers of [Via](https://github.com/
+hypothesis/via) and related components. Some items of interest: *
+[Configuration](https://github.com/hypothesis/h-vialib/blob/main/src/h_vialib/
+configuration.py) - Configuration parameter management ## Setting up Your h-
+vialib Development Environment First you'll need to install: * [Git](https://
+git-scm.com/). On Ubuntu: `sudo apt install git`, on macOS: `brew install git`.
+* [GNU Make](https://www.gnu.org/software/make/). This is probably already
+installed, run `make --version` to check. * [pyenv](https://github.com/pyenv/
+pyenv). Follow the instructions in pyenv's README to install it. The
+**Homebrew** method works best on macOS. The **Basic GitHub Checkout** method
+works best on Ubuntu. You _don't_ need to set up pyenv's shell integration
+("shims"), you can [use pyenv without shims](https://github.com/pyenv/
+pyenv#using-pyenv-without-shims). Then to set up your development environment:
+```terminal git clone https://github.com/hypothesis/h-vialib.git cd h-vialib
+make help ``` ## Releasing a New Version of the Project 1. First, to get PyPI
+publishing working you need to go to:
 github.com/organizations/hypothesis/settings/secrets/actions/PYPI_TOKEN> and
 add h-vialib to the `PYPI_TOKEN` secret's selected repositories. 2. Now that
 the h-vialib project has access to the `PYPI_TOKEN` secret you can release a
 new version by just [creating a new GitHub release](https://docs.github.com/en/
 repositories/releasing-projects-on-github/managing-releases-in-a-repository).
 Publishing a new GitHub release will automatically trigger [a GitHub Actions
 workflow](.github/workflows/pypi.yml) that will build the new version of your
```

### Comparing `h-vialib-1.1.0/src/h_vialib.egg-info/SOURCES.txt` & `h-vialib-1.2.0/src/h_vialib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/tests/pyproject.toml` & `h-vialib-1.2.0/tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/tests/unit/h_vialib/_params_test.py` & `h-vialib-1.2.0/tests/unit/h_vialib/_params_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/tests/unit/h_vialib/client_test.py` & `h-vialib-1.2.0/tests/unit/h_vialib/client_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,44 @@
 import pytest
 from h_matchers import Any
 
-from h_vialib import ViaClient, ViaDoc
+from h_vialib import ContentType, ViaClient, ViaDoc
 
 
 class TestViaDoc:
     @pytest.mark.parametrize(
-        "url,content_type,is_pdf",
+        "url,content_type,expected_content_type",
         (
-            ("http://example.com", None, False),
-            ("http://example.com", "html", False),
-            ("http://example.com", "pdf", True),
+            ("http://example.com", None, None),
+            ("http://example.com", ContentType.HTML, ContentType.HTML),
+            ("http://example.com", ContentType.PDF, ContentType.PDF),
             # We know about Google Drive links and assume them to be PDF
-            ("https://drive.google.com/uc?id=0&export=download", None, True),
+            ("https://drive.google.com/uc?id=0&export=download", None, ContentType.PDF),
         ),
     )
-    def test_is_pdf(self, url, content_type, is_pdf):
+    def test_content_type(self, url, content_type, expected_content_type):
         doc = ViaDoc(url, content_type)
 
-        assert doc.is_pdf == is_pdf
-
-    @pytest.mark.parametrize(
-        "url,content_type,is_html",
-        (
-            ("http://example.com", None, False),
-            ("http://example.com", "pdf", False),
-            ("http://example.com", "html", True),
-        ),
-    )
-    def test_is_htmlf(self, url, content_type, is_html):
-        doc = ViaDoc(url, content_type)
-
-        assert doc.is_html == is_html
+        assert doc.content_type == expected_content_type
 
 
 class TestViaClient:
     VIA_URL = "http://via.localhost"
     VIAHTML_URL = "http://viahtml.localhost"
     ORIGIN_URL = "http://random.localhost"
 
     DEFAULT_VALUES = {
         "via.client.ignoreOtherConfiguration": "1",
         "via.client.openSidebar": "1",
         "via.external_link_mode": "new-tab",
     }
 
-    @pytest.mark.parametrize("content_type,path", ((None, "/route"), ("pdf", "/pdf")))
+    @pytest.mark.parametrize(
+        "content_type,path", ((None, "/route"), ("pdf", "/pdf"), ("video", "/video"))
+    )
     def test_url_for(self, client, content_type, path):
         url = "http://example.com&a=1&a=2"
 
         final_url = client.url_for(url, content_type)
 
         expected_query = dict(self.DEFAULT_VALUES)
         expected_query["url"] = url
```

### Comparing `h-vialib-1.1.0/tests/unit/h_vialib/configuration_test.py` & `h-vialib-1.2.0/tests/unit/h_vialib/configuration_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/tests/unit/h_vialib/secure/encryption_test.py` & `h-vialib-1.2.0/tests/unit/h_vialib/secure/encryption_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/tests/unit/h_vialib/secure/expiry_test.py` & `h-vialib-1.2.0/tests/unit/h_vialib/secure/expiry_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/tests/unit/h_vialib/secure/token_test.py` & `h-vialib-1.2.0/tests/unit/h_vialib/secure/token_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/tests/unit/h_vialib/secure/url_test.py` & `h-vialib-1.2.0/tests/unit/h_vialib/secure/url_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.1.0/tox.ini` & `h-vialib-1.2.0/tox.ini`

 * *Files identical despite different names*

