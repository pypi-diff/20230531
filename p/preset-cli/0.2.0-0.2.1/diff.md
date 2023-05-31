# Comparing `tmp/preset-cli-0.2.0.tar.gz` & `tmp/preset-cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preset-cli-0.2.0.tar", last modified: Tue May 23 17:55:28 2023, max compression
+gzip compressed data, was "preset-cli-0.2.1.tar", last modified: Wed May 31 02:14:06 2023, max compression
```

## Comparing `preset-cli-0.2.0.tar` & `preset-cli-0.2.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.972757 preset-cli-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.976757 preset-cli-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 17:55:16.000000 preset-cli-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 17:55:16.000000 preset-cli-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-05-23 17:55:16.000000 preset-cli-0.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-05-23 17:55:16.000000 preset-cli-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 17:55:16.000000 preset-cli-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-23 17:55:16.000000 preset-cli-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    24095 2023-05-23 17:55:28.988757 preset-cli-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-05-23 17:55:16.000000 preset-cli-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 17:55:16.000000 preset-cli-0.2.0/dev-requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-23 17:55:16.000000 preset-cli-0.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.976757 preset-cli-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.976757 preset-cli-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.976757 preset-cli-0.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/images/export_dashboards.png
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-23 17:55:16.000000 preset-cli-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.972757 preset-cli-0.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/charts/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/charts/Total_count_134.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/dashboards/White_label_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/databases/Google_Sheets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.972757 preset-cli-0.2.0/examples/exports/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/datasets/Google_Sheets/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/datasets/Google_Sheets/country_cnt.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/examples/exports/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/functions/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 17:55:16.000000 preset-cli-0.2.0/examples/exports/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 17:55:16.000000 preset-cli-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 17:55:16.000000 preset-cli-0.2.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-23 17:55:16.000000 preset-cli-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-23 17:55:28.988757 preset-cli-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-23 17:55:16.000000 preset-cli-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.972757 preset-cli-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/clients/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/clients/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)    35266 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/clients/superset.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/api/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/src/preset_cli/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/exposures.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/cli/superset/sync/native/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 17:55:16.000000 preset-cli-0.2.0/src/preset_cli/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.980757 preset-cli-0.2.0/src/preset_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24095 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 17:55:28.000000 preset-cli-0.2.0/src/preset_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47038 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/clients/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/clients/preset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    87530 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/api/clients/superset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/jwt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/password_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/auth/preset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.984757 preset-cli-0.2.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/tests/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sql_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/tests/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/tests/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32583 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/databases_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/exposures_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/dbt/metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:28.988757 preset-cli-0.2.0/tests/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/cli/superset/sync/native/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-23 17:55:16.000000 preset-cli-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.751784 preset-cli-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.759784 preset-cli-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 02:13:53.000000 preset-cli-0.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-31 02:13:53.000000 preset-cli-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-05-31 02:13:53.000000 preset-cli-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 02:13:53.000000 preset-cli-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-31 02:13:53.000000 preset-cli-0.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    24095 2023-05-31 02:14:06.775785 preset-cli-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-05-31 02:13:53.000000 preset-cli-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 02:13:53.000000 preset-cli-0.2.1/dev-requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-31 02:13:53.000000 preset-cli-0.2.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.759784 preset-cli-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.759784 preset-cli-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/images/export_dashboards.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.751784 preset-cli-0.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/charts/Total_count_134.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/dashboards/White_label_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/databases/Google_Sheets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.751784 preset-cli-0.2.1/examples/exports/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/datasets/Google_Sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/datasets/Google_Sheets/country_cnt.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/functions/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-31 02:13:53.000000 preset-cli-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 02:13:53.000000 preset-cli-0.2.1/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-31 02:13:53.000000 preset-cli-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-31 02:14:06.779785 preset-cli-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 02:13:53.000000 preset-cli-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.755784 preset-cli-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/src/preset_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/src/preset_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/clients/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/clients/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35569 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/clients/superset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/exposures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/native/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/src/preset_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24095 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/tests/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47038 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/clients/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/clients/preset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90501 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/clients/superset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/jwt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/password_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/preset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sql_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32583 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/databases_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/exposures_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/native/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tox.ini
```

### Comparing `preset-cli-0.2.0/.coveragerc` & `preset-cli-0.2.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/.github/workflows/python-package-daily.yml` & `preset-cli-0.2.1/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/.github/workflows/python-package.yml` & `preset-cli-0.2.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/.github/workflows/python-publish.yml` & `preset-cli-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/.gitignore` & `preset-cli-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/.pre-commit-config.yaml` & `preset-cli-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/CHANGELOG.rst` & `preset-cli-0.2.1/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,77 @@
 =========
 Changelog
 =========
 
+Version 0.2.1 - 2023-05-30
+==========================
+
+- Fix for https://github.com/apache/superset/pull/24067 (`#211 <https://github.com/preset-io/backend-sdk/pull/211>`_).
+
 Version 0.2.0 - 2023-05-23
 ==========================
 
-- Column descriptions and labels are now synced from dbt models (`PR #72 <https://github.com/preset-io/backend-sdk/pull/72>`_, `PR #111 <https://github.com/preset-io/backend-sdk/pull/111>`_, `PR #195 <https://github.com/preset-io/backend-sdk/pull/195>`_ and `PR #197 <https://github.com/preset-io/backend-sdk/pull/197>`_).
-- CLI can now provision users directly to the team (doesn't require accepting the invitation) with the ``import-users`` command. The ``export-users`` command can now also be used with Preset Workspaces.  (`PR #74 <https://github.com/preset-io/backend-sdk/pull/74>`_, `PR #100 <https://github.com/preset-io/backend-sdk/pull/100>`_ and `PR #148 <https://github.com/preset-io/backend-sdk/pull/148>`_).
-- It's possible to export roles information using the ``export-roles`` command (`PR #75 <https://github.com/preset-io/backend-sdk/pull/75>`_ and `PR #161 <https://github.com/preset-io/backend-sdk/pull/161>`_). 
-- Exported roles information can be imported via the ``import-roles`` command (`PR #76 <https://github.com/preset-io/backend-sdk/pull/76>`_, `PR #167 <https://github.com/preset-io/backend-sdk/pull/167>`_ and `PR #179 <https://github.com/preset-io/backend-sdk/pull/179>`_).
-- Improved session object logic (`PR #77 <https://github.com/preset-io/backend-sdk/pull/77>`_). 
-- Improved export/import logic for owernship and role information (`PR #79 <https://github.com/preset-io/backend-sdk/pull/79>`_).
-- CLI can now add users to imported roles (`PR #81 <https://github.com/preset-io/backend-sdk/pull/81>`_).
-- A JWT token can now be passed for authentication (`PR #82 <https://github.com/preset-io/backend-sdk/pull/82>`_).
-- Added debug logging to API requests (`PR #83 <https://github.com/preset-io/backend-sdk/pull/83>_`).
-- CLI can now export specific asset types, using the ``--asset-type`` flag (`PR #84 <https://github.com/preset-io/backend-sdk/pull/84>`_).
-- CLI can now export specific assets only, using the ``--$asset_type-ids`` (for example ``--dashboard-ids``) flag (`PR #85 <https://github.com/preset-io/backend-sdk/pull/85>`_ and `PR #88 <https://github.com/preset-io/backend-sdk/pull/88>`_).
-- CLI can now authenticate to Superset (On Premises) without CSRF token (`PR #87 <https://github.com/preset-io/backend-sdk/pull/87>`_).
-- Workspace/Team prompt no longer happens in case ``--help`` was pased (`PR #89 <https://github.com/preset-io/backend-sdk/pull/89>`_).
-- Team Roles, Workspace Roles and DARs can now be synced to a Preset team based on a YAML file (`PR #90 <https://github.com/preset-io/backend-sdk/pull/90>`_).
-- Added ``--version`` command to display the installed version (`PR #91 <https://github.com/preset-io/backend-sdk/pull/91>`_).
-- Fixed parent/child node selection in dbt Core for proper graph selection (`PR #92 <https://github.com/preset-io/backend-sdk/pull/92>`_).
-- Improved logging for the dbt Client (`PR #94 <https://github.com/preset-io/backend-sdk/pull/94>`_).
-- CLI now can create datasets for different databases (for DB Engines that supports multiple databases like Snowflake, BigQuery, etc) (`PR #95 <https://github.com/preset-io/backend-sdk/pull/95>`_).
-- BQ connection can now successfully be created/updated from the ``profiles.yml`` information (`PR #96 <https://github.com/preset-io/backend-sdk/pull/96>`_).
-- Redshift connectons now get created with the ``redshift+psycopg2`` driver (`PR #97 <https://github.com/preset-io/backend-sdk/pull/97>`_).
-- YAML files outside of asset folders aren't imported in the native sync (`PR #99 <https://github.com/preset-io/backend-sdk/pull/99>`_).
-- Improved BQ DB detection (`PR #102 <https://github.com/preset-io/backend-sdk/pull/102>`_).
-- Reduced the maximum amount of files included in an export file (`PR #105 <https://github.com/preset-io/backend-sdk/pull/105>`_).
-- Workspaces can now be defined as environment variables (`PR #106 <https://github.com/preset-io/backend-sdk/pull/106>`_).
-- CLI can now create Snowflake connections authenticated via private key pair (`PR #108 <https://github.com/preset-io/backend-sdk/pull/108>`_).
-- Improved the ``--exclude`` filter for the dbt sync (`PR #109 <https://github.com/preset-io/backend-sdk/pull/109>`_).
-- Improved database connection logic (`PR #111 <https://github.com/preset-io/backend-sdk/pull/111>`_).
-- CLI can now create Snowflake connections authenticated with DUO MFA (`PR #112 <https://github.com/preset-io/backend-sdk/pull/112>`_).
-- dbt target definition now defaults to the ``profile.yml`` if not specified (`PR #114 <https://github.com/preset-io/backend-sdk/pull/114>`_).
-- The dbt sync can now be triggered using the ``dbt_project.yml`` file rather than the ``manifest.json`` (`PR #115 <https://github.com/preset-io/backend-sdk/pull/115>`_).
-- CLI now supports `None` as column type (`PR #116 <https://github.com/preset-io/backend-sdk/pull/116>`_).
-- Database connection is now tested before triggering the import (`PR #118 <https://github.com/preset-io/backend-sdk/pull/118>`_).
-- Added support for companion YAML templates (`PR #120 <https://github.com/preset-io/backend-sdk/pull/120>`_).
-- YAML rendering logic is now improved (`PR #121 <https://github.com/preset-io/backend-sdk/pull/121>`_ and `PR #205 <https://github.com/preset-io/backend-sdk/pull/205>`_).
-- DB connection password is no longer logged in case the connection fails (`PR #122 <https://github.com/preset-io/backend-sdk/pull/122>`_).
-- Import assets is now performed through the ``assets`` endpoint (`PR #124 <https://github.com/preset-io/backend-sdk/pull/124>`_).
-- Large imports can be performed with the ``--split`` flag to prevent timeouts (`PR #124 <https://github.com/preset-io/backend-sdk/pull/124>`_). It also creates a ``checkpoint`` in case it fails so the retry would ignore already imported assets (`PR #137 <https://github.com/preset-io/backend-sdk/pull/137>`_ and `PR #139 <https://github.com/preset-io/backend-sdk/pull/139>`_).
-- Preset Manager requests updated to use ``api.app.preset.io`` (`PR #127 <https://github.com/preset-io/backend-sdk/pull/127>`_).
-- CLI now prompts user for job information if not specified when triggering a sync from dbt Cloud (`PR #128 <https://github.com/preset-io/backend-sdk/pull/128>`_).
-- dbt exposures now includes assets that were created by manual datasets, based on the schema and table name (`PR #132 <https://github.com/preset-io/backend-sdk/pull/132>`_).
-- Added support for Python 3.11 (`PR #133 <https://github.com/preset-io/backend-sdk/pull/133>`_).
-- CLI now refreshes JWT token if needed (`PR #134 <https://github.com/preset-io/backend-sdk/pull/134>`_).
-- Import failures due to connection errors are automatically retried (`PR #135 <https://github.com/preset-io/backend-sdk/pull/135>`_).
-- Improved Get Resources logic (`PR #136 <https://github.com/preset-io/backend-sdk/pull/136>`_).
-- CLI no longer prompts user to enter the DB password in case the connection already exists (`PR #140 <https://github.com/preset-io/backend-sdk/pull/140>`_).
-- It's now possible to trigger a sync only for exposures back to dbt, using the ``--exposures-only`` flag (`PR #142 <https://github.com/preset-io/backend-sdk/pull/142>`_).
-- CLI can be used to list SCIM groups and membership with the ``list-group-membership`` command (`PR #143 <https://github.com/preset-io/backend-sdk/pull/143>`_).
-- The dbt profile name is now used to look for an existing DB connection in the Workspace, instead of the project name (`PR #151 <https://github.com/preset-io/backend-sdk/pull/151>`_).
-- Added support for dbt derived metrics (`PR #154 <https://github.com/preset-io/backend-sdk/pull/154>`_, `PR #160 <https://github.com/preset-io/backend-sdk/pull/160>`_, `PR #196 <https://github.com/preset-io/backend-sdk/pull/196>`_, `PR #198 <https://github.com/preset-io/backend-sdk/pull/198>`_ and `PR #199 <https://github.com/preset-io/backend-sdk/pull/199>`_).
-- Fixed column configuration issues after a dbt sync (`PR #156 <https://github.com/preset-io/backend-sdk/pull/156>`_ and `PR #165 <https://github.com/preset-io/backend-sdk/pull/165>`_).
-- Added support for dbt 1.3 (`PR #159 <https://github.com/preset-io/backend-sdk/pull/159>`_).
-- Improved the ``MetricSchema`` loading (`PR #159 <https://github.com/preset-io/backend-sdk/pull/159>`_).
-- Added support for Secondary Contributor Workspace Role (`PR #186 <https://github.com/preset-io/backend-sdk/pull/186>`_).
-- Use model table alias for dataset creation (`PR #192 <https://github.com/preset-io/backend-sdk/pull/192>`_).
-- The dbt sync now only updates the DB connection in case ``--import-db`` is passed. It's also possible to trigger a sync without this flag (`PR #193 <https://github.com/preset-io/backend-sdk/pull/193>`_ and `PR #200 <https://github.com/preset-io/backend-sdk/pull/200>`_).
-- Added support for specifying a certification payload for dbt syncs (`PR #203 <https://github.com/preset-io/backend-sdk/pull/203>`_).
-- dbt models can now be filtered using ``config`` options (`PR #204 <https://github.com/preset-io/backend-sdk/pull/204>`_).
-- It's now possible to disable Jinja syntax escaping during export, and Jinja syntax rendering during import (`PR #205 <https://github.com/preset-io/backend-sdk/pull/205>`_).
+- Column descriptions and labels are now synced from dbt models (`#72 <https://github.com/preset-io/backend-sdk/pull/72>`_, `#111 <https://github.com/preset-io/backend-sdk/pull/111>`_, `#195 <https://github.com/preset-io/backend-sdk/pull/195>`_ and `#197 <https://github.com/preset-io/backend-sdk/pull/197>`_).
+- CLI can now provision users directly to the team (doesn't require accepting the invitation) with the ``import-users`` command. The ``export-users`` command can now also be used with Preset Workspaces.  (`#74 <https://github.com/preset-io/backend-sdk/pull/74>`_, `#100 <https://github.com/preset-io/backend-sdk/pull/100>`_ and `#148 <https://github.com/preset-io/backend-sdk/pull/148>`_).
+- It's possible to export roles information using the ``export-roles`` command (`#75 <https://github.com/preset-io/backend-sdk/pull/75>`_ and `#161 <https://github.com/preset-io/backend-sdk/pull/161>`_). 
+- Exported roles information can be imported via the ``import-roles`` command (`#76 <https://github.com/preset-io/backend-sdk/pull/76>`_, `#167 <https://github.com/preset-io/backend-sdk/pull/167>`_ and `#179 <https://github.com/preset-io/backend-sdk/pull/179>`_).
+- Improved session object logic (`#77 <https://github.com/preset-io/backend-sdk/pull/77>`_). 
+- Improved export/import logic for owernship and role information (`#79 <https://github.com/preset-io/backend-sdk/pull/79>`_).
+- CLI can now add users to imported roles (`#81 <https://github.com/preset-io/backend-sdk/pull/81>`_).
+- A JWT token can now be passed for authentication (`#82 <https://github.com/preset-io/backend-sdk/pull/82>`_).
+- Added debug logging to API requests (`#83 <https://github.com/preset-io/backend-sdk/pull/83>_`).
+- CLI can now export specific asset types, using the ``--asset-type`` flag (`#84 <https://github.com/preset-io/backend-sdk/pull/84>`_).
+- CLI can now export specific assets only, using the ``--$asset_type-ids`` (for example ``--dashboard-ids``) flag (`#85 <https://github.com/preset-io/backend-sdk/pull/85>`_ and `#88 <https://github.com/preset-io/backend-sdk/pull/88>`_).
+- CLI can now authenticate to Superset (On Premises) without CSRF token (`#87 <https://github.com/preset-io/backend-sdk/pull/87>`_).
+- Workspace/Team prompt no longer happens in case ``--help`` was pased (`#89 <https://github.com/preset-io/backend-sdk/pull/89>`_).
+- Team Roles, Workspace Roles and DARs can now be synced to a Preset team based on a YAML file (`#90 <https://github.com/preset-io/backend-sdk/pull/90>`_).
+- Added ``--version`` command to display the installed version (`#91 <https://github.com/preset-io/backend-sdk/pull/91>`_).
+- Fixed parent/child node selection in dbt Core for proper graph selection (`#92 <https://github.com/preset-io/backend-sdk/pull/92>`_).
+- Improved logging for the dbt Client (`#94 <https://github.com/preset-io/backend-sdk/pull/94>`_).
+- CLI now can create datasets for different databases (for DB Engines that supports multiple databases like Snowflake, BigQuery, etc) (`#95 <https://github.com/preset-io/backend-sdk/pull/95>`_).
+- BQ connection can now successfully be created/updated from the ``profiles.yml`` information (`#96 <https://github.com/preset-io/backend-sdk/pull/96>`_).
+- Redshift connectons now get created with the ``redshift+psycopg2`` driver (`#97 <https://github.com/preset-io/backend-sdk/pull/97>`_).
+- YAML files outside of asset folders aren't imported in the native sync (`#99 <https://github.com/preset-io/backend-sdk/pull/99>`_).
+- Improved BQ DB detection (`#102 <https://github.com/preset-io/backend-sdk/pull/102>`_).
+- Reduced the maximum amount of files included in an export file (`#105 <https://github.com/preset-io/backend-sdk/pull/105>`_).
+- Workspaces can now be defined as environment variables (`#106 <https://github.com/preset-io/backend-sdk/pull/106>`_).
+- CLI can now create Snowflake connections authenticated via private key pair (`#108 <https://github.com/preset-io/backend-sdk/pull/108>`_).
+- Improved the ``--exclude`` filter for the dbt sync (`#109 <https://github.com/preset-io/backend-sdk/pull/109>`_).
+- Improved database connection logic (`#111 <https://github.com/preset-io/backend-sdk/pull/111>`_).
+- CLI can now create Snowflake connections authenticated with DUO MFA (`#112 <https://github.com/preset-io/backend-sdk/pull/112>`_).
+- dbt target definition now defaults to the ``profile.yml`` if not specified (`#114 <https://github.com/preset-io/backend-sdk/pull/114>`_).
+- The dbt sync can now be triggered using the ``dbt_project.yml`` file rather than the ``manifest.json`` (`#115 <https://github.com/preset-io/backend-sdk/pull/115>`_).
+- CLI now supports `None` as column type (`#116 <https://github.com/preset-io/backend-sdk/pull/116>`_).
+- Database connection is now tested before triggering the import (`#118 <https://github.com/preset-io/backend-sdk/pull/118>`_).
+- Added support for companion YAML templates (`#120 <https://github.com/preset-io/backend-sdk/pull/120>`_).
+- YAML rendering logic is now improved (`#121 <https://github.com/preset-io/backend-sdk/pull/121>`_ and `#205 <https://github.com/preset-io/backend-sdk/pull/205>`_).
+- DB connection password is no longer logged in case the connection fails (`#122 <https://github.com/preset-io/backend-sdk/pull/122>`_).
+- Import assets is now performed through the ``assets`` endpoint (`#124 <https://github.com/preset-io/backend-sdk/pull/124>`_).
+- Large imports can be performed with the ``--split`` flag to prevent timeouts (`#124 <https://github.com/preset-io/backend-sdk/pull/124>`_). It also creates a ``checkpoint`` in case it fails so the retry would ignore already imported assets (`#137 <https://github.com/preset-io/backend-sdk/pull/137>`_ and `#139 <https://github.com/preset-io/backend-sdk/pull/139>`_).
+- Preset Manager requests updated to use ``api.app.preset.io`` (`#127 <https://github.com/preset-io/backend-sdk/pull/127>`_).
+- CLI now prompts user for job information if not specified when triggering a sync from dbt Cloud (`#128 <https://github.com/preset-io/backend-sdk/pull/128>`_).
+- dbt exposures now includes assets that were created by manual datasets, based on the schema and table name (`#132 <https://github.com/preset-io/backend-sdk/pull/132>`_).
+- Added support for Python 3.11 (`#133 <https://github.com/preset-io/backend-sdk/pull/133>`_).
+- CLI now refreshes JWT token if needed (`#134 <https://github.com/preset-io/backend-sdk/pull/134>`_).
+- Import failures due to connection errors are automatically retried (`#135 <https://github.com/preset-io/backend-sdk/pull/135>`_).
+- Improved Get Resources logic (`#136 <https://github.com/preset-io/backend-sdk/pull/136>`_).
+- CLI no longer prompts user to enter the DB password in case the connection already exists (`#140 <https://github.com/preset-io/backend-sdk/pull/140>`_).
+- It's now possible to trigger a sync only for exposures back to dbt, using the ``--exposures-only`` flag (`#142 <https://github.com/preset-io/backend-sdk/pull/142>`_).
+- CLI can be used to list SCIM groups and membership with the ``list-group-membership`` command (`#143 <https://github.com/preset-io/backend-sdk/pull/143>`_).
+- The dbt profile name is now used to look for an existing DB connection in the Workspace, instead of the project name (`#151 <https://github.com/preset-io/backend-sdk/pull/151>`_).
+- Added support for dbt derived metrics (`#154 <https://github.com/preset-io/backend-sdk/pull/154>`_, `#160 <https://github.com/preset-io/backend-sdk/pull/160>`_, `#196 <https://github.com/preset-io/backend-sdk/pull/196>`_, `#198 <https://github.com/preset-io/backend-sdk/pull/198>`_ and `#199 <https://github.com/preset-io/backend-sdk/pull/199>`_).
+- Fixed column configuration issues after a dbt sync (`#156 <https://github.com/preset-io/backend-sdk/pull/156>`_ and `#165 <https://github.com/preset-io/backend-sdk/pull/165>`_).
+- Added support for dbt 1.3 (`#159 <https://github.com/preset-io/backend-sdk/pull/159>`_).
+- Improved the ``MetricSchema`` loading (`#159 <https://github.com/preset-io/backend-sdk/pull/159>`_).
+- Added support for Secondary Contributor Workspace Role (`#186 <https://github.com/preset-io/backend-sdk/pull/186>`_).
+- Use model table alias for dataset creation (`#192 <https://github.com/preset-io/backend-sdk/pull/192>`_).
+- The dbt sync now only updates the DB connection in case ``--import-db`` is passed. It's also possible to trigger a sync without this flag (`#193 <https://github.com/preset-io/backend-sdk/pull/193>`_ and `#200 <https://github.com/preset-io/backend-sdk/pull/200>`_).
+- Added support for specifying a certification payload for dbt syncs (`#203 <https://github.com/preset-io/backend-sdk/pull/203>`_).
+- dbt models can now be filtered using ``config`` options (`#204 <https://github.com/preset-io/backend-sdk/pull/204>`_).
+- It's now possible to disable Jinja syntax escaping during export, and Jinja syntax rendering during import (`#205 <https://github.com/preset-io/backend-sdk/pull/205>`_).
 
 Version 0.1.1 - 2022-09-13
 ==========================
 
 - File path is now passed to template as ``filepath`` in the ``sync native`` command.
 - CLI can now invite users to Preset from a YAML file created by ``export-users``.
 - Fix database update in the dbt sync.
```

### Comparing `preset-cli-0.2.0/CONTRIBUTING.rst` & `preset-cli-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/Makefile` & `preset-cli-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/PKG-INFO` & `preset-cli-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
```

### Comparing `preset-cli-0.2.0/README.rst` & `preset-cli-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/dev-requirements.txt` & `preset-cli-0.2.1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/docs/Makefile` & `preset-cli-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/docs/conf.py` & `preset-cli-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/docs/images/export_dashboards.png` & `preset-cli-0.2.1/docs/images/export_dashboards.png`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/docs/index.rst` & `preset-cli-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/examples/exports/charts/Total_count_134.yaml` & `preset-cli-0.2.1/examples/exports/charts/Total_count_134.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/examples/exports/dashboards/White_label_test.yaml` & `preset-cli-0.2.1/examples/exports/dashboards/White_label_test.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/examples/exports/datasets/Google_Sheets/country_cnt.yaml` & `preset-cli-0.2.1/examples/exports/datasets/Google_Sheets/country_cnt.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/requirements.txt` & `preset-cli-0.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/setup.cfg` & `preset-cli-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/setup.py` & `preset-cli-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/api/clients/dbt.py` & `preset-cli-0.2.1/src/preset_cli/api/clients/dbt.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/api/clients/preset.py` & `preset-cli-0.2.1/src/preset_cli/api/clients/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/api/clients/superset.py` & `preset-cli-0.2.1/src/preset_cli/api/clients/superset.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,15 +473,25 @@
 
         return resource
 
     def get_database(self, database_id: int) -> Any:
         """
         Return a single database.
         """
-        return self.get_resource("database", database_id)
+        database = self.get_resource("database", database_id)
+        if "sqlalchemy_uri" in database:
+            return database
+
+        url = self.baseurl / "api/v1/database" / str(database_id) / "connection"
+        response = self.session.get(url)
+        validate_response(response)
+
+        resource = response.json()["result"]
+
+        return resource
 
     def get_databases(self, **kwargs: str) -> List[Any]:
         """
         Return databases, possibly filtered.
         """
         return self.get_resources("database", **kwargs)
```

### Comparing `preset-cli-0.2.0/src/preset_cli/auth/jwt.py` & `preset-cli-0.2.1/src/preset_cli/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/auth/lib.py` & `preset-cli-0.2.1/src/preset_cli/auth/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/auth/main.py` & `preset-cli-0.2.1/src/preset_cli/auth/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/auth/password.py` & `preset-cli-0.2.1/src/preset_cli/auth/password.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/auth/preset.py` & `preset-cli-0.2.1/src/preset_cli/auth/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/main.py` & `preset-cli-0.2.1/src/preset_cli/cli/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/export.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/export.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/import_.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/import_.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/main.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/sql.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/sql.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/command.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/databases.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/databases.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/datasets.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/datasets.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/exposures.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/exposures.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/lib.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/dbt/metrics.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/metrics.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/cli/superset/sync/native/command.py` & `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/native/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/exceptions.py` & `preset-cli-0.2.1/src/preset_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli/lib.py` & `preset-cli-0.2.1/src/preset_cli/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli.egg-info/PKG-INFO` & `preset-cli-0.2.1/src/preset_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
```

### Comparing `preset-cli-0.2.0/src/preset_cli.egg-info/SOURCES.txt` & `preset-cli-0.2.1/src/preset_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/src/preset_cli.egg-info/requires.txt` & `preset-cli-0.2.1/src/preset_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/api/clients/dbt_test.py` & `preset-cli-0.2.1/tests/api/clients/dbt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/api/clients/preset_test.py` & `preset-cli-0.2.1/tests/api/clients/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/api/clients/superset_test.py` & `preset-cli-0.2.1/tests/api/clients/superset_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -885,15 +885,19 @@
 
 def test_get_database(mocker: MockerFixture) -> None:
     """
     Test the ``get_database`` method.
     """
     auth = Auth()
     client = SupersetClient("https://superset.example.org/", auth)
-    get_resource = mocker.patch.object(client, "get_resource")
+    get_resource = mocker.patch.object(
+        client,
+        "get_resource",
+        return_value={"sqlalchemy_uri": "preset://"},
+    )
 
     client.get_database(1)
     get_resource.assert_called_with("database", 1)
 
 
 def test_get_databases(mocker: MockerFixture) -> None:
     """
@@ -2953,7 +2957,88 @@
                 "is_dttm": False,
                 "column_name": "complex",
                 "groupby": True,
                 "type_generic": 1,
             },
         ],
     }
+
+
+def test_get_database_connection(requests_mock: Mocker) -> None:
+    """
+    Test that the client uses the new database endpoint for DB info.
+    """
+    requests_mock.get(
+        "https://superset.example.org/api/v1/database/1",
+        json={
+            "id": 1,
+            "result": {
+                "allow_ctas": False,
+                "allow_cvas": False,
+                "allow_dml": True,
+                "allow_file_upload": True,
+                "allow_run_async": False,
+                "backend": "preset",
+                "cache_timeout": None,
+                "configuration_method": "sqlalchemy_form",
+                "database_name": "File Uploads",
+                "driver": "apsw",
+                "engine_information": {
+                    "disable_ssh_tunneling": False,
+                    "supports_file_upload": True,
+                },
+                "expose_in_sqllab": True,
+                "force_ctas_schema": None,
+                "id": 1,
+                "impersonate_user": False,
+                "is_managed_externally": False,
+                "uuid": "d21c03ce-86ec-461f-ac82-0add92a8ee07",
+            },
+        },
+    )
+    requests_mock.get(
+        "https://superset.example.org/api/v1/database/1/connection",
+        json={
+            "id": 1,
+            "result": {
+                "allow_ctas": False,
+                "allow_cvas": False,
+                "allow_dml": True,
+                "allow_file_upload": True,
+                "allow_run_async": False,
+                "backend": "preset",
+                "cache_timeout": None,
+                "configuration_method": "sqlalchemy_form",
+                "database_name": "File Uploads",
+                "driver": "apsw",
+                "engine_information": {
+                    "disable_ssh_tunneling": False,
+                    "supports_file_upload": True,
+                },
+                "expose_in_sqllab": True,
+                "extra": json.dumps(
+                    {
+                        "allows_virtual_table_explore": True,
+                        "metadata_params": {},
+                        "engine_params": {},
+                        "schemas_allowed_for_file_upload": ["main"],
+                    },
+                ),
+                "force_ctas_schema": None,
+                "id": 1,
+                "impersonate_user": False,
+                "is_managed_externally": False,
+                "masked_encrypted_extra": None,
+                "parameters": {},
+                "parameters_schema": {},
+                "server_cert": None,
+                "sqlalchemy_uri": "preset://",
+                "uuid": "d21c03ce-86ec-461f-ac82-0add92a8ee07",
+            },
+        },
+    )
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+
+    response = client.get_database(1)
+    assert response["sqlalchemy_uri"] == "preset://"
```

### Comparing `preset-cli-0.2.0/tests/auth/jwt_test.py` & `preset-cli-0.2.1/tests/auth/jwt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/auth/lib_test.py` & `preset-cli-0.2.1/tests/auth/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/auth/main_test.py` & `preset-cli-0.2.1/tests/auth/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/auth/password_test.py` & `preset-cli-0.2.1/tests/auth/password_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/auth/preset_test.py` & `preset-cli-0.2.1/tests/auth/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/main_test.py` & `preset-cli-0.2.1/tests/cli/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/export_test.py` & `preset-cli-0.2.1/tests/cli/superset/export_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/import_test.py` & `preset-cli-0.2.1/tests/cli/superset/import_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/main_test.py` & `preset-cli-0.2.1/tests/cli/superset/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/sql_test.py` & `preset-cli-0.2.1/tests/cli/superset/sql_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/sync/dbt/command_test.py` & `preset-cli-0.2.1/tests/cli/superset/sync/dbt/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/sync/dbt/databases_test.py` & `preset-cli-0.2.1/tests/cli/superset/sync/dbt/databases_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/sync/dbt/datasets_test.py` & `preset-cli-0.2.1/tests/cli/superset/sync/dbt/datasets_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/sync/dbt/exposures_test.py` & `preset-cli-0.2.1/tests/cli/superset/sync/dbt/exposures_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/sync/dbt/lib_test.py` & `preset-cli-0.2.1/tests/cli/superset/sync/dbt/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/sync/dbt/manifest.json` & `preset-cli-0.2.1/tests/cli/superset/sync/dbt/manifest.json`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/sync/dbt/metrics_test.py` & `preset-cli-0.2.1/tests/cli/superset/sync/dbt/metrics_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/cli/superset/sync/native/command_test.py` & `preset-cli-0.2.1/tests/cli/superset/sync/native/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tests/lib_test.py` & `preset-cli-0.2.1/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.0/tox.ini` & `preset-cli-0.2.1/tox.ini`

 * *Files identical despite different names*

