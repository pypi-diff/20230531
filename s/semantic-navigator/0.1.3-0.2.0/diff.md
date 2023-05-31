# Comparing `tmp/semantic-navigator-0.1.3.tar.gz` & `tmp/semantic-navigator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic-navigator-0.1.3.tar", last modified: Tue May  9 20:44:05 2023, max compression
+gzip compressed data, was "semantic-navigator-0.2.0.tar", last modified: Wed May 31 04:44:51 2023, max compression
```

## Comparing `semantic-navigator-0.1.3.tar` & `semantic-navigator-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.674122 semantic-navigator-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.666122 semantic-navigator-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.666122 semantic-navigator-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.666122 semantic-navigator-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 20:44:05.674122 semantic-navigator-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.666122 semantic-navigator-0.1.3/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.666122 semantic-navigator-0.1.3/infra/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/infra/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/infra/.gcloudignore
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/infra/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/infra/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/infra/cors.json
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.670122 semantic-navigator-0.1.3/semantic_navigator/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.670122 semantic-navigator-0.1.3/semantic_navigator/app/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.670122 semantic-navigator-0.1.3/semantic_navigator/app/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/app/static/loader.css
--rw-r--r--   0 runner    (1001) docker     (123)   105911 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/app/static/protocol-components.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   324175 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/app/static/protocol-components.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    55695 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/app/static/protocol.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   179510 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/app/static/protocol.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.674122 semantic-navigator-0.1.3/semantic_navigator/app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/app/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/app/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/app/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.674122 semantic-navigator-0.1.3/semantic_navigator/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/bin/fetch_model_for_sem_nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/bin/semantic_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.674122 semantic-navigator-0.1.3/semantic_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.674122 semantic-navigator-0.1.3/semantic_navigator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/semantic_navigator/tests/test_empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:05.670122 semantic-navigator-0.1.3/semantic_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 20:44:05.000000 semantic-navigator-0.1.3/semantic_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 20:44:05.000000 semantic-navigator-0.1.3/semantic_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:44:05.000000 semantic-navigator-0.1.3/semantic_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 20:44:05.000000 semantic-navigator-0.1.3/semantic_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:44:05.000000 semantic-navigator-0.1.3/semantic_navigator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 20:44:05.000000 semantic-navigator-0.1.3/semantic_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 20:44:05.000000 semantic-navigator-0.1.3/semantic_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:44:05.674122 semantic-navigator-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 20:43:47.000000 semantic-navigator-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.623516 semantic-navigator-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.615516 semantic-navigator-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.615516 semantic-navigator-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.615516 semantic-navigator-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-31 04:44:51.623516 semantic-navigator-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    47347 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/active-learning-example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.619516 semantic-navigator-0.2.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.619516 semantic-navigator-0.2.0/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/infra/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/infra/.gcloudignore
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/infra/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/infra/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/infra/cors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.619516 semantic-navigator-0.2.0/semantic_navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.619516 semantic-navigator-0.2.0/semantic_navigator/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.619516 semantic-navigator-0.2.0/semantic_navigator/app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/static/loader.css
+-rw-r--r--   0 runner    (1001) docker     (123)   105911 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/static/protocol-components.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   324175 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/static/protocol-components.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    55695 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/static/protocol.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   179510 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/static/protocol.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.619516 semantic-navigator-0.2.0/semantic_navigator/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/templates/results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/templates/train.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.623516 semantic-navigator-0.2.0/semantic_navigator/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/bin/fetch_model_for_sem_nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/bin/semantic_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.623516 semantic-navigator-0.2.0/semantic_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/query_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.623516 semantic-navigator-0.2.0/semantic_navigator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/tests/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/semantic_navigator/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:44:51.619516 semantic-navigator-0.2.0/semantic_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-31 04:44:51.000000 semantic-navigator-0.2.0/semantic_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-31 04:44:51.000000 semantic-navigator-0.2.0/semantic_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:44:51.000000 semantic-navigator-0.2.0/semantic_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 04:44:51.000000 semantic-navigator-0.2.0/semantic_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:44:51.000000 semantic-navigator-0.2.0/semantic_navigator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-31 04:44:51.000000 semantic-navigator-0.2.0/semantic_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 04:44:51.000000 semantic-navigator-0.2.0/semantic_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 04:44:51.623516 semantic-navigator-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 04:44:29.000000 semantic-navigator-0.2.0/setup.py
```

### Comparing `semantic-navigator-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `semantic-navigator-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `semantic-navigator-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/.github/PULL_REQUEST_TEMPLATE.md` & `semantic-navigator-0.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/.github/workflows/ci.yml` & `semantic-navigator-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/.github/workflows/docs.yml` & `semantic-navigator-0.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/.gitignore` & `semantic-navigator-0.2.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -114,8 +114,11 @@
 
 # Project specific
 cdp-datasets/
 sem-nav-cdp-sea-small-processed-chunks/
 
 # Keys
 .keys/
-dataset.parquet
+dataset.parquet
+
+# Random generated files
+*.code-workspace
```

### Comparing `semantic-navigator-0.1.3/CODE_OF_CONDUCT.md` & `semantic-navigator-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/CONTRIBUTING.md` & `semantic-navigator-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/Justfile` & `semantic-navigator-0.2.0/Justfile`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/LICENSE` & `semantic-navigator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/PKG-INFO` & `semantic-navigator-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-navigator
-Version: 0.1.3
+Version: 0.2.0
 Summary: An active learning approach to query and search through large archival datasets.
 Author-email: Eva Maxfield Brown <evamxb@uw.edu>, Madeleine Grunde-McLaughlin <mgrunde@uw.edu>, Isabella Pestovski <pestoi@uw.edu>, Lanyi Zhu <lanyizhu@uw.edu>
 License: MPLv2.0
 Project-URL: Homepage, https://github.com/CouncilDataProject/semantic-navigator
 Project-URL: Bug Tracker, https://github.com/CouncilDataProject/semantic-navigator/issues
 Project-URL: Documentation, https://CouncilDataProject.github.io/semantic-navigator
 Project-URL: User Support, https://github.com/CouncilDataProject/semantic-navigator/issues
```

### Comparing `semantic-navigator-0.1.3/README.md` & `semantic-navigator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/docs/conf.py` & `semantic-navigator-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/docs/installation.rst` & `semantic-navigator-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/infra/Dockerfile` & `semantic-navigator-0.2.0/infra/Dockerfile`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/infra/Justfile` & `semantic-navigator-0.2.0/infra/Justfile`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/pyproject.toml` & `semantic-navigator-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
   "CODE_OF_CONDUCT.md",
   "CONTRIBUTING.md",
   "Justfile",
   ".cookiecutter.yaml",
   "*docs/**",
   "*notebooks/*",
   "*infra/*",
+  "active-learning-example.ipynb",
 ]
 
 [tool.mypy]
 files = "semantic_navigator/*.py"
 ignore_missing_imports = true
 disallow_untyped_defs = true
 check_untyped_defs = true
```

### Comparing `semantic-navigator-0.1.3/semantic_navigator/app/static/loader.css` & `semantic-navigator-0.2.0/semantic_navigator/app/static/loader.css`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/semantic_navigator/app/static/protocol-components.min.css` & `semantic-navigator-0.2.0/semantic_navigator/app/static/protocol-components.min.css`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/semantic_navigator/app/static/protocol-components.min.css.map` & `semantic-navigator-0.2.0/semantic_navigator/app/static/protocol-components.min.css.map`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/semantic_navigator/app/static/protocol.min.css` & `semantic-navigator-0.2.0/semantic_navigator/app/static/protocol.min.css`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/semantic_navigator/app/static/protocol.min.css.map` & `semantic-navigator-0.2.0/semantic_navigator/app/static/protocol.min.css.map`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/semantic_navigator/app/templates/index.html` & `semantic-navigator-0.2.0/semantic_navigator/app/templates/results.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,93 @@
 00000000: 7b25 2065 7874 656e 6473 2022 6261 7365  {% extends "base
 00000010: 2e68 746d 6c22 2025 7d0a 7b25 2062 6c6f  .html" %}.{% blo
-00000020: 636b 2063 6f6e 7465 6e74 2025 7d0a 3c73  ck content %}.<s
-00000030: 6563 7469 6f6e 2063 6c61 7373 3d22 6d7a  ection class="mz
-00000040: 702d 632d 6865 726f 2220 7374 796c 653d  p-c-hero" style=
-00000050: 226d 696e 2d68 6569 6768 743a 2038 3276  "min-height: 82v
-00000060: 683b 223e 0a20 2020 203c 6469 7620 636c  h;">.    <div cl
-00000070: 6173 733d 226d 7a70 2d6c 2d63 6f6e 7465  ass="mzp-l-conte
-00000080: 6e74 206d 7a70 2d74 2d63 6f6e 7465 6e74  nt mzp-t-content
-00000090: 2d6c 6722 3e0a 2020 2020 2020 2020 3c21  -lg">.        <!
-000000a0: 2d2d 2042 6173 6963 2069 6e74 726f 202d  -- Basic intro -
-000000b0: 2d3e 0a20 2020 2020 2020 203c 6831 2063  ->.        <h1 c
-000000c0: 6c61 7373 3d22 6d7a 702d 632d 6865 726f  lass="mzp-c-hero
-000000d0: 2d74 6974 6c65 223e 5365 6d61 6e74 6963  -title">Semantic
-000000e0: 204e 6176 6967 6174 6f72 3c2f 6831 3e0a   Navigator</h1>.
-000000f0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00000100: 7373 3d22 6d7a 702d 632d 6865 726f 2d62  ss="mzp-c-hero-b
-00000110: 6f64 7922 3e0a 2020 2020 2020 2020 2020  ody">.          
-00000120: 2020 3c64 6976 2063 6c61 7373 3d22 6d7a    <div class="mz
-00000130: 702d 632d 6865 726f 2d64 6573 6322 3e0a  p-c-hero-desc">.
-00000140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000150: 3c70 3e49 7465 7261 7469 7665 6c79 2072  <p>Iteratively r
-00000160: 6566 696e 6520 7365 6172 6368 2075 7369  efine search usi
-00000170: 6e67 2070 6f73 6974 6976 6520 616e 6420  ng positive and 
-00000180: 6e65 6761 7469 7665 2065 7861 6d70 6c65  negative example
-00000190: 732e 3c2f 703e 0a20 2020 2020 2020 2020  s.</p>.         
-000001a0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-000001b0: 2020 3c2f 6469 763e 0a0a 2020 2020 2020    </div>..      
-000001c0: 2020 3c21 2d2d 2053 6561 7263 6820 6261    <!-- Search ba
-000001d0: 7220 2d2d 3e0a 2020 2020 2020 2020 3c66  r -->.        <f
-000001e0: 6f72 6d3e 0a20 2020 2020 2020 2020 2020  orm>.           
-000001f0: 203c 6469 7620 636c 6173 733d 2269 6e70   <div class="inp
-00000200: 7574 2d67 726f 7570 223e 0a20 2020 2020  ut-group">.     
-00000210: 2020 2020 2020 2020 203c 696e 7075 740a           <input.
-00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000230: 7479 7065 3d22 7365 6172 6368 220a 2020  type="search".  
-00000240: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00000250: 6163 6568 6f6c 6465 723d 2253 6561 7263  aceholder="Searc
-00000260: 6820 666f 7220 6120 746f 7069 63e2 80a6  h for a topic...
-00000270: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
-00000280: 2020 203c 6275 7474 6f6e 2063 6c61 7373     <button class
-00000290: 3d22 6d7a 702d 632d 6275 7474 6f6e 2220  ="mzp-c-button" 
-000002a0: 7479 7065 3d22 6275 7474 6f6e 223e 5365  type="button">Se
-000002b0: 6172 6368 3c2f 6275 7474 6f6e 3e0a 2020  arch</button>.  
-000002c0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000002d0: 0a20 2020 2020 2020 203c 2f66 6f72 6d3e  .        </form>
-000002e0: 0a0a 2020 2020 2020 2020 3c21 2d2d 2056  ..        <!-- V
-000002f0: 6964 656f 2070 6c61 6365 686f 6c64 6572  ideo placeholder
-00000300: 202d 2d3e 0a20 2020 2020 2020 203c 6966   -->.        <if
-00000310: 7261 6d65 2077 6964 7468 3d22 3634 3022  rame width="640"
-00000320: 2068 6569 6768 743d 2233 3630 2220 0a20   height="360" . 
-00000330: 2020 2020 2020 2020 2020 2073 7263 3d22             src="
-00000340: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
-00000350: 7562 652e 636f 6d2f 656d 6265 642f 7a56  ube.com/embed/zV
-00000360: 5277 5548 6248 6774 3822 3e0a 2020 2020  RwUHbHgt8">.    
-00000370: 2020 2020 3c2f 6966 7261 6d65 3e0a 0a20      </iframe>.. 
-00000380: 2020 2020 2020 203c 212d 2d20 5261 6e64         <!-- Rand
-00000390: 6f6d 2074 6578 7420 7661 7269 6162 6c65  om text variable
-000003a0: 2066 696c 6c20 2d2d 3e0a 2020 2020 2020   fill -->.      
-000003b0: 2020 3c64 6976 2063 6c61 7373 3d22 6d7a    <div class="mz
-000003c0: 702d 632d 656d 7068 6173 6973 2d62 6f78  p-c-emphasis-box
-000003d0: 2220 7374 796c 653d 2274 6578 742d 616c  " style="text-al
-000003e0: 6967 6e3a 206c 6566 743b 6d61 7267 696e  ign: left;margin
-000003f0: 2d74 6f70 3a20 3130 7668 3b6d 6172 6769  -top: 10vh;margi
-00000400: 6e2d 626f 7474 6f6d 3a20 3130 7668 3b22  n-bottom: 10vh;"
-00000410: 3e0a 2020 2020 2020 2020 2020 2020 3c62  >.            <b
-00000420: 3e52 616e 646f 6d20 4578 616d 706c 6520  >Random Example 
-00000430: 5465 7874 3a3c 2f62 3e0a 2020 2020 2020  Text:</b>.      
-00000440: 2020 2020 2020 3c70 3e7b 7b20 6578 616d        <p>{{ exam
-00000450: 706c 655f 7261 6e64 6f6d 5f74 6578 7420  ple_random_text 
-00000460: 7d7d 3c2f 703e 0a20 2020 2020 2020 2020  }}</p>.         
-00000470: 2020 203c 703e 3c65 6d3e 7b7b 2065 7861     <p><em>{{ exa
-00000480: 6d70 6c65 5f72 616e 646f 6d5f 7465 7874  mple_random_text
-00000490: 5f70 6174 6820 7d7d 3c2f 656d 3e3c 2f70  _path }}</em></p
-000004a0: 3e0a 2020 2020 2020 2020 3c2f 6469 763e  >.        </div>
-000004b0: 0a20 2020 203c 2f64 6976 3e0a 3c2f 7365  .    </div>.</se
-000004c0: 6374 696f 6e3e 0a7b 2520 656e 6462 6c6f  ction>.{% endblo
-000004d0: 636b 2025 7d                             ck %}
+00000020: 636b 2063 6f6e 7465 6e74 2025 7d0a 0a3c  ck content %}..<
+00000030: 7365 6374 696f 6e20 636c 6173 733d 226d  section class="m
+00000040: 7a70 2d63 2d68 6572 6f22 2073 7479 6c65  zp-c-hero" style
+00000050: 3d22 6d69 6e2d 6865 6967 6874 3a20 3832  ="min-height: 82
+00000060: 7668 3b22 3e0a 0a20 2020 203c 6469 7620  vh;">..    <div 
+00000070: 636c 6173 733d 226d 7a70 2d6c 2d63 6f6e  class="mzp-l-con
+00000080: 7465 6e74 206d 7a70 2d74 2d63 6f6e 7465  tent mzp-t-conte
+00000090: 6e74 2d6c 6722 3e0a 2020 2020 2020 2020  nt-lg">.        
+000000a0: 3c68 3120 636c 6173 733d 226d 7a70 2d63  <h1 class="mzp-c
+000000b0: 2d68 6572 6f2d 7469 746c 6522 3e41 6c6c  -hero-title">All
+000000c0: 2052 6573 756c 7473 3c2f 6831 3e0a 2020   Results</h1>.  
+000000d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000000e0: 3d22 6d7a 702d 632d 6865 726f 2d62 6f64  ="mzp-c-hero-bod
+000000f0: 7922 203e 0a20 2020 2020 2020 2020 2020  y" >.           
+00000100: 203c 703e 5265 7375 6c74 7320 696e 636c   <p>Results incl
+00000110: 7564 6520 626f 7468 206c 6162 656c 6564  ude both labeled
+00000120: 2061 7320 2252 656c 6576 616e 7422 2061   as "Relevant" a
+00000130: 6e64 2070 7265 6469 6374 6564 2061 7320  nd predicted as 
+00000140: 2252 656c 6576 616e 7422 2e3c 2f70 3e0a  "Relevant".</p>.
+00000150: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
+00000160: 2020 2020 2020 2020 3c21 2d2d 2054 6578          <!-- Tex
+00000170: 7420 7361 6d70 6c65 7320 2d2d 3e0a 2020  t samples -->.  
+00000180: 2020 2020 2020 3c64 6976 2069 643d 2261        <div id="a
+00000190: 6e6e 6f74 6174 696f 6e2d 636f 6e74 6169  nnotation-contai
+000001a0: 6e65 7222 2063 6c61 7373 3d22 6d7a 702d  ner" class="mzp-
+000001b0: 6c2d 7369 6465 6261 722d 6c65 6674 223e  l-sidebar-left">
+000001c0: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+000001d0: 666f 7220 7465 7874 2069 6e20 7465 7874  for text in text
+000001e0: 735f 696e 666f 2025 7d0a 2020 2020 2020  s_info %}.      
+000001f0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000200: 6c61 7373 3d22 6d7a 702d 632d 656d 7068  lass="mzp-c-emph
+00000210: 6173 6973 2d62 6f78 2220 7374 796c 653d  asis-box" style=
+00000220: 2274 6578 742d 616c 6967 6e3a 206c 6566  "text-align: lef
+00000230: 743b 6d61 7267 696e 2d74 6f70 3a20 3130  t;margin-top: 10
+00000240: 7668 3b6d 6172 6769 6e2d 626f 7474 6f6d  vh;margin-bottom
+00000250: 3a20 3130 7668 3b22 3e0a 2020 2020 2020  : 10vh;">.      
+00000260: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000270: 6976 2073 7479 6c65 3d22 6469 7370 6c61  iv style="displa
+00000280: 793a 696e 6c69 6e65 2d62 6c6f 636b 223e  y:inline-block">
+00000290: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
+000002a0: 2020 2020 2020 2020 2020 203c 6834 3e7b             <h4>{
+000002b0: 7b20 7465 7874 5b22 6461 7465 225d 207d  { text["date"] }
+000002c0: 7d3c 2f68 343e 0a20 2020 2020 2020 2020  }</h4>.         
+000002d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000002e0: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+000002f0: 2020 2020 2020 2020 2020 2020 2020 6872                hr
+00000300: 6566 3d22 7b7b 2074 6578 745b 276c 696e  ef="{{ text['lin
+00000310: 6b27 5d20 7d7d 2222 0a20 2020 2020 2020  k'] }}"".       
+00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000330: 2020 2020 2074 6172 6765 743d 225f 626c       target="_bl
+00000340: 616e 6b22 0a20 2020 2020 2020 2020 2020  ank".           
+00000350: 2020 2020 2020 2020 2020 2020 203e 0a20               >. 
+00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000370: 2020 2020 2020 2020 2020 203c 6275 7474             <butt
+00000380: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003a0: 2020 2063 6c61 7373 3d22 6d7a 702d 632d     class="mzp-c-
+000003b0: 6275 7474 6f6e 206d 7a70 2d74 2d73 6d22  button mzp-t-sm"
+000003c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003e0: 2073 7479 6c65 3d22 6261 636b 6772 6f75   style="backgrou
+000003f0: 6e64 2d63 6f6c 6f72 3a20 2361 3663 6565  nd-color: #a6cee
+00000400: 333b 2062 6f72 6465 722d 636f 6c6f 723a  3; border-color:
+00000410: 2337 3139 3841 4322 0a20 2020 2020 2020  #7198AC".       
+00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000430: 2020 2020 203e 0a20 2020 2020 2020 2020       >.         
+00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000450: 2020 2020 2020 2056 6965 7720 6f6e 2043         View on C
+00000460: 4450 2045 7665 6e74 2050 6167 650a 2020  DP Event Page.  
+00000470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000480: 2020 2020 2020 2020 2020 3c2f 6275 7474            </butt
+00000490: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+000004a0: 2020 2020 2020 2020 2020 2020 3c2f 613e              </a>
+000004b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004c0: 2020 2020 203c 2f64 6976 3e20 200a 2020       </div>  .  
+000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004e0: 2020 3c62 723e 3c2f 6272 3e0a 2020 2020    <br></br>.    
+000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000500: 3c70 3e7b 7b20 7465 7874 5b22 7465 7874  <p>{{ text["text
+00000510: 225d 207d 7d3c 2f70 3e0a 2020 2020 2020  "] }}</p>.      
+00000520: 2020 2020 2020 2020 2020 2020 2020 3c65                <e
+00000530: 6d3e 5072 6564 6963 7465 6420 7072 6f62  m>Predicted prob
+00000540: 6162 696c 6974 793a 207b 7b20 7465 7874  ability: {{ text
+00000550: 5b22 7072 6f62 6122 5d20 7d7d 3c2f 656d  ["proba"] }}</em
+00000560: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000570: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000580: 2020 2020 207b 2520 656e 6466 6f72 2025       {% endfor %
+00000590: 7d0a 2020 2020 2020 2020 3c2f 6469 763e  }.        </div>
+000005a0: 0a20 2020 203c 2f64 6976 3e0a 3c2f 7365  .    </div>.</se
+000005b0: 6374 696f 6e3e 0a0a 7b25 2065 6e64 626c  ction>..{% endbl
+000005c0: 6f63 6b20 257d                           ock %}
```

### Comparing `semantic-navigator-0.1.3/semantic_navigator/bin/fetch_model_for_sem_nav.py` & `semantic-navigator-0.2.0/semantic_navigator/bin/fetch_model_for_sem_nav.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/semantic_navigator/bin/semantic_navigator.py` & `semantic-navigator-0.2.0/semantic_navigator/bin/semantic_navigator.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/semantic_navigator/data/__init__.py` & `semantic-navigator-0.2.0/semantic_navigator/data/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/semantic_navigator/tests/conftest.py` & `semantic-navigator-0.2.0/semantic_navigator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.3/semantic_navigator.egg-info/PKG-INFO` & `semantic-navigator-0.2.0/semantic_navigator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-navigator
-Version: 0.1.3
+Version: 0.2.0
 Summary: An active learning approach to query and search through large archival datasets.
 Author-email: Eva Maxfield Brown <evamxb@uw.edu>, Madeleine Grunde-McLaughlin <mgrunde@uw.edu>, Isabella Pestovski <pestoi@uw.edu>, Lanyi Zhu <lanyizhu@uw.edu>
 License: MPLv2.0
 Project-URL: Homepage, https://github.com/CouncilDataProject/semantic-navigator
 Project-URL: Bug Tracker, https://github.com/CouncilDataProject/semantic-navigator/issues
 Project-URL: Documentation, https://CouncilDataProject.github.io/semantic-navigator
 Project-URL: User Support, https://github.com/CouncilDataProject/semantic-navigator/issues
```

### Comparing `semantic-navigator-0.1.3/semantic_navigator.egg-info/SOURCES.txt` & `semantic-navigator-0.2.0/semantic_navigator.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .gitignore
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 Justfile
 LICENSE
 README.md
+active-learning-example.ipynb
 pyproject.toml
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/ci.yml
@@ -23,14 +24,16 @@
 infra/.gcloudignore
 infra/Dockerfile
 infra/Justfile
 infra/cors.json
 semantic_navigator/__init__.py
 semantic_navigator/constants.py
 semantic_navigator/py.typed
+semantic_navigator/query_embedding.py
+semantic_navigator/train.py
 semantic_navigator.egg-info/PKG-INFO
 semantic_navigator.egg-info/SOURCES.txt
 semantic_navigator.egg-info/dependency_links.txt
 semantic_navigator.egg-info/entry_points.txt
 semantic_navigator.egg-info/not-zip-safe
 semantic_navigator.egg-info/requires.txt
 semantic_navigator.egg-info/top_level.txt
@@ -39,13 +42,15 @@
 semantic_navigator/app/static/loader.css
 semantic_navigator/app/static/protocol-components.min.css
 semantic_navigator/app/static/protocol-components.min.css.map
 semantic_navigator/app/static/protocol.min.css
 semantic_navigator/app/static/protocol.min.css.map
 semantic_navigator/app/templates/base.html
 semantic_navigator/app/templates/index.html
+semantic_navigator/app/templates/results.html
+semantic_navigator/app/templates/train.html
 semantic_navigator/bin/__init__.py
 semantic_navigator/bin/fetch_model_for_sem_nav.py
 semantic_navigator/bin/semantic_navigator.py
 semantic_navigator/data/__init__.py
 semantic_navigator/tests/conftest.py
 semantic_navigator/tests/test_empty.py
```

