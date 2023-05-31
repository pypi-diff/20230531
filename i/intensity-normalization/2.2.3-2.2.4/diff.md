# Comparing `tmp/intensity_normalization-2.2.3.tar.gz` & `tmp/intensity_normalization-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intensity_normalization-2.2.3.tar", last modified: Tue Mar 15 16:29:46 2022, max compression
+gzip compressed data, was "intensity_normalization-2.2.4.tar", last modified: Wed May 31 21:10:38 2023, max compression
```

## Comparing `intensity_normalization-2.2.3.tar` & `intensity_normalization-2.2.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.819909 intensity_normalization-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3545 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13411 2022-03-15 16:29:46.819909 intensity_normalization-2.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.815909 intensity_normalization-2.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.807909 intensity_normalization-2.2.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.815909 intensity_normalization-2.2.3/docs/_static/imgs/
--rw-r--r--   0 runner    (1001) docker     (121)   405830 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/_static/imgs/intnorm_illustration.png
--rw-r--r--   0 runner    (1001) docker     (121)    10941 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/algorithm.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     5471 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/intensity_normalization.cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/intensity_normalization.normalize.rst
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/intensity_normalization.plot.rst
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/intensity_normalization.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/intensity_normalization.util.rst
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10424 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.815909 intensity_normalization-2.2.3/intensity_normalization/
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8738 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/base_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.819909 intensity_normalization-2.2.3/intensity_normalization/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/coregister.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/fcm.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/kde.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/lsq.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/nyul.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/ravel.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/tissue_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/whitestripe.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/cli/zscore.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.819909 intensity_normalization-2.2.3/intensity_normalization/normalize/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/normalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14292 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/normalize/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7910 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/normalize/fcm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/normalize/kde.py
--rw-r--r--   0 runner    (1001) docker     (121)    12181 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/normalize/lsq.py
--rw-r--r--   0 runner    (1001) docker     (121)     9665 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/normalize/nyul.py
--rw-r--r--   0 runner    (1001) docker     (121)    16344 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/normalize/ravel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/normalize/whitestripe.py
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/normalize/zscore.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.819909 intensity_normalization-2.2.3/intensity_normalization/plot/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8131 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/plot/histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    13535 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.819909 intensity_normalization-2.2.3/intensity_normalization/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8365 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/util/coregister.py
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/util/histogram_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     4427 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/util/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     9088 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/util/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/intensity_normalization/util/tissue_membership.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.815909 intensity_normalization-2.2.3/intensity_normalization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13411 2022-03-15 16:29:46.000000 intensity_normalization-2.2.3/intensity_normalization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-03-15 16:29:46.000000 intensity_normalization-2.2.3/intensity_normalization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 16:29:46.000000 intensity_normalization-2.2.3/intensity_normalization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-03-15 16:29:46.000000 intensity_normalization-2.2.3/intensity_normalization.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 16:29:45.000000 intensity_normalization-2.2.3/intensity_normalization.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-03-15 16:29:46.000000 intensity_normalization-2.2.3/intensity_normalization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-03-15 16:29:46.000000 intensity_normalization-2.2.3/intensity_normalization.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     3040 2022-03-15 16:29:46.823910 intensity_normalization-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 16:29:46.819909 intensity_normalization-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7590 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/tests/run_all_clis.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/tests/test_ants_required_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-03-15 16:29:31.000000 intensity_normalization-2.2.3/tests/test_intensity_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.604049 intensity_normalization-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-05-31 21:10:38.604049 intensity_normalization-2.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.596048 intensity_normalization-2.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.592049 intensity_normalization-2.2.4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.596048 intensity_normalization-2.2.4/docs/_static/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)   405830 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/_static/imgs/intnorm_illustration.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5437 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/intensity_normalization.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/intensity_normalization.normalize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/intensity_normalization.plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/intensity_normalization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/intensity_normalization.util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.596048 intensity_normalization-2.2.4/intensity_normalization/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/base_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.600048 intensity_normalization-2.2.4/intensity_normalization/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/coregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/fcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/lsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/nyul.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/ravel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/tissue_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/whitestripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/cli/zscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.600048 intensity_normalization-2.2.4/intensity_normalization/normalize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/normalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/normalize/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/normalize/fcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/normalize/kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/normalize/lsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/normalize/nyul.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/normalize/ravel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/normalize/whitestripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/normalize/zscore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.600048 intensity_normalization-2.2.4/intensity_normalization/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/plot/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.600048 intensity_normalization-2.2.4/intensity_normalization/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/util/coregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/util/histogram_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/util/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/intensity_normalization/util/tissue_membership.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.596048 intensity_normalization-2.2.4/intensity_normalization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-05-31 21:10:38.000000 intensity_normalization-2.2.4/intensity_normalization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-31 21:10:38.000000 intensity_normalization-2.2.4/intensity_normalization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:10:38.000000 intensity_normalization-2.2.4/intensity_normalization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-31 21:10:38.000000 intensity_normalization-2.2.4/intensity_normalization.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:10:38.000000 intensity_normalization-2.2.4/intensity_normalization.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-31 21:10:38.000000 intensity_normalization-2.2.4/intensity_normalization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 21:10:38.000000 intensity_normalization-2.2.4/intensity_normalization.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-31 21:10:38.604049 intensity_normalization-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:10:38.604049 intensity_normalization-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7590 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/tests/run_all_clis.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/tests/test_ants_required_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-31 21:10:25.000000 intensity_normalization-2.2.4/tests/test_intensity_normalization.py
```

### Comparing `intensity_normalization-2.2.3/CONTRIBUTING.rst` & `intensity_normalization-2.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/HISTORY.rst` & `intensity_normalization-2.2.4/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2.2.4 (2023-05-31)
+------------------
+
+* Update to allow Python >=3.9
+
 2.2.3 (2022-03-15)
 ------------------
 
 * Revert error on different image shapes from ``RavelNormalize``; it is required!
 
 2.2.2 (2022-03-15)
 ------------------
```

### Comparing `intensity_normalization-2.2.3/LICENSE` & `intensity_normalization-2.2.4/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Apache Software License 2.0
 
-Copyright (c) 2021, Jacob Reinhold
+Copyright (c) 2023, Jacob Reinhold
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `intensity_normalization-2.2.3/PKG-INFO` & `intensity_normalization-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: intensity_normalization
-Version: 2.2.3
+Version: 2.2.4
 Summary: normalize the intensities of various MR image modalities
 Home-page: https://github.com/jcreinhold/intensity-normalization
 Author: Jacob Reinhold
 Author-email: jcreinhold@gmail.com
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/jcreinhold/intensity-normalization/issues
 Project-URL: Documentation, https://intensity-normalization.readthedocs.io/
 Keywords: intensity,normalization,mri
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
-Requires-Python: !=3.10.*,!=3.11.*,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: ants
 Provides-Extra: plot
 License-File: LICENSE
 
 =======================
 intensity-normalization
@@ -239,14 +237,19 @@
 .. [5] Iglesias, Juan Eugenio, Cheng-Yi Liu, Paul M. Thompson, and Zhuowen Tu. "Robust brain extraction across datasets and
        comparison with publicly available methods." IEEE transactions on medical imaging 30, no. 9 (2011): 1617-1634.
 
 =======
 History
 =======
 
+2.2.4 (2023-05-31)
+------------------
+
+* Update to allow Python >=3.9
+
 2.2.3 (2022-03-15)
 ------------------
 
 * Revert error on different image shapes from ``RavelNormalize``; it is required!
 
 2.2.2 (2022-03-15)
 ------------------
@@ -317,9 +320,7 @@
 
 * Major refactor to reduce redundancy, make code more usable outside of the CLIs, and generally improve code quality.
 
 1.4.0 (2021-03-16)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `intensity_normalization-2.2.3/docs/Makefile` & `intensity_normalization-2.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/docs/_static/imgs/intnorm_illustration.png` & `intensity_normalization-2.2.4/docs/_static/imgs/intnorm_illustration.png`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/docs/algorithm.rst` & `intensity_normalization-2.2.4/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/docs/conf.py` & `intensity_normalization-2.2.4/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # serve to show the default.
 
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 
-import builtins
 import os
 import sys
 import typing
 
 sys.path.insert(0, os.path.abspath(".."))
 
 autodoc_mock_imports = [
@@ -64,15 +63,15 @@
 source_suffix = [".rst", ".md"]
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "intensity-normalization"
-copyright = "2021, Jacob Reinhold"
+copyright = "2023, Jacob Reinhold"
 author = "Jacob Reinhold"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
@@ -81,15 +80,15 @@
 release = intensity_normalization.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -122,15 +121,15 @@
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "intensity_normalizationdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
-latex_elements: builtins.dict[builtins.str, typing.Any] = {
+latex_elements: dict[str, typing.Any] = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
```

### Comparing `intensity_normalization-2.2.3/docs/installation.rst` & `intensity_normalization-2.2.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/docs/intensity_normalization.cli.rst` & `intensity_normalization-2.2.4/docs/intensity_normalization.cli.rst`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/docs/intensity_normalization.normalize.rst` & `intensity_normalization-2.2.4/docs/intensity_normalization.normalize.rst`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/docs/intensity_normalization.rst` & `intensity_normalization-2.2.4/docs/intensity_normalization.rst`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/docs/intensity_normalization.util.rst` & `intensity_normalization-2.2.4/docs/intensity_normalization.util.rst`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/docs/make.bat` & `intensity_normalization-2.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/docs/readme.rst` & `intensity_normalization-2.2.4/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/intensity_normalization/__init__.py` & `intensity_normalization-2.2.4/intensity_normalization/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import logging
 
 __title__ = "intensity-normalization"
 __description__ = "normalize the intensities of various MR image modalities"
 __url__ = "https://github.com/jcreinhold/intensity-normalization"
 __author__ = """Jacob Reinhold"""
 __email__ = "jcreinhold@gmail.com"
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __license__ = "Apache-2.0"
-__copyright__ = "Copyright 2021 Jacob Reinhold"
+__copyright__ = "Copyright 2023 Jacob Reinhold"
 
 PEAK = {
     "last": ("t1", "other", "last"),
     "largest": ("t2", "flair", "largest"),
     "first": ("pd", "md", "first"),
 }
 VALID_PEAKS = frozenset({m for modalities in PEAK.values() for m in modalities})
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/base_cli.py` & `intensity_normalization-2.2.4/intensity_normalization/base_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from __future__ import annotations
 
 __all__ = ["CLIMixin", "DirectoryCLI", "setup_log", "SingleImageCLI"]
 
 import abc
 import argparse
-import builtins
 import logging
 import pathlib
 import sys
 import typing
 
 import pymedio.image as mioi
 
@@ -23,44 +22,44 @@
 from intensity_normalization import __version__ as int_norm_version
 
 logger = logging.getLogger(__name__)
 
 T = typing.TypeVar("T")
 
 
-def setup_log(verbosity: builtins.int) -> None:
+def setup_log(verbosity: int) -> None:
     """set logger with verbosity logging level and message"""
     if verbosity == 1:
         level = logging.getLevelName("INFO")
     elif verbosity >= 2:
         level = logging.getLevelName("DEBUG")
     else:
         level = logging.getLevelName("WARNING")
     fmt = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     logging.basicConfig(format=fmt, level=level)
     logging.captureWarnings(True)
 
 
 class CLIMixin(metaclass=abc.ABCMeta):
-    def __str__(self) -> builtins.str:
+    def __str__(self) -> str:
         return self.__class__.__name__
 
     @staticmethod
     @abc.abstractmethod
-    def description() -> builtins.str:
+    def description() -> str:
         raise NotImplementedError
 
     @staticmethod
     @abc.abstractmethod
-    def name() -> builtins.str:
+    def name() -> str:
         raise NotImplementedError
 
     @staticmethod
     @abc.abstractmethod
-    def fullname() -> builtins.str:
+    def fullname() -> str:
         raise NotImplementedError
 
     def append_name_to_file(
         self,
         filepath: intnormt.PathLike,
         alternate_path: intnormt.PathLike | None = None,
     ) -> pathlib.Path:
@@ -71,16 +70,16 @@
         new_path: pathlib.Path = path / (base + f"_{self.name()}" + ext)
         return new_path
 
     @classmethod
     @abc.abstractmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         raise NotImplementedError
 
     @staticmethod
     def add_method_specific_arguments(
         parent_parser: argparse.ArgumentParser,
@@ -92,15 +91,15 @@
         parser = cls.get_parent_parser(cls.description())
         parser = cls.add_method_specific_arguments(parser)
         return parser
 
     @classmethod
     def main(
         cls, parser: argparse.ArgumentParser
-    ) -> typing.Callable[[intnormt.ArgType], builtins.int]:
+    ) -> typing.Callable[[intnormt.ArgType], int]:
         def _main(args: intnormt.ArgType = None) -> int:
             if args is None:
                 if len(sys.argv) == 2 and sys.argv[1] == "--version":
                     print(f"intensity-normalization version {int_norm_version}")
                     return 0
                 args = parser.parse_args()
             elif isinstance(args, list):
@@ -144,16 +143,16 @@
         **kwargs: typing.Any,
     ) -> typing.Any:
         raise NotImplementedError
 
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             description=desc,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         parser.add_argument(
@@ -218,16 +217,16 @@
             raise ValueError("Unexpected image type")
 
 
 class DirectoryCLI(CLIMixin, metaclass=abc.ABCMeta):
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             description=desc,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         parser.add_argument(
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/normalize/base.py` & `intensity_normalization-2.2.4/intensity_normalization/normalize/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     "SingleImageNormalizeCLI",
     "DirectoryNormalizeCLI",
     "LocationScaleCLIMixin",
 ]
 
 import abc
 import argparse
-import builtins
 import collections.abc
 import logging
 import pathlib
 import typing
 import warnings
 
 import pymedio.image as mioi
@@ -75,15 +74,15 @@
     @staticmethod
     def estimate_foreground(image: intnormt.ImageLike, /) -> intnormt.ImageLike:
         foreground: intnormt.ImageLike = image > image.mean()
         return foreground
 
     @staticmethod
     def skull_stripped_foreground(
-        image: intnormt.ImageLike, /, *, background_threshold: builtins.float = 1e-6
+        image: intnormt.ImageLike, /, *, background_threshold: float = 1e-6
     ) -> intnormt.ImageLike:
         if image.min() < 0.0:
             msg = "Data contains negative values; "
             msg += "skull-stripped functionality assumes "
             msg += "the foreground is all positive. "
             msg += "Provide the brain mask if otherwise."
             warnings.warn(msg)
@@ -93,15 +92,15 @@
     def _get_mask(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-        background_threshold: builtins.float = 1e-6,
+        background_threshold: float = 1e-6,
     ) -> intnormt.ImageLike:
         if mask is None:
             mask = self.skull_stripped_foreground(
                 image, background_threshold=background_threshold
             )
         out: intnormt.ImageLike = mask > 0.0
         return out
@@ -115,38 +114,38 @@
         modality: intnormt.Modality = intnormt.Modality.T1,
     ) -> intnormt.ImageLike:
         voi: intnormt.ImageLike = image[self._get_mask(image, mask, modality=modality)]
         return voi
 
 
 class LocationScaleMixin(NormalizeMixin, metaclass=abc.ABCMeta):
-    def __init__(self, *, norm_value: builtins.float = 1.0, **kwargs: typing.Any):
+    def __init__(self, *, norm_value: float = 1.0, **kwargs: typing.Any):
         super().__init__(**kwargs)
         self.norm_value = norm_value
 
     @abc.abstractmethod
     def calculate_location(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.float:
+    ) -> float:
         raise NotImplementedError
 
     @abc.abstractmethod
     def calculate_scale(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.float:
+    ) -> float:
         raise NotImplementedError
 
     def normalize_image(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
@@ -166,32 +165,33 @@
         self,
         image_path: intnormt.PathLike,
         /,
         mask_path: intnormt.PathLike | None = None,
         *,
         out_path: intnormt.PathLike | None = None,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.tuple[mioi.Image, mioi.Image | None]:
-        image = mioi.Image.from_path(image_path)
+    ) -> tuple[mioi.Image, mioi.Image | None]:
+        image: mioi.Image = mioi.Image.from_path(image_path)
+        mask: typing.Optional[mioi.Image]
         mask = None if mask_path is None else mioi.Image.from_path(mask_path)
         if out_path is None:
             out_path = self.append_name_to_file(image_path)
         logger.info(f"Normalizing image: {image_path}")
         normalized = typing.cast(
             mioi.Image, self.normalize_image(image, mask, modality=modality)
         )
         logger.info(f"Saving normalized image: {out_path}")
         normalized.to_filename(out_path)
         return normalized, mask
 
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = super().get_parent_parser(
             desc, valid_modalities=valid_modalities, **kwargs
         )
         parser.add_argument(
             "-p",
@@ -220,16 +220,16 @@
         return
 
 
 class LocationScaleCLIMixin(LocationScaleMixin, NormalizeCLIMixin):
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = super().get_parent_parser(
             desc, valid_modalities=valid_modalities, **kwargs
         )
         parser.add_argument(
             "-n",
@@ -294,23 +294,23 @@
     def process_directories(
         self,
         image_dir: intnormt.PathLike,
         /,
         mask_dir: intnormt.PathLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-        ext: builtins.str = "nii*",
-        return_normalized_and_masks: builtins.bool = False,
+        ext: str = "nii*",
+        return_normalized_and_masks: bool = False,
         **kwargs: typing.Any,
-    ) -> builtins.tuple[ImageSeq, MaskSeqOrNone] | None:
+    ) -> tuple[ImageSeq, MaskSeqOrNone] | None:
         logger.debug("Grabbing images")
         images, masks = intnormio.gather_images_and_masks(image_dir, mask_dir, ext=ext)
         self.fit(images, masks, modality=modality, **kwargs)
         if return_normalized_and_masks:
-            normalized: builtins.list[intnormt.ImageLike] = []
+            normalized: list[intnormt.ImageLike] = []
             n_images = len(images)
             zipped = intnormio.zip_with_nones(images, masks)
             for i, (image, mask) in enumerate(zipped, 1):
                 logger.info(f"Normalizing image {i}/{n_images}")
                 normalized.append(self(image, mask, modality=modality))
             return normalized, masks
         return None
@@ -335,15 +335,15 @@
         plt.savefig(output)
 
     def call_from_argparse_args(
         self,
         args: argparse.Namespace,
         /,
         *,
-        use_masks_in_plot: builtins.bool = True,
+        use_masks_in_plot: bool = True,
         **kwargs: typing.Any,
     ) -> None:
         out = self.process_directories(
             args.image_dir,
             args.mask_dir,
             modality=intnormt.Modality.from_string(args.modality),
             ext=args.extension,
@@ -404,15 +404,15 @@
         self,
         images: collections.abc.Sequence[intnormt.ImageLike],
         /,
         masks: collections.abc.Sequence[intnormt.ImageLike] | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
         **kwargs: typing.Any,
-    ) -> builtins.tuple[ImageSeq, MaskSeqOrNone]:
+    ) -> tuple[ImageSeq, MaskSeqOrNone]:
         assert len(images) > 0
         logger.info("Loading data")
         if hasattr(images[0], "get_fdata"):
             images = [img.get_fdata() for img in images]  # type: ignore[attr-defined]
         if masks is not None:
             if hasattr(masks[0], "get_fdata"):
                 masks = [msk.get_fdata() for msk in masks]  # type: ignore[attr-defined]
@@ -422,18 +422,18 @@
     def fit_from_directories(
         self,
         image_dir: intnormt.PathLike,
         /,
         mask_dir: intnormt.PathLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-        ext: builtins.str = "nii*",
-        return_normalized_and_masks: builtins.bool = False,
+        ext: str = "nii*",
+        return_normalized_and_masks: bool = False,
         **kwargs: typing.Any,
-    ) -> builtins.tuple[ImageSeq, MaskSeqOrNone] | None:
+    ) -> tuple[ImageSeq, MaskSeqOrNone] | None:
         return self.process_directories(
             image_dir,
             mask_dir,
             modality=modality,
             ext=ext,
             return_normalized_and_masks=return_normalized_and_masks,
             **kwargs,
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/normalize/fcm.py` & `intensity_normalization-2.2.4/intensity_normalization/normalize/fcm.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["FCMNormalize"]
 
 import argparse
-import builtins
 import logging
 import pathlib
 import typing
 
 import numpy as np
 import numpy.typing as npt
 import pymedio.image as mioi
@@ -26,15 +25,15 @@
 logger = logging.getLogger(__name__)
 
 
 class FCMNormalize(intnormb.LocationScaleCLIMixin, intnormb.SingleImageNormalizeCLI):
     def __init__(
         self,
         *,
-        norm_value: builtins.float = 1.0,
+        norm_value: float = 1.0,
         tissue_type: intnormt.TissueType = intnormt.TissueType.WM,
         **kwargs: typing.Any,
     ):
         """
         Use fuzzy c-means-generated tissue membership (found on a T1-w image) to
         normalize the specified tissue type's mean to norm_value (default = 1.)
         """
@@ -45,26 +44,26 @@
     def calculate_location(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.float:
+    ) -> float:
         return 0.0
 
     def calculate_scale(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.float:
-        tissue_mean: builtins.float
+    ) -> float:
+        tissue_mean: float
         if modality == intnormt.Modality.T1:
             mask = self._get_mask(image, mask, modality=modality)
             tissue_name = self.tissue_type.to_fullname()
             logger.debug(f"Finding {tissue_name} membership.")
             tissue_memberships = intnormtm.find_tissue_memberships(image, mask)
             self.tissue_membership = tissue_memberships[..., self.tissue_type.to_int()]
             logger.debug(f"Calculated {tissue_name} membership.")
@@ -76,36 +75,36 @@
         else:
             msg = "Either a T1-w image must be passed to initialize a tissue "
             msg += "membership mask or the tissue memberships must be provided."
             raise ValueError(msg)
         return tissue_mean
 
     @property
-    def is_fit(self) -> builtins.bool:
+    def is_fit(self) -> bool:
         return self.tissue_membership is not None
 
     @staticmethod
-    def name() -> builtins.str:
+    def name() -> str:
         return "fcm"
 
     @staticmethod
-    def fullname() -> builtins.str:
+    def fullname() -> str:
         return "Fuzzy C-Means"
 
     @staticmethod
-    def description() -> builtins.str:
+    def description() -> str:
         desc = "Use fuzzy c-means to find memberships of CSF/GM/WM in the brain. "
         desc += "Use the specified tissue's mean to normalize a MRI."
         return desc
 
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             description=desc,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         parser.add_argument(
@@ -210,15 +209,15 @@
     def save_additional_info(
         self,
         args: argparse.Namespace,
         **kwargs: typing.Any,
     ) -> None:
         if self.is_fit and args.tissue_mask is None:
             assert self.tissue_membership is not None
-            tissue_membership = mioi.Image(
+            tissue_membership: mioi.Image = mioi.Image(
                 self.tissue_membership,
                 kwargs["normalized"].affine,
             )
             base, name, ext = intnormio.split_filename(args.image)
             new_name = name + f"_{self.tissue_type.value}_membership" + ext
             if args.output is None:
                 output = base / new_name
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/normalize/kde.py` & `intensity_normalization-2.2.4/intensity_normalization/normalize/kde.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 Created on: 01 Jun 2021
 """
 
 from __future__ import annotations
 
 __all__ = ["KDENormalize"]
 
-import builtins
 import typing
 
 import intensity_normalization.normalize.base as intnormb
 import intensity_normalization.typing as intnormt
 import intensity_normalization.util.histogram_tools as intnormhisttool
 
 
 class KDENormalize(intnormb.LocationScaleCLIMixin, intnormb.SingleImageNormalizeCLI):
-    def __init__(self, norm_value: builtins.float = 1.0, **kwargs: typing.Any):
+    def __init__(self, norm_value: float = 1.0, **kwargs: typing.Any):
         """
         Use kernel density estimation to fit a smoothed histogram of intensities
         of a (skull-stripped) brain MR image, then find the peak of the white
         matter (by default) in the smoothed histogram. Finally, normalize the
         white matter mode of the image to norm_value (default = 1.)
         """
         super().__init__(norm_value=norm_value, **kwargs)
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/normalize/lsq.py` & `intensity_normalization-2.2.4/intensity_normalization/normalize/lsq.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["LeastSquaresNormalize"]
 
 import argparse
-import builtins
 import collections.abc
 import logging
 import pathlib
 import typing
 
 import numpy as np
 import numpy.typing as npt
@@ -32,15 +31,15 @@
 
 class LeastSquaresNormalize(
     intnormb.LocationScaleCLIMixin, intnormb.DirectoryNormalizeCLI
 ):
     def __init__(self, *, norm_value: float = 1.0, **kwargs: typing.Any):
         """Minimize the distance tissue means in a set of images via least-squares"""
         super().__init__(norm_value=norm_value, **kwargs)
-        self.tissue_memberships: builtins.list[mioi.Image] = []
+        self.tissue_memberships: list[mioi.Image] = []
         self.standard_tissue_means: npt.NDArray | None = None
 
     def calculate_location(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
@@ -121,26 +120,26 @@
         n_tissues = tissue_membership.shape[-1]
         weighted_avgs = [
             np.average(image, weights=tissue_membership[..., i])
             for i in range(n_tissues)
         ]
         return np.asarray([weighted_avgs]).T
 
-    def scaling_factor(self, tissue_means: npt.NDArray) -> builtins.float:
+    def scaling_factor(self, tissue_means: npt.NDArray) -> float:
         numerator = tissue_means.T @ tissue_means
         denominator = tissue_means.T @ self.standard_tissue_means
-        sf: builtins.float = (numerator / denominator).item()
+        sf: float = (numerator / denominator).item()
         return sf
 
     @staticmethod
-    def name() -> builtins.str:
+    def name() -> str:
         return "lsq"
 
     @staticmethod
-    def fullname() -> builtins.str:
+    def fullname() -> str:
         return "Least Squares"
 
     @staticmethod
     def description() -> str:
         desc = "Minimize distance between tissue means (CSF/GM/WM) in a "
         desc += "least squares-sense within a set of MR images."
         return desc
@@ -163,15 +162,15 @@
         if len(self.tissue_memberships) != len(normed):
             msg = f"'tissue_memberships' ({len(self.tissue_memberships)}) "
             msg += f"and 'normalized' ({len(normed)}) "
             msg += "must be in correspondence."
             raise RuntimeError(msg)
         for memberships, norm, fn in zip(self.tissue_memberships, normed, image_fns):
             if hasattr(norm, "affine"):
-                tissue_memberships = mioi.Image(memberships, norm.affine)
+                tissue_memberships: mioi.Image = mioi.Image(memberships, norm.affine)
             elif hasattr(memberships, "affine"):
                 tissue_memberships = mioi.Image(memberships, memberships.affine)
             else:
                 tissue_memberships = mioi.Image(memberships, None)
             base, name, ext = intnormio.split_filename(fn)
             new_name = name + "_tissue_memberships" + ext
             if args.output_dir is None:
@@ -199,15 +198,15 @@
         return out
 
     def call_from_argparse_args(
         self, args: argparse.Namespace, /, **kwargs: typing.Any
     ) -> None:
         if args.load_standard_tissue_means is not None:
             self.load_standard_tissue_means(args.load_standard_tissue_means)
-            self.fit = lambda *args, **kwargs: None  # type: ignore[assignment]
+            self.fit = lambda *args, **kwargs: None  # type: ignore[method-assign]
 
         args.modality = intnormt.Modality.from_string(args.modality)
         use_masks = True
         if args.mask_dir is not None:
             if args.modality != intnormt.Modality.T1:
                 msg = f"If brain masks provided, 'modality' must be 't1'. Got '{args.modality}'."  # noqa: E501
                 raise ValueError(msg)
@@ -215,16 +214,16 @@
             use_masks = False
             args.mask_dir = args.tissue_membership_dir
         super().call_from_argparse_args(args, use_masks_in_plot=use_masks)
 
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             description=desc,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         parser.add_argument(
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/normalize/nyul.py` & `intensity_normalization-2.2.4/intensity_normalization/normalize/nyul.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["NyulNormalize"]
 
 import argparse
-import builtins
 import collections.abc
 import typing
 
 import numpy as np
 import numpy.typing as npt
 from scipy.interpolate import interp1d
 
@@ -22,21 +21,21 @@
 import intensity_normalization.util.io as intnormio
 
 
 class NyulNormalize(intnormb.DirectoryNormalizeCLI):
     def __init__(
         self,
         *,
-        output_min_value: builtins.float = 1.0,
-        output_max_value: builtins.float = 100.0,
-        min_percentile: builtins.float = 1.0,
-        max_percentile: builtins.float = 99.0,
-        percentile_after_min: builtins.float = 10.0,
-        percentile_before_max: builtins.float = 90.0,
-        percentile_step: builtins.float = 10.0,
+        output_min_value: float = 1.0,
+        output_max_value: float = 100.0,
+        min_percentile: float = 1.0,
+        max_percentile: float = 99.0,
+        percentile_after_min: float = 10.0,
+        percentile_before_max: float = 90.0,
+        percentile_step: float = 10.0,
     ):
         """Nyul & Udupa piecewise linear histogram matching normalization
 
         Args:
             output_min_value: where min-percentile mapped for output normalized image
             output_max_value: where max-percentile mapped for output normalized image
             min_percentile: min percentile to account for while finding
@@ -83,21 +82,21 @@
         if self._percentiles is None:
             percs = np.arange(
                 self.percentile_after_min,
                 self.percentile_before_max + self.percentile_step,
                 self.percentile_step,
             )
             _percs = ([self.min_percentile], percs, [self.max_percentile])
-            self._percentiles = np.concatenate(_percs)
+            self._percentiles = np.concatenate(_percs)  # type: ignore[arg-type]
         assert isinstance(self._percentiles, np.ndarray)
         return self._percentiles
 
     def get_landmarks(self, image: intnormt.ImageLike, /) -> npt.NDArray:
         landmarks = np.percentile(image, self.percentiles)
-        return landmarks  # type: ignore[return-value]
+        return typing.cast(npt.NDArray, landmarks)
 
     def _fit(
         self,
         images: collections.abc.Sequence[intnormt.ImageLike],
         /,
         masks: collections.abc.Sequence[intnormt.ImageLike] | None = None,
         *,
@@ -142,23 +141,23 @@
 
     def load_standard_histogram(self, filename: intnormt.PathLike) -> None:
         data = np.load(filename)
         self.standard_scale = data[0, :]
         self._percentiles = data[1, :]
 
     @staticmethod
-    def name() -> builtins.str:
+    def name() -> str:
         return "nyul"
 
     @staticmethod
-    def fullname() -> builtins.str:
+    def fullname() -> str:
         return "Nyul & Udupa"
 
     @staticmethod
-    def description() -> builtins.str:
+    def description() -> str:
         desc = "Perform piecewise-linear histogram matching per "
         desc += "Nyul and Udupa given a set of MR images."
         return desc
 
     @staticmethod
     def add_method_specific_arguments(
         parent_parser: argparse.ArgumentParser,
@@ -228,15 +227,15 @@
         return parent_parser
 
     def call_from_argparse_args(
         self, args: argparse.Namespace, /, **kwargs: typing.Any
     ) -> None:
         if args.load_standard_histogram is not None:
             self.load_standard_histogram(args.load_standard_histogram)
-            self.fit = lambda *args, **kwargs: None  # type: ignore[assignment]
+            self.fit = lambda *args, **kwargs: None  # type: ignore[method-assign]
         super().call_from_argparse_args(args)
 
     @classmethod
     def from_argparse_args(cls, args: argparse.Namespace, /) -> NyulNormalize:
         return cls(
             output_min_value=args.output_min_value,
             output_max_value=args.output_max_value,
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/normalize/ravel.py` & `intensity_normalization-2.2.4/intensity_normalization/normalize/ravel.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["RavelNormalize"]
 
 import argparse
-import builtins
 import collections.abc
 import functools
 import logging
 import operator
 import pathlib
 import typing
 
@@ -40,38 +39,54 @@
     from intensity_normalization.util.coregister import register, to_ants
 
 
 class RavelNormalize(intnormb.DirectoryNormalizeCLI):
     def __init__(
         self,
         *,
-        membership_threshold: builtins.float = 0.99,
-        register: builtins.bool = True,
-        num_unwanted_factors: builtins.int = 1,
-        sparse_svd: builtins.bool = False,
-        whitestripe_kwargs: builtins.dict[builtins.str, typing.Any] | None = None,
-        quantile_to_label_csf: builtins.float = 1.0,
-        masks_are_csf: builtins.bool = False,
+        membership_threshold: float = 0.99,
+        register: bool = True,
+        num_unwanted_factors: int = 1,
+        sparse_svd: bool = False,
+        whitestripe_kwargs: dict[str, typing.Any] | None = None,
+        quantile_to_label_csf: float = 1.0,
+        masks_are_csf: bool = False,
     ):
-        """Normalize a set of images with WhiteStripe and a CSF correction"""
+        """Normalize a set of co-registered images with WhiteStripe and a CSF correction
+
+        Args:
+            membership_threshold: threshold in FCM for CSF membership
+            register: if the images aren't deformably co-registered,
+                set this to True to do so before calculating the unwanted factors
+                NOTE: The images must be rigidly or affine registered, at a minimum,
+                before using this process. Good results, however, are only
+                reliable for deformably co-registered images!
+            num_unwanted_factors: see 'b' from the original paper
+            sparse_svd: if you're hitting out-of-memory errors, try setting this to true
+            whitestripe_kwargs: keyword args to pass to WhiteStripe
+            quantile_to_label_csf: lower this if you want some wiggle room in the number
+                of images in which CSF must be found. Don't change this in general.
+            masks_are_csf: flag to signify that the masks are actually CSF boolean masks
+                so CSF masks are not created, and the CSF masks are used directly.
+        """
         super().__init__()
         self.membership_threshold = membership_threshold
         self.register = register
         self.num_unwanted_factors = num_unwanted_factors
         self.sparse_svd = sparse_svd
         self.whitestripe_kwargs = whitestripe_kwargs or dict()
         self.quantile_to_label_csf = quantile_to_label_csf
         self.masks_are_csf = masks_are_csf
         if register and masks_are_csf:
             msg = "If 'masks_are_csf', then images are assumed to be co-registered."
             raise ValueError(msg)
         self._template: intnormt.ImageLike | None = None
         self._template_mask: intnormt.ImageLike | None = None
         self._normalized: intnormt.ImageLike | None = None
-        self._control_masks: builtins.list[intnormt.ImageLike] = []
+        self._control_masks: list[intnormt.ImageLike] = []
 
     def normalize_image(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
@@ -101,15 +116,15 @@
         self,
         template_mask: intnormt.ImageLike | ants.ANTsImage | None,
     ) -> None:
         if template_mask is None:
             self._template_mask = None
         else:
             if hasattr(template_mask, "astype"):
-                template_mask = template_mask.astype(np.uint32)  # type: ignore[union-attr] # noqa: E501
+                template_mask = template_mask.astype(np.uint32)
             self._template_mask = to_ants(template_mask)
 
     def use_mni_as_template(self) -> None:
         standard_mni = ants.get_ants_data("mni")
         self.set_template(ants.image_read(standard_mni))
         assert self.template is not None
         self.set_template_mask(self.template > 0.0)
@@ -160,15 +175,15 @@
         fitted = (unwanted_factors @ beta).T
         residuals: np.ndarray = control_voxels - fitted
         voxel_means = np.mean(control_voxels, axis=1, keepdims=True)
         normalized: npt.NDArray = residuals + voxel_means
         return normalized
 
     def _register(self, image: ants.ANTsImage) -> npt.NDArray:
-        registered = register(
+        registered: ants.ANTsImage = register(
             image,
             template=self.template,
             type_of_transform="SyN",
             interpolator="linear",
             template_mask=self.template_mask,
         )
         out: npt.NDArray = registered.numpy()
@@ -177,15 +192,15 @@
     def create_image_matrix_and_control_voxels(
         self,
         images: collections.abc.Sequence[intnormt.ImageLike],
         /,
         masks: collections.abc.Sequence[intnormt.ImageLike] | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.tuple[npt.NDArray, npt.NDArray]:
+    ) -> tuple[npt.NDArray, npt.NDArray]:
         """creates a matrix of images; rows correspond to voxels, columns are images
 
         Args:
             images: list of MR images of interest
             masks: list of corresponding brain masks
             modality: modality of the set of images (e.g., t1)
 
@@ -194,15 +209,16 @@
             control_voxels: rows are csf intersection voxels, columns are images
         """
         n_images = len(images)
         image_shapes = [image.shape for image in images]
         image_shape = image_shapes[0]
         image_size = int(np.prod(image_shape))
         if any([shape != image_shape for shape in image_shapes]):
-            msg = "All images must be the same size. Resample/co-register the images."
+            msg = "All images must be the same size and have (approximate) voxel-wise "
+            msg += "correspondence. At a minimum, rigid/affine co-register the images."
             raise RuntimeError(msg)
         image_matrix = np.zeros((image_size, n_images))
         whitestripe_norm = intnormws.WhiteStripeNormalize(**self.whitestripe_kwargs)
         self._control_masks = []  # reset control masks to prevent run-to-run issues
         registered_images = []
 
         for i, (image, mask) in enumerate(intnormio.zip_with_nones(images, masks), 1):
@@ -290,26 +306,24 @@
     def process_directories(
         self,
         image_dir: intnormt.PathLike,
         /,
         mask_dir: intnormt.PathLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-        ext: builtins.str = "nii*",
-        return_normalized_and_masks: builtins.bool = False,
+        ext: str = "nii*",
+        return_normalized_and_masks: bool = False,
         **kwargs: typing.Any,
-    ) -> builtins.tuple[
-        builtins.list[mioi.Image], builtins.list[mioi.Image] | None
-    ] | None:
+    ) -> tuple[list[mioi.Image], list[mioi.Image] | None] | None:
         logger.debug("Gathering images.")
         images, masks = intnormio.gather_images_and_masks(image_dir, mask_dir, ext=ext)
         self.fit(images, masks, modality=modality, **kwargs)
         assert self._normalized is not None
         if return_normalized_and_masks:
-            norm_lst: builtins.list[mioi.Image] = []
+            norm_lst: list[mioi.Image] = []
             for normed, image in zip(self._normalized, images):
                 norm_lst.append(mioi.Image(normed.reshape(image.shape), image.affine))
             return norm_lst, masks
         return None
 
     @staticmethod
     def name() -> str:
@@ -399,18 +413,19 @@
             raise RuntimeError(msg)
         if len(self._control_masks) != len(normed):
             msg = f"'control_masks' ({len(self._control_masks)}) "
             msg += f"and 'normalized' ({len(normed)}) "
             msg += "must be in correspondence."
             raise RuntimeError(msg)
         for _csf_mask, norm, fn in zip(self._control_masks, normed, image_fns):
+            csf_mask: mioi.Image
             if hasattr(norm, "affine"):
                 csf_mask = mioi.Image(_csf_mask, norm.affine)
             elif hasattr(_csf_mask, "affine"):
-                csf_mask = mioi.Image(_csf_mask, _csf_mask.affine)  # type: ignore[attr-defined] # noqa: E501
+                csf_mask = mioi.Image(_csf_mask, _csf_mask.affine)
             else:
                 csf_mask = mioi.Image(_csf_mask, None)
             base, name, ext = intnormio.split_filename(fn)
             new_name = name + "_csf_mask" + ext
             if args.output_dir is None:
                 output = base / new_name
             else:
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/normalize/whitestripe.py` & `intensity_normalization-2.2.4/intensity_normalization/normalize/whitestripe.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["WhiteStripeNormalize"]
 
 import argparse
-import builtins
 import typing
 
 import numpy as np
 import numpy.typing as npt
 
 import intensity_normalization.normalize.base as intnormb
 import intensity_normalization.typing as intnormt
@@ -21,18 +20,18 @@
 
 class WhiteStripeNormalize(
     intnormb.LocationScaleCLIMixin, intnormb.SingleImageNormalizeCLI
 ):
     def __init__(
         self,
         *,
-        norm_value: builtins.float = 1.0,
-        width: builtins.float = 0.05,
-        width_l: builtins.float | None = None,
-        width_u: builtins.float | None = None,
+        norm_value: float = 1.0,
+        width: float = 0.05,
+        width_l: float | None = None,
+        width_u: float | None = None,
         **kwargs: typing.Any,
     ):
         """
         Find the normal-appearing white matter of the input MR image and
         use those values to standardize the data (i.e., subtract the mean of
         the values in the indices and divide by the std of those values).
         See the original paper for details on width.
@@ -45,27 +44,27 @@
     def calculate_location(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.float:
-        loc: builtins.float = image[self.whitestripe].mean()
+    ) -> float:
+        loc: float = image[self.whitestripe].mean()
         return loc
 
     def calculate_scale(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.float:
-        scale: builtins.float = image[self.whitestripe].std()
+    ) -> float:
+        scale: float = image[self.whitestripe].std()
         return scale
 
     def setup(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
@@ -74,35 +73,35 @@
     ) -> None:
         if modality is None:
             modality = "t1"
         mask = self._get_mask(image, mask, modality=modality)
         masked = image * mask
         voi = image[mask]
         wm_mode = intnormhisttool.get_tissue_mode(voi, modality=modality)
-        wm_mode_quantile: builtins.float = np.mean(voi < wm_mode).item()
+        wm_mode_quantile: float = np.mean(voi < wm_mode).item()
         lower_bound = max(wm_mode_quantile - self.width_l, 0.0)
         upper_bound = min(wm_mode_quantile + self.width_u, 1.0)
-        ws_l: builtins.float
-        ws_u: builtins.float
-        ws_l, ws_u = np.quantile(voi, (lower_bound, upper_bound))  # type: ignore[misc]
+        ws_l: float
+        ws_u: float
+        ws_l, ws_u = np.quantile(voi, (lower_bound, upper_bound))
         self.whitestripe = (masked > ws_l) & (masked < ws_u)
 
     def teardown(self) -> None:
         del self.whitestripe
 
     @staticmethod
-    def name() -> builtins.str:
+    def name() -> str:
         return "ws"
 
     @staticmethod
-    def fullname() -> builtins.str:
+    def fullname() -> str:
         return "WhiteStripe"
 
     @staticmethod
-    def description() -> builtins.str:
+    def description() -> str:
         return "Standardize the normal appearing WM of a MR image."
 
     @staticmethod
     def add_method_specific_arguments(
         parent_parser: argparse.ArgumentParser,
     ) -> argparse.ArgumentParser:
         parser = parent_parser.add_argument_group("method-specific arguments")
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/normalize/zscore.py` & `intensity_normalization-2.2.4/intensity_normalization/normalize/zscore.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,52 +4,51 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["ZScoreNormalize"]
 
 import argparse
-import builtins
 import typing
 
 import intensity_normalization.errors as intnorme
 import intensity_normalization.normalize.base as intnormb
 import intensity_normalization.typing as intnormt
 
 
 class ZScoreNormalize(intnormb.LocationScaleCLIMixin, intnormb.SingleImageNormalizeCLI):
-    def __init__(self, *, norm_value: builtins.float = 1.0, **kwargs: typing.Any):
+    def __init__(self, *, norm_value: float = 1.0, **kwargs: typing.Any):
         """Voxel-wise subtract the mean and divide by the standard deviation."""
         super().__init__(norm_value=norm_value, **kwargs)
         self.voi: intnormt.ImageLike | None = None
 
     def calculate_location(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.float:
+    ) -> float:
         if self.voi is None:
             raise intnorme.NormalizationError("'voi' needs to be set.")
-        loc: builtins.float = float(self.voi.mean())
+        loc: float = float(self.voi.mean())
         return loc
 
     def calculate_scale(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
         *,
         modality: intnormt.Modality = intnormt.Modality.T1,
-    ) -> builtins.float:
+    ) -> float:
         if self.voi is None:
             raise intnorme.NormalizationError("'voi' needs to be set.")
-        scale: builtins.float = float(self.voi.std())
+        scale: float = float(self.voi.std())
         return scale
 
     def setup(
         self,
         image: intnormt.ImageLike,
         /,
         mask: intnormt.ImageLike | None = None,
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/plot/histogram.py` & `intensity_normalization-2.2.4/intensity_normalization/plot/histogram.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["HistogramPlotter", "plot_histogram"]
 
 import argparse
-import builtins
 import collections.abc
 import logging
 import pathlib
 import typing
 import warnings
 
 import matplotlib.pyplot as plt
@@ -34,17 +33,17 @@
     sns = None
 
 
 class HistogramPlotter(intnormcli.DirectoryCLI):
     def __init__(
         self,
         *,
-        figsize: builtins.tuple[builtins.int, builtins.int] = (12, 10),
-        alpha: builtins.float = 0.8,
-        title: builtins.str | None = None,
+        figsize: tuple[int, int] = (12, 10),
+        alpha: float = 0.8,
+        title: str | None = None,
     ):
         super().__init__()
         self.figsize = figsize
         self.alpha = alpha
         self.title = title
 
     def __call__(
@@ -89,40 +88,40 @@
 
     def from_directories(
         self,
         image_dir: intnormt.PathLike,
         /,
         mask_dir: intnormt.PathLike | None = None,
         *,
-        ext: builtins.str = "nii*",
-        exclude: collections.abc.Sequence[builtins.str] = ("membership",),
+        ext: str = "nii*",
+        exclude: collections.abc.Sequence[str] = ("membership",),
         **kwargs: typing.Any,
     ) -> plt.Axes:
         images, masks = intnormio.gather_images_and_masks(
             image_dir, mask_dir, ext=ext, exclude=exclude
         )
         return self(images, masks, **kwargs)
 
     @staticmethod
-    def name() -> builtins.str:
+    def name() -> str:
         return "hist"
 
     @staticmethod
-    def fullname() -> builtins.str:
+    def fullname() -> str:
         return "Histogram plotter"
 
     @staticmethod
-    def description() -> builtins.str:
+    def description() -> str:
         return "Plot the histogram of an image."
 
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             description=desc,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         parser.add_argument(
@@ -212,18 +211,18 @@
 
 def plot_histogram(
     image: intnormt.ImageLike,
     /,
     mask: intnormt.ImageLike | None = None,
     *,
     ax: plt.Axes | None = None,
-    n_bins: builtins.int = 200,
-    log: builtins.bool = True,
-    alpha: builtins.float = 0.8,
-    linewidth: builtins.float = 3.0,
+    n_bins: int = 200,
+    log: bool = True,
+    alpha: float = 0.8,
+    linewidth: float = 3.0,
     **kwargs: typing.Any,
 ) -> plt.Axes:
     """
     plots the histogram of the intensities of a numpy array within a given brain mask
     or estimated foreground mask (the estimate is just all intensities above the mean)
 
     Args:
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/typing.py` & `intensity_normalization-2.2.4/intensity_normalization/typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,45 +28,44 @@
     "probability_float_or_none",
     "save_file_path",
     "SplitFilename",
     "TissueType",
 ]
 
 import argparse
-import builtins
 import collections.abc
 import enum
 import os
 import pathlib
 import typing
 
 import numpy as np
 import numpy.typing as npt
 
 import intensity_normalization as intnorm
 
-ArgType = typing.Union[argparse.Namespace, builtins.list[builtins.str], None]
-PathLike = typing.Union[builtins.str, os.PathLike]
+ArgType = typing.Union[argparse.Namespace, list[str], None]
+PathLike = typing.Union[str, os.PathLike]
 ShapeLike = typing.Union[
     typing.SupportsIndex, collections.abc.Sequence[typing.SupportsIndex]
 ]
 
 _MODALITIES = [(vm.upper(), vm) for vm in sorted(intnorm.VALID_MODALITIES)]
 
 
 class Modality(enum.Enum):
-    FLAIR: builtins.str = "flair"
-    MD: builtins.str = "md"
-    OTHER: builtins.str = "other"
-    PD: builtins.str = "pd"
-    T1: builtins.str = "t1"
-    T2: builtins.str = "t2"
+    FLAIR: str = "flair"
+    MD: str = "md"
+    OTHER: str = "other"
+    PD: str = "pd"
+    T1: str = "t1"
+    T2: str = "t2"
 
     @classmethod
-    def from_string(cls: typing.Type, string: builtins.str | Modality) -> Modality:
+    def from_string(cls: typing.Type, string: str | Modality) -> Modality:
         if isinstance(string, cls):
             modality: Modality = string
             return modality
         for name, value in _MODALITIES:
             if string == value:
                 modality = getattr(cls, name)
                 return modality
@@ -76,54 +75,54 @@
 
 # not ideal DRY, but avoid functional enum API for better IDE support & flake8
 if set(m.value for m in Modality) != set(intnorm.VALID_MODALITIES):
     raise RuntimeError("Modalities enum out of sync with VALID_MODALITIES.")
 
 
 class TissueType(enum.Enum):
-    CSF: builtins.str = "csf"
-    GM: builtins.str = "gm"
-    WM: builtins.str = "wm"
+    CSF: str = "csf"
+    GM: str = "gm"
+    WM: str = "wm"
 
     @classmethod
-    def from_string(cls, string: builtins.str) -> TissueType:
+    def from_string(cls, string: str) -> TissueType:
         if string.lower() == "csf":
             return TissueType.CSF
         elif string.lower() == "gm":
             return TissueType.GM
         elif string.lower() == "wm":
             return TissueType.WM
         else:
             raise ValueError(f"'string' must be 'csf', 'gm', or 'wm'. Got '{string}'.")
 
-    def to_int(self) -> builtins.int:
+    def to_int(self) -> int:
         if self == TissueType.CSF:
             return 0
         elif self == TissueType.GM:
             return 1
         elif self == TissueType.WM:
             return 2
         else:
             raise ValueError("Unexpected enum.")
 
-    def to_fullname(self) -> builtins.str:
+    def to_fullname(self) -> str:
         if self == TissueType.CSF:
             return "Cerebrospinal fluid"
         elif self == TissueType.GM:
             return "Grey matter"
         elif self == TissueType.WM:
             return "White matter"
         else:
             raise ValueError("Unexpected enum.")
 
 
 class SplitFilename(typing.NamedTuple):
     path: pathlib.Path
-    base: builtins.str
-    ext: builtins.str
+    base: str
+    ext: str
 
 
 interp_type_dict = dict(
     linear=0,
     nearest_neighbor=1,
     gaussian=2,
     windowed_sinc=3,
@@ -287,157 +286,155 @@
     }
 )
 
 
 def return_none(
     func: typing.Callable[[typing.Any, typing.Any], typing.Any]
 ) -> typing.Callable[[typing.Any, typing.Any], typing.Any]:
-    def new_func(self: builtins.object, string: typing.Any) -> typing.Any:
+    def new_func(self: object, string: typing.Any) -> typing.Any:
         if string is None:
             return None
         elif isinstance(string, str):
             if string.lower() in ("none", "null"):
                 return None
         return func(self, string)
 
     return new_func
 
 
 class _ParseType:
     @property
-    def __name__(self) -> builtins.str:
+    def __name__(self) -> str:
         name = self.__class__.__name__
         assert isinstance(name, str)
         return name
 
-    def __str__(self) -> builtins.str:
+    def __str__(self) -> str:
         return self.__name__
 
 
 class save_file_path(_ParseType):
-    def __call__(self, string: builtins.str) -> pathlib.Path:
+    def __call__(self, string: str) -> pathlib.Path:
         if not string.isprintable():
             msg = f"'{string}' must only contain printable characters."
             raise argparse.ArgumentTypeError(msg)
         path = pathlib.Path(string)
         return path
 
 
 class dir_path(_ParseType):
-    def __call__(self, string: builtins.str) -> builtins.str:
+    def __call__(self, string: str) -> str:
         path = pathlib.Path(string)
         if not path.is_dir():
             msg = f"'{string}' is not a valid directory path."
             raise argparse.ArgumentTypeError(msg)
         return str(path.resolve())
 
 
 class file_path(_ParseType):
-    def __call__(self, string: builtins.str) -> builtins.str:
+    def __call__(self, string: str) -> str:
         path = pathlib.Path(string)
         if not path.is_file():
             msg = f"'{string}' is not a valid file path."
             raise argparse.ArgumentTypeError(msg)
         return str(path)
 
 
 class positive_float(_ParseType):
-    def __call__(self, string: builtins.str) -> builtins.float:
+    def __call__(self, string: str) -> float:
         num = float(string)
         if num <= 0.0:
             msg = f"'{string}' needs to be a positive float."
             raise argparse.ArgumentTypeError(msg)
         return num
 
 
 class positive_int(_ParseType):
-    def __call__(self, string: builtins.str) -> builtins.int:
+    def __call__(self, string: str) -> int:
         num = int(string)
         if num <= 0:
             msg = f"'{string}' needs to be a positive integer."
             raise argparse.ArgumentTypeError(msg)
         return num
 
 
 class positive_odd_int_or_none(_ParseType):
     @return_none
-    def __call__(self, string: builtins.str) -> builtins.int | None:
+    def __call__(self, string: str) -> int | None:
         num = int(string)
         if num <= 0 or not (num % 2):
             msg = f"'{string}' needs to be a positive odd integer."
             raise argparse.ArgumentTypeError(msg)
         return num
 
 
 class positive_int_or_none(_ParseType):
     @return_none
-    def __call__(self, string: builtins.str) -> builtins.int | None:
+    def __call__(self, string: str) -> int | None:
         return positive_int()(string)
 
 
 class nonnegative_int(_ParseType):
-    def __call__(self, string: builtins.str) -> builtins.int:
+    def __call__(self, string: str) -> int:
         num = int(string)
         if num < 0:
             msg = f"'{string}' needs to be a non-negative integer."
             raise argparse.ArgumentTypeError(msg)
         return num
 
 
 class nonnegative_float(_ParseType):
-    def __call__(self, string: builtins.str) -> builtins.float:
+    def __call__(self, string: str) -> float:
         num = float(string)
         if num < 0.0:
             msg = f"'{string}' needs to be a non-negative float."
             raise argparse.ArgumentTypeError(msg)
         return num
 
 
 class probability_float(_ParseType):
-    def __call__(self, string: builtins.str) -> builtins.float:
+    def __call__(self, string: str) -> float:
         num = float(string)
         if num < 0.0 or num > 1.0:
             msg = f"'{string}' needs to be between 0 and 1."
             raise argparse.ArgumentTypeError(msg)
         return num
 
 
 class probability_float_or_none(_ParseType):
     @return_none
-    def __call__(self, string: builtins.str) -> builtins.float | None:
+    def __call__(self, string: str) -> float | None:
         return probability_float()(string)
 
 
 class NewParseType:
-    def __init__(
-        self, func: typing.Callable[[typing.Any], typing.Any], name: builtins.str
-    ):
+    def __init__(self, func: typing.Callable[[typing.Any], typing.Any], name: str):
         self.name = name
         self.func = func
 
     def __str__(self) -> str:
         return self.name
 
     def __call__(self, val: typing.Any) -> typing.Any:
         return self.func(val)
 
 
 def new_parse_type(
-    func: typing.Callable[[typing.Any], typing.Any], name: builtins.str
+    func: typing.Callable[[typing.Any], typing.Any], name: str
 ) -> NewParseType:
     return NewParseType(func, name)
 
 
 S_co = typing.TypeVar("S_co", bound="ImageLike", covariant=True)
 T_co = typing.TypeVar("T_co", bound="ImageLike", covariant=True)
 U_co = typing.TypeVar("U_co", bound="ImageLike", covariant=True)
 
 NBit = typing.TypeVar("NBit", bound=npt.NBitBase)
-Float = typing.Union[np.floating[NBit], builtins.float]
-Int = typing.Union[np.integer[NBit], builtins.int]
+Float = typing.Union[np.floating[NBit], float]
+Int = typing.Union[np.integer[NBit], int]
 
 
 class ImageLike(typing.Protocol[S_co, T_co, U_co]):
     """support anything that implements the methods here"""
 
     def __gt__(self: T_co, other: typing.Any) -> U_co:
         ...
@@ -483,42 +480,42 @@
 
     @property
     def ndim(self) -> Int:
         ...
 
     def any(
         self,
-        axis: builtins.int | builtins.tuple[builtins.int, ...] | None = None,
+        axis: int | tuple[int, ...] | None = None,
     ) -> typing.Any:
         ...
 
     def nonzero(self) -> typing.Any:
         ...
 
     def squeeze(self) -> typing.Any:
         ...
 
     @property
-    def shape(self) -> builtins.tuple[builtins.int, ...]:
+    def shape(self) -> tuple[int, ...]:
         ...
 
-    def mean(self) -> builtins.float:
+    def mean(self) -> float:
         ...
 
-    def std(self) -> builtins.float:
+    def std(self) -> float:
         ...
 
-    def min(self) -> builtins.float:
+    def min(self) -> float:
         ...
 
     def flatten(self: T_co) -> T_co:
         ...
 
     def reshape(
         self: T_co,
         *shape: typing.SupportsIndex,
         order: typing.Literal["A", "C", "F"] | None = ...,
     ) -> T_co:
         ...
 
-    def transpose(self: T_co, *axes: builtins.int) -> T_co:
+    def transpose(self: T_co, *axes: int) -> T_co:
         ...
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/util/coregister.py` & `intensity_normalization-2.2.4/intensity_normalization/util/coregister.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["register", "Registrator"]
 
 import argparse
-import builtins
 import collections.abc
 import logging
 import typing
 
 import nibabel as nib
 import numpy as np
 
@@ -24,48 +23,48 @@
 
 try:
     import ants
 except ImportError as ants_imp_exn:
     msg = "ANTsPy not installed. Install antspyx to use co-registration."
     raise RuntimeError(msg) from ants_imp_exn
 
+ValidImage = typing.Union[nib.nifti1.Nifti1Image, ants.ANTsImage, intnormt.ImageLike]
 
-def to_ants(
-    image: nib.Nifti1Image | ants.ANTsImage | intnormt.ImageLike, /
-) -> ants.ANTsImage:
+
+def to_ants(image: ValidImage, /) -> ants.ANTsImage:
     if isinstance(image, ants.ANTsImage):
         ants_image = image
-    elif isinstance(image, nib.Nifti1Image):
+    elif isinstance(image, nib.nifti1.Nifti1Image):
         ants_image = ants.from_nibabel(image)
     elif isinstance(image, np.ndarray):
         ants_image = ants.from_numpy(image)
     else:
         msg = "Provided image must be an ANTsImage, Nifti1Image,"
         msg += f" or (a subclass of) np.ndarray. Got '{type(image)}'."
         raise ValueError(msg)
     return ants_image
 
 
 def register(
-    image: nib.Nifti1Image | ants.ANTsImage | intnormt.ImageLike,
+    image: ValidImage,
     /,
-    template: nib.Nifti1Image | ants.ANTsImage | intnormt.ImageLike | None = None,
+    template: typing.Optional[ValidImage] = None,
     *,
-    type_of_transform: builtins.str = "Affine",
-    interpolator: builtins.str = "bSpline",
-    metric: builtins.str = "mattes",
-    initial_rigid: builtins.bool = True,
-    template_mask: nib.Nifti1Image | ants.ANTsImage | intnormt.ImageLike | None = None,
-) -> nib.Nifti1Image | ants.ANTsImage:
+    type_of_transform: str = "Affine",
+    interpolator: str = "bSpline",
+    metric: str = "mattes",
+    initial_rigid: bool = True,
+    template_mask: typing.Optional[ValidImage] = None,
+) -> nib.nifti1.Nifti1Image | ants.ANTsImage:
     if template is None:
         standard_mni = ants.get_ants_data("mni")
         template = ants.image_read(standard_mni)
     else:
         template = to_ants(template)
-    is_nibabel = isinstance(image, nib.Nifti1Image)
+    is_nibabel = isinstance(image, nib.nifti1.Nifti1Image)
     image = to_ants(image)
     if initial_rigid:
         logger.debug("Doing initial rigid registration.")
         transforms = ants.registration(
             fixed=template,
             moving=image,
             type_of_transform="Rigid",
@@ -94,20 +93,20 @@
     )
     return registered.to_nibabel() if is_nibabel else registered
 
 
 class Registrator(intnormcli.SingleImageCLI):
     def __init__(
         self,
-        template: nib.Nifti1Image | ants.ANTsImage = None,
+        template: nib.nifti1.Nifti1Image | ants.ANTsImage = None,
         *,
-        type_of_transform: builtins.str = "Affine",
-        interpolator: builtins.str = "bSpline",
-        metric: builtins.str = "mattes",
-        initial_rigid: builtins.bool = True,
+        type_of_transform: str = "Affine",
+        interpolator: str = "bSpline",
+        metric: str = "mattes",
+        initial_rigid: bool = True,
     ):
         super().__init__()
         if template is None:
             logger.info("Using MNI (in RAS orientation) as template.")
             standard_mni = ants.get_ants_data("mni")
             self.template = ants.image_read(standard_mni).reorient_image2("RAS")
         else:
@@ -116,66 +115,68 @@
         self.type_of_transform = type_of_transform
         self.interpolator = interpolator
         self.metric = metric
         self.initial_rigid = initial_rigid
 
     def __call__(
         self,
-        image: nib.Nifti1Image | ants.ANTsImage,
+        image: nib.nifti1.Nifti1Image | ants.ANTsImage,
         /,
         *args: typing.Any,
         **kwargs: typing.Any,
-    ) -> nib.Nifti1Image | ants.ANTsImage:
+    ) -> nib.nifti1.Nifti1Image | ants.ANTsImage:
         return register(
             image,
             template=self.template,
             type_of_transform=self.type_of_transform,
             interpolator=self.interpolator,
             metric=self.metric,
             initial_rigid=self.initial_rigid,
         )
 
     def register_images(
-        self, images: collections.abc.Sequence[nib.Nifti1Image | ants.ANTsImage], /
-    ) -> collections.abc.Sequence[nib.Nifti1Image | ants.ANTsImage]:
+        self,
+        images: collections.abc.Sequence[nib.nifti1.Nifti1Image | ants.ANTsImage],
+        /,
+    ) -> collections.abc.Sequence[nib.nifti1.Nifti1Image | ants.ANTsImage]:
         return [self(image) for image in images]
 
     def register_images_to_templates(
         self,
-        images: collections.abc.Sequence[nib.Nifti1Image | ants.ANTsImage],
+        images: collections.abc.Sequence[nib.nifti1.Nifti1Image | ants.ANTsImage],
         /,
         *,
-        templates: collections.abc.Sequence[nib.Nifti1Image | ants.ANTsImage],
-    ) -> collections.abc.Sequence[nib.Nifti1Image | ants.ANTsImage]:
+        templates: collections.abc.Sequence[nib.nifti1.Nifti1Image | ants.ANTsImage],
+    ) -> collections.abc.Sequence[nib.nifti1.Nifti1Image | ants.ANTsImage]:
         assert len(images) == len(templates)
         registered = []
         original_template = self.template
         for image, template in zip(images, templates):
             self.template = template
             registered.append(self(image))
         self.template = original_template
         return registered
 
     @staticmethod
-    def name() -> builtins.str:
+    def name() -> str:
         return "registered"
 
     @staticmethod
-    def fullname() -> builtins.str:
+    def fullname() -> str:
         return Registrator.name()
 
     @staticmethod
-    def description() -> builtins.str:
+    def description() -> str:
         return "Co-register an image to MNI or another image."
 
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             description=desc,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         parser.add_argument(
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/util/histogram_tools.py` & `intensity_normalization-2.2.4/intensity_normalization/util/histogram_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Process the histograms of MR (brain) images
 Author: Jacob Reinhold <jcreinhold@gmail.com>
 Created on: 01 Jun 2021
 """
 
+from __future__ import annotations
+
 __all__ = [
     "get_first_tissue_mode",
     "get_largest_tissue_mode",
     "get_last_tissue_mode",
     "get_tissue_mode",
     "smooth_histogram",
 ]
 
-import builtins
-
 import numpy as np
 import scipy.signal
 import statsmodels.api as sm
 
 import intensity_normalization as intnorm
 import intensity_normalization.typing as intnormt
 
 
 def smooth_histogram(
     image: intnormt.ImageLike, /
-) -> builtins.tuple[intnormt.ImageLike, intnormt.ImageLike]:
+) -> tuple[intnormt.ImageLike, intnormt.ImageLike]:
     """Use kernel density estimate to get smooth histogram
 
     Args:
         image: array of image data (like an np.ndarray)
 
     Returns:
         grid: domain of the pdf
@@ -38,35 +38,35 @@
     kde = sm.nonparametric.KDEUnivariate(image_vec)
     kde.fit(kernel="gau", bw=bandwidth, gridsize=80, fft=True)
     pdf = 100.0 * kde.density
     grid = kde.support
     return grid, pdf
 
 
-def get_largest_tissue_mode(image: intnormt.ImageLike, /) -> builtins.float:
+def get_largest_tissue_mode(image: intnormt.ImageLike, /) -> float:
     """Mode of the largest tissue class
 
     Args:
         image: array of image data (like an np.ndarray)
 
     Returns:
         largest_tissue_mode: value of the largest tissue mode
     """
     grid, pdf = smooth_histogram(image)
-    largest_tissue_mode: builtins.float = float(grid[int(np.argmax(pdf))])
+    largest_tissue_mode: float = float(grid[int(np.argmax(pdf))])
     return largest_tissue_mode
 
 
 def get_last_tissue_mode(
     image: intnormt.ImageLike,
     /,
     *,
-    remove_tail: builtins.bool = True,
-    tail_percentage: builtins.float = 96.0,
-) -> builtins.float:
+    remove_tail: bool = True,
+    tail_percentage: float = 96.0,
+) -> float:
     """Mode of the highest-intensity tissue class
 
     Args:
         image: array of image data (like an np.ndarray)
         remove_tail: remove tail from histogram
         tail_percentage: if remove_tail, use the
             histogram below this percentage
@@ -74,30 +74,30 @@
     Returns:
         last_tissue_mode: mode of the highest-intensity tissue class
     """
     if not (0.0 < tail_percentage < 100.0):
         msg = f"'tail_percentage' must be in (0, 100). Got '{tail_percentage}'."
         raise ValueError(msg)
     if remove_tail:
-        threshold: builtins.float = float(np.percentile(image, tail_percentage))
+        threshold: float = float(np.percentile(image, tail_percentage))
         valid_mask: intnormt.ImageLike = image <= threshold
         image = image[valid_mask]
     grid, pdf = smooth_histogram(image)
     maxima = scipy.signal.argrelmax(pdf)[0]
     last_tissue_mode: float = grid[maxima[-1]]
     return last_tissue_mode
 
 
 def get_first_tissue_mode(
     image: intnormt.ImageLike,
     /,
     *,
-    remove_tail: builtins.bool = True,
-    tail_percentage: builtins.float = 99.0,
-) -> builtins.float:
+    remove_tail: bool = True,
+    tail_percentage: float = 99.0,
+) -> float:
     """Mode of the lowest-intensity tissue class
 
     Args:
         image: array of image data (like an np.ndarray)
         remove_tail: remove tail from histogram
         tail_percentage: if remove_tail, use the
             histogram below this percentage
@@ -105,26 +105,26 @@
     Returns:
         first_tissue_mode: mode of the lowest-intensity tissue class
     """
     if not (0.0 < tail_percentage < 100.0):
         msg = f"'tail_percentage' must be in (0, 100). Got '{tail_percentage}'."
         raise ValueError(msg)
     if remove_tail:
-        threshold: builtins.float = float(np.percentile(image, tail_percentage))
+        threshold: float = float(np.percentile(image, tail_percentage))
         valid_mask: intnormt.ImageLike = image <= threshold
         image = image[valid_mask]
     grid, pdf = smooth_histogram(image)
     maxima = scipy.signal.argrelmax(pdf)[0]
     first_tissue_mode: float = grid[maxima[0]]
     return first_tissue_mode
 
 
 def get_tissue_mode(
     image: intnormt.ImageLike, /, *, modality: intnormt.Modality
-) -> builtins.float:
+) -> float:
     """Find the appropriate tissue mode given a modality"""
     modality_ = modality.value
     if modality_ in intnorm.PEAK["last"]:
         mode = get_last_tissue_mode(image)
     elif modality_ in intnorm.PEAK["largest"]:
         mode = get_largest_tissue_mode(image)
     elif modality_ in intnorm.PEAK["first"]:
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/util/io.py` & `intensity_normalization-2.2.4/intensity_normalization/util/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,68 +9,67 @@
     "gather_images",
     "gather_images_and_masks",
     "glob_ext",
     "split_filename",
     "zip_with_nones",
 ]
 
-import builtins
 import collections.abc
 import pathlib
 import typing
 
 import pymedio.image as mioi
 
 import intensity_normalization.typing as intnormt
 
-PymedioImageList = builtins.list[mioi.Image]
+PymedioImageList = list[mioi.Image]
 PymedioMaskListOrNone = typing.Union[PymedioImageList, None]
 
 
 def gather_images(
     dirpath: intnormt.PathLike,
     *,
-    ext: builtins.str = "nii*",
-    exclude: collections.abc.Sequence[builtins.str] = (),
+    ext: str = "nii*",
+    exclude: collections.abc.Sequence[str] = (),
 ) -> PymedioImageList:
     """return all images of extension `ext` from a directory"""
     if not isinstance(dirpath, pathlib.Path):
         dirpath = pathlib.Path(dirpath)
     if not dirpath.is_dir():
         raise ValueError("'dirpath' must be a valid directory.")
     image_filenames = glob_ext(dirpath, ext=ext, exclude=exclude)
     images: PymedioImageList = []
     for fn in image_filenames:
-        image = mioi.Image.from_path(fn)
+        image: mioi.Image = mioi.Image.from_path(fn)
         images.append(image)
     return images
 
 
 def gather_images_and_masks(
     image_dir: intnormt.PathLike,
     mask_dir: intnormt.PathLike | None = None,
     *,
-    ext: builtins.str = "nii*",
-    exclude: collections.abc.Sequence[builtins.str] = (),
-) -> builtins.tuple[PymedioImageList, PymedioMaskListOrNone]:
+    ext: str = "nii*",
+    exclude: collections.abc.Sequence[str] = (),
+) -> tuple[PymedioImageList, PymedioMaskListOrNone]:
     images = gather_images(image_dir, ext=ext, exclude=exclude)
     masks: PymedioMaskListOrNone
     if mask_dir is not None:
         masks = gather_images(mask_dir, ext=ext, exclude=exclude)
     else:
         masks = None
     return images, masks
 
 
 def glob_ext(
     dirpath: intnormt.PathLike,
     *,
-    ext: builtins.str = "nii*",
-    exclude: collections.abc.Sequence[builtins.str] = (),
-) -> builtins.list[pathlib.Path]:
+    ext: str = "nii*",
+    exclude: collections.abc.Sequence[str] = (),
+) -> list[pathlib.Path]:
     """return a sorted list of ext files for a given directory path"""
     dirpath = pathlib.Path(dirpath)
     if not dirpath.is_dir():
         raise ValueError("'dirpath' must be a directory.")
     filenames = sorted(
         dp
         for dp in dirpath.resolve().glob(f"*.{ext}")
@@ -79,15 +78,15 @@
     return filenames
 
 
 def split_filename(
     filepath: intnormt.PathLike,
     /,
     *,
-    resolve: builtins.bool = False,
+    resolve: bool = False,
 ) -> intnormt.SplitFilename:
     """split a filepath into the directory, base, and extension
     Examples:
         >>> split_filename("path/base.ext")
         SplitFilename(path=PosixPath('path'), base='base', ext='.ext')
     """
     if not str(filepath):
@@ -103,42 +102,42 @@
         base = str(_base.stem)
         ext = ext2 + ext
     else:
         base = str(_base)
     return intnormt.SplitFilename(pathlib.Path(path), base, ext)
 
 
-Zipped = typing.Generator[builtins.tuple[typing.Any, ...], None, None]
+Zipped = typing.Generator[tuple[typing.Any, ...], None, None]
 
 
 def zip_with_nones(*args: typing.Sequence[typing.Any] | None) -> Zipped:
     """zip sequence args but if an arg is None, yield None in that argument index
     Examples:
         >>> for x, y, z in zip_with_nones((1, 2), None, ("a", "b")):
         ...    print(x, y, z)
         1 None a
         2 None b
     """
-    _args: builtins.list[typing.Any] = list(args)
-    none_indices: builtins.list[builtins.int] = []
-    length: builtins.int | None = None
+    _args: list[typing.Any] = list(args)
+    none_indices: list[int] = []
+    length: int | None = None
     for i, seq_or_none in enumerate(args):
         try:
             _length = len(seq_or_none)  # type: ignore[arg-type]
         except TypeError:
             if seq_or_none is not None:
                 raise RuntimeError("Only sequences or 'None' allowed.")
             none_indices.append(i)
         else:
             if length is None:
                 length = _length
             elif length is not None and length != _length:
                 raise RuntimeError("All sequences should be the same length.")
 
-    def nones(length: builtins.int) -> typing.Generator[None, None, None]:
+    def nones(length: int) -> typing.Generator[None, None, None]:
         for _ in range(length):
             yield None
 
     if length is None:
         raise RuntimeError("At least one argument needs to be a sequence.")
 
     for idx in none_indices:
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/util/preprocess.py` & `intensity_normalization-2.2.4/intensity_normalization/util/preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["preprocess", "Preprocessor"]
 
 import argparse
-import builtins
 import logging
 import typing
 
 import nibabel as nib
 import numpy as np
 import pymedio.image as mioi
 
@@ -36,20 +35,20 @@
 
 
 def preprocess(
     image: intnormt.ImageLike,
     /,
     mask: intnormt.ImageLike | None = None,
     *,
-    resolution: builtins.tuple[builtins.float, ...] | None = None,
-    orientation: builtins.str = "RAS",
-    n4_convergence_options: builtins.dict[builtins.str, typing.Any] | None = None,
-    interp_type: builtins.str = "linear",
-    second_n4_with_smoothed_mask: builtins.bool = True,
-) -> builtins.tuple[mioi.Image, mioi.Image]:
+    resolution: tuple[float, ...] | None = None,
+    orientation: str = "RAS",
+    n4_convergence_options: dict[str, typing.Any] | None = None,
+    interp_type: str = "linear",
+    second_n4_with_smoothed_mask: bool = True,
+) -> tuple[mioi.Image, mioi.Image]:
     """Preprocess an MR image
 
     Preprocess an MR image according to a simple scheme:
     1) N4 bias field correction
     2) resample to X mm x Y mm x ...
     3) reorient images to RAI
 
@@ -107,29 +106,29 @@
                 resolution,
                 use_voxels=False,
                 interp_type=intnormt.interp_type_dict[interp_type],
             )
     ants_image = ants_image.reorient_image2(orientation)
     ants_mask = ants_mask.reorient_image2(orientation)
     _image = ants_image.to_nibabel()
-    pp_image = mioi.Image(_image.get_fdata(), _image.affine)
+    pp_image: mioi.Image = mioi.Image(_image.get_fdata(), _image.affine)
     _mask = ants_mask.to_nibabel()
-    pp_mask = mioi.Image(_mask.get_fdata(), _mask.affine)
+    pp_mask: mioi.Image = mioi.Image(_mask.get_fdata(), _mask.affine)
     return pp_image, pp_mask
 
 
 class Preprocessor(intnormcli.SingleImageCLI):
     def __init__(
         self,
         *,
-        resolution: builtins.tuple[builtins.float, ...] | None = None,
-        orientation: builtins.str = "RAI",
-        n4_convergence_options: builtins.dict[builtins.str, typing.Any] | None = None,
-        interp_type: builtins.str = "linear",
-        second_n4_with_smoothed_mask: builtins.bool = True,
+        resolution: tuple[float, ...] | None = None,
+        orientation: str = "RAI",
+        n4_convergence_options: dict[str, typing.Any] | None = None,
+        interp_type: str = "linear",
+        second_n4_with_smoothed_mask: bool = True,
     ):
         super().__init__()
         self.resolution = resolution
         self.orientation = orientation
         self.n4_convergence_options = n4_convergence_options
         self.interp_type = interp_type
         self.second_n4_with_smoothed_mask = second_n4_with_smoothed_mask
@@ -165,16 +164,16 @@
         desc = "Basic preprocessing of an MR image: "
         desc += "bias field-correction, resampling, and reorientation."
         return desc
 
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             description=desc,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         parser.add_argument(
@@ -254,15 +253,15 @@
 
     @staticmethod
     def load_image(image_path: intnormt.PathLike) -> ants.ANTsImage:
         return ants.image_read(image_path)
 
 
 def _to_ants(image: typing.Any) -> ants.ANTsImage:
-    if isinstance(image, nib.Nifti1Image):
+    if isinstance(image, nib.nifti1.Nifti1Image):
         ants_image = ants.from_nibabel(image)
     elif isinstance(image, mioi.Image):
         ants_image = ants.from_numpy(
             image, origin=image.origin, spacing=image.spacing, direction=image.direction
         )
     elif isinstance(image, np.ndarray):
         ants_image = ants.from_numpy(image)
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization/util/tissue_membership.py` & `intensity_normalization-2.2.4/intensity_normalization/util/tissue_membership.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["find_tissue_memberships", "TissueMembershipFinder"]
 
 import argparse
-import builtins
 import operator
 import typing
 
 import numpy as np
 import numpy.typing as npt
 import pymedio.image as mioi
 from skfuzzy import cmeans
@@ -23,16 +22,16 @@
 
 
 def find_tissue_memberships(
     image: intnormt.ImageLike,
     /,
     mask: intnormt.ImageLike | None = None,
     *,
-    hard_segmentation: builtins.bool = False,
-    n_classes: builtins.int = 3,
+    hard_segmentation: bool = False,
+    n_classes: int = 3,
 ) -> mioi.Image:
     """Tissue memberships for a T1-w brain image with fuzzy c-means
 
     Args:
         image: image to find tissue masks for (must be T1-w)
         mask: mask covering the brain of image (none if already skull-stripped)
         hard_segmentation: pick the maximum membership as the true class in output
@@ -46,15 +45,15 @@
     if n_classes <= 0:
         raise ValueError(f"n_classes must be positive. Got '{n_classes}'.")
     if mask is None:
         mask = _image > 0.0
     else:
         mask = mask > 0.0
     assert mask is not None
-    foreground_size = mask.sum()
+    foreground_size = typing.cast(int, mask.sum())
     foreground = _image[mask].reshape(-1, foreground_size)
     centers, memberships_, *_ = cmeans(foreground, n_classes, 2, 0.005, 50)
     # sort the tissue memberships to CSF/GM/WM (assuming T1-w image)
     sorted_memberships = sorted(zip(centers, memberships_), key=operator.itemgetter(0))
     memberships = [m for _, m in sorted_memberships]
     tissue_mask = np.zeros(_image.shape + (n_classes,))
     for i in range(n_classes):
@@ -62,22 +61,22 @@
     if hard_segmentation:
         tmp_mask = np.zeros(_image.shape)
         masked = tissue_mask[mask]
         tmp_mask[mask] = np.argmax(masked, axis=1) + 1
         tissue_mask = tmp_mask
     affine: npt.NDArray | None
     if hasattr(image, "affine"):
-        affine = image.affine.copy()  # type: ignore[attr-defined]
+        affine = image.affine.copy()
     else:
         affine = None
     return mioi.Image(tissue_mask, affine=affine)
 
 
 class TissueMembershipFinder(intnormcli.SingleImageCLI):
-    def __init__(self, hard_segmentation: builtins.bool = False):
+    def __init__(self, hard_segmentation: bool = False):
         super().__init__()
         self.hard_segmentation = hard_segmentation
 
     def __call__(
         self,
         image: intnormt.ImageLike,
         /,
@@ -88,30 +87,30 @@
             image,
             mask,
             hard_segmentation=self.hard_segmentation,
         )
         return tissue_memberships
 
     @staticmethod
-    def name() -> builtins.str:
+    def name() -> str:
         return "tm"
 
     @staticmethod
-    def fullname() -> builtins.str:
+    def fullname() -> str:
         return "tissue_membership"
 
     @staticmethod
-    def description() -> builtins.str:
+    def description() -> str:
         return "Find tissue memberships of an MR image."
 
     @classmethod
     def get_parent_parser(
         cls,
-        desc: builtins.str,
-        valid_modalities: builtins.frozenset[builtins.str] = intnorm.VALID_MODALITIES,
+        desc: str,
+        valid_modalities: frozenset[str] = intnorm.VALID_MODALITIES,
         **kwargs: typing.Any,
     ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             description=desc,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         parser.add_argument(
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization.egg-info/PKG-INFO` & `intensity_normalization-2.2.4/intensity_normalization.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: intensity-normalization
-Version: 2.2.3
+Version: 2.2.4
 Summary: normalize the intensities of various MR image modalities
 Home-page: https://github.com/jcreinhold/intensity-normalization
 Author: Jacob Reinhold
 Author-email: jcreinhold@gmail.com
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/jcreinhold/intensity-normalization/issues
 Project-URL: Documentation, https://intensity-normalization.readthedocs.io/
 Keywords: intensity,normalization,mri
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
-Requires-Python: !=3.10.*,!=3.11.*,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: ants
 Provides-Extra: plot
 License-File: LICENSE
 
 =======================
 intensity-normalization
@@ -239,14 +237,19 @@
 .. [5] Iglesias, Juan Eugenio, Cheng-Yi Liu, Paul M. Thompson, and Zhuowen Tu. "Robust brain extraction across datasets and
        comparison with publicly available methods." IEEE transactions on medical imaging 30, no. 9 (2011): 1617-1634.
 
 =======
 History
 =======
 
+2.2.4 (2023-05-31)
+------------------
+
+* Update to allow Python >=3.9
+
 2.2.3 (2022-03-15)
 ------------------
 
 * Revert error on different image shapes from ``RavelNormalize``; it is required!
 
 2.2.2 (2022-03-15)
 ------------------
@@ -317,9 +320,7 @@
 
 * Major refactor to reduce redundancy, make code more usable outside of the CLIs, and generally improve code quality.
 
 1.4.0 (2021-03-16)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `intensity_normalization-2.2.3/intensity_normalization.egg-info/SOURCES.txt` & `intensity_normalization-2.2.4/intensity_normalization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/intensity_normalization.egg-info/entry_points.txt` & `intensity_normalization-2.2.4/intensity_normalization.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/setup.cfg` & `intensity_normalization-2.2.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: Implementation :: CPython
 	Typing :: Typed
 keywords = intensity, normalization, mri
 project_urls = 
 	Bug Tracker = https://github.com/jcreinhold/intensity-normalization/issues
 	Documentation = https://intensity-normalization.readthedocs.io/
 
@@ -34,15 +33,15 @@
 	pydicom>=2.2.2,<3
 	pymedio>=0.2.8,<1
 	scikit-fuzzy>=0.4.2,<1
 	scikit-image>=0.17,<1
 	scikit-learn>=0.24,<2
 	scipy>=1.5,<2
 	statsmodels>=0.12,<1
-python_requires = >=3.9, !=3.10.*, !=3.11.*
+python_requires = >=3.9
 include_package_data = True
 test_suite = tests
 zip_safe = False
 
 [options.packages.find]
 exclude = 
 	tests
@@ -71,15 +70,15 @@
 plot = 
 	matplotlib>=3,<4
 
 [options.package_data]
 intensity_normalization = py.typed
 
 [bumpversion]
-current_version = 2.2.3
+current_version = 2.2.4
 commit = True
 tag = False
 
 [bumpversion:file:intensity_normalization/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
@@ -93,15 +92,15 @@
 max-line-length = 88
 statistics = True
 
 [aliases]
 test = pytest
 
 [tool:pytest]
-addopts = --doctest-modules --ignore=setup.py
+addopts = --ignore=setup.py
 doctest_optionflags = NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL NUMBER
 testpaths = 
 	intensity_normalization
 	tests
 
 [egg_info]
 tag_build =
```

### Comparing `intensity_normalization-2.2.3/tests/conftest.py` & `intensity_normalization-2.2.4/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import builtins
 import pathlib
 import typing
 
 import nibabel as nib
 import numpy as np
 import pytest
 
@@ -24,15 +23,15 @@
     return image_dir
 
 
 @pytest.fixture
 def image(image_dir: pathlib.Path) -> pathlib.Path:
     image_data = np.random.randn(5, 5, 5)
     image_path = image_dir / "test_image.nii"
-    image = nib.Nifti1Image(image_data, np.eye(4))
+    image = nib.nifti1.Nifti1Image(image_data, np.eye(4))
     image.to_filename(image_path)
     return image_path
 
 
 @pytest.fixture
 def mask_dir(temp_dir: pathlib.Path) -> pathlib.Path:
     mask_dir = temp_dir / "mask"
@@ -47,25 +46,21 @@
     return mask_dir
 
 
 @pytest.fixture
 def mask(mask_dir: pathlib.Path) -> pathlib.Path:
     mask_data: np.ndarray = np.random.randint(0, 2, (5, 5, 5)).astype(np.float32)
     mask_path = mask_dir / "test_mask.nii"
-    mask = nib.Nifti1Image(mask_data, np.eye(4))
+    mask = nib.nifti1.Nifti1Image(mask_data, np.eye(4))
     mask.to_filename(mask_path)
     return mask_path
 
 
 @pytest.fixture
-def base_cli_image_args(
-    image: pathlib.Path, mask: pathlib.Path
-) -> typing.List[builtins.str]:
+def base_cli_image_args(image: pathlib.Path, mask: pathlib.Path) -> typing.List[str]:
     return f"{image} -m {mask}".split()
 
 
 @pytest.fixture
-def base_cli_dir_args(
-    image: pathlib.Path, mask: pathlib.Path
-) -> typing.List[builtins.str]:
+def base_cli_dir_args(image: pathlib.Path, mask: pathlib.Path) -> typing.List[str]:
     # use image, mask instead of image_dir, mask_dir so they are created
     return f"{image.parent} -m {mask.parent}".split()
```

### Comparing `intensity_normalization-2.2.3/tests/run_all_clis.sh` & `intensity_normalization-2.2.4/tests/run_all_clis.sh`

 * *Files identical despite different names*

### Comparing `intensity_normalization-2.2.3/tests/test_ants_required_funcs.py` & `intensity_normalization-2.2.4/tests/test_ants_required_funcs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Tests for ants-required `intensity_normalization` functions."""
 
-import builtins
 import pathlib
 import typing
 
 import numpy as np
 import pytest
 
 try:
@@ -16,48 +15,48 @@
 
 
 ANTSPY_DIR = pathlib.Path.home() / ".antspy"
 ANTSPY_DIR_EXISTS = ANTSPY_DIR.is_dir()
 
 
 @pytest.fixture
-def coregister_cli_args(image: pathlib.Path) -> typing.List[builtins.str]:
+def coregister_cli_args(image: pathlib.Path) -> typing.List[str]:
     return f"{image}".split()
 
 
 @pytest.mark.skipif(not ANTSPY_DIR_EXISTS, reason="ANTsPy directory wasn't found.")
-def test_coregister_mni_cli(coregister_cli_args: typing.List[builtins.str]) -> None:
+def test_coregister_mni_cli(coregister_cli_args: typing.List[str]) -> None:
     retval = coregister_main(coregister_cli_args)
     assert retval == 0
 
 
 @pytest.fixture
 def coregister_template_cli_args(
     image: pathlib.Path, mask: pathlib.Path
-) -> typing.List[builtins.str]:
+) -> typing.List[str]:
     return f"{image} -t {mask}".split()
 
 
 @pytest.mark.skip("Test images are problematic.")
 def test_coregister_template_cli(
-    coregister_template_cli_args: typing.List[builtins.str],
+    coregister_template_cli_args: typing.List[str],
 ) -> None:
     retval = coregister_main(coregister_template_cli_args)
     assert retval == 0
 
 
 @pytest.fixture
-def preprocess_cli_args(image: pathlib.Path) -> typing.List[builtins.str]:
+def preprocess_cli_args(image: pathlib.Path) -> typing.List[str]:
     return f"{image} -2n4".split()
 
 
 @pytest.mark.skip("Takes too long.")
-def test_preprocess_cli(preprocess_cli_args: typing.List[builtins.str]) -> None:
+def test_preprocess_cli(preprocess_cli_args: typing.List[str]) -> None:
     retval = preprocess_main(preprocess_cli_args)
     assert retval == 0
 
 
-def test_ravel_normalization_cli(base_cli_dir_args: typing.List[builtins.str]) -> None:
+def test_ravel_normalization_cli(base_cli_dir_args: typing.List[str]) -> None:
     args = base_cli_dir_args + ["--membership-threshold", "0.1"]
     np.random.seed(1337)
     retval = ravel_main(args)
     assert retval == 0
```

### Comparing `intensity_normalization-2.2.3/tests/test_intensity_normalization.py` & `intensity_normalization-2.2.4/tests/test_intensity_normalization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Tests for non-antspy `intensity_normalization` functions."""
 
-import builtins
 import os
 import pathlib
 import typing
 
 import pytest
 
 from intensity_normalization.cli.fcm import fcm_main
@@ -15,38 +14,36 @@
 from intensity_normalization.cli.tissue_membership import (
     tissue_membership_main as tm_main,
 )
 from intensity_normalization.cli.whitestripe import whitestripe_main as ws_main
 from intensity_normalization.cli.zscore import zscore_main as zs_main
 
 
-def test_fcm_normalization_cli(base_cli_image_args: typing.List[builtins.str]) -> None:
+def test_fcm_normalization_cli(base_cli_image_args: typing.List[str]) -> None:
     retval = fcm_main(base_cli_image_args)
     assert retval == 0
 
 
 def test_fcm_normalization_nont1w_cli(image: pathlib.Path, mask: pathlib.Path) -> None:
     args = f"{image} -tm {mask} -mo t2".split()
     retval = fcm_main(args)
     assert retval == 0
 
 
-def test_kde_normalization_cli(base_cli_image_args: typing.List[builtins.str]) -> None:
+def test_kde_normalization_cli(base_cli_image_args: typing.List[str]) -> None:
     retval = kde_main(base_cli_image_args)
     assert retval == 0
 
 
-def test_ws_normalization_cli(base_cli_image_args: typing.List[builtins.str]) -> None:
+def test_ws_normalization_cli(base_cli_image_args: typing.List[str]) -> None:
     retval = ws_main(base_cli_image_args)
     assert retval == 0
 
 
-def test_zscore_normalization_cli(
-    base_cli_image_args: typing.List[builtins.str],
-) -> None:
+def test_zscore_normalization_cli(base_cli_image_args: typing.List[str]) -> None:
     retval = zs_main(base_cli_image_args)
     assert retval == 0
 
 
 def test_lsq_normalization_cli(
     image: pathlib.Path, mask: pathlib.Path, out_dir: pathlib.Path
 ) -> None:
@@ -70,15 +67,15 @@
     retval = lsq_main(args)
     assert retval == 0
     args = base_args + ["-lstm", f"{temp_dir}/test.npy"]
     retval = lsq_main(args)
     assert retval == 0
 
 
-def test_nyul_normalization_cli(base_cli_dir_args: typing.List[builtins.str]) -> None:
+def test_nyul_normalization_cli(base_cli_dir_args: typing.List[str]) -> None:
     retval = nyul_main(base_cli_dir_args)
     assert retval == 0
 
 
 def test_nyul_normalization_save_load_cli(
     image: pathlib.Path,
     mask: pathlib.Path,
@@ -92,35 +89,33 @@
     args = base_args + ["-lsh", f"{temp_dir}/test.npy"]
     retval = nyul_main(args)
     assert retval == 0
 
 
 @pytest.fixture
 def histogram_cli_args(
-    base_cli_dir_args: typing.List[builtins.str], temp_dir: pathlib.Path
-) -> typing.List[builtins.str]:
+    base_cli_dir_args: typing.List[str], temp_dir: pathlib.Path
+) -> typing.List[str]:
     return base_cli_dir_args + f"-o {temp_dir}/hist.png".split()
 
 
-def test_histogram_cli(histogram_cli_args: typing.List[builtins.str]) -> None:
+def test_histogram_cli(histogram_cli_args: typing.List[str]) -> None:
     retval = hist_main(histogram_cli_args)
     assert retval == 0
 
 
 @pytest.fixture
-def tissue_membership_cli_args(image: pathlib.Path) -> typing.List[builtins.str]:
+def tissue_membership_cli_args(image: pathlib.Path) -> typing.List[str]:
     return f"{image}".split()
 
 
-def test_tissue_membership_cli(
-    tissue_membership_cli_args: typing.List[builtins.str],
-) -> None:
+def test_tissue_membership_cli(tissue_membership_cli_args: typing.List[str]) -> None:
     retval = tm_main(tissue_membership_cli_args)
     assert retval == 0
 
 
 def test_tissue_membership_hard_seg_cli(
-    tissue_membership_cli_args: typing.List[builtins.str],
+    tissue_membership_cli_args: typing.List[str],
 ) -> None:
     tissue_membership_cli_args.append("-hs")
     retval = tm_main(tissue_membership_cli_args)
     assert retval == 0
```

