# Comparing `tmp/finagg-0.0.0b1.tar.gz` & `tmp/finagg-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finagg-0.0.0b1.tar", last modified: Sat Mar 25 04:20:02 2023, max compression
+gzip compressed data, was "finagg-0.1.0.tar", last modified: Wed May 31 21:52:52 2023, max compression
```

## Comparing `finagg-0.0.0b1.tar` & `finagg-0.1.0.tar`

### file list

```diff
@@ -1,111 +1,127 @@
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.880000 finagg-0.0.0b1/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.860000 finagg-0.0.0b1/.github/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/.github/workflows/
--rw-r--r--   0 berger    (1000) berger    (1000)     1164 2023-03-25 03:37:25.000000 finagg-0.0.0b1/.github/workflows/python-package.yml
--rw-r--r--   0 berger    (1000) berger    (1000)     1854 2023-03-15 16:29:59.000000 finagg-0.0.0b1/.gitignore
--rw-r--r--   0 berger    (1000) berger    (1000)      662 2023-03-25 03:11:34.000000 finagg-0.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0 berger    (1000) berger    (1000)    11357 2022-09-25 15:16:53.000000 finagg-0.0.0b1/LICENSE
--rw-r--r--   0 berger    (1000) berger    (1000)    24988 2023-03-25 04:20:02.880000 finagg-0.0.0b1/PKG-INFO
--rw-r--r--   0 berger    (1000) berger    (1000)    11158 2023-03-24 02:17:49.000000 finagg-0.0.0b1/README.rst
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/docs/
--rw-r--r--   0 berger    (1000) berger    (1000)      636 2023-03-15 16:29:59.000000 finagg-0.0.0b1/docs/Makefile
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/docs/_static/
--rw-r--r--   0 berger    (1000) berger    (1000)      480 2023-03-15 16:29:59.000000 finagg-0.0.0b1/docs/_static/custom.css
--rw-r--r--   0 berger    (1000) berger    (1000)      639 2023-03-15 16:29:59.000000 finagg-0.0.0b1/docs/cli.rst
--rw-r--r--   0 berger    (1000) berger    (1000)     3777 2023-03-15 16:29:59.000000 finagg-0.0.0b1/docs/conf.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1854 2023-03-15 16:29:59.000000 finagg-0.0.0b1/docs/configuration.rst
--rw-r--r--   0 berger    (1000) berger    (1000)     1144 2023-03-15 16:29:59.000000 finagg-0.0.0b1/docs/faq.rst
--rw-r--r--   0 berger    (1000) berger    (1000)     7997 2023-03-17 21:24:38.000000 finagg-0.0.0b1/docs/index.rst
--rw-r--r--   0 berger    (1000) berger    (1000)     1034 2023-03-18 19:17:42.000000 finagg-0.0.0b1/docs/installation.rst
--rw-r--r--   0 berger    (1000) berger    (1000)      800 2023-03-15 16:29:59.000000 finagg-0.0.0b1/docs/make.bat
--rw-r--r--   0 berger    (1000) berger    (1000)     1709 2023-03-15 16:29:59.000000 finagg-0.0.0b1/docs/references.rst
--rw-r--r--   0 berger    (1000) berger    (1000)       87 2023-03-15 16:29:59.000000 finagg-0.0.0b1/docs/requirements.txt
--rw-r--r--   0 berger    (1000) berger    (1000)     4135 2023-03-25 03:21:33.000000 finagg-0.0.0b1/pyproject.toml
--rw-r--r--   0 berger    (1000) berger    (1000)       38 2023-03-25 04:20:02.880000 finagg-0.0.0b1/setup.cfg
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.860000 finagg-0.0.0b1/src/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/src/finagg/
--rw-r--r--   0 berger    (1000) berger    (1000)      301 2023-02-28 02:24:08.000000 finagg-0.0.0b1/src/finagg/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     6325 2023-03-24 01:57:04.000000 finagg-0.0.0b1/src/finagg/__main__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     3046 2023-03-18 19:17:42.000000 finagg-0.0.0b1/src/finagg/backend.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/src/finagg/bea/
--rw-r--r--   0 berger    (1000) berger    (1000)       61 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/bea/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1046 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/bea/_cli.py
--rw-r--r--   0 berger    (1000) berger    (1000)    20603 2023-03-18 19:17:42.000000 finagg-0.0.0b1/src/finagg/bea/api.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1735 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/bea/sql.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1901 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/feat.py
--rw-r--r--   0 berger    (1000) berger    (1000)     6460 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/frame.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/src/finagg/fred/
--rw-r--r--   0 berger    (1000) berger    (1000)       68 2023-02-26 19:29:38.000000 finagg-0.0.0b1/src/finagg/fred/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     5308 2023-03-22 00:26:44.000000 finagg-0.0.0b1/src/finagg/fred/_cli.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/src/finagg/fred/api/
--rw-r--r--   0 berger    (1000) berger    (1000)     1157 2023-03-18 19:17:42.000000 finagg-0.0.0b1/src/finagg/fred/api/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2772 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/fred/api/_api.py
--rw-r--r--   0 berger    (1000) berger    (1000)    18389 2023-03-17 21:24:38.000000 finagg-0.0.0b1/src/finagg/fred/api/category_.py
--rw-r--r--   0 berger    (1000) berger    (1000)    22318 2023-03-17 21:24:38.000000 finagg-0.0.0b1/src/finagg/fred/api/release_.py
--rw-r--r--   0 berger    (1000) berger    (1000)    34287 2023-03-17 21:24:38.000000 finagg-0.0.0b1/src/finagg/fred/api/series_.py
--rw-r--r--   0 berger    (1000) berger    (1000)     8700 2023-03-17 21:24:38.000000 finagg-0.0.0b1/src/finagg/fred/api/source_.py
--rw-r--r--   0 berger    (1000) berger    (1000)    11462 2023-03-17 21:24:38.000000 finagg-0.0.0b1/src/finagg/fred/api/tags_.py
--rw-r--r--   0 berger    (1000) berger    (1000)    26898 2023-03-22 00:26:40.000000 finagg-0.0.0b1/src/finagg/fred/feat.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2474 2023-03-22 00:03:35.000000 finagg-0.0.0b1/src/finagg/fred/sql.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/src/finagg/fundam/
--rw-r--r--   0 berger    (1000) berger    (1000)       84 2023-02-26 19:29:38.000000 finagg-0.0.0b1/src/finagg/fundam/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1901 2023-03-18 19:08:17.000000 finagg-0.0.0b1/src/finagg/fundam/_cli.py
--rw-r--r--   0 berger    (1000) berger    (1000)    36932 2023-03-22 00:03:35.000000 finagg-0.0.0b1/src/finagg/fundam/feat.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1209 2023-03-22 00:03:35.000000 finagg-0.0.0b1/src/finagg/fundam/sql.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/src/finagg/indices/
--rw-r--r--   0 berger    (1000) berger    (1000)       65 2023-02-26 19:29:38.000000 finagg-0.0.0b1/src/finagg/indices/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2992 2023-03-18 20:43:31.000000 finagg-0.0.0b1/src/finagg/indices/_cli.py
--rw-r--r--   0 berger    (1000) berger    (1000)     8245 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/indices/api.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2358 2023-03-22 00:03:35.000000 finagg-0.0.0b1/src/finagg/indices/sql.py
--rw-r--r--   0 berger    (1000) berger    (1000)    12943 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/portfolio.py
--rw-r--r--   0 berger    (1000) berger    (1000)     9162 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/ratelimit.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/src/finagg/sec/
--rw-r--r--   0 berger    (1000) berger    (1000)       67 2023-02-26 19:29:38.000000 finagg-0.0.0b1/src/finagg/sec/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     6226 2023-03-22 00:16:38.000000 finagg-0.0.0b1/src/finagg/sec/_cli.py
--rw-r--r--   0 berger    (1000) berger    (1000)    23250 2023-03-18 19:17:42.000000 finagg-0.0.0b1/src/finagg/sec/api.py
--rw-r--r--   0 berger    (1000) berger    (1000)    50422 2023-03-22 00:03:35.000000 finagg-0.0.0b1/src/finagg/sec/feat.py
--rw-r--r--   0 berger    (1000) berger    (1000)    12294 2023-03-22 00:03:35.000000 finagg-0.0.0b1/src/finagg/sec/sql.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1800 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/testing.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4413 2023-03-22 00:11:31.000000 finagg-0.0.0b1/src/finagg/utils.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/src/finagg/yfinance/
--rw-r--r--   0 berger    (1000) berger    (1000)       72 2023-02-26 19:29:38.000000 finagg-0.0.0b1/src/finagg/yfinance/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4931 2023-03-22 00:16:50.000000 finagg-0.0.0b1/src/finagg/yfinance/_cli.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2111 2023-03-15 16:29:59.000000 finagg-0.0.0b1/src/finagg/yfinance/api.py
--rw-r--r--   0 berger    (1000) berger    (1000)    18809 2023-03-22 00:03:35.000000 finagg-0.0.0b1/src/finagg/yfinance/feat.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2510 2023-03-22 00:03:35.000000 finagg-0.0.0b1/src/finagg/yfinance/sql.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/src/finagg.egg-info/
--rw-r--r--   0 berger    (1000) berger    (1000)    24988 2023-03-25 04:20:02.000000 finagg-0.0.0b1/src/finagg.egg-info/PKG-INFO
--rw-r--r--   0 berger    (1000) berger    (1000)     2192 2023-03-25 04:20:02.000000 finagg-0.0.0b1/src/finagg.egg-info/SOURCES.txt
--rw-r--r--   0 berger    (1000) berger    (1000)        1 2023-03-25 04:20:02.000000 finagg-0.0.0b1/src/finagg.egg-info/dependency_links.txt
--rw-r--r--   0 berger    (1000) berger    (1000)       48 2023-03-25 04:20:02.000000 finagg-0.0.0b1/src/finagg.egg-info/entry_points.txt
--rw-r--r--   0 berger    (1000) berger    (1000)      314 2023-03-25 04:20:02.000000 finagg-0.0.0b1/src/finagg.egg-info/requires.txt
--rw-r--r--   0 berger    (1000) berger    (1000)        7 2023-03-25 04:20:02.000000 finagg-0.0.0b1/src/finagg.egg-info/top_level.txt
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/tests/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:07:40.000000 finagg-0.0.0b1/tests/__init__.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/tests/test_bea/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:07:57.000000 finagg-0.0.0b1/tests/test_bea/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)      432 2022-12-27 07:50:28.000000 finagg-0.0.0b1/tests/test_bea/test_api.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4023 2022-12-27 07:52:12.000000 finagg-0.0.0b1/tests/test_frame.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/tests/test_fred/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:08:07.000000 finagg-0.0.0b1/tests/test_fred/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)      480 2022-12-30 04:42:52.000000 finagg-0.0.0b1/tests/test_fred/test_api.py
--rw-r--r--   0 berger    (1000) berger    (1000)      757 2023-03-15 16:29:59.000000 finagg-0.0.0b1/tests/test_fred/test_feat.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/tests/test_fundam/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-02-26 19:29:38.000000 finagg-0.0.0b1/tests/test_fundam/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1793 2023-03-21 23:53:25.000000 finagg-0.0.0b1/tests/test_fundam/test_feat.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.870000 finagg-0.0.0b1/tests/test_indices/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:08:36.000000 finagg-0.0.0b1/tests/test_indices/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)      298 2023-02-24 02:58:30.000000 finagg-0.0.0b1/tests/test_indices/test_api.py
--rw-r--r--   0 berger    (1000) berger    (1000)     3278 2023-03-09 02:04:14.000000 finagg-0.0.0b1/tests/test_portfolio.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2559 2023-03-15 16:29:59.000000 finagg-0.0.0b1/tests/test_ratelimit.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.880000 finagg-0.0.0b1/tests/test_sec/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:08:22.000000 finagg-0.0.0b1/tests/test_sec/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)      351 2022-12-27 07:50:28.000000 finagg-0.0.0b1/tests/test_sec/test_api.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1532 2023-03-21 23:42:57.000000 finagg-0.0.0b1/tests/test_sec/test_feat.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1279 2023-03-25 03:25:21.000000 finagg-0.0.0b1/tests/test_sec/test_sql.py
--rw-r--r--   0 berger    (1000) berger    (1000)      718 2022-12-27 07:52:12.000000 finagg-0.0.0b1/tests/test_utils.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-03-25 04:20:02.880000 finagg-0.0.0b1/tests/test_yfinance/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:08:58.000000 finagg-0.0.0b1/tests/test_yfinance/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)       76 2022-12-27 07:50:28.000000 finagg-0.0.0b1/tests/test_yfinance/test_api.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1351 2023-03-21 23:41:21.000000 finagg-0.0.0b1/tests/test_yfinance/test_feat.py
--rw-r--r--   0 berger    (1000) berger    (1000)      416 2023-03-22 00:03:35.000000 finagg-0.0.0b1/tests/test_yfinance/test_sql.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.850000 finagg-0.1.0/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.830000 finagg-0.1.0/.github/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/.github/workflows/
+-rw-r--r--   0 berger    (1000) berger    (1000)      916 2023-04-19 01:16:38.000000 finagg-0.1.0/.github/workflows/build-docs.yml
+-rw-r--r--   0 berger    (1000) berger    (1000)      744 2023-03-26 13:59:46.000000 finagg-0.1.0/.github/workflows/test-and-publish.yml
+-rw-r--r--   0 berger    (1000) berger    (1000)      894 2023-03-25 14:25:22.000000 finagg-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0 berger    (1000) berger    (1000)     1888 2023-04-21 01:18:56.000000 finagg-0.1.0/.gitignore
+-rw-r--r--   0 berger    (1000) berger    (1000)      694 2023-05-24 02:08:12.000000 finagg-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 berger    (1000) berger    (1000)    11357 2022-09-25 15:16:53.000000 finagg-0.1.0/LICENSE
+-rw-r--r--   0 berger    (1000) berger    (1000)    26764 2023-05-31 21:52:52.850000 finagg-0.1.0/PKG-INFO
+-rw-r--r--   0 berger    (1000) berger    (1000)    12872 2023-04-19 01:16:38.000000 finagg-0.1.0/README.rst
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/docs/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-03-25 23:12:41.000000 finagg-0.1.0/docs/.nojekyll
+-rw-r--r--   0 berger    (1000) berger    (1000)      635 2023-03-25 23:29:53.000000 finagg-0.1.0/docs/Makefile
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/docs/_static/
+-rw-r--r--   0 berger    (1000) berger    (1000)      480 2023-03-15 16:29:59.000000 finagg-0.1.0/docs/_static/custom.css
+-rw-r--r--   0 berger    (1000) berger    (1000)      639 2023-03-25 23:12:41.000000 finagg-0.1.0/docs/cli.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)     4239 2023-04-14 19:49:09.000000 finagg-0.1.0/docs/conf.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2134 2023-04-07 03:11:36.000000 finagg-0.1.0/docs/configuration.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)     9830 2023-04-18 01:05:55.000000 finagg-0.1.0/docs/conventions.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)     1895 2023-04-07 18:04:47.000000 finagg-0.1.0/docs/faq.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)       71 2023-03-25 23:29:53.000000 finagg-0.1.0/docs/index.html
+-rw-r--r--   0 berger    (1000) berger    (1000)     8615 2023-04-19 01:16:38.000000 finagg-0.1.0/docs/index.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)     1167 2023-04-07 03:11:36.000000 finagg-0.1.0/docs/installation.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)      799 2023-03-25 23:29:53.000000 finagg-0.1.0/docs/make.bat
+-rw-r--r--   0 berger    (1000) berger    (1000)     1842 2023-04-07 03:11:36.000000 finagg-0.1.0/docs/references.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)       87 2023-03-25 23:12:41.000000 finagg-0.1.0/docs/requirements.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)    16317 2023-04-19 01:16:38.000000 finagg-0.1.0/docs/walkthroughs.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)     4193 2023-04-14 19:49:09.000000 finagg-0.1.0/pyproject.toml
+-rw-r--r--   0 berger    (1000) berger    (1000)       38 2023-05-31 21:52:52.850000 finagg-0.1.0/setup.cfg
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.830000 finagg-0.1.0/src/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/
+-rw-r--r--   0 berger    (1000) berger    (1000)      301 2023-02-28 02:24:08.000000 finagg-0.1.0/src/finagg/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     6820 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/__main__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2256 2023-04-18 01:05:55.000000 finagg-0.1.0/src/finagg/backend.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/bea/
+-rw-r--r--   0 berger    (1000) berger    (1000)       61 2023-03-15 16:29:59.000000 finagg-0.1.0/src/finagg/bea/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1046 2023-03-15 16:29:59.000000 finagg-0.1.0/src/finagg/bea/_cli.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    21084 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/bea/api.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2459 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/bea/sql.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     6691 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/frame.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/fred/
+-rw-r--r--   0 berger    (1000) berger    (1000)       68 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/fred/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     5490 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/fred/_cli.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/fred/api/
+-rw-r--r--   0 berger    (1000) berger    (1000)     3592 2023-05-24 21:51:51.000000 finagg-0.1.0/src/finagg/fred/api/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2772 2023-04-10 03:29:11.000000 finagg-0.1.0/src/finagg/fred/api/_api.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    18380 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/fred/api/_category.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    22359 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/fred/api/_release.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    40143 2023-05-24 21:51:53.000000 finagg-0.1.0/src/finagg/fred/api/_series.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     8459 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/fred/api/_source.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    11198 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/fred/api/_tags.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/fred/feat/
+-rw-r--r--   0 berger    (1000) berger    (1000)      400 2023-04-18 01:05:55.000000 finagg-0.1.0/src/finagg/fred/feat/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     6696 2023-05-24 21:51:53.000000 finagg-0.1.0/src/finagg/fred/feat/_raw.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    10635 2023-05-24 21:51:53.000000 finagg-0.1.0/src/finagg/fred/feat/_refined.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3935 2023-05-24 21:51:53.000000 finagg-0.1.0/src/finagg/fred/sql.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/fundam/
+-rw-r--r--   0 berger    (1000) berger    (1000)       71 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/fundam/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2800 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/fundam/_cli.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    33691 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/fundam/feat.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2142 2023-04-18 01:05:55.000000 finagg-0.1.0/src/finagg/fundam/sql.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/indices/
+-rw-r--r--   0 berger    (1000) berger    (1000)       65 2023-02-26 19:29:38.000000 finagg-0.1.0/src/finagg/indices/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2992 2023-03-18 20:43:31.000000 finagg-0.1.0/src/finagg/indices/_cli.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     8168 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/indices/api.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3056 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/indices/sql.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    14390 2023-04-18 01:05:55.000000 finagg-0.1.0/src/finagg/portfolio.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     9160 2023-04-19 01:16:38.000000 finagg-0.1.0/src/finagg/ratelimit.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/sec/
+-rw-r--r--   0 berger    (1000) berger    (1000)       67 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/sec/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     7194 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/sec/_cli.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    33993 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/sec/api.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/sec/feat/
+-rw-r--r--   0 berger    (1000) berger    (1000)      920 2023-04-18 01:05:55.000000 finagg-0.1.0/src/finagg/sec/feat/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    18047 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/sec/feat/_raw.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/sec/feat/_refined/
+-rw-r--r--   0 berger    (1000) berger    (1000)      201 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/sec/feat/_refined/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    38102 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/sec/feat/_refined/annual.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    39236 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/sec/feat/_refined/quarterly.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    25535 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/sec/sql.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1800 2023-03-15 16:29:59.000000 finagg-0.1.0/src/finagg/testing.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     9318 2023-04-18 01:05:55.000000 finagg-0.1.0/src/finagg/utils.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/yfinance/
+-rw-r--r--   0 berger    (1000) berger    (1000)       72 2023-02-26 19:29:38.000000 finagg-0.1.0/src/finagg/yfinance/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     5344 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/yfinance/_cli.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2145 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/yfinance/api.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg/yfinance/feat/
+-rw-r--r--   0 berger    (1000) berger    (1000)      381 2023-04-14 19:49:09.000000 finagg-0.1.0/src/finagg/yfinance/feat/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     7210 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/yfinance/feat/_raw.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    13508 2023-05-24 02:08:12.000000 finagg-0.1.0/src/finagg/yfinance/feat/_refined.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3173 2023-04-18 01:05:55.000000 finagg-0.1.0/src/finagg/yfinance/sql.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/src/finagg.egg-info/
+-rw-r--r--   0 berger    (1000) berger    (1000)    26764 2023-05-31 21:52:52.000000 finagg-0.1.0/src/finagg.egg-info/PKG-INFO
+-rw-r--r--   0 berger    (1000) berger    (1000)     2586 2023-05-31 21:52:52.000000 finagg-0.1.0/src/finagg.egg-info/SOURCES.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)        1 2023-05-31 21:52:52.000000 finagg-0.1.0/src/finagg.egg-info/dependency_links.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)       48 2023-05-31 21:52:52.000000 finagg-0.1.0/src/finagg.egg-info/entry_points.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)      314 2023-05-31 21:52:52.000000 finagg-0.1.0/src/finagg.egg-info/requires.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)        7 2023-05-31 21:52:52.000000 finagg-0.1.0/src/finagg.egg-info/top_level.txt
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.840000 finagg-0.1.0/tests/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:07:40.000000 finagg-0.1.0/tests/__init__.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.850000 finagg-0.1.0/tests/test_bea/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:07:57.000000 finagg-0.1.0/tests/test_bea/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)      432 2022-12-27 07:50:28.000000 finagg-0.1.0/tests/test_bea/test_api.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4023 2022-12-27 07:52:12.000000 finagg-0.1.0/tests/test_frame.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.850000 finagg-0.1.0/tests/test_fred/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:08:07.000000 finagg-0.1.0/tests/test_fred/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)      480 2022-12-30 04:42:52.000000 finagg-0.1.0/tests/test_fred/test_api.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1221 2023-04-18 01:05:55.000000 finagg-0.1.0/tests/test_fred/test_feat.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.850000 finagg-0.1.0/tests/test_fundam/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-02-26 19:29:38.000000 finagg-0.1.0/tests/test_fundam/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2103 2023-05-24 02:08:12.000000 finagg-0.1.0/tests/test_fundam/test_feat.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.850000 finagg-0.1.0/tests/test_indices/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:08:36.000000 finagg-0.1.0/tests/test_indices/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)      298 2023-02-24 02:58:30.000000 finagg-0.1.0/tests/test_indices/test_api.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3278 2023-03-09 02:04:14.000000 finagg-0.1.0/tests/test_portfolio.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2559 2023-03-15 16:29:59.000000 finagg-0.1.0/tests/test_ratelimit.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.850000 finagg-0.1.0/tests/test_sec/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:08:22.000000 finagg-0.1.0/tests/test_sec/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)      351 2022-12-27 07:50:28.000000 finagg-0.1.0/tests/test_sec/test_api.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4494 2023-05-24 02:08:12.000000 finagg-0.1.0/tests/test_sec/test_feat.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1285 2023-04-07 03:11:36.000000 finagg-0.1.0/tests/test_sec/test_sql.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2755 2023-04-18 01:05:55.000000 finagg-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:52:52.850000 finagg-0.1.0/tests/test_yfinance/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2022-11-07 00:08:58.000000 finagg-0.1.0/tests/test_yfinance/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)       76 2022-12-27 07:50:28.000000 finagg-0.1.0/tests/test_yfinance/test_api.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2382 2023-05-24 02:08:12.000000 finagg-0.1.0/tests/test_yfinance/test_feat.py
```

### Comparing `finagg-0.0.0b1/.github/workflows/python-package.yml` & `finagg-0.1.0/.github/workflows/test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,21 @@
-name: Python package
+name: Test
 
-on: [push]
+on:
+  push:
+    branches:
+      - main
+  workflow_call:
+    secrets:
+      BEA_API_KEY:
+        required: true
+      FRED_API_KEY:
+        required: true
+      SEC_API_USER_AGENT:
+        required: true
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.10"]
@@ -22,26 +33,7 @@
           FRED_API_KEY: ${{ secrets.FRED_API_KEY }}
           SEC_API_USER_AGENT: ${{ secrets.SEC_API_USER_AGENT }}
         run: tox -e test
       - name: Run static typechecks
         run: tox -e typecheck
       - name: Run lint
         run: tox -e lint
-
-  build:
-    needs: test
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version: ["3.10", "3.11"]
-    steps:
-      - uses: actions/checkout@v3
-      - name: Setup Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python-version }}
-      - name: Install tox
-        run: pip install tox
-      - name: Build
-        run: tox -e build
-      - name: Publish
-        run: tox -e publish
```

### Comparing `finagg-0.0.0b1/.gitignore` & `finagg-0.1.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -72,15 +72,18 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/build/
 docs/api/
+doctrees/
+singlehtml/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `finagg-0.0.0b1/.pre-commit-config.yaml` & `finagg-0.1.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -19,12 +19,14 @@
         - --remove-all-unused-imports
         - --remove-unused-variables
 
   - repo: https://github.com/psf/black
     rev: 22.8.0
     hooks:
     - id: black
+      args:
+        - --preview
 
   - repo: https://github.com/pycqa/isort
     rev: 5.11.5
     hooks:
       - id: isort
```

### Comparing `finagg-0.0.0b1/LICENSE` & `finagg-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finagg-0.0.0b1/PKG-INFO` & `finagg-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finagg
-Version: 0.0.0b1
+Version: 0.1.0
 Summary: Data aggregation with popular and free financial APIs.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,15 +201,16 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: repository, https://github.com/theOGognf/finagg
+Project-URL: Repository, https://github.com/theOGognf/finagg
+Project-URL: Documentation, https://theogognf.github.io/finagg/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.10
@@ -227,21 +228,31 @@
 ========================================
 
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
+* **Documentation**: https://theogognf.github.io/finagg/
+* **PyPI**: https://pypi.org/project/finagg/
+* **Repository**: https://github.com/theOGognf/finagg
+
 Quick Start
 ===========
 
 Installation
 ------------
 
-Install **finagg** from GitHub directly.
+Install with pip for the latest (stable) version.
+
+.. code:: console
+
+  pip install finagg
+
+Install from GitHub for the latest (unstable) version.
 
 .. code:: console
 
     git clone https://github.com/theOGognf/finagg.git
     pip install ./finagg/
 
 Optionally install the recommended datasets from 3rd party APIs into a local
@@ -253,26 +264,31 @@
 
 The installation will point you where to get free API keys and write them to a
 local ``.env`` file for storage.
 
 Basic Usage
 -----------
 
+These are just **finagg** usage samples. See the `documentation`_ for all the
+supported APIs and features.
+
 Explore the APIs directly
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
+*These methods require internet access and API keys/user agent declarations.*
+
 Get Bureau of Economic Analysis (BEA) data.
 
 >>> finagg.bea.api.gdp_by_industry.get(year=[2019]).head(5)
-   table_id freq  year quarter industry                         industry_description       value
-0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting  156.300003
-1         1    Q  2019       1    111CA                                        Farms  117.599998
-2         1    Q  2019       1    113FF    Forestry, fishing, and related activities   38.700001
-3         1    Q  2019       1       21                                       Mining  305.700012
-4         1    Q  2019       1      211                       Oil and gas extraction  190.199997
+   table_id freq  year quarter industry                         industry_description ...
+0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting ...
+1         1    Q  2019       1    111CA                                        Farms ...
+2         1    Q  2019       1    113FF    Forestry, fishing, and related activities ...
+3         1    Q  2019       1       21                                       Mining ...
+4         1    Q  2019       1      211                       Oil and gas extraction ...
 
 Get Federal Reserve Economic Data (FRED).
 
 >>> finagg.fred.api.series.observations.get(
 ...   "CPIAUCNS",
 ...   realtime_start=0,
 ...   realtime_end=-1,
@@ -294,69 +310,86 @@
 2  2009-10-16  900678473.0  0001193125-10-012091  2009  FY  10-K/A  2010-01-25 ...
 3  2010-01-15  906794589.0  0001193125-10-012085  2010  Q1    10-Q  2010-01-25 ...
 4  2010-04-09  909938383.0  0001193125-10-088957  2010  Q2    10-Q  2010-04-21 ...
 
 Use installed raw data for exploring the most popular features
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+*These methods require internet access, API keys/user agent declarations, and
+downloading and installing raw data through the* ``finagg install`` *or*
+``finagg <api/subpackage> install`` *commands.*
+
 Get the most popular FRED features all in one dataframe.
 
 >>> finagg.fred.feat.economic.from_raw().head(5)
-            CIVPART_pct_change  CPIAUCNS_pct_change  CSUSHPINSA_pct_change  FEDFUNDS ...
-date                                                                                 ...
-2014-10-06                 0.0                  0.0                    0.0      0.09 ...
-2014-10-08                 0.0                  0.0                    0.0      0.09 ...
-2014-10-13                 0.0                  0.0                    0.0      0.09 ...
-2014-10-15                 0.0                  0.0                    0.0      0.09 ...
-2014-10-20                 0.0                  0.0                    0.0      0.09 ...
+            CIVPART  LOG_CHANGE(CPIAUCNS)  LOG_CHANGE(CSUSHPINSA)  FEDFUNDS ...
+date                                                                        ...
+2014-10-06     62.8                   0.0                     0.0      0.09 ...
+2014-10-08     62.8                   0.0                     0.0      0.09 ...
+2014-10-13     62.8                   0.0                     0.0      0.09 ...
+2014-10-15     62.8                   0.0                     0.0      0.09 ...
+2014-10-20     62.8                   0.0                     0.0      0.09 ...
 
 Get quarterly report features from SEC data.
 
 >>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)
-                    AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-fy   fp filed                                                                   ...
-2010 Q1 2010-01-25                 -0.023398         0.363654              2.54 ...
-     Q2 2010-04-21                  0.000000         0.363654              4.35 ...
-     Q3 2010-07-21                  0.000000         0.363654              6.40 ...
-2011 Q1 2011-01-19                  0.320805         0.433596              3.74 ...
-     Q2 2011-04-21                  0.000000         0.433596              7.12 ...
+                    LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent) ...
+fy   fp filed                                                     ...
+2010 Q1 2010-01-25            0.182629                  -0.023676 ...
+     Q2 2010-04-21            0.000000                   0.000000 ...
+     Q3 2010-07-21            0.000000                   0.000000 ...
+2011 Q1 2011-01-19            0.459174                   0.278241 ...
+     Q2 2011-04-21            0.000000                   0.000000 ...
 
 Get an aggregation of quarterly and daily features for a particular ticker.
 
 >>> finagg.fundam.feat.fundam.from_raw("AAPL").head(5)
+            PriceBookRatio  PriceEarningsRatio
+date
+2010-01-25        0.175061            2.423509
+2010-01-26        0.178035            2.464678
+2010-01-27        0.178813            2.475448
+2010-01-28        0.177154            2.452471
+2010-01-29        0.173825            2.406396
 
 Use installed features for exploring refined aggregations of raw data
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+*These methods require installing refined data through the* ``finagg install``
+*or* ``finagg <api/subpackage> install`` *commands.*
+
 Get a ticker's industry's averaged quarterly report features.
 
 >>> finagg.sec.feat.quarterly.industry.from_refined(ticker="AAPL").head(5)
-                                        avg                                  ...
-name               AssetsCurrent_pct_change DebtEquityRatio EarningsPerShare ...
-fy   fp filed                                                                ...
-2009 Q3 2009-10-30                 0.000000        0.573255         3.065000 ...
-2010 Q1 2010-04-29                -0.012229        0.402497         0.865000 ...
-     Q2 2010-07-30                 0.000000        0.500347         0.538571 ...
-     Q3 2010-11-04                 0.001145        0.456791         1.203750 ...
-2011 Q1 2011-05-05                 0.271624        0.465244         0.992000 ...
+                                 mean                           ...
+name               AssetCoverageRatio BookRatio DebtEquityRatio ...
+fy   fp filed                                                   ...
+2014 Q1 2014-05-15          10.731301  9.448954        0.158318 ...
+     Q2 2014-08-14          10.731301  9.448954        0.158318 ...
+     Q3 2014-11-14          10.731301  9.448954        0.158318 ...
+2015 Q1 2015-05-15          16.738972  9.269250        0.294238 ...
+     Q2 2015-08-13          16.738972  9.269250        0.294238 ...
 
 Get a ticker's industry-averaged quarterly report features.
 
 >>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)
-                    AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-fy   fp filed                                                                   ...
-2010 Q1 2010-01-25                 -0.257265        -0.260642          1.697972 ...
-     Q2 2010-04-21                  0.000000        -0.530932          1.508060 ...
-     Q3 2010-07-21                 -0.377964        -0.348547          1.932276 ...
-2011 Q1 2011-01-19                  0.269259        -0.110688          2.880060 ...
-     Q2 2011-04-21                  0.000000        -0.065501          2.899716 ...
+                    NORM(LOG_CHANGE(Assets))  NORM(LOG_CHANGE(AssetsCurrent)) ...
+fy   fp filed                                                                 ...
+2010 Q2 2010-04-21                  0.000000                         0.000000 ...
+     Q3 2010-07-21                  0.000000                         0.000000 ...
+2011 Q1 2011-01-19                  0.978816                         0.074032 ...
+     Q2 2011-04-21                  0.000000                         0.000000 ...
+     Q3 2011-07-20                 -0.353553                        -0.353553 ...
 
 Get tickers sorted by an industry-averaged quarterly report feature.
 
->>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by("EarningsPerShare", year=2019)[:5]
+>>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by(
+...   "EarningsPerShareBasic",
+...   year=2019
+... )[:5]
 ['XRAY', 'TSLA', 'SYY', 'WHR', 'KMB']
 
 Get tickers sorted by an industry-averaged fundamental feature.
 
 >>> finagg.fundam.feat.fundam.normalized.get_tickers_sorted_by(
 ...   "PriceEarningsRatio",
 ...   date="2019-01-04"
@@ -401,32 +434,35 @@
   ``./findata/finagg.sqlite``.
 
 Dependencies
 ============
 
 * `pandas`_ for fast, flexible, and expressive representations of relational data.
 * `requests`_ for HTTP requests to 3rd party APIs.
-* `requests-cache`_ for caching HTTP requests to avoid getting throttled by 3rd party API servers.
+* `requests-cache`_ for caching HTTP requests to avoid getting throttled by 3rd
+  party API servers.
 * `SQLAlchemy`_ for a SQL Python interface.
 * `yfinance`_ for historical stock data from Yahoo! Finance.
 
 API References
 ==============
 
 * The `BEA API`_ and the `BEA API key registration link`_.
 * The `FRED API`_ and the `FRED API key registration link`_.
 * The `SEC API`_.
 
 Related Projects
 ================
 
-* `FinRL`_ is a collection of financial reinforcement learning environments and tools.
+* `FinRL`_ is a collection of financial reinforcement learning environments
+  and tools.
 * `fredapi`_ is an implementation of the FRED API.
-* `OpenBBTerminal`_ an open-source version of the Bloomberg Terminal.
+* `OpenBBTerminal`_ is an open-source version of the Bloomberg Terminal.
 * `sec-edgar`_ is an implementation of a file-based SEC EDGAR parser.
+* `sec-edgar-api`_ is an implementation of the SEC EDGAR REST API.
 
 Frequently Asked Questions
 ==========================
 
 Where should I start?
 ---------------------
 
@@ -434,14 +470,26 @@
 environments using the implemented data features and SQL tables. This
 project was originally created to make RL environments for financial
 applications but has since focused its purpose to just aggregating financial
 data and features. That being said, all the implemented features are
 defined in such a way to make it very easy to develop financial AI/ML,
 so we encourage you to do just that!
 
+Why aren't features being installed for a specific ticker or economic data series?
+----------------------------------------------------------------------------------
+
+Implemented APIs may be relatively new and simply may not provide data for a
+particular ticker or economic data series. For example, earnings per share may
+not be accessible for all companies through the SEC EDGAR API. In some cases,
+APIs may raise an HTTP error, causing installations to skip the ticker or
+series. Additionally, not all tickers and economic data series contain
+sufficient data for feature normalization. If a ticker or series only has one
+data point, that data point could be dropped when computing a feature (such as
+percent change), causing no data to be installed.
+
 What Python versions are supported?
 -----------------------------------
 
 Python 3.10 and up are supported. We don't plan on supporting lower versions
 because 3.10 introduces some nice quality of life updates that are used
 throughout the package.
 
@@ -452,20 +500,22 @@
 using Linux or WSL in practice. The package performs a good amount of I/O and
 interprocess operations that could result in a noticeable performance
 degradation on Windows.
 
 .. _`BEA API`: https://apps.bea.gov/api/signup/
 .. _`BEA API key registration link`: https://apps.bea.gov/API/signup/
 .. _`BEA API site`: https://apps.bea.gov/API/signup/
+.. _`documentation`: https://theogognf.github.io/finagg/
 .. _`FinRL`: https://github.com/AI4Finance-Foundation/FinRL
 .. _`FRED API`: https://fred.stlouisfed.org/docs/api/fred/
 .. _`FRED API key registration link`: https://fredaccount.stlouisfed.org/login/secure/
 .. _`FRED API site`: https://fredaccount.stlouisfed.org/login/secure/
 .. _`fredapi`: https://github.com/mortada/fredapi
 .. _`OpenBBTerminal`: https://github.com/OpenBB-finance/OpenBBTerminal
 .. _`pandas`: https://pandas.pydata.org/
 .. _`requests`: https://requests.readthedocs.io/en/latest/
 .. _`requests-cache`: https://requests-cache.readthedocs.io/en/stable/
 .. _`SEC API`: https://www.sec.gov/edgar/sec-api-documentation
 .. _`sec-edgar`: https://github.com/sec-edgar/sec-edgar
+.. _`sec-edgar-api`: https://github.com/jadchaar/sec-edgar-api
 .. _`SQLAlchemy`: https://www.sqlalchemy.org/
 .. _`yfinance`: https://github.com/ranaroussi/yfinance
```

### Comparing `finagg-0.0.0b1/README.rst` & `finagg-0.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,31 @@
 ========================================
 
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
+* **Documentation**: https://theogognf.github.io/finagg/
+* **PyPI**: https://pypi.org/project/finagg/
+* **Repository**: https://github.com/theOGognf/finagg
+
 Quick Start
 ===========
 
 Installation
 ------------
 
-Install **finagg** from GitHub directly.
+Install with pip for the latest (stable) version.
+
+.. code:: console
+
+  pip install finagg
+
+Install from GitHub for the latest (unstable) version.
 
 .. code:: console
 
     git clone https://github.com/theOGognf/finagg.git
     pip install ./finagg/
 
 Optionally install the recommended datasets from 3rd party APIs into a local
@@ -28,26 +38,31 @@
 
 The installation will point you where to get free API keys and write them to a
 local ``.env`` file for storage.
 
 Basic Usage
 -----------
 
+These are just **finagg** usage samples. See the `documentation`_ for all the
+supported APIs and features.
+
 Explore the APIs directly
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
+*These methods require internet access and API keys/user agent declarations.*
+
 Get Bureau of Economic Analysis (BEA) data.
 
 >>> finagg.bea.api.gdp_by_industry.get(year=[2019]).head(5)
-   table_id freq  year quarter industry                         industry_description       value
-0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting  156.300003
-1         1    Q  2019       1    111CA                                        Farms  117.599998
-2         1    Q  2019       1    113FF    Forestry, fishing, and related activities   38.700001
-3         1    Q  2019       1       21                                       Mining  305.700012
-4         1    Q  2019       1      211                       Oil and gas extraction  190.199997
+   table_id freq  year quarter industry                         industry_description ...
+0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting ...
+1         1    Q  2019       1    111CA                                        Farms ...
+2         1    Q  2019       1    113FF    Forestry, fishing, and related activities ...
+3         1    Q  2019       1       21                                       Mining ...
+4         1    Q  2019       1      211                       Oil and gas extraction ...
 
 Get Federal Reserve Economic Data (FRED).
 
 >>> finagg.fred.api.series.observations.get(
 ...   "CPIAUCNS",
 ...   realtime_start=0,
 ...   realtime_end=-1,
@@ -69,69 +84,86 @@
 2  2009-10-16  900678473.0  0001193125-10-012091  2009  FY  10-K/A  2010-01-25 ...
 3  2010-01-15  906794589.0  0001193125-10-012085  2010  Q1    10-Q  2010-01-25 ...
 4  2010-04-09  909938383.0  0001193125-10-088957  2010  Q2    10-Q  2010-04-21 ...
 
 Use installed raw data for exploring the most popular features
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+*These methods require internet access, API keys/user agent declarations, and
+downloading and installing raw data through the* ``finagg install`` *or*
+``finagg <api/subpackage> install`` *commands.*
+
 Get the most popular FRED features all in one dataframe.
 
 >>> finagg.fred.feat.economic.from_raw().head(5)
-            CIVPART_pct_change  CPIAUCNS_pct_change  CSUSHPINSA_pct_change  FEDFUNDS ...
-date                                                                                 ...
-2014-10-06                 0.0                  0.0                    0.0      0.09 ...
-2014-10-08                 0.0                  0.0                    0.0      0.09 ...
-2014-10-13                 0.0                  0.0                    0.0      0.09 ...
-2014-10-15                 0.0                  0.0                    0.0      0.09 ...
-2014-10-20                 0.0                  0.0                    0.0      0.09 ...
+            CIVPART  LOG_CHANGE(CPIAUCNS)  LOG_CHANGE(CSUSHPINSA)  FEDFUNDS ...
+date                                                                        ...
+2014-10-06     62.8                   0.0                     0.0      0.09 ...
+2014-10-08     62.8                   0.0                     0.0      0.09 ...
+2014-10-13     62.8                   0.0                     0.0      0.09 ...
+2014-10-15     62.8                   0.0                     0.0      0.09 ...
+2014-10-20     62.8                   0.0                     0.0      0.09 ...
 
 Get quarterly report features from SEC data.
 
 >>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)
-                    AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-fy   fp filed                                                                   ...
-2010 Q1 2010-01-25                 -0.023398         0.363654              2.54 ...
-     Q2 2010-04-21                  0.000000         0.363654              4.35 ...
-     Q3 2010-07-21                  0.000000         0.363654              6.40 ...
-2011 Q1 2011-01-19                  0.320805         0.433596              3.74 ...
-     Q2 2011-04-21                  0.000000         0.433596              7.12 ...
+                    LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent) ...
+fy   fp filed                                                     ...
+2010 Q1 2010-01-25            0.182629                  -0.023676 ...
+     Q2 2010-04-21            0.000000                   0.000000 ...
+     Q3 2010-07-21            0.000000                   0.000000 ...
+2011 Q1 2011-01-19            0.459174                   0.278241 ...
+     Q2 2011-04-21            0.000000                   0.000000 ...
 
 Get an aggregation of quarterly and daily features for a particular ticker.
 
 >>> finagg.fundam.feat.fundam.from_raw("AAPL").head(5)
+            PriceBookRatio  PriceEarningsRatio
+date
+2010-01-25        0.175061            2.423509
+2010-01-26        0.178035            2.464678
+2010-01-27        0.178813            2.475448
+2010-01-28        0.177154            2.452471
+2010-01-29        0.173825            2.406396
 
 Use installed features for exploring refined aggregations of raw data
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+*These methods require installing refined data through the* ``finagg install``
+*or* ``finagg <api/subpackage> install`` *commands.*
+
 Get a ticker's industry's averaged quarterly report features.
 
 >>> finagg.sec.feat.quarterly.industry.from_refined(ticker="AAPL").head(5)
-                                        avg                                  ...
-name               AssetsCurrent_pct_change DebtEquityRatio EarningsPerShare ...
-fy   fp filed                                                                ...
-2009 Q3 2009-10-30                 0.000000        0.573255         3.065000 ...
-2010 Q1 2010-04-29                -0.012229        0.402497         0.865000 ...
-     Q2 2010-07-30                 0.000000        0.500347         0.538571 ...
-     Q3 2010-11-04                 0.001145        0.456791         1.203750 ...
-2011 Q1 2011-05-05                 0.271624        0.465244         0.992000 ...
+                                 mean                           ...
+name               AssetCoverageRatio BookRatio DebtEquityRatio ...
+fy   fp filed                                                   ...
+2014 Q1 2014-05-15          10.731301  9.448954        0.158318 ...
+     Q2 2014-08-14          10.731301  9.448954        0.158318 ...
+     Q3 2014-11-14          10.731301  9.448954        0.158318 ...
+2015 Q1 2015-05-15          16.738972  9.269250        0.294238 ...
+     Q2 2015-08-13          16.738972  9.269250        0.294238 ...
 
 Get a ticker's industry-averaged quarterly report features.
 
 >>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)
-                    AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-fy   fp filed                                                                   ...
-2010 Q1 2010-01-25                 -0.257265        -0.260642          1.697972 ...
-     Q2 2010-04-21                  0.000000        -0.530932          1.508060 ...
-     Q3 2010-07-21                 -0.377964        -0.348547          1.932276 ...
-2011 Q1 2011-01-19                  0.269259        -0.110688          2.880060 ...
-     Q2 2011-04-21                  0.000000        -0.065501          2.899716 ...
+                    NORM(LOG_CHANGE(Assets))  NORM(LOG_CHANGE(AssetsCurrent)) ...
+fy   fp filed                                                                 ...
+2010 Q2 2010-04-21                  0.000000                         0.000000 ...
+     Q3 2010-07-21                  0.000000                         0.000000 ...
+2011 Q1 2011-01-19                  0.978816                         0.074032 ...
+     Q2 2011-04-21                  0.000000                         0.000000 ...
+     Q3 2011-07-20                 -0.353553                        -0.353553 ...
 
 Get tickers sorted by an industry-averaged quarterly report feature.
 
->>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by("EarningsPerShare", year=2019)[:5]
+>>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by(
+...   "EarningsPerShareBasic",
+...   year=2019
+... )[:5]
 ['XRAY', 'TSLA', 'SYY', 'WHR', 'KMB']
 
 Get tickers sorted by an industry-averaged fundamental feature.
 
 >>> finagg.fundam.feat.fundam.normalized.get_tickers_sorted_by(
 ...   "PriceEarningsRatio",
 ...   date="2019-01-04"
@@ -176,32 +208,35 @@
   ``./findata/finagg.sqlite``.
 
 Dependencies
 ============
 
 * `pandas`_ for fast, flexible, and expressive representations of relational data.
 * `requests`_ for HTTP requests to 3rd party APIs.
-* `requests-cache`_ for caching HTTP requests to avoid getting throttled by 3rd party API servers.
+* `requests-cache`_ for caching HTTP requests to avoid getting throttled by 3rd
+  party API servers.
 * `SQLAlchemy`_ for a SQL Python interface.
 * `yfinance`_ for historical stock data from Yahoo! Finance.
 
 API References
 ==============
 
 * The `BEA API`_ and the `BEA API key registration link`_.
 * The `FRED API`_ and the `FRED API key registration link`_.
 * The `SEC API`_.
 
 Related Projects
 ================
 
-* `FinRL`_ is a collection of financial reinforcement learning environments and tools.
+* `FinRL`_ is a collection of financial reinforcement learning environments
+  and tools.
 * `fredapi`_ is an implementation of the FRED API.
-* `OpenBBTerminal`_ an open-source version of the Bloomberg Terminal.
+* `OpenBBTerminal`_ is an open-source version of the Bloomberg Terminal.
 * `sec-edgar`_ is an implementation of a file-based SEC EDGAR parser.
+* `sec-edgar-api`_ is an implementation of the SEC EDGAR REST API.
 
 Frequently Asked Questions
 ==========================
 
 Where should I start?
 ---------------------
 
@@ -209,14 +244,26 @@
 environments using the implemented data features and SQL tables. This
 project was originally created to make RL environments for financial
 applications but has since focused its purpose to just aggregating financial
 data and features. That being said, all the implemented features are
 defined in such a way to make it very easy to develop financial AI/ML,
 so we encourage you to do just that!
 
+Why aren't features being installed for a specific ticker or economic data series?
+----------------------------------------------------------------------------------
+
+Implemented APIs may be relatively new and simply may not provide data for a
+particular ticker or economic data series. For example, earnings per share may
+not be accessible for all companies through the SEC EDGAR API. In some cases,
+APIs may raise an HTTP error, causing installations to skip the ticker or
+series. Additionally, not all tickers and economic data series contain
+sufficient data for feature normalization. If a ticker or series only has one
+data point, that data point could be dropped when computing a feature (such as
+percent change), causing no data to be installed.
+
 What Python versions are supported?
 -----------------------------------
 
 Python 3.10 and up are supported. We don't plan on supporting lower versions
 because 3.10 introduces some nice quality of life updates that are used
 throughout the package.
 
@@ -227,20 +274,22 @@
 using Linux or WSL in practice. The package performs a good amount of I/O and
 interprocess operations that could result in a noticeable performance
 degradation on Windows.
 
 .. _`BEA API`: https://apps.bea.gov/api/signup/
 .. _`BEA API key registration link`: https://apps.bea.gov/API/signup/
 .. _`BEA API site`: https://apps.bea.gov/API/signup/
+.. _`documentation`: https://theogognf.github.io/finagg/
 .. _`FinRL`: https://github.com/AI4Finance-Foundation/FinRL
 .. _`FRED API`: https://fred.stlouisfed.org/docs/api/fred/
 .. _`FRED API key registration link`: https://fredaccount.stlouisfed.org/login/secure/
 .. _`FRED API site`: https://fredaccount.stlouisfed.org/login/secure/
 .. _`fredapi`: https://github.com/mortada/fredapi
 .. _`OpenBBTerminal`: https://github.com/OpenBB-finance/OpenBBTerminal
 .. _`pandas`: https://pandas.pydata.org/
 .. _`requests`: https://requests.readthedocs.io/en/latest/
 .. _`requests-cache`: https://requests-cache.readthedocs.io/en/stable/
 .. _`SEC API`: https://www.sec.gov/edgar/sec-api-documentation
 .. _`sec-edgar`: https://github.com/sec-edgar/sec-edgar
+.. _`sec-edgar-api`: https://github.com/jadchaar/sec-edgar-api
 .. _`SQLAlchemy`: https://www.sqlalchemy.org/
 .. _`yfinance`: https://github.com/ranaroussi/yfinance
```

### Comparing `finagg-0.0.0b1/docs/Makefile` & `finagg-0.1.0/docs/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = api
-BUILDDIR      = _build
+BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `finagg-0.0.0b1/docs/cli.rst` & `finagg-0.1.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `finagg-0.0.0b1/docs/conf.py` & `finagg-0.1.0/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,15 +75,26 @@
     "sphinx.ext.extlinks",
     "sphinx_copybutton",
     "sphinx_rtd_theme",
     "sphinxcontrib.programoutput",
 ]
 
 templates_path = ["_templates"]
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+exclude_patterns = ["_build", "build", "Thumbs.db", ".DS_Store"]
+nitpicky = True
+nitpick_ignore = [
+    ("py:class", "requests.models.Response"),
+    ("py:class", "requests.exceptions.RequestException"),
+    ("py:class", "sqlalchemy.sql.schema.MetaData"),
+    ("py:class", "sqlalchemy.sql.schema.Table"),
+    ("py:class", "sqlalchemy.engine.base.Engine"),
+    ("py:class", "_P"),
+    ("py:exc", "NoResultFound"),
+    ("py:obj", "finagg.ratelimit._P"),
+]
 
 # -- Autodoc options ---------------------------------------------------------
 
 autodoc_member_order = "bysource"
 
 # -- doctest options ---------------------------------------------------------
 
@@ -105,8 +116,9 @@
 # -- External mapping --------------------------------------------------------
 
 python_version = ".".join(map(str, sys.version_info[0:2]))
 intersphinx_mapping = {
     "python": ("https://docs.python.org/" + python_version, None),
     "numpy": ("https://numpy.org/doc/stable", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
+    "sqlalchemy": ("https://docs.sqlalchemy.org/en/20/", None),
 }
```

### Comparing `finagg-0.0.0b1/docs/configuration.rst` & `finagg-0.1.0/docs/configuration.rst`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,19 @@
   a free API key from the `FRED API site`_.
 * ``INDICES_API_USER_AGENT`` is for scraping popular indices' compositions from
   Wikipedia and should be equivalent to a browser's user agent declaration.
   This defaults to a hardcoded value, but it may not always work.
 * ``SEC_API_USER_AGENT`` is for the Securities and Exchange Commission's API. This
   should be of the format ``FIRST_NAME LAST_NAME E_MAIL``.
 
+The ``finagg install`` CLI will point you where to get free API keys for each
+of the APIs that require one and write those API keys to a local ``.env`` file
+for storage. See the :doc:`installation docs <installation>` and
+:doc:`CLI docs <cli>` for more installation CLI details.
+
 Data Locations
 --------------
 
 **finagg**'s root path, HTTP cache path, and database path are all configurable
 through environment variables. By default, all data related to **finagg** is put
 in a ``./findata`` directory relative to a root directory. You can change these
 locations by modifying the respective environment variables:
```

### Comparing `finagg-0.0.0b1/docs/faq.rst` & `finagg-0.1.0/docs/faq.rst`

 * *Files 25% similar despite different names*

```diff
@@ -2,20 +2,32 @@
 ==========================
 
 Where should I start?
 ---------------------
 
 Aggregate some data, create some analysis notebooks, or create some RL
 environments using the implemented data features and SQL tables. This
-project was originally created for making RL environments for financial
+project was originally created to make RL environments for financial
 applications but has since focused its purpose to just aggregating financial
 data and features. That being said, all the implemented features are
 defined in such a way to make it very easy to develop financial AI/ML,
 so we encourage you to do just that!
 
+Why aren't features being installed for a specific ticker or economic data series?
+----------------------------------------------------------------------------------
+
+Implemented APIs may be relatively new and simply may not provide data for a
+particular ticker or economic data series. For example, earnings per share may
+not be accessible for all companies through the SEC EDGAR API. In some cases,
+APIs may raise an HTTP error, causing installations to skip the ticker or
+series. Additionally, not all tickers and economic data series contain
+sufficient data for feature normalization. If a ticker or series only has one
+data point, that data point could be dropped when computing a feature (such as
+percent change), causing no data to be installed.
+
 What Python versions are supported?
 -----------------------------------
 
 Python 3.10 and up are supported. We don't plan on supporting lower versions
 because 3.10 introduces some nice quality of life updates that are used
 throughout the package.
```

### Comparing `finagg-0.0.0b1/docs/index.rst` & `finagg-0.1.0/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-.. finagg documentation master file, created by
-   sphinx-quickstart on Mon Feb 27 20:01:04 2023.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
 finagg: Financial Aggregation for Python
 ========================================
 
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
 **finagg** currently supports the following free APIs:
 
-* The Bureau of Economic Analysis `(BEA) API`_.
-* The Federal Reserve Economic Data `(FRED) API`_.
-* The Securities and Exchange Commission’s `(SEC) EDGAR API`_.
+* The Bureau of Economic Analysis `(BEA) API`_. The BEA API provides methods
+  for retrieving a subset of economic statistical data as published by the BEA
+  along with metadata that describes that economic statistical data.
+* The Federal Reserve Economic Data `(FRED) API`_. The FRED API provides
+  methods for retrieving, searching, and describing economic data from a variety
+  of sources. The FRED API is one of the most popular APIs in the finance
+  industry.
+* The Securities and Exchange Commission’s `(SEC) EDGAR API`_. The SEC EDGAR
+  API provides methods for retrieving XBRL data (e.g., earnings per share) from
+  financial statements and methods for retrieving SEC filing submission
+  histories (e.g., 10-Q/10-K forms). The SEC EDGAR API is one of the few APIs
+  that provides historical and current company financial data for free.
 
 Methods for aggregating data from these APIs are organized according to their
 API/subpackage and usage (i.e., ``finagg.<api/subpackage>.<usage>``). For
 example, SEC EDGAR API methods are accesible under the subpackage
 :mod:`finagg.sec.api` (e.g., the SEC company facts API is accessible as
 :data:`finagg.sec.api.company_facts`) while features aggregated from the SEC
 EDGAR API are accessible under the fully qualified name :mod:`finagg.sec.feat`
@@ -35,119 +39,135 @@
 Explore the APIs directly
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 *These methods require internet access and API keys/user agent declarations.*
 
 Getting data from the BEA API.
 
->>> finagg.bea.api.gdp_by_industry.get(year=[2019]).head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-   table_id freq  year quarter industry                         industry_description       value
-0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting  156.300003
-1         1    Q  2019       1    111CA                                        Farms  117.599998
-2         1    Q  2019       1    113FF    Forestry, fishing, and related activities   38.700001
-3         1    Q  2019       1       21                                       Mining  305.700012
-4         1    Q  2019       1      211                       Oil and gas extraction  190.199997
+>>> finagg.bea.api.gdp_by_industry.get(year=[2019]).head(5)  # doctest: +SKIP
+   table_id freq  year quarter industry                         industry_description ...
+0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting ...
+1         1    Q  2019       1    111CA                                        Farms ...
+2         1    Q  2019       1    113FF    Forestry, fishing, and related activities ...
+3         1    Q  2019       1       21                                       Mining ...
+4         1    Q  2019       1      211                       Oil and gas extraction ...
 
 Getting data from the FRED API.
 
 >>> finagg.fred.api.series.observations.get(
 ...   "CPIAUCNS",
 ...   realtime_start=0,
 ...   realtime_end=-1,
 ...   output_type=4
-... ).head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+... ).head(5)  # doctest: +SKIP
   realtime_start realtime_end        date  value series_id
 0     1949-04-22   1953-02-26  1949-03-01  169.5  CPIAUCNS
 1     1949-05-23   1953-02-26  1949-04-01  169.7  CPIAUCNS
 2     1949-06-24   1953-02-26  1949-05-01  169.2  CPIAUCNS
 3     1949-07-22   1953-02-26  1949-06-01  169.6  CPIAUCNS
 4     1949-08-26   1953-02-26  1949-07-01  168.5  CPIAUCNS
 
 Getting data from the SEC EDGAR API.
 
->>> finagg.sec.api.company_facts.get(ticker="AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+>>> finagg.sec.api.company_facts.get(ticker="AAPL").head(5)  # doctest: +SKIP
           end        value                  accn    fy  fp    form       filed ...
 0  2009-06-27  895816758.0  0001193125-09-153165  2009  Q3    10-Q  2009-07-22 ...
 1  2009-10-16  900678473.0  0001193125-09-214859  2009  FY    10-K  2009-10-27 ...
 2  2009-10-16  900678473.0  0001193125-10-012091  2009  FY  10-K/A  2010-01-25 ...
 3  2010-01-15  906794589.0  0001193125-10-012085  2010  Q1    10-Q  2010-01-25 ...
 4  2010-04-09  909938383.0  0001193125-10-088957  2010  Q2    10-Q  2010-04-21 ...
 
 Use installed raw data for exploring the most popular features
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 *These methods require internet access, API keys/user agent declarations, and
 downloading and installing raw data through the* ``finagg install`` *or*
-the ``finagg <api/subpackage> install`` *commands.*
+``finagg <api/subpackage> install`` *commands.*
 
 Getting FRED features.
 
->>> finagg.fred.feat.economic.from_raw().head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-            CIVPART_pct_change  CPIAUCNS_pct_change  CSUSHPINSA_pct_change  FEDFUNDS ...
-date                                                                                 ...
-2014-10-06                 0.0                  0.0                    0.0      0.09 ...
-2014-10-08                 0.0                  0.0                    0.0      0.09 ...
-2014-10-13                 0.0                  0.0                    0.0      0.09 ...
-2014-10-15                 0.0                  0.0                    0.0      0.09 ...
-2014-10-20                 0.0                  0.0                    0.0      0.09 ...
+>>> finagg.fred.feat.economic.from_raw().head(5)  # doctest: +SKIP
+            CIVPART  LOG_CHANGE(CPIAUCNS)  LOG_CHANGE(CSUSHPINSA)  FEDFUNDS ...
+date                                                                        ...
+2014-10-06     62.8                   0.0                     0.0      0.09 ...
+2014-10-08     62.8                   0.0                     0.0      0.09 ...
+2014-10-13     62.8                   0.0                     0.0      0.09 ...
+2014-10-15     62.8                   0.0                     0.0      0.09 ...
+2014-10-20     62.8                   0.0                     0.0      0.09 ...
 
 Getting SEC EDGAR features.
 
->>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                    AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-fy   fp filed                                                                   ...
-2010 Q1 2010-01-25                 -0.023398         0.363654              2.54 ...
-     Q2 2010-04-21                  0.000000         0.363654              4.35 ...
-     Q3 2010-07-21                  0.000000         0.363654              6.40 ...
-2011 Q1 2011-01-19                  0.320805         0.433596              3.74 ...
-     Q2 2011-04-21                  0.000000         0.433596              7.12 ...
+>>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)  # doctest: +SKIP
+                    LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent) ...
+fy   fp filed                                                     ...
+2010 Q1 2010-01-25            0.182629                  -0.023676 ...
+     Q2 2010-04-21            0.000000                   0.000000 ...
+     Q3 2010-07-21            0.000000                   0.000000 ...
+2011 Q1 2011-01-19            0.459174                   0.278241 ...
+     Q2 2011-04-21            0.000000                   0.000000 ...
+
+Getting fundamental financial features.
+
+>>> finagg.fundam.feat.fundam.from_raw("AAPL").head(5)  # doctest: +SKIP
+            PriceBookRatio  PriceEarningsRatio
+date
+2010-01-25        0.175061            2.423509
+2010-01-26        0.178035            2.464678
+2010-01-27        0.178813            2.475448
+2010-01-28        0.177154            2.452471
+2010-01-29        0.173825            2.406396
 
 Use installed features for exploring refined aggregations of raw data
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 *These methods require installing refined data through the* ``finagg install``
 *or* ``finagg <api/subpackage> install`` *commands.*
 
 Getting industry-wide SEC EDGAR features.
 
->>> finagg.sec.feat.quarterly.industry.from_refined(ticker="AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                                        avg                                  ...
-name               AssetsCurrent_pct_change DebtEquityRatio EarningsPerShare ...
-fy   fp filed                                                                ...
-2009 Q3 2009-10-30                 0.000000        0.573255         3.065000 ...
-2010 Q1 2010-04-29                -0.012229        0.402497         0.865000 ...
-     Q2 2010-07-30                 0.000000        0.500347         0.538571 ...
-     Q3 2010-11-04                 0.001145        0.456791         1.203750 ...
-2011 Q1 2011-05-05                 0.271624        0.465244         0.992000 ...
+>>> finagg.sec.feat.quarterly.industry.from_refined(ticker="AAPL").head(5)  # doctest: +SKIP
+                                 mean                           ...            std ...
+name               AssetCoverageRatio BookRatio DebtEquityRatio ... ReturnOnAssets ...
+fy   fp filed                                                   ...                ...
+2014 Q1 2014-05-15          10.731301  9.448954        0.158318 ...       0.002048 ...
+     Q2 2014-08-14          10.731301  9.448954        0.158318 ...       0.004264 ...
+     Q3 2014-11-14          10.731301  9.448954        0.158318 ...       0.027235 ...
+2015 Q1 2015-05-15          16.738972  9.269250        0.294238 ...       0.006839 ...
+     Q2 2015-08-13          16.738972  9.269250        0.294238 ...       0.015112 ...
 
 Getting industry-normalized SEC EDGAR features.
 
->>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                    AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-fy   fp filed                                                                   ...
-2010 Q1 2010-01-25                 -0.257265        -0.260642          1.697972 ...
-     Q2 2010-04-21                  0.000000        -0.530932          1.508060 ...
-     Q3 2010-07-21                 -0.377964        -0.348547          1.932276 ...
-2011 Q1 2011-01-19                  0.269259        -0.110688          2.880060 ...
-     Q2 2011-04-21                  0.000000        -0.065501          2.899716 ...
+>>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)  # doctest: +SKIP
+                    NORM(LOG_CHANGE(Assets))  NORM(LOG_CHANGE(AssetsCurrent)) ...
+fy   fp filed                                                                 ...
+2010 Q2 2010-04-21                  0.000000                         0.000000 ...
+     Q3 2010-07-21                  0.000000                         0.000000 ...
+2011 Q1 2011-01-19                  0.978816                         0.074032 ...
+     Q2 2011-04-21                  0.000000                         0.000000 ...
+     Q3 2011-07-20                 -0.353553                        -0.353553 ...
 
 Getting tickers sorted according to industry-normalized SEC EDGAR features.
 
->>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by("EarningsPerShare", year=2019)[:5]
+>>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by(
+...   "EarningsPerShareBasic",
+...   year=2019
+... )[:5]  # doctest: +SKIP
 ['XRAY', 'TSLA', 'SYY', 'WHR', 'KMB']
 >>> finagg.fundam.feat.fundam.normalized.get_tickers_sorted_by(
 ...   "PriceEarningsRatio",
 ...   date="2019-01-04"
-... )[:5]
+... )[:5]  # doctest: +SKIP
 ['AMD', 'TRGP', 'HPE', 'CZR', 'TSLA']
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents
 
+   Conventions <conventions>
+   Walkthroughs <walkthroughs>
    Installation <installation>
    Configuration <configuration>
    CLI <cli>
    API <api/modules>
    References <references>
    FAQ <faq>
```

### Comparing `finagg-0.0.0b1/docs/installation.rst` & `finagg-0.1.0/docs/installation.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Installation
 ============
 
-Install **finagg** from GitHub directly.
+Install with pip for the latest (stable) version.
+
+.. code:: console
+
+  pip install finagg
+
+Install from GitHub for the latest (unstable) version.
 
 .. code:: console
 
     git clone https://github.com/theOGognf/finagg.git
     pip install ./finagg/
 
 Optionally install the recommended datasets from 3rd party APIs into a local
 SQL database.
 
 .. code:: console
 
-    finagg install
+    finagg install --help
 
 The installation will point you where to get free API keys for each API that
 requires one and write those API keys to a local ``.env`` file for storage.
-``finagg install`` is effectively an alias for installing the
-recommended datasets from each 3rd party API individually.
-``finagg install`` is equivalent to:
+``finagg install`` is effectively an alias for installing the recommended
+datasets from each 3rd party API individually. ``finagg install`` is equivalent
+to:
 
 .. code:: console
 
     finagg bea install
-    finagg fred install -a
-    finagg indices install -a
-    finagg sec install -a
-    finagg yfinance install -a
-    finagg fundam install -a
+    finagg fred install -a ...
+    finagg indices install -a ...
+    finagg sec install -a ...
+    finagg yfinance install -a ...
+    finagg fundam install -a ...
 
 Installation will enable offline usage of aggregated and refined financial
 features without internet access or API keys (the recommended way to explore
 data uninterrupted). See the :doc:`CLI docs <cli>` for more **finagg** CLI
 details.
```

### Comparing `finagg-0.0.0b1/docs/make.bat` & `finagg-0.1.0/docs/make.bat`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
 set SOURCEDIR=.
-set BUILDDIR=_build
+set BUILDDIR=build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
```

### Comparing `finagg-0.0.0b1/docs/references.rst` & `finagg-0.1.0/docs/references.rst`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 * The `SEC API`_.
 
 Related Projects
 ----------------
 
 * `FinRL`_ is a collection of financial reinforcement learning environments and tools.
 * `fredapi`_ is an implementation of the FRED API.
-* `OpenBBTerminal`_ an open-source version of the Bloomberg Terminal.
+* `OpenBBTerminal`_ is an open-source version of the Bloomberg Terminal.
 * `sec-edgar`_ is an implementation of a file-based SEC EDGAR parser.
+* `sec-edgar-api`_ is an implementation of the SEC EDGAR REST API.
 
 .. _`BEA API`: https://apps.bea.gov/api/signup/
 .. _`BEA API key registration link`: https://apps.bea.gov/API/signup/
 .. _`FinRL`: https://github.com/AI4Finance-Foundation/FinRL
 .. _`FRED API`: https://fred.stlouisfed.org/docs/api/fred/
 .. _`FRED API key registration link`: https://fredaccount.stlouisfed.org/login/secure/
 .. _`fredapi`: https://github.com/mortada/fredapi
 .. _`OpenBBTerminal`: https://github.com/OpenBB-finance/OpenBBTerminal
 .. _`pandas`: https://pandas.pydata.org/
 .. _`requests`: https://requests.readthedocs.io/en/latest/
 .. _`requests-cache`: https://requests-cache.readthedocs.io/en/stable/
 .. _`SEC API`: https://www.sec.gov/edgar/sec-api-documentation
 .. _`sec-edgar`: https://github.com/sec-edgar/sec-edgar
+.. _`sec-edgar-api`: https://github.com/jadchaar/sec-edgar-api
 .. _`SQLAlchemy`: https://www.sqlalchemy.org/
 .. _`yfinance`: https://github.com/ranaroussi/yfinance
```

### Comparing `finagg-0.0.0b1/pyproject.toml` & `finagg-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 readme = "README.rst"
 requires-python = ">=3.10"
 
 [project.scripts]
 finagg = "finagg.__main__:main"
 
 [project.urls]
-repository = "https://github.com/theOGognf/finagg"
+Repository = "https://github.com/theOGognf/finagg"
+Documentation = "https://theogognf.github.io/finagg/"
 
 [project.optional-dependencies]
 dev = [
     "build[virtualenv]",
     "mypy",
     "pre-commit",
     "pytest",
@@ -118,37 +119,37 @@
     build: Build the package in isolation according to PEP517, see https://github.com/pypa/build
 # https://setuptools.pypa.io/en/latest/build_meta.html#how-to-use-it
 skip_install = True
 changedir = {toxinidir}
 deps =
     build: build[virtualenv]
 commands =
-    clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/_build")]'
+    clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/build")]'
     clean: python -c 'import pathlib, shutil; [shutil.rmtree(p, True) for p in pathlib.Path("src").glob("*.egg-info")]'
     build: python -m build {posargs}
 
 [testenv:{docs,doctests,linkcheck}]
 description =
     docs: Invoke sphinx-build to build the docs
     doctests: Invoke sphinx-build to run doctests
     linkcheck: Check for broken links in the documentation
 setenv =
     DOCSDIR = {toxinidir}/docs
-    BUILDDIR = {toxinidir}/docs/_build
+    BUILDDIR = {toxinidir}/docs/build
     docs: BUILD = html
     doctests: BUILD = doctest
     linkcheck: BUILD = linkcheck
 passenv =
     BEA_API_KEY
     FRED_API_KEY
     SEC_API_USER_AGENT
 deps =
     -r {toxinidir}/docs/requirements.txt
 commands =
-    sphinx-build --color -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
+    sphinx-build -E -a --color -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
 
 [testenv:publish]
 description =
     Publish the package you have been developing to a package index server.
     By default, it uses testpypi. If you really want to publish your package
     to be publicly accessible in PyPI, use the `-- --repository pypi` option.
 skip_install = True
```

### Comparing `finagg-0.0.0b1/src/finagg/__main__.py` & `finagg-0.1.0/src/finagg/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 cli.add_command(fundam._cli.entry_point, "fundam")
 cli.add_command(indices._cli.entry_point, "indices")
 cli.add_command(sec._cli.entry_point, "sec")
 cli.add_command(yfinance._cli.entry_point, "yfinance")
 
 
 @cli.command(
-    help="Set API keys/user agents, drop and recreate tables, "
-    "and install the recommended datasets into the SQL database.",
+    help=(
+        "Set API keys/user agents, drop and recreate tables, "
+        "and install the recommended datasets into the SQL database."
+    ),
 )
 @click.option(
     "--skip",
     "-s",
     type=click.Choice(["bea", "fred", "indices", "sec", "yfinance", "fundam"]),
     multiple=True,
     help=(
@@ -112,14 +114,24 @@
         "popular and large market cap companies, while 'sec' will "
         "attempt to download and install data for nearly all "
         "publicly-traded US companies. Choosing 'indices' will be fast, "
         "while choosing 'sec' will be slow but will include more diverse data."
     ),
 )
 @click.option(
+    "--recreate-tables",
+    "-r",
+    is_flag=True,
+    default=False,
+    help=(
+        "Whether to reset the tables associated with the install options by "
+        "dropping and recreating them."
+    ),
+)
+@click.option(
     "--verbose",
     "-v",
     is_flag=True,
     default=False,
     help="Sets the log level to DEBUG to show installation errors for each ticker.",
 )
 @click.pass_context
@@ -127,14 +139,15 @@
     ctx: click.Context,
     skip: list[str] = [],
     series: list[str] = [],
     series_set: None | Literal["economic"] = None,
     stock_data: bool = False,
     ticker: list[str] = [],
     ticker_set: None | Literal["indices", "sec"] = None,
+    recreate_tables: bool = False,
     verbose: bool = False,
 ) -> None:
     if "FINAGG_ROOT_PATH" not in os.environ:
         entered_root_path = input(
             "Enter the path to your finagg root directory. finagg data will "
             "be written to /path/to/root/findata/.\n\n"
             "Root path (hit ENTER to use your current working directory): "
@@ -154,40 +167,47 @@
 
     if not stock_data and "fred" not in all_skips:
         ctx.invoke(
             fred._cli.install,
             all_=True,
             series=series,
             series_set=series_set,
+            recreate_tables=recreate_tables,
             verbose=verbose,
         )
 
     if not stock_data and "indices" not in all_skips:
         ctx.invoke(indices._cli.install, all_=True)
 
     if "sec" not in all_skips:
         ctx.invoke(
             sec._cli.install,
             all_=True,
             ticker=ticker,
             ticker_set=ticker_set,
+            recreate_tables=recreate_tables,
             verbose=verbose,
         )
 
     if "yfinance" not in all_skips:
         ctx.invoke(
             yfinance._cli.install,
             all_=True,
             ticker=ticker,
             ticker_set=ticker_set,
+            recreate_tables=recreate_tables,
             verbose=verbose,
         )
 
     if "fundam" not in all_skips:
-        ctx.invoke(fundam._cli.install, all_=True)
+        ctx.invoke(
+            fundam._cli.install,
+            all_=True,
+            recreate_tables=recreate_tables,
+        )
 
 
 def main() -> int:
     """Create and run parsers according to the given commands."""
     cli()
     return 0
```

### Comparing `finagg-0.0.0b1/src/finagg/backend.py` & `finagg-0.1.0/src/finagg/backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 Environment variables assigned in the ``.env`` file are loaded on the
 :mod:`finagg` module's first instantiation.
 
 """
 
 import os
 import pathlib
-import sqlite3
-from urllib.parse import urlparse
 
-import numpy as np
 from sqlalchemy import create_engine
 
 root_path = pathlib.Path(os.environ.get("FINAGG_ROOT_PATH", pathlib.Path.cwd()))
 """Parent directory of the ``findata`` directory where the backend database
 and API cache file will be stored (unless otherwise configured according
 to the relevant environment variables). This can be set with the
 ``FINAGG_ROOT_PATH`` environment variable. This defaults to and is typically
@@ -50,42 +47,14 @@
 """SQLAlchemy URL to the database. This can be set with the
 ``FINAGG_DATABASE_URL`` environment variable and should include a file extension.
 This defaults to ``f"sqlite:///{finagg.backend.database_path}"``.
 
 :meta hide-value:
 """
 
-
-class _NumPyStdAggregate:
-
-    values: list[float]
-
-    def __init__(self) -> None:
-        self.values = []
-
-    def step(self, value: float) -> None:
-        self.values.append(value)
-
-    def finalize(self) -> float:
-        return float(np.std(self.values))
-
-
-def _creator() -> sqlite3.Connection:
-    """Custom connection creator for enabling Write-Ahead Logging (WAL) and adding
-    aggregate functions.
-
-    Adding aggregate functions is inspired by https://stackoverflow.com/a/997467.
-
-    """
-    conn = sqlite3.connect(urlparse(database_url).path)
-    conn.create_aggregate("std", 1, _NumPyStdAggregate)  # type: ignore[arg-type]
-    conn.execute("PRAGMA journal_mode=WAL;")
-    return conn
-
-
-engine = create_engine(database_url, creator=_creator)
+engine = create_engine(database_url)
 """The default SQLAlchemy engine for the backend database. All feature and SQL
 submodules use this engine and the database URL as configured by
 :data:`database_url` for reading and writing to and from the database by default.
 
 :meta hide-value:
 """
```

### Comparing `finagg-0.0.0b1/src/finagg/bea/_cli.py` & `finagg-0.1.0/src/finagg/bea/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-0.0.0b1/src/finagg/bea/api.py` & `finagg-0.1.0/src/finagg/bea/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 """An implementation of the Bureau of Economic Analysis (BEA) API.
 
+The BEA API provides methods for retrieving a subset of economic
+statistical data as published by the BEA along with metadata that
+describes that economic statistical data.
+
 A BEA API key is required to use this API. You can register for
 a BEA API key at the `BEA API signup page`_. You can pass your
 BEA API key directly to the implemented API getters, or you
 can set the ``BEA_API_KEY`` environment variable to have the
 BEA API key be passed to the implemented API getters for you.
 
 Alternatively, running ``finagg bea install`` (or the broader
@@ -52,15 +56,15 @@
     ignored_parameters=["ResultFormat"],
     expire_after=timedelta(days=1),
 )
 
 _YEAR = int | str
 
 
-class _API(ABC):
+class API(ABC):
     """Interface for BEA Dataset APIs."""
 
     #: Request API URL.
     name: ClassVar[str]
 
     @classmethod
     @abstractmethod
@@ -76,15 +80,15 @@
     def get_parameter_values(
         cls, param: str, /, *, api_key: None | str = None
     ) -> pd.DataFrame:
         """Return all possible parameter values associated with the dataset API."""
         return _get_parameter_values(cls.name, param, api_key=api_key)
 
 
-class FixedAssets(_API):
+class FixedAssets(API):
     """US fixed assets (assets for long-term use)."""
 
     name = "FixedAssets"
 
     @classmethod
     def get(
         cls,
@@ -93,15 +97,16 @@
         *,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get US fixed assets by asset and year.
 
         Args:
             table_id: IDs associated with assets of concern.
-                Use :meth:`get_parameter_values` to see possible values.
+                Use :meth:`~finagg.bea.api.API.get_parameter_values` to see
+                possible values.
             year: Years to return.
 
         Returns:
             Dataframe with normalized column names and true dtypes.
 
         """
         if table_id == "ALL":
@@ -149,43 +154,43 @@
                 )
             )
             df["value"] = df["value"].str.replace(",", "").astype("float32")
             results.append(df)
         return pd.concat(results)
 
 
-class GDPByIndustry(_API):
+class GDPByIndustry(API):
     """GDP (a single summary statistic) for each industry.
 
     The module variable :data:`finagg.bea.api.gdp_by_industry` is an instance
     of this API implementation and is the most popular interface for querying
     this API.
 
     Data provided by this API is considered coarse/high-level.
     See :class:`InputOutput` for more granular/low-level industry data.
 
     Examples:
         List the GDP by industry API parameters.
 
-        >>> finagg.bea.api.gdp_by_industry.get_parameter_list()  # doctest: +ELLIPSIS
+        >>> finagg.bea.api.gdp_by_industry.get_parameter_list()  # doctest: +SKIP
           ParameterName ParameterDataType                               ParameterDescription ... AllValue
         0     Frequency            string                            A - Annual, Q-Quarterly ...      ALL
         1      Industry            string       List of industries to retrieve (ALL for All) ...      ALL
         2       TableID           integer  The unique GDP by Industry table identifier (A... ...      ALL
         3          Year           integer  List of year(s) of data to retrieve (ALL for All) ...      ALL
 
         List possible GDP by industry tables we can query.
 
-        >>> finagg.bea.api.gdp_by_industry.get_parameter_values("TableID").head(5)
-                                                  ParamValue
-        0  {'Key': '1', 'Desc': 'Value Added by Industry ...
-        1  {'Key': '5', 'Desc': 'Value added by Industry ...
-        2  {'Key': '6', 'Desc': 'Components of Value Adde...
-        3  {'Key': '7', 'Desc': 'Components of Value Adde...
-        4  {'Key': '8', 'Desc': 'Chain-Type Quantity Inde...
+        >>> finagg.bea.api.gdp_by_industry.get_parameter_values("TableID").head(5)  # doctest: +SKIP
+          Key                                               Desc
+        0   1                    Value Added by Industry (A) (Q)
+        1   5  Value added by Industry as a Percentage of Gro...
+        2   6          Components of Value Added by Industry (A)
+        3   7  Components of Value Added by Industry as a Per...
+        4   8  Chain-Type Quantity Indexes for Value Added by...
 
     """
 
     name = "GdpByIndustry"
 
     @classmethod
     def get(
@@ -196,31 +201,33 @@
         industry: str | Sequence[str] = "ALL",
         *,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get GDP by industry.
 
         Args:
-            table_id: IDs associated with GDP value type. Use :meth:`get_parameter_values`
-                to see possible values. `"ALL"` indicates retrieve all GDP value
+            table_id: IDs associated with GDP value type. Use
+                :meth:`~finagg.bea.api.API.get_parameter_values` to see
+                possible values. `"ALL"` indicates retrieve all GDP value
                 measurement type tables.
             freq: Data frequency to return. `"Q"` for quarterly, `"A"` for
                 annually, and `"A,Q"` for both annually and quarterly.
             year: Years to return. `"ALL"` indicates retrieve data for all
                 available years.
-            industry: IDs associated with industries. Use :meth:`get_parameter_values`
-                to see possible values.
+            industry: IDs associated with industries. Use
+                :meth:`~finagg.bea.api.API.get_parameter_values` to see
+                possible values.
 
         Returns:
             Dataframe with GDP by industry, separated by year and/or quarter.
 
         Examples:
             Get the GDP value added by an industry for a specific year.
 
-            >>> finagg.bea.api.gdp_by_industry.get(table_id=1, freq="A", year=2020).head(5)
+            >>> finagg.bea.api.gdp_by_industry.get(table_id=1, freq="A", year=2020).head(5)  # doctest: +SKIP
                table_id freq  year quarter industry                         industry_description  value
             0         1    A  2020    2020       11  Agriculture, forestry, fishing, and hunting  162.2
             1         1    A  2020    2020    111CA                                        Farms  120.7
             2         1    A  2020    2020    113FF    Forestry, fishing, and related activities   41.5
             3         1    A  2020    2020       21                                       Mining  201.1
             4         1    A  2020    2020      211                       Oil and gas extraction  110.9
 
@@ -265,15 +272,15 @@
                 "industry": "category",
                 "industry_description": "object",
                 "value": "float32",
             }
         )
 
 
-class InputOutput(_API):
+class InputOutput(API):
     """Specific input-output statistics for each industry.
 
     Data provided by this API is considered granular/low-level.
     See :class:`GDPByIndustry` for more coarse/high-level industry data.
 
     Data is provided for different "rows" and "columns" where:
         - a row is an industry and
@@ -295,17 +302,17 @@
         *,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get input-output statistics by industry.
 
         Args:
             table_id: IDs associated with input-output stats. Use
-                :meth:`get_parameter_values` to see possible values.
-                `"ALL"` indicates retrieve all tables for all types
-                of input-output statistics by industry.
+                :meth:`~finagg.bea.api.API.get_parameter_values` to see
+                possible values. `"ALL"` indicates retrieve all tables for
+                all types of input-output statistics by industry.
             year: Years to return. `"ALL"` indicates retrieve data for all
                 available years.
 
         Returns:
             Dataframe organized by table row and column codes.
 
         """
@@ -345,15 +352,15 @@
                     "col_type": "category",
                     "value": "float32",
                 }
             )
         )
 
 
-class NIPA(_API):
+class NIPA(API):
     """National income and product accounts.
 
     Details high-level US economic details in several
     metrics.
 
     """
 
@@ -368,15 +375,16 @@
         *,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get US income and product accounts by metric.
 
         Args:
             table_id: IDs associated with metric of concern.
-                Use :meth:`get_parameter_values` to see possible values.
+                Use :meth:`~finagg.bea.api.API.get_parameter_values` to see
+                possible values.
             freq: Data frequency to return. `"Q"` for quarterly, `"A"` for annually.
             year: Years to return.
 
         Returns:
             Dataframe with normalized column names and true dtypes.
 
         """
@@ -428,36 +436,37 @@
             )
             df["value"] = df["value"].str.replace(",", "").astype("float32")
             results.append(df)
         return pd.concat(results)
 
 
 fixed_assets = FixedAssets()
-"""The most popular way for accessing the :class:`FixedAssets` API
-implementation.
+"""The most popular way for accessing the :class:`finagg.bea.api.FixedAssets`
+API implementation.
 
 :meta hide-value:
 """
 
 gdp_by_industry = GDPByIndustry()
-"""The most popular way for accessing the :class:`GDPByIndustry` API
-implementation.
+"""The most popular way for accessing the :class:`finagg.bea.api.GDPByIndustry`
+API implementation.
 
 :meta hide-value:
 """
 
 input_output = InputOutput()
-"""The most popular way for accessing the :class:`InputOutput` API
-implementation.
+"""The most popular way for accessing the :class:`finagg.bea.api.InputOutput`
+API implementation.
 
 :meta hide-value:
 """
 
 nipa = NIPA()
-"""The most popular way for accessing the :class:`NIPA` API implementation.
+"""The most popular way for accessing the :class:`finagg.bea.api.NIPA`
+API implementation.
 
 :meta hide-value:
 """
 
 #: The BEA API endpoint URL. All API requests are made to this URL.
 url = "https://apps.bea.gov/api/data"
 
@@ -547,15 +556,15 @@
 
     """
     params = {
         "Method": "GetParameterValues",
         "DatasetName": dataset,
         "ParameterName": param,
     }
-    results = _get(params, api_key=api_key)
+    results = _get(params, api_key=api_key)["ParamValue"]
     return pd.DataFrame(results)
 
 
 @ratelimit.guard(
     [
         ratelimit.RequestLimit(90, timedelta(minutes=1)),
         ratelimit.ErrorLimit(20, timedelta(minutes=1)),
@@ -570,15 +579,15 @@
 def get_dataset_list(*, api_key: None | str = None) -> pd.DataFrame:
     """Return a list of datasets provided by the BEA API.
 
     Returns:
         A dataframe describing the datasets available through the BEA API.
 
     Examples:
-        >>> finagg.bea.api.get_dataset_list()
+        >>> finagg.bea.api.get_dataset_list()  # doctest: +SKIP
                         DatasetName                    DatasetDescription
         0                      NIPA                  Standard NIPA tables
         1        NIUnderlyingDetail  Standard NI underlying detail tables
         2                       MNE             Multinational Enterprises
         3               FixedAssets          Standard Fixed Assets tables
         4                       ITA   International Transactions Accounts
         5                       IIP     International Investment Position
```

### Comparing `finagg-0.0.0b1/src/finagg/frame.py` & `finagg-0.1.0/src/finagg/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,25 @@
         if seq[0] not in {1, 2}:
             return False
     return True
 
 
 @dataclass
 class FiscalDelta:
-    """A displacement or change from a :class:`FiscalFrame`."""
+    """A displacement or change from a :class:`FiscalFrame`.
+
+    Examples:
+        Get the total number of quarters from a fiscal delta.
+
+        >>> from finagg.frame import FiscalDelta
+        >>> delta = FiscalDelta(2, 2)
+        >>> int(delta)
+        10
+
+    """
 
     #: Year delta.
     years: int = 0
 
     #: Quarter delta.
     quarters: int = 0
 
@@ -92,25 +102,25 @@
         FiscalFrame(year=1997, quarter=3)
 
         Adding/subtracting with integers assumes integers are quarters.
 
         >>> frame + 2
         FiscalFrame(year=1995, quarter=3)
 
-        Adding/subtracting with tuples converts tuuples to :class:`FiscalDelta`.
+        Adding/subtracting with tuples converts tuples to :class:`FiscalDelta`.
 
         >>> frame + (2, 2)
         FiscalFrame(year=1997, quarter=3)
 
         Getting quarter differences between frames and determining if the sequence
         is a valid, ordered quarterly sequence.
 
         >>> from finagg.frame import FiscalFrame, is_valid_fiscal_seq
         >>> df = finagg.sec.api.company_concept.get("AssetsCurrent", ticker="AAPL")
-        >>> df = finagg.sec.feat.get_unique_filings(df, form="10-Q", units="USD")
+        >>> df = finagg.sec.api.get_unique_filings(df, form="10-Q", units="USD")
         >>> frames: pd.Series = df["fy"].astype(int).astype(str) + df["fp"].astype(str)
         >>> frames = frames.apply(lambda row: FiscalFrame.fromstr(row))
         >>> frames = frames.diff(periods=1).dropna().astype(int)
         >>> is_valid_fiscal_seq(frames.tolist())
         True
 
     """
@@ -163,26 +173,28 @@
         self.year = int(self.year) + (quarters_place // 4)
         self.quarter = (quarters_place % 4) + 1
 
     def __sub__(self, other: object) -> Union[FiscalDelta, "FiscalFrame"]:
         """Subtract quarters and/or years from a fiscal frame."""
         if not isinstance(other, int | FiscalDelta | FiscalFrame | tuple):
             raise TypeError(
-                f"can only subtract {int.__name__}, {FiscalDelta.__name__}, "
-                f"{tuple.__name__}, and {self.__class__.__name__} from "
-                f"{self.__class__.__name__} but got `{other.__class__.__name__}` instead."
+                f"can only subtract {int.__name__}, {FiscalDelta.__name__},"
+                f" {tuple.__name__}, and {self.__class__.__name__} from"
+                f" {self.__class__.__name__} but got `{other.__class__.__name__}`"
+                " instead."
             )
 
         if isinstance(other, tuple):
             years, quarters = other
             other = FiscalDelta(years, quarters)
 
         if isinstance(other, int | FiscalDelta):
             return self.__add__(-other)
 
         return FiscalDelta(self.year - other.year, self.quarter - other.quarter)
 
     @classmethod
     def fromstr(cls, s: str, /) -> "FiscalFrame":
-        """Split a string into year-quarter parts by splitting on alphabetical characters."""
+        """Split a string into year-quarter parts by splitting on alphabetical characters.
+        """
         year, quarter = [c for c in re.split("[a-zA-Z]", s) if c]
         return cls(int(year), int(quarter))
```

### Comparing `finagg-0.0.0b1/src/finagg/fred/api/_api.py` & `finagg-0.1.0/src/finagg/fred/api/_api.py`

 * *Files identical despite different names*

### Comparing `finagg-0.0.0b1/src/finagg/fred/api/category_.py` & `finagg-0.1.0/src/finagg/fred/api/_category.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 """
 
 import pandas as pd
 
 from . import _api
 
 
-class Children(_api.API):
+class CategoryChildren(_api.API):
     """Get FRED child categories.
 
-    The class variable :data:`finagg.fred.api.category.children` is an instance
-    of this API implementation and is the most popular interface for calling
-    this API.
+    The class variable :attr:`finagg.fred.api.Category.children`
+    is an instance of this API implementation and is the most popular
+    interface for calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/category/children"
 
     @classmethod
     def get(
@@ -47,15 +47,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for a category's children.
 
         Examples:
-            >>> finagg.fred.api.category.children.get()  # doctest: NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.category.children.get()  # doctest: +SKIP
                   id                                     name  parent_id
             0  32991                Money, Banking, & Finance          0
             1     10  Population, Employment, & Labor Markets          0
             2  32992                        National Accounts          0
             3      1           Production & Business Activity          0
             4  32455                                   Prices          0
             5  32263                       International Data          0
@@ -70,18 +70,18 @@
             realtime_end=realtime_end,
             api_key=api_key,
         ).json()
         data = data["categories"]
         return pd.DataFrame(data)
 
 
-class Related(_api.API):
+class CategoryRelated(_api.API):
     """Get FRED related categories.
 
-    The class variable :data:`finagg.fred.api.category.related` is an instance
+    The class variable :attr:`finagg.fred.api.Category.related` is an instance
     of this API implementation and is the most popular interface for calling
     this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/category/related"
 
@@ -119,23 +119,22 @@
         data = _api.get(
             cls.url,
             category_id=category_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             api_key=api_key,
         ).json()
-        print(data)
         data = data["categories"]
         return pd.DataFrame(data)
 
 
-class Series(_api.API):
+class CategorySeries(_api.API):
     """Get FRED series within a category.
 
-    The class variable :data:`finagg.fred.api.category.series` is an instance
+    The class variable :attr:`finagg.fred.api.Category.series` is an instance
     of this API implementation and is the most popular interface for calling
     this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/category/series"
 
@@ -197,15 +196,15 @@
                 environment variable.
 
         Returns:
             A dataframe containing data for a category's series
             according to the given parameters.
 
         Examples:
-            >>> finagg.fred.api.category.series.get(33951)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.category.series.get(33951)  # doctest: +SKIP
                       id realtime_start realtime_end                                              title ...
             0   FFHTHIGH     2023-03-15   2023-03-15  High Value of the Federal Funds Rate for the I... ...
             1    FFHTLOW     2023-03-15   2023-03-15  Low Value of the Federal Funds Rate for the In... ...
             2  FFWSJHIGH     2023-03-15   2023-03-15  High Value of the Federal Funds Rate for the I... ...
             3   FFWSJLOW     2023-03-15   2023-03-15  Low Value of the Federal Funds Rate for the In... ...
 
         """
@@ -224,18 +223,18 @@
             exclude_tag_names=exclude_tag_names,
             api_key=api_key,
         ).json()
         data = data["seriess"]
         return pd.DataFrame(data)
 
 
-class Tags(_api.API):
+class CategoryTags(_api.API):
     """Get FRED category's tags.
 
-    The class variable :data:`finagg.fred.api.category.tags` is an instance
+    The class variable :attr:`finagg.fred.api.Category.tags` is an instance
     of this API implementation and is the most popular interface for calling
     this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/category/tags"
 
@@ -297,15 +296,15 @@
                 environment variable.
 
         Returns:
             A dataframe containing data for a category's tags
             according to the given parameters.
 
         Examples:
-            >>> finagg.fred.api.category.tags.get(33951, limit=5)  # doctest: +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.category.tags.get(33951, limit=5)  # doctest: +SKIP
                         name group_id notes                 created  popularity  series_count
             0   anbil, sriya      src        2020-07-03 11:52:33-05          16             8
             1  carlson, mark      src        2020-07-03 11:53:20-05          16             8
             2          daily     freq        2012-02-27 10:18:19-06          71             8
             3        federal      gen        2012-02-27 10:18:19-06          60             8
             4          funds      gen  None  2020-05-11 13:13:02-05          28             8
 
@@ -324,18 +323,18 @@
             search_text=search_text,
             api_key=api_key,
         ).json()
         data = data["tags"]
         return pd.DataFrame(data)
 
 
-class RelatedTags(_api.API):
+class CategoryRelatedTags(_api.API):
     """Get FRED category's related tags.
 
-    The class variable :data:`finagg.fred.api.category.related_tags` is an
+    The class variable :attr:`finagg.fred.api.Category.related_tags` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/category/related_tags"
 
@@ -399,15 +398,15 @@
                 environment variable.
 
         Returns:
             A dataframe containing data for tags related to a category
             according to the given parameters.
 
         Examples:
-            >>> finagg.fred.api.category.related_tags.get(33951, tag_names="funds")  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.category.related_tags.get(33951, tag_names="funds")  # doctest: +SKIP
                                              name group_id                     notes ...
             0                        anbil, sriya      src                           ...
             1                       carlson, mark      src                           ...
             2                               daily     freq                           ...
             3                             federal      gen                           ...
             4                  hanes, christopher      src                           ...
             5                            interest      gen                           ...
@@ -437,53 +436,58 @@
             api_key=api_key,
         ).json()
         data = data["tags"]
         return pd.DataFrame(data)
 
 
 class Category(_api.API):
-    """Collection of `fred/category` APIs.
+    """Collection of "fred/category" APIs.
 
     The class variable :data:`finagg.fred.api.category` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
-    children = Children()
+    children = CategoryChildren()
     """"category/children" FRED API. Get the children of a category.
-    The most popular way for accessing the :class:`Children` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.CategoryChildren` API.
 
     :meta hide-value:
     """
 
-    related = Related()
+    related = CategoryRelated()
     """"category/related" FRED API. Get categories related to a category.
-    The most popular way for accessing the :class:`Related` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.CategoryRelated` API.
 
     :meta hide-value:
     """
 
-    related_tags = RelatedTags()
+    related_tags = CategoryRelatedTags()
     """"category/related_tags" FRED API. Get tags related to a category.
-    The most popular way for accessing the :class:`RelatedTags` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.CategoryRelatedTags` API.
 
     :meta hide-value:
     """
 
-    series = Series()
+    series = CategorySeries()
     """"category/series" FRED API. Get a category's series.
-    The most popular way for accessing the :class:`Series` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.CategorySeries` API.
 
     :meta hide-value:
     """
 
-    tags = Tags()
+    tags = CategoryTags()
     """"category/tags" FRED API. Get a category's tags.
-    The most popular way for accessing the :class:`Tags` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.CategoryTags` API.
 
     :meta hide-value:
     """
 
     url = "https://api.stlouisfed.org/fred/category"
 
     @classmethod
@@ -496,22 +500,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             Dataframe of category details.
 
         Examples:
-            >>> finagg.fred.api.category.get()  # doctest: +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.category.get()  # doctest: +SKIP
                id        name  parent_id
             0   0  Categories          0
 
         """
         data = _api.get(cls.url, category_id=category_id, api_key=api_key).json()
         data = data["categories"]
         return pd.DataFrame(data)
-
-
-category = Category()
-"""The most popular way for accessing the :class:`Category`.
-
-:meta hide-value:
-"""
```

### Comparing `finagg-0.0.0b1/src/finagg/fred/api/release_.py` & `finagg-0.1.0/src/finagg/fred/api/_release.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from . import _api
 
 
 class ReleasesDates(_api.API):
     """Get all release dates of FRED economic data.
 
-    The class variable :data:`finagg.fred.api.releases.dates` is an instance
+    The class variable :attr:`finagg.fred.api.Releases.dates` is an instance
     of this API implementation and is the most popular interface for calling
     this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/releases/dates"
 
@@ -82,15 +82,16 @@
 
 
 class Releases(_api.API):
     """Get all releases of economic data."""
 
     dates = ReleasesDates()
     """"releases/dates" FRED API. Get dates for releases of economic data.
-    The most popular way for accessing the :class:`ReleasesDates` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.ReleasesDates` API.
 
     :meta hide-value:
     """
 
     url = "https://api.stlouisfed.org/fred/releases"
 
     @classmethod
@@ -149,15 +150,15 @@
         data = data["releases"]
         return pd.DataFrame(data)
 
 
 class ReleaseDates(_api.API):
     """Get dates associated with an economic release.
 
-    The class variable :data:`finagg.fred.api.release.dates` is an
+    The class variable :attr:`finagg.fred.api.Release.dates` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/release/dates"
 
@@ -211,18 +212,18 @@
             include_release_dates_with_no_data=include_release_dates_with_no_data,
             api_key=api_key,
         ).json()
         data = data["release_dates"]
         return pd.DataFrame(data)
 
 
-class Series(_api.API):
+class ReleaseSeries(_api.API):
     """Get series associated with an economic release.
 
-    The class variable :data:`finagg.fred.api.release.series` is an
+    The class variable :attr:`finagg.fred.api.Release.series` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/release/series"
 
@@ -308,18 +309,18 @@
             exclude_tag_names=exclude_tag_names,
             api_key=api_key,
         ).json()
         data = data["seriess"]
         return pd.DataFrame(data)
 
 
-class Sources(_api.API):
+class ReleaseSources(_api.API):
     """Get sources associated with an economic release.
 
-    The class variable :data:`finagg.fred.api.release.sources` is an
+    The class variable :attr:`finagg.fred.api.Release.sources` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/release/sources"
 
@@ -359,18 +360,18 @@
             realtime_end=realtime_end,
             api_key=api_key,
         ).json()
         data = data["sources"]
         return pd.DataFrame(data)
 
 
-class Tags(_api.API):
+class ReleaseTags(_api.API):
     """Get tags for an economic release.
 
-    The class variable :data:`finagg.fred.api.release.tags` is an
+    The class variable :attr:`finagg.fred.api.Release.tags` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/release/tags"
 
@@ -449,18 +450,18 @@
             sort_order=sort_order,
             api_key=api_key,
         ).json()
         data = data["tags"]
         return pd.DataFrame(data)
 
 
-class RelatedTags(_api.API):
+class ReleaseRelatedTags(_api.API):
     """Get tags related to an economic release.
 
-    The class variable :data:`finagg.fred.api.release.related_tags` is an
+    The class variable :attr:`finagg.fred.api.Release.related_tags` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/release/related_tags"
 
@@ -542,18 +543,18 @@
             sort_order=sort_order,
             api_key=api_key,
         ).json()
         data = data["tags"]
         return pd.DataFrame(data)
 
 
-class Tables(_api.API):
+class ReleaseTables(_api.API):
     """Get tables associated with an economic release.
 
-    The class variable :data:`finagg.fred.api.release.tables` is an instance of
+    The class variable :attr:`finagg.fred.api.Release.tables` is an instance of
     this API implementation and is the most popular interface for calling this
     API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/release/tables"
 
@@ -606,50 +607,56 @@
     The class variable :data:`finagg.fred.api.release` is an instance of this
     API implementation and is the most popular interface for calling this API.
 
     """
 
     dates = ReleaseDates()
     """"release/dates" FRED API. Get economic release dates.
-    The most popular way for accessing the :class:`ReleaseDates` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.ReleaseDates` API.
 
     :meta hide-value:
     """
 
-    related_tags = RelatedTags()
+    related_tags = ReleaseRelatedTags()
     """"release/related_tags" FRED API. Get tags related to an economic release.
-    The most popular way for accessing the :class:`RelatedTags` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.ReleaseRelatedTags` API.
 
     :meta hide-value:
     """
 
-    series = Series()
+    series = ReleaseSeries()
     """"release/series" FRED API. Get the series of an economic release.
-    The most popular way for accessing the :class:`Series` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.ReleaseSeries` API.
 
     :meta hide-value:
     """
 
-    sources = Sources()
+    sources = ReleaseSources()
     """"release/sources" FRED API. Get the sources for an economic release.
-    The most popular way for accessing the :class:`Sources` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.ReleaseSources` API.
 
     :meta hide-value:
     """
 
-    tables = Tables()
+    tables = ReleaseTables()
     """"release/tables" FRED API. Get the tables of an economic release.
-    The most popular way for accessing the :class:`Tables` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.ReleaseTables` API.
 
     :meta hide-value:
     """
 
-    tags = Tags()
+    tags = ReleaseTags()
     """"release/tags" FRED API. Get tags of an economic release.
-    The most popular way for accessing the :class:`Tags` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.ReleaseTags` API.
 
     :meta hide-value:
     """
 
     url = "https://api.stlouisfed.org/fred/release"
 
     @classmethod
@@ -686,20 +693,7 @@
             release_id=release_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             api_key=api_key,
         ).json()
         data = data["releases"]
         return pd.DataFrame(data)
-
-
-releases = Releases()
-"""The most popular way for accessing :class:`Releases`.
-
-:meta hide-value:
-"""
-
-release = Release()
-"""The most popular way for accessing :class:`Release`.
-
-:meta hide-value:
-"""
```

### Comparing `finagg-0.0.0b1/src/finagg/fred/api/series_.py` & `finagg-0.1.0/src/finagg/fred/api/_series.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 See the official FRED API docs for more info:
 
     https://fred.stlouisfed.org/docs/api/fred/
 
 """
 
 import pandas as pd
+from requests import HTTPError
 
 from . import _api
 
 
-class Categories(_api.API):
+class SeriesCategories(_api.API):
     """Get the categories for an economic data series.
 
-    The class variable :data:`finagg.fred.api.series.categories` is an
+    The class variable :attr:`finagg.fred.api.Series.categories` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/series/categories"
 
@@ -53,15 +54,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data on categories for the economic data series.
 
         Examples:
-            >>> finagg.fred.api.series.categories.get("CPIAUCNS")  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.series.categories.get("CPIAUCNS")  # doctest: +SKIP
                id                                  name  parent_id
             0   9  Consumer Price Indexes (CPI and PCE)      32455
 
         """
         data = _api.get(
             cls.url,
             series_id=series_id,
@@ -69,19 +70,19 @@
             realtime_end=realtime_end,
             api_key=api_key,
         ).json()
         data = data["categories"]
         return pd.DataFrame(data)
 
 
-class Observations(_api.API):
+class SeriesObservations(_api.API):
     """Get the observations or data values for an economic data series.
 
     This is by far the most popular FRED API method. The class variable
-    :data:`finagg.fred.api.series.observations` is an instance of this
+    :attr:`finagg.fred.api.Series.observations` is an instance of this
     API implementation and is the most popular interface for calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/series/observations"
 
     @classmethod
@@ -185,15 +186,15 @@
 
         Examples:
             >>> finagg.fred.api.series.observations.get(
             ...     "CPIAUCNS",
             ...     realtime_start=0,
             ...     realtime_end=-1,
             ...     output_type=4
-            ... ).head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            ... ).head(5)  # doctest: +SKIP
               realtime_start realtime_end        date  value series_id
             0     1949-04-22   1953-02-26  1949-03-01  169.5  CPIAUCNS
             1     1949-05-23   1953-02-26  1949-04-01  169.7  CPIAUCNS
             2     1949-06-24   1953-02-26  1949-05-01  169.2  CPIAUCNS
             3     1949-07-22   1953-02-26  1949-06-01  169.6  CPIAUCNS
             4     1949-08-26   1953-02-26  1949-07-01  168.5  CPIAUCNS
 
@@ -214,21 +215,143 @@
             output_type=output_type,
             vintage_dates=vintage_dates,
             api_key=api_key,
         ).json()
         data = data["observations"]
         df = pd.DataFrame(data)
         df["series_id"] = series_id
+        df["value"] = pd.to_numeric(df["value"], errors="coerce")
         return df
 
+    @classmethod
+    def get_first_observations(
+        cls,
+        series_id: str,
+        /,
+        *,
+        limit: None | int = 100000,
+        offset: None | int = 0,
+        sort_order: None | str = None,
+        observation_start: None | int | str = None,
+        observation_end: None | int | str = None,
+        units: None | str = "lin",
+        frequency: None | str = None,
+        aggregation_method: None | str = "avg",
+        api_key: None | str = None,
+    ) -> pd.DataFrame:
+        """Get only the initial releases/observations for an
+        economic data series.
+
+        Similar to :meth:`SeriesObservations.get`, but tries to get initial
+        releases/observations only.
+
+        Args:
+            series_id: The ID for a series.
+            limit: Maximum number of results to return.
+            offset: Result start offset.
+            sort_order: Sort results in ascending ("asc") or
+                descending ("desc") order.
+            observation_start: The start date of the observation period.
+            observation_end: The end date of the observation period.
+            units: Units to return the series values in. Options include:
+
+                - "lin" = levels (no unit transformation)
+                - "chg" = change
+                - "ch1" = change from a year ago
+                - "pch" = percent change
+                - "pc1" = percent change from a year ago
+                - "pca" = compounded annual rate of change
+                - "cch" = continuously compounded rate of change
+                - "cca" = continuously compounded annual rate of change
+                - "log" = natural log
+
+            frequency: An optional parameter that indicates a lower frequency to
+                aggregate values to. Frequency options without period descriptions
+                include:
+
+                    - "d" = daily
+                    - "w" = weekly
+                    - "bw" = biweekly
+                    - "m" = monthly
+                    - "q" = quarterly
+                    - "sa" = semiannual
+                    - "a" = annual
+
+                Frequency options with period descriptions include:
+
+                    - "wef" = weekly, ending Friday
+                    - "weth" = weekly, ending Thursday
+                    - "wetu" = weekly, ending Wednesday
+                    - "wem" = weekly, ending Monday
+                    - "wesu" = weekly, ending Sunday
+                    - "wesa" = weekly, ending Saturday
+                    - "bwew" = weekly, ending Wednesday
+                    - "bwem" = weekly, Monday
+
+            aggregation_method: A key that indicates the aggregation method used
+                for frequency aggregation. Options include:
+
+                    - "avg" = average
+                    - "sum" = sum
+                    - "eop" = end of period
 
-class Release(_api.API):
+            api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
+                environment variable.
+
+        Returns:
+            A dataframe containing economic data series observations/values according to
+            the given parameters.
+
+        Examples:
+            >>> finagg.fred.api.series.observations.get_first_observations(
+            ...     "CPIAUCNS",
+            ... ).head(5)  # doctest: +SKIP
+              realtime_start realtime_end        date  value series_id
+            0     1949-04-22   1953-02-26  1949-03-01  169.5  CPIAUCNS
+            1     1949-05-23   1953-02-26  1949-04-01  169.7  CPIAUCNS
+            2     1949-06-24   1953-02-26  1949-05-01  169.2  CPIAUCNS
+            3     1949-07-22   1953-02-26  1949-06-01  169.6  CPIAUCNS
+            4     1949-08-26   1953-02-26  1949-07-01  168.5  CPIAUCNS
+
+        """
+        try:
+            return cls.get(
+                series_id,
+                realtime_start=0,
+                realtime_end=-1,
+                limit=limit,
+                offset=offset,
+                sort_order=sort_order,
+                observation_start=observation_start,
+                observation_end=observation_end,
+                units=units,
+                frequency=frequency,
+                aggregation_method=aggregation_method,
+                output_type=4,
+                api_key=api_key,
+            )
+        except HTTPError:
+            return cls.get(
+                series_id,
+                limit=limit,
+                offset=offset,
+                sort_order=sort_order,
+                observation_start=observation_start,
+                observation_end=observation_end,
+                units=units,
+                frequency=frequency,
+                aggregation_method=aggregation_method,
+                api_key=api_key,
+            )
+
+
+class SeriesRelease(_api.API):
     """Get the latest release for an economic data seris.
 
-    The class variable :data:`finagg.fred.api.series.release` is an
+    The class variable :attr:`finagg.fred.api.Series.release` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/series/release"
 
@@ -268,18 +391,18 @@
             realtime_end=realtime_end,
             api_key=api_key,
         ).json()
         data = data["releases"]
         return pd.DataFrame(data)
 
 
-class SearchRelatedTags(_api.API):
+class SeriesSearchRelatedTags(_api.API):
     """Search for series tags related to a series's tags.
 
-    The class variable :data:`finagg.fred.api.series.search.related_tags` is an
+    The class variable :attr:`finagg.fred.api.SeriesSearch.related_tags` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/series/search/related_tags"
 
@@ -344,15 +467,15 @@
 
         Returns:
             A dataframe containing related FRED tags for a series search.
             The dataframe can have results optionally filtered by the FRED
             servers according to the method's args.
 
         Examples:
-            >>> finagg.fred.api.series.search.related_tags.get("price index", tag_names="price", limit=5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.series.search.related_tags.get("price index", tag_names="price", limit=5)  # doctest: +SKIP
                                             name group_id                    notes                 created ...
             0                                nsa     seas  Not Seasonally Adjusted  2012-02-27 10:18:19-06 ...
             1                            indexes      gen                           2012-02-27 10:18:19-06 ...
             2                        price index      gen                           2012-02-27 10:18:19-06 ...
             3                            monthly     freq                           2012-02-27 10:18:19-06 ...
             4  public domain: citation requested       cc                     None  2018-12-17 23:33:13-06 ...
 
@@ -372,18 +495,18 @@
             sort_order=sort_order,
             api_key=api_key,
         ).json()
         data = data["tags"]
         return pd.DataFrame(data)
 
 
-class SearchTags(_api.API):
+class SeriesSearchTags(_api.API):
     """Get FRED series tags.
 
-    The class variable :data:`finagg.fred.api.series.search.tags` is an
+    The class variable :attr:`finagg.fred.api.SeriesSearch.tags` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/series/search/tags"
 
@@ -446,15 +569,15 @@
 
         Returns:
             A dataframe containing FRED tags for a series search.
             The dataframe can have results optionally filtered by the FRED
             servers according to the method's args.
 
         Examples:
-            >>> finagg.fred.api.series.search.tags.get("price index", limit=5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.series.search.tags.get("price index", limit=5)  # doctest: +SKIP
                                             name group_id                    notes ...
             0                                nsa     seas  Not Seasonally Adjusted ...
             1                              price      gen                          ...
             2                            indexes      gen                          ...
             3                        price index      gen                          ...
             4  public domain: citation requested       cc                     None ...
 
@@ -473,34 +596,35 @@
             sort_order=sort_order,
             api_key=api_key,
         ).json()
         data = data["tags"]
         return pd.DataFrame(data)
 
 
-class Search(_api.API):
+class SeriesSearch(_api.API):
     """Get economic data series that match search text.
 
-    The class variable :data:`finagg.fred.api.series.search` is an
+    The class variable :attr:`finagg.fred.api.Series.search` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
-    related_tags = SearchRelatedTags()
+    related_tags = SeriesSearchRelatedTags()
     """"series/search/related_tags" FRED API. Get the related tags for a
-    series search. The most popular way for accessing the :class:`SearchTags`
-    API.
+    series search. The most popular way for accessing the
+    :class:`finagg.fred.api.SeriesSearchRelatedTags` API.
 
     :meta hide-value:
     """
 
-    tags = SearchTags()
+    tags = SeriesSearchTags()
     """"series/search/tags" FRED API. Get the tags for a series search.
-    The most popular way for accessing the :class:`SearchTags` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.SeriesSearchTags` API.
 
     :meta hide-value:
     """
 
     url = "https://api.stlouisfed.org/fred/series/search"
 
     @classmethod
@@ -529,15 +653,15 @@
             https://fred.stlouisfed.org/docs/api/fred/series_search.html
 
         Args:
             search_text: The words to match against economic data series.
             search_type: Determines the type of search to perform. Options include:
 
                 - "full_text" = search series attributes, units, frequency,
-                    and tags by parsing words into stems.
+                  and tags by parsing words into stems.
                 - "series_id" = performs a substring search on series IDs.
 
             realtime_start: Start date for fetching results
                 according to their publication date.
             realtime_end: End date for fetching results according
                 to their publication date.
             limit: Maximum number of results to return.
@@ -574,15 +698,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data on series matching the search.
 
         Examples:
-            >>> finagg.fred.api.series.search.get("price index", limit=5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.series.search.get("price index", limit=5)  # doctest: +SKIP
                         id realtime_start realtime_end                                              title ...
             0     CPIAUCSL     2023-03-16   2023-03-16  Consumer Price Index for All Urban Consumers: ... ...
             1     CPIAUCNS     2023-03-16   2023-03-16  Consumer Price Index for All Urban Consumers: ... ...
             2  CUUS0000SA0     2023-03-16   2023-03-16  Consumer Price Index for All Urban Consumers: ... ...
             3   CSUSHPINSA     2023-03-16   2023-03-16    S&P/Case-Shiller U.S. National Home Price Index ...
             4    CSUSHPISA     2023-03-16   2023-03-16    S&P/Case-Shiller U.S. National Home Price Index ...
 
@@ -603,18 +727,18 @@
             exclude_tag_names=exclude_tag_names,
             api_key=api_key,
         ).json()
         data = data["seriess"]
         return pd.DataFrame(data)
 
 
-class Tags(_api.API):
+class SeriesTags(_api.API):
     """Get FRED tags for an economic data series.
 
-    The class variable :data:`finagg.fred.api.series.tags` is an
+    The class variable :attr:`finagg.fred.api.Series.tags` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/series/tags"
 
@@ -656,15 +780,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data on FRED tags for series.
 
         Examples:
-            >>> finagg.fred.api.series.tags.get("CPIAUCNS").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.series.tags.get("CPIAUCNS").head(5)  # doctest: +SKIP
                                             name group_id                     notes ...
             0                                nsa     seas   Not Seasonally Adjusted ...
             1                                usa      geo  United States of America ...
             2  public domain: citation requested       cc                      None ...
             3                             nation     geot                           ...
             4                            monthly     freq                           ...
 
@@ -678,18 +802,18 @@
             sort_order=sort_order,
             api_key=api_key,
         ).json()
         data = data["tags"]
         return pd.DataFrame(data)
 
 
-class Updates(_api.API):
+class SeriesUpdates(_api.API):
     """Get data on when economic data series where updated on the FRED server.
 
-    The class variable :data:`finagg.fred.api.series.updates` is an
+    The class variable :attr:`finagg.fred.api.Series.updates` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/series/updates"
 
@@ -753,18 +877,18 @@
             end_time=end_time,
             api_key=api_key,
         ).json()
         data = data["seriess"]
         return pd.DataFrame(data)
 
 
-class VintageDates(_api.API):
+class SeriesVintageDates(_api.API):
     """Get FRED series revision dates.
 
-    The class variable :data:`finagg.fred.api.series.vintage_dates` is an
+    The class variable :attr:`finagg.fred.api.Series.vintage_dates` is an
     instance of this API implementation and is the most popular interface for
     calling this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/series/vintage_dates"
 
@@ -824,65 +948,69 @@
     """Get an economic data series.
 
     The class variable :data:`finagg.fred.api.series` is an instance of this
     API implementation and is the most popular interface for calling this API.
 
     """
 
-    categories = Categories()
+    categories = SeriesCategories()
     """"series/categories" FRED API. Get the categories for an economic
-    data series. The most popular way for accessing the :class:`Categories`
-    API.
+    data series. The most popular way for accessing the
+    :class:`finagg.fred.api.SeriesCategories` API.
 
     :meta hide-value:
     """
 
-    observations = Observations()
+    observations = SeriesObservations()
     """"series/observations" FRED API. Get the observations or
     data values for an economic data series. The most popular way
-    for accessing the :class:`Observations` API.
+    for accessing the :class:`finagg.fred.api.SeriesObservations` API.
 
     :meta hide-value:
     """
 
-    release = Release()
+    release = SeriesRelease()
     """"series/release" FRED API. Get the release for an economic data series.
-    The most popular way for accessing the :class:`Release` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.SeriesRelease` API.
 
     :meta hide-value:
     """
 
-    search = Search()
+    search = SeriesSearch()
     """"series/search" FRED API. Get economic data series that match search
-    text. The most popular way for accessing the :class:`Search` API.
+    text. The most popular way for accessing the
+    :class:`finagg.fred.api.SeriesSearch` API.
 
     :meta hide-value:
     """
 
-    tags = Tags()
+    tags = SeriesTags()
     """"series/tags" FRED API. Get FRED tags for a series.
-    The most popular way for accessing the :class:`Tags` API.
+    The most popular way for accessing the :class:`finagg.fred.api.SeriesTags`
+    API.
 
     :meta hide-value:
     """
 
-    updates = Updates()
+    updates = SeriesUpdates()
     """"series/updates" FRED API. Get economic data series sorted by
     when observations were updated on the FRED server. The most popular
-    way for accessing the :class:`Updates` API.
+    way for accessing the :class:`finagg.fred.api.SeriesUpdates` API.
 
     :meta hide-value:
     """
 
     url = "https://api.stlouisfed.org/fred/series"
 
-    vintage_dates = VintageDates()
+    vintage_dates = SeriesVintageDates()
     """"series/vintage_dates" FRED API. Get the dates in history when a
     a series' data values were revised or new data values were released.
-    The most popular way for accessing the :class:`VintageDates` API.
+    The most popular way for accessing the
+    :class:`finagg.fred.api.SeriesVintageDates` API.
 
     :meta hide-value:
     """
 
     @classmethod
     def get(
         cls,
@@ -908,15 +1036,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing info on an economic data series.
 
         Examples:
-            >>> finagg.fred.api.series.get("CPIAUCNS", realtime_start=0, realtime_end=-1).head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.series.get("CPIAUCNS", realtime_start=0, realtime_end=-1).head(5)  # doctest: +SKIP
                      id realtime_start realtime_end                                              title ...
             0  CPIAUCNS     1949-03-24   1953-02-26  Consumer Price Index for Urban Wage Earners an... ...
             1  CPIAUCNS     1953-02-27   1962-02-27  Consumer Price Index for Urban Wage Earners an... ...
             2  CPIAUCNS     1962-02-28   1971-02-18  Consumer Price Index for Urban Wage Earners an... ...
             3  CPIAUCNS     1971-02-19   1978-02-26  Consumer Price Index for Urban Wage Earners an... ...
             4  CPIAUCNS     1978-02-27   1988-02-25  Consumer Price Index for All Urban Consumers: ... ...
 
@@ -928,12 +1056,31 @@
             realtime_end=realtime_end,
             api_key=api_key,
         ).json()
         data = data["seriess"]
         return pd.DataFrame(data)
 
 
-series = Series()
-"""The most popular way for accessing :class:`Series`.
+popular_series = [
+    "CIVPART",  # Labor force participation rate
+    "CPIAUCNS",  # Consumer price index
+    "CSUSHPINSA",  # S&P/Case-Shiller national home price index
+    "DJIA",  # Dow Jones Industrial Average index
+    "FEDFUNDS",  # Federal funds interest rate
+    "GDP",  # Gross domestic product
+    "GDPC1",  # Real gross domestic product
+    "GS10",  # 10-Year treasury yield
+    "M2",  # Money stock measures (i.e., savings and related balances)
+    "MICH",  # University of Michigan: inflation expectation
+    "NASDAQ100",  # Nasdaq 100 index
+    "NASDAQCOM",  # Nasdaq Composite index
+    "PSAVERT",  # Personal savings rate
+    "SP500",  # S&P 500 index
+    "UMCSENT",  # University of Michigan: consumer sentiment
+    "UNRATE",  # Unemployment rate
+    "WALCL",  # US assets, total assets (less eliminations from consolidation)
+]
+"""Economic data series that are relatively popular for economic analysis.
+Includes things like gross domestic product, unemployment rate, etc..
 
 :meta hide-value:
 """
```

### Comparing `finagg-0.0.0b1/src/finagg/fred/api/source_.py` & `finagg-0.1.0/src/finagg/fred/api/_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 """
 
 import pandas as pd
 
 from . import _api
 
 
-class Releases(_api.API):
+class SourceReleases(_api.API):
     """Get all of a source's releases of economic data.
 
-    The class variable :data:`finagg.fred.api.source.releases` is an instance
+    The class variable :attr:`finagg.fred.api.Source.releases` is an instance
     of this API implementation and is the most popular interface for calling
     this API.
 
     """
 
     url = "https://api.stlouisfed.org/fred/source/releases"
 
@@ -64,15 +64,15 @@
                 environment variable.
 
         Returns:
             A dataframe containing data on all releases for a
             source of economic data.
 
         Examples:
-            >>> finagg.fred.api.source.releases.get(1, limit=5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.source.releases.get(1, limit=5)  # doctest: +SKIP
                id realtime_start realtime_end                                               name  press_release                                         link
             0  13     2023-03-15   2023-03-15  G.17 Industrial Production and Capacity Utiliz...           True  http://www.federalreserve.gov/releases/g17/
             1  14     2023-03-15   2023-03-15                               G.19 Consumer Credit           True  http://www.federalreserve.gov/releases/g19/
             2  15     2023-03-15   2023-03-15                         G.5 Foreign Exchange Rates           True   http://www.federalreserve.gov/releases/g5/
             3  17     2023-03-15   2023-03-15                        H.10 Foreign Exchange Rates           True  http://www.federalreserve.gov/releases/h10/
             4  18     2023-03-15   2023-03-15                       H.15 Selected Interest Rates           True  http://www.federalreserve.gov/releases/h15/
 
@@ -97,17 +97,18 @@
 
     The module variable :data:`finagg.fred.api.source` is an instance
     of this API implementation and is the most popular interface for calling
     this API.
 
     """
 
-    releases = Releases()
+    releases = SourceReleases()
     """"source/releases" FRED API. Get the releases for a source of economic
-    data. The most popular way for accessing the :class:`Releases` API.
+    data. The most popular way for accessing the
+    :class:`finagg.fred.api.SourceReleases` API.
 
     :meta hide-value:
     """
 
     url = "https://api.stlouisfed.org/fred/source"
 
     @classmethod
@@ -135,15 +136,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing high-level info on an economic source.
 
         Examples:
-            >>> finagg.fred.api.source.get(1)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.source.get(1)  # doctest: +SKIP
                id realtime_start realtime_end                                               name                            link
             0   1     2023-03-15   2023-03-15  Board of Governors of the Federal Reserve Syst...  http://www.federalreserve.gov/
 
         """
         data = _api.get(
             cls.url,
             source_id=source_id,
@@ -204,15 +205,15 @@
                 environment variable.
 
         Returns:
             A dataframe containing data on all sources of economic
             data.
 
         Examples:
-            >>> finagg.fred.api.sources.get(limit=5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.sources.get(limit=5)  # doctest: +SKIP
                id realtime_start realtime_end                                               name                              link
             0   1     2023-03-15   2023-03-15  Board of Governors of the Federal Reserve Syst...    http://www.federalreserve.gov/
             1   3     2023-03-15   2023-03-15               Federal Reserve Bank of Philadelphia  https://www.philadelphiafed.org/
             2   4     2023-03-15   2023-03-15                  Federal Reserve Bank of St. Louis        http://www.stlouisfed.org/
             3   6     2023-03-15   2023-03-15  Federal Financial Institutions Examination Cou...             http://www.ffiec.gov/
             4  11     2023-03-15   2023-03-15                                Dow Jones & Company           http://www.dowjones.com
 
@@ -225,20 +226,7 @@
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
             api_key=api_key,
         ).json()
         data = data["sources"]
         return pd.DataFrame(data)
-
-
-source = Source()
-"""The most popular way for accessing :class:`Source`.
-
-:meta hide-value:
-"""
-
-sources = Sources()
-"""The most popular way for accessing :class:`Sources`.
-
-:meta hide-value:
-"""
```

### Comparing `finagg-0.0.0b1/src/finagg/fred/api/tags_.py` & `finagg-0.1.0/src/finagg/fred/api/_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for related FRED tags.
 
         Examples:
-            >>> finagg.fred.api.related_tags.get(tag_names="bea", limit=5)  # doctest: +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.related_tags.get(tag_names="bea", limit=5)  # doctest: +SKIP
                                             name group_id                     notes                 created  popularity  series_count
             0  public domain: citation requested       cc                      None  2018-12-17 23:33:13-06          99         78680
             1                                usa      geo  United States of America  2012-02-27 10:18:19-06         100         78434
             2                                nsa     seas   Not Seasonally Adjusted  2012-02-27 10:18:19-06          99         67720
             3                             annual     freq                            2012-02-27 10:18:19-06          88         66478
             4                                gdp      gen    Gross Domestic Product  2012-02-27 10:18:19-06          81         60040
 
@@ -168,15 +168,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing series data for related tags.
 
         Examples:
-            >>> finagg.fred.api.tags.series.get(tag_names="bea", limit=5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.tags.series.get(tag_names="bea", limit=5)  # doctest: +SKIP
                             id realtime_start realtime_end                                             title ...
             0  A001RD3A086NBEA     2023-03-15   2023-03-15  Gross national product (implicit price deflator) ...
             1  A001RG3A086NBEA     2023-03-15   2023-03-15   Gross national product (chain-type price index) ...
             2  A001RI1A225NBEA     2023-03-15   2023-03-15   Gross National Product: Implicit Price Deflator ...
             3  A001RI1Q225SBEA     2023-03-15   2023-03-15   Gross National Product: Implicit Price Deflator ...
             4  A001RL1A225NBEA     2023-03-15   2023-03-15                       Real Gross National Product ...
 
@@ -269,15 +269,15 @@
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for all FRED economic data tags.
 
         Examples:
-            >>> finagg.fred.api.tags.get(tag_group_id="src", limit=5)  # doctest: +NORMALIZE_WHITESPACE
+            >>> finagg.fred.api.tags.get(tag_group_id="src", limit=5)  # doctest: +SKIP
                       name group_id                        notes                 created  popularity  series_count
             0       census      src                       Census  2012-02-27 10:18:19-06          79        237692
             1          bls      src   Bureau of Labor Statistics  2012-02-27 10:18:19-06          89        175376
             2  realtor.com      src                               2020-03-24 11:15:04-05          66         90632
             3          bea      src  Bureau of Economic Analysis  2012-02-27 10:18:19-06          78         78842
             4      frb stl      src                St. Louis Fed  2012-02-27 10:18:19-06          68         78442
 
@@ -293,20 +293,7 @@
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
             api_key=api_key,
         ).json()
         data = data["tags"]
         return pd.DataFrame(data)
-
-
-tags = Tags()
-"""The most popular way for accessing :class:`Tags`.
-
-:meta hide-value:
-"""
-
-related_tags = RelatedTags()
-"""The most popular way for accessing :class:`RelatedTags`.
-
-:meta hide-value:
-"""
```

### Comparing `finagg-0.0.0b1/src/finagg/fred/sql.py` & `finagg-0.1.0/src/finagg/fundam/sql.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,81 @@
-"""FRED SQLAlchemy interfaces."""
+"""SQLAlchemy interfaces for fundamental features."""
 
 
 import sqlalchemy as sa
-from sqlalchemy.engine import Engine
 
-from .. import backend
+from .. import sec, yfinance
 
 metadata = sa.MetaData()
+"""The metadata associated with all SQL tables defined in this module.
 
-series = sa.Table(
-    "fred.raw.series",
+:meta hide-value:
+"""
+
+fundam = sa.Table(
+    "fundam.refined.fundam",
     metadata,
-    sa.Column("series_id", sa.String, primary_key=True, doc="Economic series ID."),
-    sa.Column(
-        "realtime_start",
-        sa.String,
-        primary_key=True,
-        doc="Start date for values according to their publication date.",
-    ),
     sa.Column(
-        "realtime_end",
+        "ticker",
         sa.String,
+        sa.ForeignKey(sec.sql.submissions.c.ticker, ondelete="CASCADE"),
+        sa.ForeignKey(yfinance.sql.prices.c.ticker, ondelete="CASCADE"),
         primary_key=True,
-        doc="End date for values according to their publication date.",
+        doc="Unique company ticker.",
     ),
+    sa.Column("date", sa.String, primary_key=True, doc="Filing and stock price dates."),
     sa.Column(
-        "date", sa.String, primary_key=True, doc="Series value publication date."
+        "PriceBookRatio",
+        sa.Float,
+        nullable=False,
+        doc="Market share price over book share price.",
     ),
     sa.Column(
-        "value",
+        "PriceEarningsRatio",
         sa.Float,
         nullable=False,
-        doc="Economic series value for a particular date.",
+        doc="Market share price over earnings per share.",
     ),
 )
+"""SQL table for storing refined data as managed by
+:data:`finagg.fundam.feat.fundam` (an alias for
+:class:`finagg.fundam.feat.Fundamental`).
+
+:meta hide-value:
+"""
 
-economic = sa.Table(
-    "fred.refined.economic",
+normalized_fundam = sa.Table(
+    "fundam.refined.fundam.normalized",
     metadata,
     sa.Column(
-        "date",
+        "ticker",
         sa.String,
+        sa.ForeignKey(fundam.c.ticker, ondelete="CASCADE"),
         primary_key=True,
-        doc="Economic data series release date.",
+        doc="Unique company ticker.",
     ),
-    sa.Column("name", sa.String, primary_key=True, doc="Feature name."),
-    sa.Column("value", sa.Float, nullable=False, doc="Feature value."),
-)
-
-normalized_economic = sa.Table(
-    "fred.refined.economic.normalized",
-    metadata,
+    sa.Column("date", sa.String, primary_key=True, doc="Filing and stock price dates."),
     sa.Column(
-        "date",
-        sa.String,
-        primary_key=True,
-        doc="Economic data series release date.",
+        "NORM(PriceBookRatio)",
+        sa.Float,
+        nullable=False,
+        doc=(
+            "Market share price over book share price normalized against the "
+            "company's industry."
+        ),
+    ),
+    sa.Column(
+        "NORM(PriceEarningsRatio)",
+        sa.Float,
+        nullable=False,
+        doc=(
+            "Market share price over earnings per share normalized against the "
+            "company's industry."
+        ),
     ),
-    sa.Column("name", sa.String, primary_key=True, doc="Feature name."),
-    sa.Column("value", sa.Float, nullable=False, doc="Feature value."),
 )
+"""SQL table for storing refined data as managed by
+:attr:`finagg.fundam.feat.Fundamental.normalized` (an alias for
+:class:`finagg.fundam.feat.NormalizedFundamental`).
 
-
-def get_id_set(lb: int = 1, *, engine: None | Engine = None) -> set[str]:
-    """Get all unique economic series IDs in the raw SQL tables that have at least
-    ``lb`` rows.
-
-    Args:
-        lb: Lower bound number of rows that a series must have for its ID
-            to be included in the set returned by this method.
-        engine: Feature store database engine. Defaults to the engine
-            at :data:`finagg.backend.engine`.
-
-    Examples:
-        >>> "FEDFUNDS" in finagg.fred.sql.get_id_set()
-        True
-
-    """
-    engine = engine or backend.engine
-    with engine.begin() as conn:
-        series_ids = (
-            conn.execute(
-                sa.select(series.c.series_id)
-                .group_by(series.c.series_id)
-                .having(sa.func.count(series.c.date) >= lb)
-            )
-            .scalars()
-            .all()
-        )
-    return set(series_ids)
+:meta hide-value:
+"""
```

### Comparing `finagg-0.0.0b1/src/finagg/fundam/_cli.py` & `finagg-0.1.0/src/finagg/fundam/_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     help=(
         "Drop and recreate tables, and install recommended tables into the "
         "SQL database."
     ),
 )
 @click.option(
     "--refined",
-    "-ref",
     type=click.Choice(["fundam", "fundam.normalized"]),
     multiple=True,
     help=(
         "Refined tables to install. This requires Yahoo! Finance and "
         "SEC refined tables to be installed beforehand."
     ),
 )
@@ -39,18 +38,40 @@
     "--all",
     "-a",
     "all_",
     is_flag=True,
     default=False,
     help="Whether to install all defined tables (including all refined tables).",
 )
+@click.option(
+    "--recreate-tables",
+    "-r",
+    is_flag=True,
+    default=False,
+    help=(
+        "Whether to reset the tables associated with the install options by "
+        "dropping and recreating them."
+    ),
+)
+@click.option(
+    "--verbose",
+    "-v",
+    is_flag=True,
+    default=False,
+    help="Sets the log level to DEBUG to show installation errors for each series.",
+)
 def install(
     refined: list[Literal["fundam", "fundam.normalized"]] = [],
     all_: bool = False,
+    recreate_tables: bool = False,
+    verbose: bool = False,
 ) -> int:
+    if verbose:
+        logging.getLogger(__package__).setLevel(logging.DEBUG)
+
     if "SEC_API_USER_AGENT" not in os.environ:
         logger.warning(
             "No SEC API user agent found in the environment. "
             "Skipping finagg.fundam installation."
         )
         return 0
 
@@ -58,20 +79,27 @@
     all_refined = set()
     if all_:
         all_refined = {"fundam", "fundam.normalized"}
     elif refined:
         all_refined = set(refined)
 
     if "fundam" in all_refined:
-        total_rows += _feat.fundam.install()
+        total_rows += _feat.fundam.install(recreate_tables=recreate_tables)
 
     if "fundam.normalized" in all_refined:
-        total_rows += _feat.fundam.normalized.install()
+        total_rows += _feat.fundam.normalized.install(recreate_tables=recreate_tables)
 
     if all_ or all_refined:
-        logger.info(f"{total_rows} total rows inserted for {__package__}")
+        if total_rows:
+            logger.info(f"{total_rows} total rows inserted for {__package__}")
+        else:
+            logger.warning(
+                f"No rows were inserted for {__package__}. This could be an error if"
+                " installations were not skipped. Set the verbose flag with the"
+                " `--verbose/-v` option to enable debug logging."
+            )
     else:
         logger.info(
             f"Skipping {__package__} installation because no installation "
             "options are provided"
         )
     return total_rows
```

### Comparing `finagg-0.0.0b1/src/finagg/fundam/feat.py` & `finagg-0.1.0/src/finagg/fundam/feat.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 import numpy as np
 import pandas as pd
 import sqlalchemy as sa
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import NoResultFound
 from tqdm import tqdm
 
-from .. import backend, feat, sec, utils, yfinance
+from .. import backend, sec, utils, yfinance
 from . import sql
 
 logging.basicConfig(
     format="%(asctime)s | %(levelname)s | %(message)s", level=logging.INFO
 )
 logger = logging.getLogger(__name__)
 
 
-class RefinedIndustryFundamental:
+class IndustryFundamental:
     """Methods for gathering industry-averaged fundamental data.
 
-    The class variable :data:`finagg.fundam.feat.fundam.industry` is an
+    The class variable :attr:`finagg.fundam.feat.Fundamental.industry` is an
     instance of this feature set implementation and is the most popular
     interface for calling feature methods.
 
     Examples:
         You can aggregate this feature set using a ticker or an industry code
         directly.
 
@@ -84,35 +84,39 @@
         Raises:
             `ValueError`: If neither a ``ticker`` nor ``code`` are provided.
             `NoResultFound`: If there are no rows for ``ticker`` or ``code``
                 in the refined SQL table.
 
         Examples:
             >>> df = finagg.fundam.feat.fundam.industry.from_refined(ticker="AAPL").head(5)
-            >>> df["avg"]  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-            name        AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            date                                                                    ...
-            2009-10-23                       0.0           0.3305              2.48 ...
-            2009-10-26                       0.0           0.3305              2.48 ...
-            2009-10-27                       0.0           0.3305              2.48 ...
-            2009-10-28                       0.0           0.3305              2.48 ...
-            2009-10-29                       0.0           0.3305              2.48 ...
-            >>> df["std"]  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-            name        AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            date                                                                    ...
-            2009-10-23                       0.0              0.0               0.0 ...
-            2009-10-26                       0.0              0.0               0.0 ...
-            2009-10-27                       0.0              0.0               0.0 ...
-            2009-10-28                       0.0              0.0               0.0 ...
-            2009-10-29                       0.0              0.0               0.0 ...
+            >>> df["mean"]  # doctest: +SKIP
+            name        PriceBookRatio  PriceEarningsRatio
+            date
+            2010-01-29        1.213018           17.020706
+            2010-02-01        1.166246           16.364503
+            2010-02-02        1.213047           17.021558
+            2010-02-03        1.222630           17.156233
+            2010-02-04        1.213401           17.026466
+            >>> df["std"]  # doctest: +SKIP
+            name        PriceBookRatio  PriceEarningsRatio
+            date
+            2010-01-29        1.469641           20.667755
+            2010-02-01        1.414144           19.887156
+            2010-02-02        1.476001           20.756459
+            2010-02-03        1.490459           20.959443
+            2010-02-04        1.475500           20.749523
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sec.sql.submissions.name):
+            sec.sql.submissions.create(engine)
+        if not sa.inspect(engine).has_table(sql.fundam.name):
+            sql.fundam.create(engine)
         with engine.begin() as conn:
             if ticker:
                 (sic,) = conn.execute(
                     sa.select(sec.sql.submissions.c.sic).where(
                         sec.sql.submissions.c.ticker == ticker
                     )
                 ).one()
@@ -120,59 +124,51 @@
             elif code:
                 code = str(code)[:level]
             else:
                 raise ValueError("Must provide a `ticker` or `code`.")
 
             df = pd.DataFrame(
                 conn.execute(
-                    sa.select(
-                        sql.fundam.c.date,
-                        sql.fundam.c.name,
-                        sa.func.avg(sql.fundam.c.value).label("avg"),
-                        sa.func.std(sql.fundam.c.value).label("std"),
-                    )
+                    sql.fundam.select()
                     .join(
                         sec.sql.submissions,
                         (sec.sql.submissions.c.ticker == sql.fundam.c.ticker)
                         & (sec.sql.submissions.c.sic.startswith(code)),
                     )
-                    .group_by(
-                        sql.fundam.c.date,
-                        sql.fundam.c.name,
-                    )
-                    .where(
-                        sql.fundam.c.date >= start,
-                        sql.fundam.c.date <= end,
-                    )
+                    .where(sql.fundam.c.date >= start, sql.fundam.c.date <= end)
                 )
             )
         if not len(df.index):
             raise NoResultFound(f"No industry fundamental rows found for {code}.")
-        df = df.pivot(
-            index="date",
-            columns="name",
-            values=["avg", "std"],
-        ).sort_index()
-        return df
+        df = df.drop(columns=["ticker"])
+        df = df.melt(["date"], var_name="name", value_name="value").set_index("date")
+        return (
+            df.groupby(["date", "name"])  # type: ignore[return-value]
+            .agg([np.mean, np.std])
+            .reset_index()
+            .pivot(index=["date"], columns="name")["value"]
+            .sort_index()
+            .dropna()
+        )
 
 
-class RefinedNormalizedFundamental:
+class NormalizedFundamental:
     """Fundamental features from quarterly and daily data, normalized
     according to industry averages and standard deviations.
 
-    The class variable :data:`finagg.fundam.feat.fundam.normalized` is an
+    The class variable :attr:`finagg.fundam.feat.Fundamental.normalized` is an
     instance of this feature set implementation and is the most popular
     interface for calling feature methods.
 
     Examples:
         It doesn't matter which data source you use to gather features.
         They all return equivalent dataframes.
 
         >>> df1 = finagg.fundam.feat.fundam.normalized.from_other_refined("AAPL").head(5)
-        >>> df2 = finagg.fundam.feat.fundam.from_refined("AAPL").head(5)
+        >>> df2 = finagg.fundam.feat.fundam.normalized.from_refined("AAPL").head(5)
         >>> pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
 
     """
 
     @classmethod
     def from_other_refined(
         cls,
@@ -204,46 +200,51 @@
                 at :data:`finagg.backend.engine`.
 
         Returns:
             Relative fundamental data dataframe with each feature as a
             separate column. Sorted by filing date.
 
         Examples:
-            >>> finagg.fundam.feat.fundam.normalized.from_other_refined("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                        AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            date                                                                    ...
-            2010-01-25                   -1.4142          -0.6309           -0.6506 ...
-            2010-01-26                    0.0000          -0.6309           -0.6506 ...
-            2010-01-27                    0.0000          -0.6309           -0.6506 ...
-            2010-01-28                    0.5774          -0.5223            0.2046 ...
-            2010-01-29                    0.0000          -0.5940            0.4365 ...
+            >>> finagg.fundam.feat.fundam.normalized.from_other_refined("AAPL").head(5)  # doctest: +SKIP
+                        NORM(PriceBookRatio)  NORM(PriceEarningsRatio)
+            date
+            2010-01-25             -0.706266                 -0.706279
+            2010-01-26             -0.698805                 -0.698935
+            2010-01-27             -0.700699                 -0.700799
+            2010-01-28             -0.701446                 -0.701534
+            2010-01-29             -0.704558                 -0.704598
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         engine = engine or backend.engine
-        company_df = RefinedFundamental.from_refined(
+        company_df = Fundamental.from_refined(
             ticker, start=start, end=end, engine=engine
-        )
-        industry_df = RefinedIndustryFundamental.from_refined(
+        ).reset_index(["date"])
+        date = company_df["date"]
+        industry_df = IndustryFundamental.from_refined(
             ticker=ticker, level=level, start=start, end=end, engine=engine
+        ).reset_index(["date"])
+        company_df = (company_df - industry_df["mean"]) / industry_df["std"]
+        company_df["date"] = date
+        company_df = (
+            company_df.reset_index()
+            .set_index("date")
+            .rename(lambda x: f"NORM({x})", axis=1)
         )
-        company_df = (company_df - industry_df["avg"]) / industry_df["std"]
-        company_df = company_df.sort_index()
-        pct_change_columns = RefinedFundamental.pct_change_target_columns()
-        company_df[pct_change_columns] = company_df[pct_change_columns].fillna(
-            value=0.0
-        )
-        return (
+        company_df = (
             company_df.fillna(method="ffill")
-            .dropna()
             .reset_index()
+            .dropna()
             .drop_duplicates("date")
             .set_index("date")
+            .sort_index()
         )
+        company_df = utils.resolve_col_order(sql.normalized_fundam, company_df)
+        return company_df
 
     @classmethod
     def from_refined(
         cls,
         ticker: str,
         /,
         *,
@@ -271,72 +272,73 @@
             separate column. Sorted by date.
 
         Raises:
             `NoResultFound`: If there are no rows for ``ticker`` in the
                 refined SQL table.
 
         Examples:
-            >>> finagg.fundam.feat.fundam.normalized.from_refined("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                        AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            date                                                                    ...
-            2010-01-25                   -1.4142          -0.6309           -0.6506 ...
-            2010-01-26                    0.0000          -0.6309           -0.6506 ...
-            2010-01-27                    0.0000          -0.6309           -0.6506 ...
-            2010-01-28                    0.5774          -0.5223            0.2046 ...
-            2010-01-29                    0.0000          -0.5940            0.4365 ...
+            >>> finagg.fundam.feat.fundam.normalized.from_refined("AAPL").head(5)  # doctest: +SKIP
+                        NORM(PriceBookRatio)  NORM(PriceEarningsRatio)
+            date
+            2010-01-25             -0.706266                 -0.706279
+            2010-01-26             -0.698805                 -0.698935
+            2010-01-27             -0.700699                 -0.700799
+            2010-01-28             -0.701446                 -0.701534
+            2010-01-29             -0.704558                 -0.704598
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.normalized_fundam.name):
+            sql.normalized_fundam.create(engine)
         with engine.begin() as conn:
             df = pd.DataFrame(
                 conn.execute(
                     sql.normalized_fundam.select().where(
                         sql.normalized_fundam.c.ticker == ticker,
                         sql.normalized_fundam.c.date >= start,
                         sql.normalized_fundam.c.date <= end,
                     )
                 )
             )
         if not len(df.index):
             raise NoResultFound(
                 f"No industry-normalized fundamental rows found for {ticker}."
             )
-        df = df.pivot(index="date", columns="name", values="value").sort_index()
-        df.columns = df.columns.rename(None)
-        df = df[RefinedFundamental.columns]
+        df = df.drop(columns=["ticker"]).set_index("date").sort_index()
         return df
 
     @classmethod
     def get_candidate_ticker_set(
         cls, lb: int = 1, *, engine: None | Engine = None
     ) -> set[str]:
         """Get all unique tickers in the fundamental SQL table that MAY BE
         ELIGIBLE to be in the feature's SQL table.
 
-        This is just an alias for :meth:`finagg.fundam.feat.fundam.get_ticker_set`.
+        This is just an alias for
+        :meth:`finagg.fundam.feat.Fundamental.get_ticker_set`.
 
         Args:
             lb: Minimum number of rows required to include a ticker in the
                 returned set.
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
 
         Returns:
             All unique tickers that may be valid for creating
             industry-normalized fundamental features that also have at least
             ``lb`` rows for each tag used for constructing the features.
 
         Examples:
-            >>> "AAPL" in finagg.fundam.feat.fundam.normalized.get_candidate_ticker_set()
+            >>> "AAPL" in finagg.fundam.feat.fundam.normalized.get_candidate_ticker_set()  # doctest: +SKIP
             True
 
         """
-        return RefinedFundamental.get_ticker_set(lb=lb, engine=engine)
+        return Fundamental.get_ticker_set(lb=lb, engine=engine)
 
     @classmethod
     def get_ticker_set(cls, lb: int = 1, *, engine: None | Engine = None) -> set[str]:
         """Get all unique tickers in the feature's SQL table.
 
         Args:
             lb: Minimum number of rows required to include a ticker in the
@@ -345,30 +347,27 @@
                 at :data:`finagg.backend.engine`.
 
         Returns:
             All unique tickers that contain all the columns for creating
             fundamental features that also have at least ``lb`` rows.
 
         Examples:
-            >>> "AAPL" in finagg.fundam.feat.fundam.normalized.get_ticker_set()
+            >>> "AAPL" in finagg.fundam.feat.fundam.normalized.get_ticker_set()  # doctest: +SKIP
             True
 
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.normalized_fundam.name):
+            sql.normalized_fundam.create(engine)
         with engine.begin() as conn:
             tickers = (
                 conn.execute(
                     sa.select(sql.normalized_fundam.c.ticker)
                     .group_by(sql.normalized_fundam.c.ticker)
-                    .having(
-                        *[
-                            sa.func.count(sql.normalized_fundam.c.name == col) >= lb
-                            for col in RefinedFundamental.columns
-                        ]
-                    )
+                    .having(sa.func.count(sql.normalized_fundam.c.date) >= lb)
                 )
                 .scalars()
                 .all()
             )
         return set(tickers)
 
     @classmethod
@@ -402,19 +401,21 @@
             `ValueError`: If the integer date is positive.
 
         Examples:
             >>> ts = finagg.fundam.feat.fundam.normalized.get_tickers_sorted_by(
             ...         "PriceEarningsRatio",
             ...         date="2019-01-04"
             ... )
-            >>> "AMD" == ts[0]
+            >>> "AMD" == ts[0]  # doctest: +SKIP
             True
 
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.normalized_fundam.name):
+            sql.normalized_fundam.create(engine)
         with engine.begin() as conn:
             if isinstance(date, int):
                 if date > 0:
                     raise ValueError("Date should be non-positive")
 
                 (max_date,) = conn.execute(
                     sa.select(sa.func.max(sql.normalized_fundam.c.date))
@@ -426,47 +427,67 @@
                         datetime.fromisoformat(str(max_date)) - timedelta(days=date)
                     ).strftime("%Y-%m-%d")
 
             tickers = (
                 conn.execute(
                     sa.select(sql.normalized_fundam.c.ticker)
                     .where(
-                        sql.normalized_fundam.c.name == column,
                         sql.normalized_fundam.c.date == date,
                     )
-                    .order_by(sql.normalized_fundam.c.value)
+                    .order_by(sql.normalized_fundam.c[column])
                 )
                 .scalars()
                 .all()
             )
         if not ascending:
             return list(reversed(tickers))
         return list(tickers)
 
     @classmethod
     def install(
-        cls, tickers: None | set[str] = None, *, engine: None | Engine = None
+        cls,
+        tickers: None | set[str] = None,
+        *,
+        engine: None | Engine = None,
+        recreate_tables: bool = False,
     ) -> int:
-        """Drop the feature's table, create a new one, and insert data
-        transformed from another raw SQL table.
+        """Install data associated with ``tickers`` by pulling data from the
+        refined SQL tables, transforming them into normalized features, and
+        then writing to the refined normalized fundamental SQL table.
+
+        Tables associated with this method are created if they don't already
+        exist.
 
         Args:
             tickers: Set of tickers to install features for. Defaults to all
-                the tickers from :meth:`finagg.fundam.feat.fundam.get_ticker_set`.
+                the tickers from :meth:`finagg.fundam.feat.Fundamental.get_ticker_set`.
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
+            recreate_tables: Whether to drop and recreate tables, wiping all
+                previously installed data.
 
         Returns:
             Number of rows written to the feature's SQL table.
 
         """
         engine = engine or backend.engine
         tickers = tickers or cls.get_candidate_ticker_set(engine=engine)
-        sql.normalized_fundam.drop(engine, checkfirst=True)
-        sql.normalized_fundam.create(engine)
+        if not tickers:
+            logger.info(
+                "Skipping finagg.fundam.feat.fundam.normalized installation because no"
+                " tickers were provided or no tickers were found with prerequisite data"
+                " (i.e., finagg.fundam.feat.fundam data)"
+            )
+            return 0
+
+        if recreate_tables or not sa.inspect(engine).has_table(
+            sql.normalized_fundam.name
+        ):
+            sql.normalized_fundam.drop(engine, checkfirst=True)
+            sql.normalized_fundam.create(engine)
 
         total_rows = 0
         for ticker in tqdm(
             tickers,
             desc="Installing refined industry-normalized fundamental data",
             position=0,
             leave=True,
@@ -507,27 +528,24 @@
 
         Raises:
             `ValueError`: If the given dataframe's columns do not match this
                 feature's columns.
 
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.normalized_fundam.name):
+            sql.normalized_fundam.create(engine)
         df = df.reset_index("date")
-        if set(df.columns) < set(RefinedFundamental.columns):
-            raise ValueError(
-                f"Dataframe must have columns {RefinedFundamental.columns} but got {df.columns}"
-            )
-        df = df.melt("date", var_name="name", value_name="value")
         df["ticker"] = ticker
         with engine.begin() as conn:
             conn.execute(sql.normalized_fundam.insert(), df.to_dict(orient="records"))  # type: ignore[arg-type]
         return len(df.index)
 
 
-class RefinedFundamental(feat.Features):
+class Fundamental:
     """Method for gathering fundamental data on a stock using several sources.
 
     The module variable :data:`finagg.fundam.feat.fundam` is an instance of
     this feature set implementation and is the most popular interface for
     calling feature methods.
 
     Examples:
@@ -538,84 +556,44 @@
         >>> df2 = finagg.fundam.feat.fundam.from_raw("AAPL").head(5)
         >>> df3 = finagg.fundam.feat.fundam.from_refined("AAPL").head(5)
         >>> pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
         >>> pd.testing.assert_frame_equal(df1, df3, rtol=1e-4)
 
     """
 
-    #: Columns within this feature set. Dataframes returned by this class's
-    #: methods will always contain these columns.
-    columns = (
-        yfinance.feat.daily.columns
-        + sec.feat.quarterly.columns
-        + ["PriceEarningsRatio"]
-    )
-
-    industry = RefinedIndustryFundamental()
+    industry = IndustryFundamental()
     """Fundamental features aggregated for an entire industry.
-    The most popular way for accessing the :class:`RefinedIndustryFundamental`
+    The most popular way for accessing the :class:`IndustryFundamental`
     feature set.
 
     :meta hide-value:
     """
 
-    normalized = RefinedNormalizedFundamental()
+    normalized = NormalizedFundamental()
     """A company's fundamental features normalized by its industry.
-    The most popular way for accessing the :class:`RefinedNormalizedFundamental`
+    The most popular way for accessing the :class:`NormalizedFundamental`
     feature set.
 
     :meta hide-value:
     """
 
     @classmethod
     def _normalize(
         cls,
         quarterly: pd.DataFrame,
-        daily: pd.DataFrame,
+        prices: pd.DataFrame,
         /,
     ) -> pd.DataFrame:
         """Normalize the feature columns."""
-        quarterly = quarterly.reset_index()
-        quarterly_abs = quarterly.groupby(["filed"], as_index=False)[
-            [
-                col
-                for col in sec.feat.RefinedQuarterly.columns
-                if not col.endswith("pct_change")
-            ]
-        ].last()
-        quarterly_pct_change_cols = (
-            sec.feat.RefinedQuarterly.pct_change_target_columns()
-        )
-        quarterly[quarterly_pct_change_cols] += 1
-        quarterly_pct_change = quarterly.groupby(["filed"], as_index=False).agg(
-            {col: np.prod for col in quarterly_pct_change_cols}
-        )
-        quarterly = pd.merge(
-            quarterly_abs,
-            quarterly_pct_change,
-            how="inner",
-            left_on="filed",
-            right_on="filed",
-        )
-        quarterly[quarterly_pct_change_cols] -= 1
-        quarterly = quarterly.set_index("filed")
-        df = pd.merge(
-            quarterly, daily, how="outer", left_index=True, right_index=True
-        ).sort_index()
-        pct_change_cols = cls.pct_change_target_columns()
-        df[pct_change_cols] = df[pct_change_cols].fillna(value=0)
+        df = pd.merge(quarterly, prices, how="outer", left_index=True, right_index=True)
         df = df.replace([-np.inf, np.inf], np.nan).fillna(method="ffill")
-        df["PriceEarningsRatio"] = df["price"] / df["EarningsPerShare"]
-        df["PriceEarningsRatio"] = (
-            df["PriceEarningsRatio"]
-            .replace([-np.inf, np.inf], np.nan)
-            .fillna(method="ffill")
-        )
+        df["PriceBookRatio"] = df["open"] / df["BookRatio"]
+        df["PriceEarningsRatio"] = df["open"] / df["EarningsPerShareBasic"]
         df.index.names = ["date"]
-        df = df[cls.columns]
+        df = utils.resolve_col_order(sql.fundam, df)
         return df.dropna()
 
     @classmethod
     def from_api(
         cls,
         ticker: str,
         /,
@@ -633,88 +611,38 @@
                 last recorded date.
 
         Returns:
             Combined quarterly and daily feature dataframe.
             Sorted by date.
 
         Examples:
-            >>> finagg.fundam.feat.fundam.from_api("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                         price  open_pct_change ... PriceEarningsRatio
-            date                                ...
-            2010-01-25  6.1727          -0.0207 ...             2.4302
-            2010-01-26  6.2600           0.0170 ...             2.4646
-            2010-01-27  6.3189           0.0044 ...             2.4878
-            2010-01-28  6.0578          -0.0093 ...             2.3850
-            2010-01-29  5.8381          -0.0188 ...             2.2984
+            >>> finagg.fundam.feat.fundam.from_api("AAPL").head(5)  # doctest: +SKIP
+                        PriceBookRatio  PriceEarningsRatio
+            date
+            2010-01-25        0.175061            2.423509
+            2010-01-26        0.178035            2.464677
+            2010-01-27        0.178813            2.475447
+            2010-01-28        0.177153            2.452471
+            2010-01-29        0.173825            2.406396
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         quarterly = sec.feat.quarterly.from_api(
             ticker,
             start=start,
             end=end,
         ).reset_index(["fy", "fp"], drop=True)
         start = str(quarterly.index[0])
-        daily = yfinance.feat.daily.from_api(ticker, start=start, end=end)
-        return cls._normalize(quarterly, daily)
-
-    @classmethod
-    def from_other_refined(
-        cls,
-        ticker: str,
-        /,
-        *,
-        start: None | str = None,
-        end: None | str = None,
-        engine: None | Engine = None,
-    ) -> pd.DataFrame:
-        """Get features directly from other refined SQL tables.
-
-        Args:
-            ticker: Company ticker.
-            start: The start date of the observation period. Defaults to the
-                first recorded date.
-            end: The end date of the observation period. Defaults to the
-                last recorded date.
-            engine: Feature store database engine. Defaults to the engine
-                at :data:`finagg.backend.engine`.
-
-        Returns:
-            Combined quarterly and daily feature dataframe.
-            Sorted by date.
-
-        Examples:
-            >>> finagg.fundam.feat.fundam.from_other_refined("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                         price  open_pct_change ... PriceEarningsRatio
-            date                                ...
-            2010-01-25  6.1727          -0.0207 ...             2.4302
-            2010-01-26  6.2600           0.0170 ...             2.4646
-            2010-01-27  6.3189           0.0044 ...             2.4878
-            2010-01-28  6.0578          -0.0093 ...             2.3850
-            2010-01-29  5.8381          -0.0188 ...             2.2984
-
-        """
-        start = start or "1776-07-04"
-        end = end or utils.today
-        engine = engine or backend.engine
-        quarterly = sec.feat.quarterly.from_refined(
+        prices = yfinance.api.get(
             ticker,
             start=start,
             end=end,
-            engine=engine,
-        ).reset_index(["fy", "fp"], drop=True)
-        start = str(quarterly.index[0])
-        daily = yfinance.feat.daily.from_refined(
-            ticker,
-            start=start,
-            end=end,
-            engine=engine,
-        )
-        return cls._normalize(quarterly, daily)
+        ).set_index("date")
+        return cls._normalize(quarterly, prices)
 
     @classmethod
     def from_raw(
         cls,
         ticker: str,
         /,
         *,
@@ -734,41 +662,41 @@
                 at :data:`finagg.backend.engine`.
 
         Returns:
             Combined quarterly and daily feature dataframe.
             Sorted by date.
 
         Examples:
-            >>> finagg.fundam.feat.fundam.from_raw("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                         price  open_pct_change ... PriceEarningsRatio
-            date                                ...
-            2010-01-25  6.1727          -0.0207 ...             2.4302
-            2010-01-26  6.2600           0.0170 ...             2.4646
-            2010-01-27  6.3189           0.0044 ...             2.4878
-            2010-01-28  6.0578          -0.0093 ...             2.3850
-            2010-01-29  5.8381          -0.0188 ...             2.2984
+            >>> finagg.fundam.feat.fundam.from_raw("AAPL").head(5)  # doctest: +SKIP
+                        PriceBookRatio  PriceEarningsRatio
+            date
+            2010-01-25        0.175061            2.423509
+            2010-01-26        0.178035            2.464677
+            2010-01-27        0.178813            2.475447
+            2010-01-28        0.177153            2.452471
+            2010-01-29        0.173825            2.406396
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         engine = engine or backend.engine
         quarterly = sec.feat.quarterly.from_raw(
             ticker,
             start=start,
             end=end,
             engine=engine,
         ).reset_index(["fy", "fp"], drop=True)
         start = str(quarterly.index[0])
-        daily = yfinance.feat.daily.from_raw(
+        prices = yfinance.feat.prices.from_raw(
             ticker,
             start=start,
             end=end,
             engine=engine,
         )
-        return cls._normalize(quarterly, daily)
+        return cls._normalize(quarterly, prices)
 
     @classmethod
     def from_refined(
         cls,
         ticker: str,
         /,
         *,
@@ -796,42 +724,42 @@
             Sorted by date.
 
         Raises:
             `NoResultFound`: If there are no rows for ``ticker`` in the
                 refined SQL table.
 
         Examples:
-            >>> finagg.fundam.feat.fundam.from_refined("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                         price  open_pct_change ... PriceEarningsRatio
-            date                                ...
-            2010-01-25  6.1727          -0.0207 ...             2.4302
-            2010-01-26  6.2600           0.0170 ...             2.4646
-            2010-01-27  6.3189           0.0044 ...             2.4878
-            2010-01-28  6.0578          -0.0093 ...             2.3850
-            2010-01-29  5.8381          -0.0188 ...             2.2984
+            >>> finagg.fundam.feat.fundam.from_refined("AAPL").head(5)  # doctest: +SKIP
+                        PriceBookRatio  PriceEarningsRatio
+            date
+            2010-01-25        0.175061            2.423509
+            2010-01-26        0.178035            2.464677
+            2010-01-27        0.178813            2.475447
+            2010-01-28        0.177153            2.452471
+            2010-01-29        0.173825            2.406396
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.fundam.name):
+            sql.fundam.create(engine)
         with engine.begin() as conn:
             df = pd.DataFrame(
                 conn.execute(
                     sql.fundam.select().where(
                         sql.fundam.c.ticker == ticker,
                         sql.fundam.c.date >= start,
                         sql.fundam.c.date <= end,
                     )
                 )
             )
         if not len(df.index):
             raise NoResultFound(f"No fundamental rows found for {ticker}.")
-        df = df.pivot(index="date", values="value", columns="name").sort_index()
-        df.columns = df.columns.rename(None)
-        df = df[cls.columns]
+        df = df.drop(columns=["ticker"]).set_index("date").sort_index()
         return df
 
     @classmethod
     def get_candidate_ticker_set(
         cls, lb: int = 1, *, engine: None | Engine = None
     ) -> set[str]:
         """Get all unique tickers in the raw SQL table that MAY BE ELIGIBLE
@@ -845,21 +773,21 @@
 
         Returns:
             All unique tickers that may be valid for both quarterly and daily
             features that also have at least ``lb`` rows used for constructing
             the features.
 
         Examples:
-            >>> "AAPL" in finagg.fundam.feat.fundam.get_candidate_ticker_set()
+            >>> "AAPL" in finagg.fundam.feat.fundam.get_candidate_ticker_set()  # doctest: +SKIP
             True
 
         """
-        return sec.feat.RefinedQuarterly.get_ticker_set(
+        return sec.feat.quarterly.get_ticker_set(
             lb=lb, engine=engine
-        ) & yfinance.feat.RefinedDaily.get_ticker_set(lb=lb, engine=engine)
+        ) & yfinance.feat.daily.get_ticker_set(lb=lb, engine=engine)
 
     @classmethod
     def get_ticker_set(cls, lb: int = 1, *, engine: None | Engine = None) -> set[str]:
         """Get all unique tickers in the feature's SQL table.
 
         Args:
             lb: Minimum number of rows required to include a ticker in the
@@ -868,67 +796,83 @@
                 at :data:`finagg.backend.engine`.
 
         Returns:
             All unique tickers that contain all the columns for creating
             fundamental features that also have at least ``lb`` rows.
 
         Examples:
-            >>> "AAPL" in finagg.fundam.feat.fundam.get_ticker_set()
+            >>> "AAPL" in finagg.fundam.feat.fundam.get_ticker_set()  # doctest: +SKIP
             True
 
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.fundam.name):
+            sql.fundam.create(engine)
         with engine.begin() as conn:
             tickers = (
                 conn.execute(
                     sa.select(sql.fundam.c.ticker)
                     .group_by(sql.fundam.c.ticker)
-                    .having(
-                        *[
-                            sa.func.count(sql.fundam.c.name == col) >= lb
-                            for col in cls.columns
-                        ]
-                    )
+                    .having(sa.func.count(sql.fundam.c.date) >= lb)
                 )
                 .scalars()
                 .all()
             )
         return set(tickers)
 
     @classmethod
     def install(
-        cls, tickers: None | set[str] = None, *, engine: None | Engine = None
+        cls,
+        tickers: None | set[str] = None,
+        *,
+        engine: None | Engine = None,
+        recreate_tables: bool = False,
     ) -> int:
-        """Drop the feature's table, create a new one, and insert data
-        transformed from another raw SQL table.
+        """Install data associated with ``tickers`` by pulling data from other
+        refined SQL tables, transforming them into fundamental features, and
+        then writing to the refined fundamental features SQL table.
+
+        Tables associated with this method are created if they don't already
+        exist.
 
         Args:
             tickers: Set of tickers to install features for. Defaults to all
-                the tickers from :meth:`finagg.sec.feat.quarterly.get_ticker_set`.
+                the tickers from :meth:`finagg.sec.feat.Quarterly.get_ticker_set`.
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
+            recreate_tables: Whether to drop and recreate tables, wiping all
+                previously installed data.
 
         Returns:
             Number of rows written to the feature's SQL table.
 
         """
         engine = engine or backend.engine
         tickers = tickers or cls.get_candidate_ticker_set(engine=engine)
-        sql.fundam.drop(engine, checkfirst=True)
-        sql.fundam.create(engine)
+        if not tickers:
+            logger.info(
+                "Skipping finagg.fundam.feat.fundam installation because no tickers"
+                " were provided or no tickers were found with prerequisite data (i.e.,"
+                " finagg.yfinance.feat.daily and finagg.sec.feat.quarterly data)"
+            )
+            return 0
+
+        if recreate_tables or not sa.inspect(engine).has_table(sql.fundam.name):
+            sql.fundam.drop(engine, checkfirst=True)
+            sql.fundam.create(engine)
 
         total_rows = 0
         for ticker in tqdm(
             tickers,
             desc="Installing refined fundamental data",
             position=0,
             leave=True,
         ):
             try:
-                df = cls.from_other_refined(ticker, engine=engine)
+                df = cls.from_raw(ticker, engine=engine)
                 rowcount = len(df.index)
                 if rowcount:
                     cls.to_refined(ticker, df, engine=engine)
                     total_rows += rowcount
                     logger.debug(f"{rowcount} rows inserted for {ticker}")
                 else:
                     logger.debug(f"Skipping {ticker} due to missing data")
@@ -953,30 +897,23 @@
                 table.
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
 
         Returns:
             Number of rows written to the SQL table.
 
-        Raises:
-            `ValueError`: If the given dataframe's columns do not match this
-                feature's columns.
-
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.fundam.name):
+            sql.fundam.create(engine)
         df = df.reset_index("date")
-        if set(df.columns) < set(cls.columns):
-            raise ValueError(
-                f"Dataframe must have columns {cls.columns} but got {df.columns}"
-            )
-        df = df.melt("date", var_name="name", value_name="value")
         df["ticker"] = ticker
         with engine.begin() as conn:
             conn.execute(sql.fundam.insert(), df.to_dict(orient="records"))  # type: ignore[arg-type]
         return len(df.index)
 
 
-fundam = RefinedFundamental()
-"""The most popular way for accessing :class:`RefinedFundamental`.
+fundam = Fundamental()
+"""The most popular way for accessing :class:`finagg.fundam.feat.Fundamental`.
 
 :meta hide-value:
 """
```

### Comparing `finagg-0.0.0b1/src/finagg/indices/_cli.py` & `finagg-0.1.0/src/finagg/indices/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-0.0.0b1/src/finagg/indices/api.py` & `finagg-0.1.0/src/finagg/indices/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 session = requests_cache.CachedSession(
     str(backend.http_cache_path),
     expire_after=timedelta(weeks=1),
 )
 
 
-class _API(ABC):
+class API(ABC):
     """Abstract indices API."""
 
     #: Request API URL.
     url: ClassVar[str]
 
     @classmethod
     @abstractmethod
@@ -33,15 +33,15 @@
     @classmethod
     def get_ticker_list(cls, *, user_agent: None | str = None) -> list[str]:
         """List the tickers in the index."""
         df = cls.get(user_agent=user_agent)
         return df["ticker"].tolist()
 
 
-class DJIA(_API):
+class DJIA(API):
     """Get data on all companies within the DJIA.
 
     The module variable :data:`finagg.indices.api.djia` is an instance of
     this API implementation and is the most popular interface for querying this
     API.
 
     """
@@ -49,15 +49,15 @@
     url = "https://en.wikipedia.org/wiki/Dow_Jones_Industrial_Average"
 
     @classmethod
     def get(cls, *, user_agent: None | str = None) -> pd.DataFrame:
         """Get a dataframe containing data on the tickers in the DJIA.
 
         Examples:
-            >>> finagg.indices.api.djia.get().head(5)  # doctest: +NORMALIZE_WHITESPACE
+            >>> finagg.indices.api.djia.get().head(5)  # doctest: +SKIP
                         company exchange ticker                industry       added  weight
             0                3M     NYSE    MMM            Conglomerate  1976-08-09  0.0241
             1  American Express     NYSE    AXP      Financial services  1982-08-30  0.0302
             2             Amgen   NASDAQ   AMGN       Biopharmaceutical  2020-08-31  0.0548
             3             Apple   NASDAQ   AAPL  Information technology  2015-03-19  0.0284
             4            Boeing     NYSE     BA   Aerospace and defense  1987-03-12  0.0336
 
@@ -83,15 +83,15 @@
                 "Index weighting": "weight",
             }
         )
         df["weight"] = df["weight"].apply(_percent_to_fraction)
         return df
 
 
-class Nasdaq100(_API):
+class Nasdaq100(API):
     """Get data on all companies within the Nasdaq 100.
 
     The module variable :data:`finagg.indices.api.nasdaq100` is an instance of
     this API implementation and is the most popular interface for querying this
     API.
 
     """
@@ -99,15 +99,15 @@
     url = "https://en.wikipedia.org/wiki/Nasdaq-100"
 
     @classmethod
     def get(cls, *, user_agent: None | str = None) -> pd.DataFrame:
         """Get a dataframe containing data on the tickers in the Nasdaq 100.
 
         Examples:
-            >>> finagg.indices.api.nasdaq100.get().head(5)  # doctest: +NORMALIZE_WHITESPACE
+            >>> finagg.indices.api.nasdaq100.get().head(5)  # doctest: +SKIP
                                    company ticker                industry                           sub_industry
             0          Activision Blizzard   ATVI  Communication Services         Interactive Home Entertainment
             1                   Adobe Inc.   ADBE  Information Technology                   Application Software
             2                          ADP    ADP  Information Technology  Data Processing & Outsourced Services
             3                       Airbnb   ABNB  Consumer Discretionary     Internet & Direct Marketing Retail
             4             Align Technology   ALGN             Health Care                   Health Care Supplies
 
@@ -123,15 +123,15 @@
                 "Ticker": "ticker",
                 "GICS Sector": "industry",
                 "GICS Sub-Industry": "sub_industry",
             }
         )
 
 
-class SP500(_API):
+class SP500(API):
     """Get data on all companies within the S&P 500.
 
     The module variable :data:`finagg.indices.api.sp500` is an instance of
     this API implementation and is the most popular interface for querying this
     API.
 
     """
@@ -139,15 +139,15 @@
     url = "https://en.wikipedia.org/wiki/List_of_S%26P_500_companies"
 
     @classmethod
     def get(cls, *, user_agent: None | str = None) -> pd.DataFrame:
         """Get a dataframe containing data on the tickers in the S&P 500.
 
         Examples:
-            >>> finagg.indices.api.sp500.get().head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
+            >>> finagg.indices.api.sp500.get().head(5)  # doctest: +SKIP
                 ticker               company                industry ...
             0      MMM                    3M             Industrials ...
             1      AOS           A. O. Smith             Industrials ...
             2      ABT                Abbott             Health Care ...
             3     ABBV                AbbVie             Health Care ...
             4      ACN             Accenture  Information Technology ...
 
@@ -206,19 +206,17 @@
 
     Raises:
         `RuntimeError`: If a user agent isn't provided or found in the environment.
 
     """
     user_agent = user_agent or os.environ.get(
         "INDICES_API_USER_AGENT",
-        (
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) "
-            "AppleWebKit/537.36 (KHTML, like Gecko) "
-            "Chrome/39.0.2171.95 Safari/537.36"
-        ),
+        "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) "
+        "AppleWebKit/537.36 (KHTML, like Gecko) "
+        "Chrome/39.0.2171.95 Safari/537.36",
     )
     if not user_agent:
         raise RuntimeError(
             "No indices API user agent declaration found. "
             "Pass your user agent declaration to the API directly, or "
             "set the `INDICES_API_USER_AGENT` environment variable."
         )
@@ -228,15 +226,15 @@
 
 
 @cache
 def get_ticker_set(*, user_agent: None | str = None) -> set[str]:
     """Get the set of tickers from all the popular indices.
 
     Examples:
-        >>> "AAPL" in finagg.indices.api.get_ticker_set()
+        >>> "AAPL" in finagg.indices.api.get_ticker_set()  # doctest: +SKIP
         True
 
     """
     tickers = set()
     tickers.update(djia.get_ticker_list(user_agent=user_agent))
     tickers.update(nasdaq100.get_ticker_list(user_agent=user_agent))
     tickers.update(sp500.get_ticker_list(user_agent=user_agent))
```

### Comparing `finagg-0.0.0b1/src/finagg/portfolio.py` & `finagg-0.1.0/src/finagg/portfolio.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,14 +156,34 @@
             >>> pos = Position(100.0, 1)
             >>> pos.total_dollar_change(50.0)
             -50.0
 
         """
         return float((Decimal(cost) - self._average_cost_basis) * self._quantity)
 
+    def total_log_change(self, cost: float, /) -> float:
+        """Compute the total log change relative to the average
+        cost basis and the current value of the security.
+
+        Args:
+            cost: Current value of one share.
+
+        Returns:
+            Total log change in value. Negative indicates loss
+            in value, positive indicates gain in value.
+
+        Examples:
+            >>> from finagg.portfolio import Position
+            >>> pos = Position(100.0, 1)
+            >>> pos.total_log_change(50.0)
+            -0.051293294387550536
+
+        """
+        return float(Decimal(cost).ln() - self._average_cost_basis.ln())
+
     def total_percent_change(self, cost: float, /) -> float:
         """Compute the total percent change relative to the average
         cost basis and the current value of the security.
 
         Args:
             cost: Current value of one share.
 
@@ -361,14 +381,38 @@
         """
         dollar_value_total = self._cash
         for symbol, cost in costs.items():
             if symbol in self.positions:
                 dollar_value_total += Decimal(cost) * self.positions[symbol]._quantity
         return float(dollar_value_total)
 
+    def total_log_change(self, costs: dict[str, float], /) -> float:
+        """Compute the total log change relative to the total
+        deposits made into the portfolio.
+
+        Args:
+            costs: Mapping of symbol to its current value of one share.
+
+        Returns:
+            Total log change in value. Negative indicates loss
+            in value, positive indicates gain in value.
+
+        Examples:
+            >>> from finagg.portfolio import Portfolio
+            >>> port = Portfolio(1000.0)
+            >>> port.buy("AAPL", 100.0, 1)
+            100.0
+            >>> port.total_log_change({"AAPL": 50.0})
+            -0.051293294387550536
+
+        """
+        return float(
+            Decimal(self.total_dollar_value(costs)).ln() - self._deposits_total.ln()
+        )
+
     def total_percent_change(self, costs: dict[str, float], /) -> float:
         """Compute the total percent change relative to the total
         deposits made into the portfolio.
 
         Args:
             costs: Mapping of symbol to its current value of one share.
```

### Comparing `finagg-0.0.0b1/src/finagg/ratelimit.py` & `finagg-0.1.0/src/finagg/ratelimit.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             response: Request response (possibly cached).
 
         Returns:
             A number indicating the request/response's contribution
             to the rate limit OR a dictionary containing:
 
                 - "limit": a number indicating the request/response's
-                    contribution to the rate limit
+                  contribution to the rate limit
                 - "wait": time to wait before a new request can be made
 
         """
 
 
 class RequestLimit(RateLimit):
     """Limit the number of requests made by the underlying getter."""
```

### Comparing `finagg-0.0.0b1/src/finagg/sec/_cli.py` & `finagg-0.1.0/src/finagg/sec/_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,29 +25,29 @@
     help=(
         "Set the SEC API key, drop and recreate tables, "
         "and install the recommended tables into the SQL database."
     ),
 )
 @click.option(
     "--raw",
-    "-r",
     type=click.Choice(["submissions", "tags"]),
     multiple=True,
     help=(
         "Raw tables to install. `submissions` indicates company metadata "
         "(e.g., company name, industry code, etc.) while `tags` indicates "
         "SEC EDGAR tags (e.g., earnings-per-share, current assets, etc.)."
         "Both `submissions` and `tags` must be specified to enable installing "
         "refined data using the `refined` flag."
     ),
 )
 @click.option(
     "--refined",
-    "-ref",
-    type=click.Choice(["quarterly", "quarterly.normalized"]),
+    type=click.Choice(
+        ["annual", "annual.normalized", "quarterly", "quarterly.normalized"]
+    ),
     multiple=True,
     help=(
         "Refined tables to install. This requires raw SEC data to be "
         "installed beforehand using the `--raw` flag or for the "
         "`--raw` flag to be set when this option is provided."
     ),
 )
@@ -92,26 +92,37 @@
         "popular and large market cap companies, while 'sec' will "
         "attempt to download and install data for nearly all "
         "publicly-traded US companies. Choosing 'indices' will be fast, "
         "while choosing 'sec' will be slow but will include more diverse data."
     ),
 )
 @click.option(
+    "--recreate-tables",
+    "-r",
+    is_flag=True,
+    default=False,
+    help=(
+        "Whether to reset the tables associated with the install options by "
+        "dropping and recreating them."
+    ),
+)
+@click.option(
     "--verbose",
     "-v",
     is_flag=True,
     default=False,
     help="Sets the log level to DEBUG to show installation errors for each ticker.",
 )
 def install(
     raw: list[Literal["submissions", "tags"]] = [],
     refined: list[Literal["quarterly", "quarterly.normalized"]] = [],
     all_: bool = False,
     ticker: list[str] = [],
     ticker_set: None | Literal["indices", "sec"] = None,
+    recreate_tables: bool = False,
     verbose: bool = False,
 ) -> int:
     if verbose:
         logging.getLogger(__package__).setLevel(logging.DEBUG)
 
     if "SEC_API_USER_AGENT" not in os.environ:
         user_agent = input(
@@ -149,39 +160,62 @@
             logger.info(
                 f"Skipping {__package__} installation because no tickers were "
                 "provided (by the `ticker` option or by the `ticker-set` option)"
             )
             return total_rows
 
         if "submissions" in all_raw:
-            total_rows += _feat.submissions.install(all_tickers)
+            total_rows += _feat.submissions.install(
+                all_tickers, recreate_tables=recreate_tables
+            )
 
         if "tags" in all_raw:
-            total_rows += _feat.tags.install(all_tickers)
+            total_rows += _feat.tags.install(
+                all_tickers, recreate_tables=recreate_tables
+            )
 
     all_refined = set()
     if all_:
-        all_refined = {"quarterly", "quarterly.normalized"}
+        all_refined = {
+            "annual",
+            "annual.normalized",
+            "quarterly",
+            "quarterly.normalized",
+        }
     elif refined:
         all_refined = set(refined)
 
+    if "annual" in all_refined:
+        total_rows += _feat.annual.install(
+            tickers=all_tickers, recreate_tables=recreate_tables
+        )
+
+    if "annual.normalized" in all_refined:
+        total_rows += _feat.annual.normalized.install(
+            tickers=all_tickers, recreate_tables=recreate_tables
+        )
+
     if "quarterly" in all_refined:
-        total_rows += _feat.quarterly.install(tickers=all_tickers)
+        total_rows += _feat.quarterly.install(
+            tickers=all_tickers, recreate_tables=recreate_tables
+        )
 
     if "quarterly.normalized" in all_refined:
-        total_rows += _feat.quarterly.normalized.install(tickers=all_tickers)
+        total_rows += _feat.quarterly.normalized.install(
+            tickers=all_tickers, recreate_tables=recreate_tables
+        )
 
     if all_ or all_refined or all_raw:
         if total_rows:
             logger.info(f"{total_rows} total rows inserted for {__package__}")
         else:
             logger.warning(
-                f"No rows were inserted for {__package__}. This is likely an "
-                "error. Set the verbose flag with the `--verbose/-v` option "
-                "to enable debug logging."
+                f"No rows were inserted for {__package__}. This could be an error if"
+                " installations were not skipped. Set the verbose flag with the"
+                " `--verbose/-v` option to enable debug logging."
             )
     else:
         logger.info(
             f"Skipping {__package__} installation because no installation "
             "options were provided"
         )
     return total_rows
```

### Comparing `finagg-0.0.0b1/src/finagg/sec/feat.py` & `finagg-0.1.0/src/finagg/sec/feat/_refined/quarterly.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,34 @@
-"""Features from SEC sources."""
+"""Quarterly features from SEC sources."""
 
 import logging
 from typing import Literal
 
 import numpy as np
 import pandas as pd
 import sqlalchemy as sa
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import NoResultFound
 from tqdm import tqdm
 
-from .. import backend, feat, indices, utils
-from . import api, sql
+from .... import backend, utils
+from ... import api, sql
+from .. import _raw
 
 logging.basicConfig(
     format="%(asctime)s | %(levelname)s | %(message)s", level=logging.INFO
 )
 logger = logging.getLogger(__name__)
 
 
-def get_unique_filings(
-    df: pd.DataFrame, /, *, form: str = "10-Q", units: None | str = None
-) -> pd.DataFrame:
-    """Get all unique rows as determined by the filing date and tag for a
-    period.
-
-    Args:
-        df: Dataframe without unique rows.
-        form: Only keep rows with form type ``form``. Most popular choices
-            include ``"10-K"`` for annual and ``"10-Q"`` for quarterly.
-        units: Only keep rows with units ``units`` if not ``None``.
-
-    Returns:
-        Dataframe with unique rows.
-
-    Examples:
-        Only get a company's original quarterly earnings-per-share filings.
-
-        >>> df = finagg.sec.api.company_concept.get(
-        ...     "EarningsPerShareBasic",
-        ...     ticker="AAPL",
-        ...     taxonomy="us-gaap",
-        ...     units="USD/shares",
-        ... )
-        >>> finagg.sec.feat.get_unique_filings(
-        ...     df,
-        ...     form="10-Q",
-        ...     units="USD/shares"
-        ... ).head(5)  # doctest: +ELLIPSIS
-             fy  fp  ...
-        0  2009  Q3  ...
-        1  2010  Q1  ...
-        2  2010  Q2  ...
-        3  2010  Q3  ...
-        4  2011  Q1  ...
-
-    """
-    mask = df["form"] == form
-    match form:
-        case "10-K":
-            mask &= df["fp"] == "FY"
-        case "10-Q":
-            mask &= df["fp"].str.startswith("Q")
-    if units:
-        mask &= df["units"] == units
-    df = df[mask]
-    return (
-        df.sort_values(["fy", "fp", "filed"])
-        .groupby(["fy", "fp", "tag"], as_index=False)
-        .first()
-    )
-
-
-class RefinedIndustryQuarterly:
+class IndustryQuarterly:
     """Methods for gathering industry-averaged quarterly data from SEC
     features.
 
-    The class variable :data:`finagg.sec.feat.quarterly.industry` is an
+    The class variable :attr:`finagg.sec.feat.Quarterly.industry` is an
     instance of this feature set implementation and is the most popular
     interface for calling feature methods.
 
     Examples:
         You can aggregate this feature set using a ticker or an industry code
         directly.
 
@@ -137,35 +85,39 @@
         Raises:
             `ValueError`: If neither a ``ticker`` nor ``code`` are provided.
             `NoResultFound`: If there are no rows for ``ticker`` or ``code``
                 in the refined SQL table.
 
         Examples:
             >>> df = finagg.sec.feat.quarterly.industry.from_refined(ticker="AAPL").head(5)
-            >>> df["avg"]  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-            name                AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            fy   fp filed                                                                   ...
-            2009 Q3 2009-10-30                    0.0000           0.5733            3.0650 ...
-            2010 Q1 2010-04-29                   -0.0122           0.4025            0.8650 ...
-                 Q2 2010-07-30                    0.0000           0.5003            0.5386 ...
-                 Q3 2010-11-04                    0.0011           0.4568            1.2038 ...
-            2011 Q1 2011-05-05                    0.2716           0.4652            0.9920 ...
-            >>> df["std"]  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-            name                AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            fy   fp filed                                                                   ...
-            2009 Q3 2009-10-30                    0.0000           0.2428            0.5850 ...
-            2010 Q1 2010-04-29                    0.0434           0.1490            0.9865 ...
-                 Q2 2010-07-30                    0.0000           0.2575            2.5274 ...
-                 Q3 2010-11-04                    0.0030           0.2672            2.6892 ...
-            2011 Q1 2011-05-05                    0.1827           0.2859            0.9541 ...
+            >>> df["mean"]  # doctest: +SKIP
+            name                AssetCoverageRatio  DebtEquityRatio  EarningsPerShareBasic ...
+            fy   fp filed                                                                  ...
+            2010 Q1 2010-04-29            1.718796         0.956111               0.865000 ...
+                 Q2 2010-07-30            1.753165         0.874013               0.380000 ...
+                 Q3 2010-11-04            1.830832         0.842663               1.062857 ...
+            2011 Q1 2011-05-05            2.164743         0.757230               1.022500 ...
+                 Q2 2011-08-08            2.222168         0.718292               2.016667 ...
+            >>> df["std"]  # doctest: +SKIP
+            name                AssetCoverageRatio  DebtEquityRatio  EarningsPerShareBasic ...
+            fy   fp filed                                                                  ...
+            2010 Q1 2010-04-29            0.394667         0.327296               1.139079 ...
+                 Q2 2010-07-30            0.310804         0.285554               2.954901 ...
+                 Q3 2010-11-04            0.351052         0.273552               3.075227 ...
+            2011 Q1 2011-05-05            1.166501         0.311317               1.137287 ...
+                 Q2 2011-08-08            1.104677         0.313766               2.075428 ...
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.submissions.name):
+            sql.submissions.create(engine)
+        if not sa.inspect(engine).has_table(sql.quarterly.name):
+            sql.quarterly.create(engine)
         with engine.begin() as conn:
             if ticker:
                 (sic,) = conn.execute(
                     sa.select(sql.submissions.c.sic).where(
                         sql.submissions.c.ticker == ticker
                     )
                 ).one()
@@ -173,55 +125,49 @@
             elif code:
                 code = str(code)[:level]
             else:
                 raise ValueError("Must provide a `ticker` or `code`.")
 
             df = pd.DataFrame(
                 conn.execute(
-                    sa.select(
-                        sql.quarterly.c.fy,
-                        sql.quarterly.c.fp,
-                        sa.func.max(sql.quarterly.c.filed).label("filed"),
-                        sql.quarterly.c.name,
-                        sa.func.avg(sql.quarterly.c.value).label("avg"),
-                        sa.func.std(sql.quarterly.c.value).label("std"),
-                    )
+                    sql.quarterly.select()
                     .join(
                         sql.submissions,
                         (sql.submissions.c.cik == sql.quarterly.c.cik)
                         & (sql.submissions.c.sic.startswith(code)),
                     )
-                    .group_by(
-                        sql.quarterly.c.fy,
-                        sql.quarterly.c.fp,
-                        sql.quarterly.c.name,
-                    )
-                    .where(
-                        sql.quarterly.c.filed >= start,
-                        sql.quarterly.c.filed <= end,
-                    )
+                    .where(sql.quarterly.c.filed >= start, sql.quarterly.c.filed <= end)
                 )
             )
         if not len(df.index):
             raise NoResultFound(
                 f"No industry quarterly rows found for industry {code}."
             )
-        df = df.pivot(
-            index=["fy", "fp", "filed"],
-            columns="name",
-            values=["avg", "std"],
-        ).sort_index()
-        return df
+        df = df.drop(columns=["cik"])
+        df = df.melt(
+            ["fy", "fp", "filed"], var_name="name", value_name="value"
+        ).set_index(["fy", "fp"])
+        df["filed"] = df.groupby(["fy", "fp"])["filed"].max()
+        return (
+            df.reset_index()  # type: ignore[return-value]
+            .set_index(["fy", "fp", "filed"])
+            .groupby(["fy", "fp", "filed", "name"])
+            .agg([np.mean, np.std])
+            .reset_index()
+            .pivot(index=["fy", "fp", "filed"], columns="name")["value"]
+            .sort_index()
+            .dropna()
+        )
 
 
-class RefinedNormalizedQuarterly:
+class NormalizedQuarterly:
     """Quarterly features from SEC EDGAR data normalized according to industry
     averages and standard deviations.
 
-    The class variable :data:`finagg.sec.feat.quarterly.normalized` is an
+    The class variable :data:`finagg.sec.feat.Quarterly.normalized` is an
     instance of this feature set implementation and is the most popular
     interface for calling feature methods.
 
     Examples:
         It doesn't matter which data source you use to gather features.
         They both return equivalent dataframes.
 
@@ -262,48 +208,55 @@
                 at :data:`finagg.backend.engine`.
 
         Returns:
             Relative quarterly data dataframe with each tag as a
             separate column. Sorted by filing date.
 
         Examples:
-            >>> finagg.sec.feat.quarterly.normalized.from_other_refined("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                                AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            fy   fp filed                                                                   ...
-            2010 Q1 2010-01-25                   -0.2573          -0.2606            1.6980 ...
-                 Q2 2010-04-21                    0.0000          -0.5309            1.5081 ...
-                 Q3 2010-07-21                   -0.3780          -0.3485            1.9323 ...
-            2011 Q1 2011-01-19                    0.2693          -0.1107            2.8801 ...
-                 Q2 2011-04-21                    0.0000          -0.0655            2.8997 ...
+            >>> finagg.sec.feat.quarterly.normalized.from_other_refined("AAPL").head(5)  # doctest: +SKIP
+                                NORM(LOG_CHANGE(Assets))  NORM(LOG_CHANGE(AssetsCurrent))  NORM(LOG_CHANGE(CommonStockSharesOutstanding)) ...
+            fy   fp filed                                                                                                                 ...
+            2010 Q2 2010-04-21                  0.000000                         0.000000                                        0.000000 ...
+                 Q3 2010-07-21                  0.000000                         0.000000                                        0.000000 ...
+            2011 Q1 2011-01-19                  0.978816                         0.074032                                        0.407282 ...
+                 Q2 2011-04-21                  0.000000                         0.000000                                        0.000000 ...
+                 Q3 2011-07-20                 -0.353553                        -0.353553                                        0.051602 ...
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         engine = engine or backend.engine
-        company_df = RefinedQuarterly.from_refined(
+        company_df = Quarterly.from_refined(
             ticker, start=start, end=end, engine=engine
         ).reset_index(["filed"])
         filed = company_df["filed"]
-        industry_df = RefinedIndustryQuarterly.from_refined(
+        industry_df = IndustryQuarterly.from_refined(
             ticker=ticker, level=level, start=start, end=end, engine=engine
         ).reset_index(["filed"])
-        company_df = (company_df - industry_df["avg"]) / industry_df["std"]
+        company_df = (company_df - industry_df["mean"]) / industry_df["std"]
         company_df["filed"] = filed
-        pct_change_columns = RefinedQuarterly.pct_change_target_columns()
-        company_df[pct_change_columns] = company_df[pct_change_columns].fillna(
-            value=0.0
+        func_cols = utils.get_func_cols(sql.quarterly)
+        company_df[func_cols] = company_df[func_cols].fillna(value=0.0)
+        company_df = (
+            company_df.reset_index()
+            .set_index(["fy", "fp", "filed"])
+            .rename(lambda x: f"NORM({x})", axis=1)
         )
-        return (
+        company_df = (
             company_df.fillna(method="ffill")
-            .dropna()
             .reset_index()
+            .dropna()
             .drop_duplicates("filed")
             .set_index(["fy", "fp", "filed"])
             .sort_index()
         )
+        company_df = utils.resolve_col_order(
+            sql.normalized_quarterly, company_df, extra_ignore=["filed"]
+        )
+        return company_df
 
     @classmethod
     def from_refined(
         cls,
         ticker: str,
         /,
         *,
@@ -331,27 +284,31 @@
             separate column. Sorted by filing date.
 
         Raises:
             `NoResultFound`: If there are no rows for ``ticker`` in the
                 refined SQL table.
 
         Examples:
-            >>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                                AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            fy   fp filed                                                                   ...
-            2010 Q1 2010-01-25                   -0.2573          -0.2606            1.6980 ...
-                 Q2 2010-04-21                    0.0000          -0.5309            1.5081 ...
-                 Q3 2010-07-21                   -0.3780          -0.3485            1.9323 ...
-            2011 Q1 2011-01-19                    0.2693          -0.1107            2.8801 ...
-                 Q2 2011-04-21                    0.0000          -0.0655            2.8997 ...
+            >>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)  # doctest: +SKIP
+                                NORM(LOG_CHANGE(Assets))  NORM(LOG_CHANGE(AssetsCurrent))  NORM(LOG_CHANGE(CommonStockSharesOutstanding)) ...
+            fy   fp filed                                                                                                                 ...
+            2010 Q2 2010-04-21                  0.000000                         0.000000                                        0.000000 ...
+                 Q3 2010-07-21                  0.000000                         0.000000                                        0.000000 ...
+            2011 Q1 2011-01-19                  0.978816                         0.074032                                        0.407282 ...
+                 Q2 2011-04-21                  0.000000                         0.000000                                        0.000000 ...
+                 Q3 2011-07-20                 -0.353553                        -0.353553                                        0.051602 ...
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.submissions.name):
+            sql.submissions.create(engine)
+        if not sa.inspect(engine).has_table(sql.normalized_quarterly.name):
+            sql.normalized_quarterly.create(engine)
         with engine.begin() as conn:
             df = pd.DataFrame(
                 conn.execute(
                     sql.normalized_quarterly.select()
                     .join(
                         sql.submissions,
                         (sql.submissions.c.cik == sql.normalized_quarterly.c.cik)
@@ -363,47 +320,43 @@
                     )
                 )
             )
         if not len(df.index):
             raise NoResultFound(
                 f"No industry-normalized quarterly rows found for {ticker}."
             )
-        df = df.pivot(
-            index=["fy", "fp", "filed"], columns="name", values="value"
-        ).sort_index()
-        df.columns = df.columns.rename(None)
-        df = df[RefinedQuarterly.columns]
+        df = df.drop(columns=["cik"]).set_index(["fy", "fp", "filed"]).sort_index()
         return df
 
     @classmethod
     def get_candidate_ticker_set(
         cls, lb: int = 1, *, engine: None | Engine = None
     ) -> set[str]:
         """Get all unique tickers in the quarterly SQL table that MAY BE
         ELIGIBLE to be in the feature's SQL table.
 
-        This is just an alias for :meth:`finagg.sec.feat.quarterly.get_ticker_set`.
+        This is just an alias for :meth:`finagg.sec.feat.Quarterly.get_ticker_set`.
 
         Args:
             lb: Minimum number of rows required to include a ticker in the
                 returned set.
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
 
         Returns:
             All unique tickers that may be valid for creating
             industry-normalized quarterly features that also have at least
             ``lb`` rows for each tag used for constructing the features.
 
         Examples:
-            >>> "AAPL" in finagg.sec.feat.quarterly.normalized.get_candidate_ticker_set()
+            >>> "AAPL" in finagg.sec.feat.quarterly.normalized.get_candidate_ticker_set()  # doctest: +SKIP
             True
 
         """
-        return RefinedQuarterly.get_ticker_set(lb=lb, engine=engine)
+        return Quarterly.get_ticker_set(lb=lb, engine=engine)
 
     @classmethod
     def get_ticker_set(cls, lb: int = 1, *, engine: None | Engine = None) -> set[str]:
         """Get all unique tickers in the feature's SQL table.
 
         Args:
             lb: Minimum number of rows required to include a ticker in the
@@ -413,34 +366,33 @@
 
         Returns:
             All unique tickers that contain all the columns for creating
             industry-normalized quarterly features that also have at least
             ``lb`` rows.
 
         Examples:
-            >>> "AAPL" in finagg.sec.feat.quarterly.normalized.get_ticker_set()
+            >>> "AAPL" in finagg.sec.feat.quarterly.normalized.get_ticker_set()  # doctest: +SKIP
             True
 
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.submissions.name):
+            sql.submissions.create(engine)
+        if not sa.inspect(engine).has_table(sql.normalized_quarterly.name):
+            sql.normalized_quarterly.create(engine)
         with engine.begin() as conn:
             tickers = (
                 conn.execute(
                     sa.select(sql.submissions.c.ticker)
                     .join(
                         sql.normalized_quarterly,
                         sql.normalized_quarterly.c.cik == sql.submissions.c.cik,
                     )
                     .group_by(sql.normalized_quarterly.c.cik)
-                    .having(
-                        *[
-                            sa.func.count(sql.normalized_quarterly.c.name == col) >= lb
-                            for col in RefinedQuarterly.columns
-                        ]
-                    )
+                    .having(sa.func.count(sql.normalized_quarterly.c.filed) >= lb)
                 )
                 .scalars()
                 .all()
             )
         return set(tickers)
 
     @classmethod
@@ -469,23 +421,25 @@
                 at :data:`finagg.backend.engine`.
 
         Returns:
             Tickers sorted by a feature column for a particular year and quarter.
 
         Examples:
             >>> ts = finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by(
-            ...         "EarningsPerShare",
+            ...         "EarningsPerShareBasic",
             ...         year=2020,
             ...         quarter=3
             ... )
-            >>> "PCGU" == ts[0]
+            >>> "AMD" == ts[0]  # doctest: +SKIP
             True
 
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.normalized_quarterly.name):
+            sql.normalized_quarterly.create(engine)
         with engine.begin() as conn:
             if year == -1:
                 (max_year,) = conn.execute(
                     sa.select(sa.func.max(sql.normalized_quarterly.c.fy))
                 ).one()
                 year = int(max_year)
 
@@ -501,49 +455,69 @@
                 conn.execute(
                     sa.select(sql.submissions.c.ticker)
                     .join(
                         sql.normalized_quarterly,
                         sql.normalized_quarterly.c.cik == sql.submissions.c.cik,
                     )
                     .where(
-                        sql.normalized_quarterly.c.name == column,
                         sql.normalized_quarterly.c.fy == year,
                         sql.normalized_quarterly.c.fp == fp,
                     )
-                    .order_by(sql.normalized_quarterly.c.value)
+                    .order_by(sql.normalized_quarterly.c[column])
                 )
                 .scalars()
                 .all()
             )
         if not ascending:
             return list(reversed(tickers))
         return list(tickers)
 
     @classmethod
     def install(
-        cls, tickers: None | set[str] = None, *, engine: None | Engine = None
+        cls,
+        tickers: None | set[str] = None,
+        *,
+        engine: None | Engine = None,
+        recreate_tables: bool = False,
     ) -> int:
-        """Drop the feature's table, create a new one, and insert data
-        transformed from another raw SQL table.
+        """Install data associated with ``tickers`` by pulling data from the
+        quarterly SQL tables, transforming them into normalized features, and
+        then writing to the refined quarterly normalized SQL table.
+
+        Tables associated with this method are created if they don't already
+        exist.
 
         Args:
             tickers: Set of tickers to install features for. Defaults to all
                 the candidate tickers from
-                :meth:`RefinedNormalizedQuarterly.get_candidate_ticker_set`.
+                :meth:`NormalizedQuarterly.get_candidate_ticker_set`.
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
+            recreate_tables: Whether to drop and recreate tables, wiping all
+                previously installed data.
 
         Returns:
             Number of rows written to the feature's SQL table.
 
         """
         tickers = tickers or cls.get_candidate_ticker_set(engine=engine)
+        if not tickers:
+            logger.info(
+                "Skipping finagg.sec.feat.quarterly.normalized installation because no"
+                " tickers were provided or no tickers were found with prerequisite data"
+                " (i.e., finagg.sec.feat.quarterly data)"
+            )
+            return 0
+
         engine = engine or backend.engine
-        sql.normalized_quarterly.drop(engine, checkfirst=True)
-        sql.normalized_quarterly.create(engine)
+        if recreate_tables or not sa.inspect(engine).has_table(
+            sql.normalized_quarterly.name
+        ):
+            sql.normalized_quarterly.drop(engine, checkfirst=True)
+            sql.normalized_quarterly.create(engine)
 
         total_rows = 0
         for ticker in tqdm(
             tickers,
             desc="Installing refined SEC industry-normalized quarterly data",
             position=0,
             leave=True,
@@ -578,33 +552,26 @@
                 table.
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
 
         Returns:
             Number of rows written to the SQL table.
 
-        Raises:
-            `ValueError`: If the given dataframe's columns do not match this
-                feature's columns.
-
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.normalized_quarterly.name):
+            sql.normalized_quarterly.create(engine)
         df = df.reset_index(["fy", "fp", "filed"])
-        if set(df.columns) < set(RefinedQuarterly.columns):
-            raise ValueError(
-                f"Dataframe must have columns {RefinedQuarterly.columns} but got {df.columns}"
-            )
-        df = df.melt(["fy", "fp", "filed"], var_name="name", value_name="value")
         df["cik"] = sql.get_cik(ticker, engine=engine)
         with engine.begin() as conn:
             conn.execute(sql.normalized_quarterly.insert(), df.to_dict(orient="records"))  # type: ignore[arg-type]
         return len(df.index)
 
 
-class RefinedQuarterly(feat.Features):
+class Quarterly:
     """Methods for gathering quarterly features from SEC EDGAR data.
 
     The module variable :data:`finagg.sec.feat.quarterly` is an instance of
     this feature set implementation and is the most popular interface for
     calling feature methods.
 
     Examples:
@@ -615,83 +582,38 @@
         >>> df2 = finagg.sec.feat.quarterly.from_raw("AAPL").head(5)
         >>> df3 = finagg.sec.feat.quarterly.from_refined("AAPL").head(5)
         >>> pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
         >>> pd.testing.assert_frame_equal(df1, df3, rtol=1e-4)
 
     """
 
-    #: Columns within this feature set. Dataframes returned by this class's
-    #: methods will always contain these columns. The refined data SQL table
-    #: corresponding to these features will also have rows that have these
-    #: names.
-    columns = [
-        "AssetsCurrent_pct_change",
-        "DebtEquityRatio",
-        "EarningsPerShare",
-        "InventoryNet_pct_change",
-        "LiabilitiesCurrent_pct_change",
-        "NetIncomeLoss_pct_change",
-        "OperatingIncomeLoss_pct_change",
-        "PriceBookRatio",
-        "QuickRatio",
-        "ReturnOnEquity",
-        "StockholdersEquity_pct_change",
-        "WorkingCapitalRatio",
-    ]
-
-    concepts = api.popular_concepts
-    """XBRL disclosure concepts to pull to construct the columns in this
-    feature set.
-
-    :meta hide-value:
-    """
-
-    industry = RefinedIndustryQuarterly()
+    industry = IndustryQuarterly()
     """Quarterly features aggregated for an entire industry.
-    The most popular way for accessing the :class:`RefinedIndustryQuarterly`
+    The most popular way for accessing the :class:`IndustryQuarterly`
     feature set.
 
     :meta hide-value:
     """
 
-    normalized = RefinedNormalizedQuarterly()
+    normalized = NormalizedQuarterly()
     """A company's quarterly features normalized by its industry.
-    The most popular way for accessing the :class:`RefinedNormalizedQuarterly`
+    The most popular way for accessing the :class:`NormalizedQuarterly`
     feature set.
 
     :meta hide-value:
     """
 
     @classmethod
     def _normalize(cls, df: pd.DataFrame, /) -> pd.DataFrame:
         """Normalize quarterly features columns."""
-        df = df.set_index(["fy", "fp"]).sort_index()
-        df["filed"] = df.groupby(["fy", "fp"])["filed"].max()
-        df = df.reset_index()
-        df = df.pivot(
-            index=["fy", "fp", "filed"],
-            columns="tag",
-            values="value",
-        ).astype(float)
-        df["EarningsPerShare"] = df["EarningsPerShareBasic"]
-        df["DebtEquityRatio"] = df["LiabilitiesCurrent"] / df["StockholdersEquity"]
-        df["PriceBookRatio"] = df["StockholdersEquity"] / (
-            df["AssetsCurrent"] - df["LiabilitiesCurrent"]
-        )
-        df["QuickRatio"] = (df["AssetsCurrent"] - df["InventoryNet"]) / df[
-            "LiabilitiesCurrent"
-        ]
-        df["ReturnOnEquity"] = df["NetIncomeLoss"] / df["StockholdersEquity"]
-        df["WorkingCapitalRatio"] = df["AssetsCurrent"] / df["LiabilitiesCurrent"]
+        df = api.get_financial_ratios(df)
         df = df.replace([-np.inf, np.inf], np.nan).fillna(method="ffill")
-        df[cls.pct_change_target_columns()] = df[cls.pct_change_source_columns()].apply(
-            utils.safe_pct_change
-        )
+        df = utils.resolve_func_cols(sql.quarterly, df, drop=True, inplace=True)
         df.columns = df.columns.rename(None)
-        df = df[cls.columns]
+        df = utils.resolve_col_order(sql.quarterly, df, extra_ignore=["filed"])
         return df.dropna()
 
     @classmethod
     def from_api(
         cls, ticker: str, /, *, start: None | str = None, end: None | str = None
     ) -> pd.DataFrame:
         """Get quarterly features directly from the SEC API.
@@ -708,38 +630,27 @@
                 last recorded date.
 
         Returns:
             Quarterly data dataframe with each tag as a
             separate column. Sorted by filing date.
 
         Examples:
-            >>> finagg.sec.feat.quarterly.from_api("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                                AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            fy   fp filed                                                                   ...
-            2010 Q1 2010-01-25                   -0.0234           0.3637              2.54 ...
-                 Q2 2010-04-21                    0.0000           0.3637              4.35 ...
-                 Q3 2010-07-21                    0.0000           0.3637              6.40 ...
-            2011 Q1 2011-01-19                    0.3208           0.4336              3.74 ...
-                 Q2 2011-04-21                    0.0000           0.4336              7.12 ...
+            >>> finagg.sec.feat.quarterly.from_api("AAPL").head(5)  # doctest: +SKIP
+                                LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent)  LOG_CHANGE(CommonStockSharesOutstanding) ...
+            fy   fp filed                                                                                               ...
+            2010 Q1 2010-01-25            0.182629                  -0.023676                                  0.012840 ...
+                 Q2 2010-04-21            0.000000                   0.000000                                  0.000000 ...
+                 Q3 2010-07-21            0.000000                   0.000000                                  0.000000 ...
+            2011 Q1 2011-01-19            0.459174                   0.278241                                  0.017805 ...
+                 Q2 2011-04-21            0.000000                   0.000000                                  0.000000 ...
 
         """
-        start = start or "1776-07-04"
-        end = end or utils.today
-        dfs = []
-        for concept in cls.concepts:
-            tag = concept["tag"]
-            taxonomy = concept["taxonomy"]
-            units = concept["units"]
-            df = api.company_concept.get(
-                tag, ticker=ticker, taxonomy=taxonomy, units=units
-            )
-            df = get_unique_filings(df, units=units)
-            df = df[(df["filed"] >= start) & (df["filed"] <= end)]
-            dfs.append(df)
-        df = pd.concat(dfs)
+        df = api.company_concept.join_get(
+            api.popular_concepts, ticker=ticker, form="10-Q", start=start, end=end
+        )
         return cls._normalize(df)
 
     @classmethod
     def from_raw(
         cls,
         ticker: str,
         /,
@@ -763,52 +674,33 @@
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
 
         Returns:
             Quarterly data dataframe with each tag as a
             separate column. Sorted by filing date.
 
-        Raises:
-            `NoResultFound`: If there are no rows for ``ticker`` in the
-                raw SQL table.
-
         Examples:
-            >>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                                AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            fy   fp filed                                                                   ...
-            2010 Q1 2010-01-25                   -0.0234           0.3637              2.54 ...
-                 Q2 2010-04-21                    0.0000           0.3637              4.35 ...
-                 Q3 2010-07-21                    0.0000           0.3637              6.40 ...
-            2011 Q1 2011-01-19                    0.3208           0.4336              3.74 ...
-                 Q2 2011-04-21                    0.0000           0.4336              7.12 ...
-
-        """
-        start = start or "1776-07-04"
-        end = end or utils.today
-        engine = engine or backend.engine
-        with engine.begin() as conn:
-            df = pd.DataFrame(
-                conn.execute(
-                    sql.tags.select()
-                    .join(
-                        sql.submissions,
-                        (sql.submissions.c.cik == sql.tags.c.cik)
-                        & (sql.submissions.c.ticker == ticker),
-                    )
-                    .where(
-                        sql.tags.c.tag.in_(
-                            [concept["tag"] for concept in cls.concepts]
-                        ),
-                        sql.tags.c.filed >= start,
-                        sql.tags.c.filed <= end,
-                    )
-                )
-            )
-        if not len(df.index):
-            raise NoResultFound(f"No quarterly rows found for {ticker}.")
+            >>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)  # doctest: +SKIP
+                                LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent)  LOG_CHANGE(CommonStockSharesOutstanding) ...
+            fy   fp filed                                                                                               ...
+            2010 Q1 2010-01-25            0.182629                  -0.023676                                  0.012840 ...
+                 Q2 2010-04-21            0.000000                   0.000000                                  0.000000 ...
+                 Q3 2010-07-21            0.000000                   0.000000                                  0.000000 ...
+            2011 Q1 2011-01-19            0.459174                   0.278241                                  0.017805 ...
+                 Q2 2011-04-21            0.000000                   0.000000                                  0.000000 ...
+
+        """
+        df = _raw.Tags.join_from_raw(
+            ticker,
+            [concept["tag"] for concept in api.popular_concepts],
+            form="10-Q",
+            start=start,
+            end=end,
+            engine=engine,
+        )
         return cls._normalize(df)
 
     @classmethod
     def from_refined(
         cls,
         ticker: str,
         /,
@@ -837,27 +729,31 @@
             separate column. Sorted by filing date.
 
         Raises:
             `NoResultFound`: If there are no rows for ``ticker`` in the
                 refined SQL table.
 
         Examples:
-            >>> finagg.sec.feat.quarterly.from_refined("AAPL").head(5)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                                AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-            fy   fp filed                                                                   ...
-            2010 Q1 2010-01-25                   -0.0234           0.3637              2.54 ...
-                 Q2 2010-04-21                    0.0000           0.3637              4.35 ...
-                 Q3 2010-07-21                    0.0000           0.3637              6.40 ...
-            2011 Q1 2011-01-19                    0.3208           0.4336              3.74 ...
-                 Q2 2011-04-21                    0.0000           0.4336              7.12 ...
+            >>> finagg.sec.feat.quarterly.from_refined("AAPL").head(5)  # doctest: +SKIP
+                                LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent)  LOG_CHANGE(CommonStockSharesOutstanding) ...
+            fy   fp filed                                                                                               ...
+            2010 Q1 2010-01-25            0.182629                  -0.023676                                  0.012840 ...
+                 Q2 2010-04-21            0.000000                   0.000000                                  0.000000 ...
+                 Q3 2010-07-21            0.000000                   0.000000                                  0.000000 ...
+            2011 Q1 2011-01-19            0.459174                   0.278241                                  0.017805 ...
+                 Q2 2011-04-21            0.000000                   0.000000                                  0.000000 ...
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.submissions.name):
+            sql.submissions.create(engine)
+        if not sa.inspect(engine).has_table(sql.quarterly.name):
+            sql.quarterly.create(engine)
         with engine.begin() as conn:
             df = pd.DataFrame(
                 conn.execute(
                     sql.quarterly.select()
                     .join(
                         sql.submissions,
                         (sql.submissions.c.cik == sql.quarterly.c.cik)
@@ -867,21 +763,15 @@
                         sql.quarterly.c.filed >= start,
                         sql.quarterly.c.filed <= end,
                     )
                 )
             )
         if not len(df.index):
             raise NoResultFound(f"No quarterly rows found for {ticker}.")
-        df = df.pivot(
-            index=["fy", "fp", "filed"],
-            columns="name",
-            values="value",
-        ).sort_index()
-        df.columns = df.columns.rename(None)
-        df = df[cls.columns]
+        df = df.drop(columns=["cik"]).set_index(["fy", "fp", "filed"]).sort_index()
         return df
 
     @classmethod
     def get_candidate_ticker_set(
         cls, lb: int = 1, *, engine: None | Engine = None
     ) -> set[str]:
         """Get all unique tickers in the raw SQL table that MAY BE ELIGIBLE
@@ -895,39 +785,44 @@
 
         Returns:
             All unique tickers that may be valid for creating quarterly features
             that also have at least ``lb`` rows for each tag used for
             constructing the features.
 
         Examples:
-            >>> "AAPL" in finagg.sec.feat.quarterly.get_candidate_ticker_set()
+            >>> "AAPL" in finagg.sec.feat.quarterly.get_candidate_ticker_set()  # doctest: +SKIP
             True
 
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.submissions.name):
+            sql.submissions.create(engine)
+        if not sa.inspect(engine).has_table(sql.tags.name):
+            sql.tags.create(engine)
         with engine.begin() as conn:
             tickers = (
                 conn.execute(
                     sa.select(
                         sql.submissions.c.ticker,
                         *[
                             sa.func.sum(
                                 sa.case(
                                     {concept["tag"]: 1}, value=sql.tags.c.tag, else_=0
                                 )
                             ).label(concept["tag"])
-                            for concept in cls.concepts
+                            for concept in api.popular_concepts
                         ],
                     )
                     .join(sql.tags, sql.tags.c.cik == sql.submissions.c.cik)
+                    .where(sql.tags.c.form == "10-Q")
                     .group_by(sql.tags.c.cik)
                     .having(
                         *[
                             sa.text(f"{concept['tag']} >= {lb}")
-                            for concept in cls.concepts
+                            for concept in api.popular_concepts
                         ]
                     )
                 )
                 .scalars()
                 .all()
             )
         return set(tickers)
@@ -948,54 +843,72 @@
 
         Examples:
             >>> "AAPL" in finagg.sec.feat.quarterly.get_ticker_set()
             True
 
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.submissions.name):
+            sql.submissions.create(engine)
+        if not sa.inspect(engine).has_table(sql.quarterly.name):
+            sql.quarterly.create(engine)
         with engine.begin() as conn:
             tickers = (
                 conn.execute(
                     sa.select(sql.submissions.c.ticker)
                     .join(sql.quarterly, sql.quarterly.c.cik == sql.submissions.c.cik)
                     .group_by(sql.quarterly.c.cik)
-                    .having(
-                        *[
-                            sa.func.count(sql.quarterly.c.name == col) >= lb
-                            for col in cls.columns
-                        ]
-                    )
+                    .having(sa.func.count(sql.quarterly.c.filed) >= lb)
                 )
                 .scalars()
                 .all()
             )
         return set(tickers)
 
     @classmethod
     def install(
-        cls, tickers: None | set[str] = None, *, engine: None | Engine = None
+        cls,
+        tickers: None | set[str] = None,
+        *,
+        engine: None | Engine = None,
+        recreate_tables: bool = False,
     ) -> int:
-        """Drop the feature's table, create a new one, and insert data
-        transformed from another raw SQL table.
+        """Install data associated with ``tickers`` by pulling data from the
+        raw SQL tables, transforming them into quarterly features, and then
+        writing to the refined quarterly SQL table.
+
+        Tables associated with this method are created if they don't already
+        exist.
 
         Args:
             tickers: Set of tickers to install features for. Defaults to all
                 the candidate tickers from
-                :meth:`RefinedQuarterly.get_candidate_ticker_set`.
+                :meth:`Quarterly.get_candidate_ticker_set`.
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
+            recreate_tables: Whether to drop and recreate tables, wiping all
+                previously installed data.
 
         Returns:
             Number of rows written to the feature's SQL table.
 
         """
         tickers = tickers or cls.get_candidate_ticker_set(engine=engine)
+        if not tickers:
+            logger.info(
+                "Skipping finagg.sec.feat.quarterly installation because no tickers"
+                " were provided or no tickers were found with prerequisite data (i.e.,"
+                " finagg.sec.feat.submissions and finagg.sec.feat.raw data)"
+            )
+            return 0
+
         engine = engine or backend.engine
-        sql.quarterly.drop(engine, checkfirst=True)
-        sql.quarterly.create(engine)
+        if recreate_tables or not sa.inspect(engine).has_table(sql.quarterly.name):
+            sql.quarterly.drop(engine, checkfirst=True)
+            sql.quarterly.create(engine)
 
         total_rows = 0
         for ticker in tqdm(
             tickers,
             desc="Installing refined SEC quarterly data",
             position=0,
             leave=True,
@@ -1030,310 +943,16 @@
             df: Dataframe to store as rows in a local SQL table
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
 
         Returns:
             Number of rows written to the SQL table.
 
-        Raises:
-            `ValueError`: If the given dataframe's columns do not match this
-                feature's columns.
-
         """
         engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.quarterly.name):
+            sql.quarterly.create(engine)
         df = df.reset_index(["fy", "fp", "filed"])
-        if set(df.columns) < set(cls.columns):
-            raise ValueError(
-                f"Dataframe must have columns {cls.columns} but got {df.columns}"
-            )
-        df = df.melt(["fy", "fp", "filed"], var_name="name", value_name="value")
         df["cik"] = sql.get_cik(ticker, engine=engine)
         with engine.begin() as conn:
             conn.execute(sql.quarterly.insert(), df.to_dict(orient="records"))  # type: ignore[arg-type]
         return len(df.index)
-
-
-class RawSubmissions:
-    """Get a single company's metadata as-is from raw SEC data.
-
-    The module variable :data:`finagg.sec.feat.submissions` is an instance of
-    this feature set implementation and is the most popular interface for
-    calling feature methods.
-
-    """
-
-    @classmethod
-    def install(
-        cls, tickers: None | set[str] = None, *, engine: None | Engine = None
-    ) -> int:
-        """Drop the feature's table, create a new one, and insert data
-        as-is from the SEC API.
-
-        Args:
-            tickers: Set of tickers to install features for. Defaults to all
-                the tickers from :meth:`finagg.indices.api.get_ticker_set`.
-            engine: Feature store database engine. Defaults to the engine
-                at :data:`finagg.backend.engine`.
-
-        Returns:
-            Number of rows written to the feature's SQL table.
-
-        """
-        tickers = tickers or indices.api.get_ticker_set()
-        engine = engine or backend.engine
-        sql.submissions.drop(engine, checkfirst=True)
-        sql.submissions.create(engine)
-
-        total_rows = 0
-        for ticker in tqdm(
-            tickers,
-            desc="Installing raw SEC submissions data",
-            position=0,
-            leave=True,
-        ):
-            try:
-                metadata = api.submissions.get(ticker=ticker)["metadata"]
-                df = pd.DataFrame(metadata, index=[0])
-                rowcount = len(df.index)
-                if rowcount:
-                    cls.to_raw(df, engine=engine)
-                    total_rows += rowcount
-                    logger.debug(f"{rowcount} rows inserted for {ticker}")
-                else:
-                    logger.debug(f"Skipping {ticker} due to missing submissions")
-            except Exception as e:
-                logger.debug(f"Skipping {ticker}", exc_info=e)
-        return total_rows
-
-    @classmethod
-    def from_raw(
-        cls,
-        ticker: str,
-        /,
-        *,
-        engine: None | Engine = None,
-    ) -> pd.DataFrame:
-        """Get a single company's metadata as-is from raw SEC data.
-
-        The metadata provided for each company varies and each company's
-        metadata may be incomplete. Only their SEC CIK and SIC industry
-        code are guaranteed to be provided.
-
-        Args:
-            ticker: Company ticker.
-            engine: Feature store database engine. Defaults to the engine
-                at :data:`finagg.backend.engine`.
-
-        Returns:
-            A dataframe containing the company's metadata.
-
-        Raises:
-            `NoResultFound`: If there are no rows for ``ticker`` in the raw
-                SQL table.
-
-        Examples:
-            >>> finagg.sec.feat.submissions.from_raw("AAPL")  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
-                      cik ticker entity_type   sic sic_description ...
-            0  0000320193   AAPL        None  3571            None ...
-
-        """
-        engine = engine or backend.engine
-        with engine.begin() as conn:
-            df = pd.DataFrame(
-                conn.execute(
-                    sql.submissions.select().where(sql.submissions.c.ticker == ticker)
-                )
-            )
-        if not len(df.index):
-            raise NoResultFound(f"No rows found for {ticker}.")
-        return df
-
-    @classmethod
-    def to_raw(cls, df: pd.DataFrame, /, *, engine: None | Engine = None) -> int:
-        """Write the given dataframe to the raw feature table.
-
-        Args:
-            df: Dataframe to store as rows in a local SQL table
-            engine: Feature store database engine. Defaults to the engine
-                at :data:`finagg.backend.engine`.
-
-        Returns:
-            Number of rows written to the SQL table.
-
-        """
-        engine = engine or backend.engine
-        with engine.begin() as conn:
-            conn.execute(sql.submissions.insert(), df.to_dict(orient="records"))  # type: ignore[arg-type]
-        return len(df)
-
-
-class RawTags:
-    """Get a single company concept tag as-is from raw SEC data.
-
-    The module variable :data:`finagg.sec.feat.tags` is an instance of
-    this feature set implementation and is the most popular interface for
-    calling feature methods.
-
-    """
-
-    @classmethod
-    def install(
-        cls, tickers: None | set[str] = None, *, engine: None | Engine = None
-    ) -> int:
-        """Drop the feature's table, create a new one, and insert data
-        as-is from the SEC API.
-
-        Args:
-            tickers: Set of tickers to install features for. Defaults to all
-                the tickers from :meth:`finagg.indices.api.get_ticker_set`.
-            engine: Feature store database engine. Defaults to the engine
-                at :data:`finagg.backend.engine`.
-
-        Returns:
-            Number of rows written to the feature's SQL table.
-
-        """
-        tickers = tickers or indices.api.get_ticker_set()
-        engine = engine or backend.engine
-        sql.tags.drop(engine, checkfirst=True)
-        sql.tags.create(engine)
-
-        total_rows = 0
-        for ticker in tqdm(
-            tickers,
-            desc="Installing raw SEC tags data",
-            position=0,
-            leave=True,
-        ):
-            for concept in api.popular_concepts:
-                tag = concept["tag"]
-                taxonomy = concept["taxonomy"]
-                units = concept["units"]
-                try:
-                    df = api.company_concept.get(
-                        tag,
-                        ticker=ticker,
-                        taxonomy=taxonomy,
-                        units=units,
-                    )
-                    df = get_unique_filings(df, form="10-Q", units=units)
-                    rowcount = len(df.index)
-                    if rowcount:
-                        cls.to_raw(df, engine=engine)
-                        total_rows += rowcount
-                        logger.debug(f"{rowcount} rows inserted for {ticker} tag {tag}")
-                    else:
-                        logger.debug(f"Skipping {ticker} due to missing filings")
-                except Exception as e:
-                    logger.debug(f"Skipping {ticker}", exc_info=e)
-        return total_rows
-
-    @classmethod
-    def from_raw(
-        cls,
-        ticker: str,
-        tag: str,
-        /,
-        *,
-        start: None | str = None,
-        end: None | str = None,
-        engine: None | Engine = None,
-    ) -> pd.DataFrame:
-        """Get a single company concept tag as-is from raw SEC data.
-
-        This is the preferred method for accessing raw SEC data without
-        using the SEC API.
-
-        Args:
-            ticker: Company ticker.
-            tag: Company concept tag to retreive.
-            start: The start date of the observation period. Defaults to the
-                first recorded date.
-            end: The end date of the observation period. Defaults to the
-                last recorded date.
-            engine: Feature store database engine. Defaults to the engine
-                at :data:`finagg.backend.engine`.
-
-        Returns:
-            A dataframe containing the company concept tag values
-            across the specified period.
-
-        Raises:
-            `NoResultFound`: If there are no rows for ``ticker`` and ``tag``
-                in the raw SQL table.
-
-        Examples:
-            >>> finagg.sec.feat.tags.from_raw("AAPL", "EarningsPerShareBasic").head(5)  # doctest: +NORMALIZE_WHITESPACE
-                                     units  value
-            fy   fp filed
-            2009 Q3 2009-07-22  USD/shares   4.20
-            2010 Q1 2010-01-25  USD/shares   2.54
-                 Q2 2010-04-21  USD/shares   4.35
-                 Q3 2010-07-21  USD/shares   6.40
-            2011 Q1 2011-01-19  USD/shares   3.74
-
-        """
-        start = start or "1776-07-04"
-        end = end or utils.today
-        engine = engine or backend.engine
-        with engine.begin() as conn:
-            df = pd.DataFrame(
-                conn.execute(
-                    sa.select(
-                        sql.tags.c.fy,
-                        sql.tags.c.fp,
-                        sql.tags.c.filed,
-                        sql.tags.c.units,
-                        sql.tags.c.value,
-                    )
-                    .join(
-                        sql.submissions,
-                        (sql.submissions.c.cik == sql.tags.c.cik)
-                        & (sql.submissions.c.ticker == ticker),
-                    )
-                    .where(
-                        sql.tags.c.tag == tag,
-                        sql.tags.c.filed >= start,
-                        sql.tags.c.filed <= end,
-                    )
-                )
-            )
-        if not len(df.index):
-            raise NoResultFound(f"No {tag} rows found for {ticker}.")
-        return df.set_index(["fy", "fp", "filed"]).sort_index()
-
-    @classmethod
-    def to_raw(cls, df: pd.DataFrame, /, *, engine: None | Engine = None) -> int:
-        """Write the given dataframe to the raw feature table.
-
-        Args:
-            df: Dataframe to store as rows in a local SQL table
-            engine: Feature store database engine. Defaults to the engine
-                at :data:`finagg.backend.engine`.
-
-        Returns:
-            Number of rows written to the SQL table.
-
-        """
-        engine = engine or backend.engine
-        with engine.begin() as conn:
-            conn.execute(sql.tags.insert(), df.to_dict(orient="records"))  # type: ignore[arg-type]
-        return len(df)
-
-
-quarterly = RefinedQuarterly()
-"""The most popular way for accessing :class:`RefinedQuarterly`.
-
-:meta hide-value:
-"""
-
-submissions = RawSubmissions()
-"""The most popular way for accessing :class:`RawSubmissions`.
-
-:meta hide-value:
-"""
-
-tags = RawTags()
-"""The most popular way for accessing :class:`RawTags`.
-
-:meta hide-value:
-"""
```

### Comparing `finagg-0.0.0b1/src/finagg/sec/sql.py` & `finagg-0.1.0/src/finagg/yfinance/feat/_refined.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,379 +1,350 @@
-"""SEC SQLAlchemy interfaces."""
+"""Refined Yahoo! Finance features (features aggregated from raw tables)."""
 
-from typing import Any, Literal
+import logging
 
+import numpy as np
+import pandas as pd
 import sqlalchemy as sa
 from sqlalchemy.engine import Engine
+from sqlalchemy.exc import NoResultFound
+from tqdm import tqdm
 
-from .. import backend
+from ... import backend, utils
+from .. import api, sql
+from . import _raw
 
-metadata = sa.MetaData()
-
-submissions = sa.Table(
-    "sec.raw.submissions",
-    metadata,
-    sa.Column("cik", sa.String, primary_key=True, doc="Unique SEC ID."),
-    sa.Column("ticker", sa.String, nullable=False, doc="Company ticker."),
-    sa.Column(
-        "entity_type", sa.String, doc="Type of company standing (e.g., operating)."
-    ),
-    sa.Column("sic", sa.String, nullable=False, doc="Industry code."),
-    sa.Column("sic_description", sa.String, doc="Industry code description."),
-    sa.Column("name", sa.String, doc="Company name."),
-    sa.Column(
-        "exchanges",
-        sa.String,
-        doc="Comma-separated exchanges the company is found on.",
-    ),
-    sa.Column("ein", sa.String, doc="Entity identification number."),
-    sa.Column("description", sa.String, doc="Entity description (often empty/null)."),
-    sa.Column("category", sa.String, doc="SEC entity category."),
-    sa.Column(
-        "fiscal_year_end",
-        sa.String,
-        doc="The company's last day of the fiscal year (MMDD).",
-    ),
-)
-
-tags = sa.Table(
-    "sec.raw.tags",
-    metadata,
-    sa.Column(
-        "cik",
-        sa.String,
-        sa.ForeignKey(submissions.c.cik, ondelete="CASCADE"),
-        primary_key=True,
-        doc="Unique SEC ID.",
-    ),
-    sa.Column("accn", sa.String, doc="Unique submission/access number."),
-    sa.Column(
-        "taxonomy", sa.String, doc="XBRL taxonomy the submission's tag belongs to."
-    ),
-    sa.Column(
-        "tag",
-        sa.String,
-        primary_key=True,
-        doc="XBRL submission tag (e.g., NetIncomeLoss).",
-    ),
-    sa.Column(
-        "form", sa.String, nullable=False, doc="Submission form type (e.g., 10-Q)."
-    ),
-    sa.Column(
-        "units",
-        sa.String,
-        nullable=False,
-        doc="Unit of measurements for tag value (e.g., USD or shares).",
-    ),
-    sa.Column(
-        "fy", sa.Integer, primary_key=True, doc="Fiscal year the submission is for."
-    ),
-    sa.Column(
-        "fp",
-        sa.String,
-        primary_key=True,
-        doc="Fiscal period the submission is for (e.g., Q1 or FY).",
-    ),
-    sa.Column(
-        "start",
-        sa.String,
-        nullable=True,
-        doc="When the tag's value's measurements started.",
-    ),
-    sa.Column(
-        "end",
-        sa.String,
-        nullable=True,
-        doc="When the tag's value's measurements ended.",
-    ),
-    sa.Column(
-        "filed",
-        sa.String,
-        nullable=False,
-        doc="When the submission was actually filed.",
-    ),
-    sa.Column(
-        "frame",
-        sa.String,
-        nullable=True,
-        doc="Often a concatenation of `fy` and `fp`.",
-    ),
-    sa.Column(
-        "label",
-        sa.String,
-        nullable=True,
-        doc="More human readable version of `tag`.",
-    ),
-    sa.Column(
-        "description",
-        sa.String,
-        nullable=True,
-        doc="Long description of `tag` and `label`.",
-    ),
-    sa.Column("entity", sa.String, doc="Company name."),
-    sa.Column("value", sa.Float, nullable=False, doc="Tag value with units `units`."),
-)
-
-quarterly = sa.Table(
-    "sec.refined.quarterly",
-    metadata,
-    sa.Column(
-        "cik",
-        sa.String,
-        sa.ForeignKey(submissions.c.cik, ondelete="CASCADE"),
-        primary_key=True,
-        doc="Unique company ticker.",
-    ),
-    sa.Column("filed", sa.String, nullable=False, doc="Filing date."),
-    sa.Column("name", sa.String, primary_key=True, doc="Feature name."),
-    sa.Column("fy", sa.Integer, primary_key=True, doc="Fiscal year the value is for."),
-    sa.Column(
-        "fp",
-        sa.String,
-        primary_key=True,
-        doc="Fiscal period the value is for (e.g., Q1 or FY).",
-    ),
-    sa.Column("value", sa.Float, nullable=False, doc="Feature value."),
+logging.basicConfig(
+    format="%(asctime)s | %(levelname)s | %(message)s", level=logging.INFO
 )
+logger = logging.getLogger(__name__)
 
 
-normalized_quarterly = sa.Table(
-    "sec.refined.quarterly.normalized",
-    metadata,
-    sa.Column(
-        "cik",
-        sa.String,
-        sa.ForeignKey(submissions.c.cik, ondelete="CASCADE"),
-        primary_key=True,
-        doc="Unique company ticker.",
-    ),
-    sa.Column("filed", sa.String, nullable=False, doc="Filing date."),
-    sa.Column("name", sa.String, primary_key=True, doc="Feature name."),
-    sa.Column("fy", sa.Integer, primary_key=True, doc="Fiscal year the value is for."),
-    sa.Column(
-        "fp",
-        sa.String,
-        primary_key=True,
-        doc="Fiscal period the value is for (e.g., Q1 or FY).",
-    ),
-    sa.Column("value", sa.Float, nullable=False, doc="Feature value."),
-)
-
-
-def get_cik(ticker: str, /, *, engine: None | Engine = None) -> str:
-    """Use raw SQL data to find a company's SEC CIK from its ticker symbol.
-
-    This is the preferred method for getting a company's SEC CIK if raw SQL
-    data is installed. This method is a convenience over
-    :meth:`finagg.sec.api.get_cik` for repeatedly getting company SEC
-    CIKs without having to query the SEC EDGAR API. Use
-    :meth:`finagg.sec.api.get_cik` if you want to get a company's ticker
-    symbol without installing or accessing locally installed raw SQL data.
-
-    Args:
-        ticker: A company's ticker symbol.
-        engine: Feature store database engine. Defaults to the engine
-            at :data:`finagg.backend.engine`.
-
-    Returns:
-        The company's corresponding SEC CIK.
-
-    Examples:
-        Get Apple's SEC CIK from its ticker.
-
-        >>> finagg.sec.sql.get_cik("AAPL") == "0000320193"
-        True
-
-    """
-    engine = engine or backend.engine
-    with engine.begin() as conn:
-        (cik,) = conn.execute(
-            sa.select(submissions.c.cik).where(submissions.c.ticker == ticker)
-        ).one()
-    return str(cik)
-
-
-def get_metadata(
-    *, cik: None | str = None, ticker: None | str = None, engine: None | Engine = None
-) -> dict[str, Any]:
-    """Return a company's metadata (its SEC CIK, ticker, name, and industry
-    code) from its SEC CIK or its ticker symbol.
-
-    A convenient method for getting a company's metadata using raw SQL
-    data. This method is a convenience over
-    :data:`finagg.sec.api.submissions` for repeatedly getting company
-    metadata without having to query the SEC EDGAR API. Use
-    :data:`finagg.sec.api.submissions` if you want to get a company's
-    metadata without installing or accessing locally installed raw SQL data.
-
-    Args:
-        cik: Company SEC CIK. Mutually exclusive with ``ticker``.
-        ticker: Company ticker. Mutually exclusive with ``cik``.
-        engine: Feature store database engine. Defaults to the engine
-            at :data:`finagg.backend.engine`.
-
-    Returns:
-        A company's metadata as a dictionary.
-
-    Examples:
-        >>> finagg.sec.sql.get_metadata(ticker="MSFT")
-        {'cik': '0000789019', 'ticker': 'MSFT', 'name': 'microsoft corp', 'sic': '7372'}
-
-    """
-    engine = engine or backend.engine
-
-    if bool(cik) == bool(ticker):
-        raise ValueError("Must provide a `cik` or a `ticker`.")
-
-    if ticker:
-        cik = str(get_cik(ticker, engine=engine))
-
-    with engine.begin() as conn:
-        row = conn.execute(
-            sa.select(
-                submissions.c.cik,
-                submissions.c.ticker,
-                submissions.c.name,
-                submissions.c.sic,
-            ).where(submissions.c.cik == cik)
-        ).one()
-    return row._asdict()
-
-
-def get_ticker(cik: str, /, *, engine: None | Engine = None) -> str:
-    """Use raw SQL data to find a company's ticker from its SEC CIK.
-
-    This is the preferred method for getting a company's ticker if raw SQL
-    data is installed. This method is a convenience over
-    :meth:`finagg.sec.api.get_ticker` for repeatedly getting company tickers
-    without having to query the SEC EDGAR API. Use
-    :meth:`finagg.sec.api.get_ticker` if you want to get a company's
-    ticker symbol without installing or accessing locally installed raw
-    SQL data.
-
-    Args:
-        cik: A company's SEC CIK.
-        engine: Feature store database engine. Defaults to the engine
-            at :data:`finagg.backend.engine`.
+class Daily:
+    """Methods for gathering daily stock data features from Yahoo! finance.
 
-    Returns:
-        The company's corresponding ticker symbol.
+    The module variable :data:`finagg.yfinance.feat.daily` is an instance of
+    this feature set implementation and is the most popular interface for
+    calling feature methods.
 
     Examples:
-        Get Apple's ticker from its SEC CIK.
+        It doesn't matter which data source you use to gather features.
+        They all return equivalent dataframes.
 
-        >>> finagg.sec.sql.get_ticker("0000320193") == "AAPL"
-        True
+        >>> df1 = finagg.yfinance.feat.daily.from_api("AAPL").head(5)
+        >>> df2 = finagg.yfinance.feat.daily.from_raw("AAPL").head(5)
+        >>> df3 = finagg.yfinance.feat.daily.from_refined("AAPL").head(5)
+        >>> pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
+        >>> pd.testing.assert_frame_equal(df1, df3, rtol=1e-4)
 
     """
-    engine = engine or backend.engine
-    with engine.begin() as conn:
-        (ticker,) = conn.execute(
-            sa.select(submissions.c.ticker).where(submissions.c.cik == cik)
-        ).one()
-    return str(ticker)
-
-
-def get_ticker_set(
-    lb: int = 1,
-    *,
-    engine: None | Engine = None,
-) -> set[str]:
-    """Get all unique ticker symbols in the raw SQL tables that have at least
-    ``lb`` rows.
-
-    This method is convenient for accessing the tickers that have raw SQL data
-    associated with them so the data associated with those tickers can be
-    further refined. A common pattern is to use this method and other
-    ``get_ticker_set`` methods (such as those found in :mod:`finagg.sec.feat`)
-    to determine which tickers are missing data from other tables or features.
-
-    Args:
-        lb: Lower bound number of rows that a company must have for its ticker
-            to be included in the set returned by this method.
-        engine: Feature store database engine. Defaults to the engine
-            at :data:`finagg.backend.engine`.
 
-    Examples:
-        >>> "AAPL" in finagg.sec.sql.get_ticker_set()
-        True
-
-    """
-    engine = engine or backend.engine
-    with engine.begin() as conn:
-        tickers = (
-            conn.execute(
-                sa.select(submissions.c.ticker)
-                .join(tags, tags.c.cik == submissions.c.cik)
-                .group_by(tags.c.cik)
-                .having(sa.func.count(tags.c.filed) >= lb)
+    @classmethod
+    def _normalize(cls, df: pd.DataFrame, /) -> pd.DataFrame:
+        """Normalize daily features columns."""
+        df = df.drop(columns=["ticker"]).set_index("date").sort_index()
+        df = df.replace([-np.inf, np.inf], np.nan).fillna(method="ffill")
+        df = utils.resolve_func_cols(sql.daily, df, drop=True, inplace=True)
+        return df.dropna()
+
+    @classmethod
+    def from_api(
+        cls, ticker: str, /, *, start: None | str = None, end: None | str = None
+    ) -> pd.DataFrame:
+        """Get daily features directly from :meth:`finagg.yfinance.api.get`.
+
+        Args:
+            ticker: Company ticker.
+            start: The start date of the stock history. Defaults to the
+                first recorded date.
+            end: The end date of the stock history. Defaults to the
+                last recorded date.
+
+        Returns:
+            Daily stock price dataframe sorted by date.
+
+        Examples:
+            >>> finagg.yfinance.feat.daily.from_api("AAPL").head(5)  # doctest: +SKIP
+                        LOG_CHANGE(open)  LOG_CHANGE(high)  LOG_CHANGE(low)  LOG_CHANGE(close) ...
+            date                                                                               ...
+            1980-12-15         -0.049005         -0.053343        -0.053581          -0.053581 ...
+            1980-12-16         -0.075870         -0.075870        -0.076231          -0.076231 ...
+            1980-12-17          0.019512          0.024331         0.024450           0.024450 ...
+            1980-12-18          0.028580          0.028445         0.028580           0.028580 ...
+            1980-12-19          0.059239          0.058970         0.059239           0.059239 ...
+
+        """
+        start = start or "1776-07-04"
+        end = end or utils.today
+        df = api.get(ticker, start=start, end=end)
+        return cls._normalize(df)
+
+    @classmethod
+    def from_raw(
+        cls,
+        ticker: str,
+        /,
+        *,
+        start: None | str = None,
+        end: None | str = None,
+        engine: None | Engine = None,
+    ) -> pd.DataFrame:
+        """Get daily features from local SQL tables.
+
+        Args:
+            ticker: Company ticker.
+            start: The start date of the stock history. Defaults to the
+                first recorded date.
+            end: The end date of the stock history. Defaults to the
+                last recorded date.
+            engine: Raw store database engine. Defaults to the engine
+                at :data:`finagg.backend.engine`.
+
+        Returns:
+            Daily stock price dataframe sorted by date.
+
+        Raises:
+            `NoResultFound`: If there are no rows for ``ticker`` in the
+                raw SQL table.
+
+        Examples:
+            >>> finagg.yfinance.feat.daily.from_raw("AAPL").head(5)  # doctest: +SKIP
+                        LOG_CHANGE(open)  LOG_CHANGE(high)  LOG_CHANGE(low)  LOG_CHANGE(close) ...
+            date                                                                               ...
+            1980-12-15         -0.049005         -0.053343        -0.053581          -0.053581 ...
+            1980-12-16         -0.075870         -0.075870        -0.076231          -0.076231 ...
+            1980-12-17          0.019512          0.024331         0.024450           0.024450 ...
+            1980-12-18          0.028580          0.028445         0.028580           0.028580 ...
+            1980-12-19          0.059239          0.058970         0.059239           0.059239 ...
+
+        """
+        start = start or "1776-07-04"
+        end = end or utils.today
+        engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.prices.name):
+            sql.prices.create(engine)
+        with engine.begin() as conn:
+            df = pd.DataFrame(
+                conn.execute(
+                    sql.prices.select().where(
+                        sql.prices.c.ticker == ticker,
+                        sql.prices.c.date >= start,
+                        sql.prices.c.date <= end,
+                    )
+                )
             )
-            .scalars()
-            .all()
-        )
-    return set(tickers)
-
-
-def get_tickers_in_industry(
-    *,
-    ticker: None | str = None,
-    code: None | str = None,
-    level: Literal[2, 3, 4] = 2,
-    engine: None | Engine = None,
-) -> set[str]:
-    """Get a set of tickers that all share the same industry using raw SQL data.
-
-    This method is convenient for finding tickers within the same
-    industry so they can be compared. A related and common pattern is to use
-    :data:`finagg.sec.feat.quarterly.normalized` to get industry-normalized
-    features for a particular company. Similar to other methods in this
-    submodule, this will only return tickers that have raw SQL data associated
-    with them.
-
-    Args:
-        ticker: Company ticker. Lookup the industry associated
-            with this company. Mutually exclusive with ``code``.
-        code: Industry SIC code to use for industry lookup.
-            Mutually exclusive with ``ticker``.
-        level: Industry level to find tickers within.
-            The industry used according to ``ticker`` or ``code``
-            is subsampled according to this value. Options include:
-
-                - 2 = major group (e.g., furniture and fixtures)
-                - 3 = industry group (e.g., office furnitures)
-                - 4 = industry (e.g., wood office furniture)
-
-        engine: Feature store database engine. Defaults to the engine
-            at :data:`finagg.backend.engine`.
-
-    Returns:
-        A set of tickers that all share the same industry as denoted by
-        another ticker (using the ``ticker`` arg) or an industry SIC code
-        (using the ``code`` arg).
-
-    Examples:
-        >>> "ETSY" in finagg.sec.sql.get_tickers_in_industry(ticker="MSFT")
-        True
-
-    """
-    engine = engine or backend.engine
-    with engine.begin() as conn:
-        if ticker:
-            (sic,) = conn.execute(
-                sa.select(submissions.c.sic).where(submissions.c.ticker == ticker)
-            ).one()
-            code = str(sic)[:level]
-        elif code:
-            code = str(code)[:level]
-        else:
-            raise ValueError("Must provide a `ticker` or `code`.")
-
-        tickers = (
-            conn.execute(
-                sa.select(submissions.c.ticker).where(
-                    submissions.c.sic.startswith(code)
+        if not len(df.index):
+            raise NoResultFound(f"No daily rows found for {ticker}.")
+        return cls._normalize(df)
+
+    @classmethod
+    def from_refined(
+        cls,
+        ticker: str,
+        /,
+        *,
+        start: None | str = None,
+        end: None | str = None,
+        engine: None | Engine = None,
+    ) -> pd.DataFrame:
+        """Get features from the feature-dedicated local SQL tables.
+
+        This is the preferred method for accessing features for
+        offline analysis (assuming data in the local SQL tables
+        is installed and is up-to-date).
+
+        Args:
+            ticker: Company ticker.
+            start: The start date of the observation period. Defaults to the
+                first recorded date.
+            end: The end date of the observation period. Defaults to the
+                last recorded date.
+            engine: Feature store database engine. Defaults to the engine
+                at :data:`finagg.backend.engine`.
+
+        Returns:
+            Daily stock price dataframe sorted by date.
+
+        Raises:
+            `NoResultFound`: If there are no rows for ``ticker`` in the
+                refined SQL table.
+
+        Examples:
+            >>> finagg.yfinance.feat.daily.from_refined("AAPL").head(5)  # doctest: +SKIP
+                        LOG_CHANGE(open)  LOG_CHANGE(high)  LOG_CHANGE(low)  LOG_CHANGE(close) ...
+            date                                                                               ...
+            1980-12-15         -0.049005         -0.053343        -0.053581          -0.053581 ...
+            1980-12-16         -0.075870         -0.075870        -0.076231          -0.076231 ...
+            1980-12-17          0.019512          0.024331         0.024450           0.024450 ...
+            1980-12-18          0.028580          0.028445         0.028580           0.028580 ...
+            1980-12-19          0.059239          0.058970         0.059239           0.059239 ...
+
+        """
+        start = start or "1776-07-04"
+        end = end or utils.today
+        engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.daily.name):
+            sql.daily.create(engine)
+        with engine.begin() as conn:
+            df = pd.DataFrame(
+                conn.execute(
+                    sql.daily.select().where(
+                        sql.daily.c.ticker == ticker,
+                        sql.daily.c.date >= start,
+                        sql.daily.c.date <= end,
+                    )
                 )
             )
-            .scalars()
-            .all()
-        )
-    return set(tickers)
+        if not len(df.index):
+            raise NoResultFound(f"No daily rows found for {ticker}.")
+        return df.drop(columns=["ticker"]).set_index("date").sort_index()
+
+    @classmethod
+    def get_candidate_ticker_set(
+        cls, lb: int = 1, *, engine: None | Engine = None
+    ) -> set[str]:
+        """Get all unique tickers in the raw SQL table that MAY BE ELIGIBLE
+        to be in the feature's refined SQL table.
+
+        Args:
+            lb: Minimum number of rows required to include a ticker in the
+                returned set.
+            engine: Feature store database engine. Defaults to the engine
+                at :data:`finagg.backend.engine`.
+
+        Returns:
+            All unique tickers that may be valid for creating daily features
+            that also have at least ``lb`` rows used for constructing the
+            features.
+
+        Examples:
+            >>> "AAPL" in finagg.yfinance.feat.daily.get_candidate_ticker_set()  # doctest: +SKIP
+            True
+
+        """
+        return _raw.Prices.get_ticker_set(lb=lb, engine=engine)
+
+    @classmethod
+    def get_ticker_set(cls, lb: int = 1, *, engine: None | Engine = None) -> set[str]:
+        """Get all unique tickers in the feature's SQL table.
+
+        Args:
+            lb: Minimum number of rows required to include a ticker in the
+                returned set.
+            engine: Feature store database engine. Defaults to the engine
+                at :data:`finagg.backend.engine`.
+
+        Returns:
+            All unique tickers that contain all the columns for creating
+            daily features that also have at least ``lb`` rows.
+
+        Examples:
+            >>> "AAPL" in finagg.yfinance.feat.daily.get_ticker_set()  # doctest: +SKIP
+            True
+
+        """
+        engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.daily.name):
+            sql.daily.create(engine)
+        with engine.begin() as conn:
+            tickers = (
+                conn.execute(
+                    sa.select(sql.daily.c.ticker)
+                    .group_by(sql.daily.c.ticker)
+                    .having(sa.func.count(sql.daily.c.date) >= lb)
+                )
+                .scalars()
+                .all()
+            )
+        return set(tickers)
+
+    @classmethod
+    def install(
+        cls,
+        tickers: None | set[str] = None,
+        *,
+        engine: None | Engine = None,
+        recreate_tables: bool = False,
+    ) -> int:
+        """Install data associated with ``tickers`` by pulling data from the
+        raw SQL tables, transforming them into daily features, and then writing
+        to the refined daily SQL table.
+
+        Tables associated with this method are created if they don't already
+        exist.
+
+        Args:
+            tickers: Set of tickers to install features for. Defaults to all
+                the tickers from :meth:`finagg.indices.api.get_ticker_set`.
+            engine: Feature store database engine. Defaults to the engine
+                at :data:`finagg.backend.engine`.
+            recreate_tables: Whether to drop and recreate tables, wiping all
+                previously installed data.
+
+        Returns:
+            Number of rows written to the feature's refined SQL table.
+
+        """
+        tickers = tickers or cls.get_candidate_ticker_set()
+        if not tickers:
+            logger.info(
+                "Skipping finagg.yfinance.feat.daily installation because no tickers"
+                " were provided or no tickers were found with prerequisite data (i.e.,"
+                " finagg.yfinance.feat.prices data)"
+            )
+            return 0
+
+        engine = engine or backend.engine
+        if recreate_tables or not sa.inspect(engine).has_table(sql.daily.name):
+            sql.daily.drop(engine, checkfirst=True)
+            sql.daily.create(engine)
+
+        total_rows = 0
+        for ticker in tqdm(
+            tickers,
+            desc="Installing refined Yahoo! Finance daily data",
+            position=0,
+            leave=True,
+        ):
+            try:
+                df = cls.from_raw(ticker, engine=engine)
+                rowcount = len(df.index)
+                if rowcount:
+                    cls.to_refined(ticker, df, engine=engine)
+                    total_rows += rowcount
+                    logger.debug(f"{rowcount} rows inserted for {ticker}")
+                else:
+                    logger.debug(f"Skipping {ticker} due to missing data")
+            except Exception as e:
+                logger.debug(f"Skipping {ticker}", exc_info=e)
+        return total_rows
+
+    @classmethod
+    def to_refined(
+        cls,
+        ticker: str,
+        df: pd.DataFrame,
+        /,
+        *,
+        engine: None | Engine = None,
+    ) -> int:
+        """Write the given dataframe to the refined feature table
+        while using the ticker ``ticker``.
+
+        Args:
+            ticker: Company ticker.
+            df: Dataframe to store as rows in a local SQL table.
+            engine: Feature store database engine. Defaults to the engine
+                at :data:`finagg.backend.engine`.
+
+        Returns:
+            Number of rows written to the SQL table.
+
+        """
+        engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.daily.name):
+            sql.daily.create(engine)
+        df = df.reset_index("date")
+        df["ticker"] = ticker
+        with engine.begin() as conn:
+            conn.execute(sql.daily.insert(), df.to_dict(orient="records"))  # type: ignore[arg-type]
+        return len(df.index)
```

### Comparing `finagg-0.0.0b1/src/finagg/testing.py` & `finagg-0.1.0/src/finagg/testing.py`

 * *Files identical despite different names*

### Comparing `finagg-0.0.0b1/src/finagg/yfinance/_cli.py` & `finagg-0.1.0/src/finagg/yfinance/_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,26 +23,24 @@
     help=(
         "Drop and recreate tables, and install the recommended "
         "tables into the SQL database."
     ),
 )
 @click.option(
     "--raw",
-    "-r",
     type=click.Choice(["prices"]),
     multiple=True,
     help=(
         "Raw tables to install. `prices` indicates daily historical stock "
         "price data. `prices` must be specified to enable installing refined "
         "data using the `refined` flag."
     ),
 )
 @click.option(
     "--refined",
-    "-ref",
     type=click.Choice(["daily"]),
     multiple=True,
     help=(
         "Refined tables to install. This requires raw data to be "
         "installed beforehand using the `--raw` flag or for the "
         "`--raw` flag to be set when this option is provided."
     ),
@@ -88,30 +86,41 @@
         "popular and large market cap companies, while 'sec' will "
         "attempt to download and install data for nearly all "
         "publicly-traded US companies. Choosing 'indices' will be fast, "
         "while choosing 'sec' will be slow but will include more diverse data."
     ),
 )
 @click.option(
+    "--recreate-tables",
+    "-r",
+    is_flag=True,
+    default=False,
+    help=(
+        "Whether to reset the tables associated with the install options by "
+        "dropping and recreating them."
+    ),
+)
+@click.option(
     "--verbose",
     "-v",
     is_flag=True,
     default=False,
     help="Sets the log level to DEBUG to show installation errors for each ticker.",
 )
 def install(
     raw: list[Literal["prices"]] = [],
     refined: list[Literal["daily"]] = [],
     all_: bool = False,
     ticker: list[str] = [],
     ticker_set: None | Literal["indices", "sec"] = None,
+    recreate_tables: bool = False,
     verbose: bool = False,
 ) -> int:
     if verbose:
-        logger.setLevel(logging.DEBUG)
+        logging.getLogger(__package__).setLevel(logging.DEBUG)
 
     total_rows = 0
     all_raw = set()
     if all_:
         all_raw = {"prices"}
     elif raw:
         all_raw = set(raw)
@@ -128,33 +137,37 @@
             logger.info(
                 f"Skipping {__package__} installation because no tickers were "
                 "provided (by the `ticker` option or by the `ticker-set` option)"
             )
             return total_rows
 
         if "prices" in all_raw:
-            total_rows += _feat.prices.install(all_tickers)
+            total_rows += _feat.prices.install(
+                all_tickers, recreate_tables=recreate_tables
+            )
 
     all_refined = set()
     if all_:
         all_refined = {"daily"}
     elif refined:
         all_refined = set(refined)
 
     if "daily" in all_refined:
-        total_rows += _feat.daily.install(tickers=all_tickers)
+        total_rows += _feat.daily.install(
+            tickers=all_tickers, recreate_tables=recreate_tables
+        )
 
     if all_ or all_refined or all_raw:
         if total_rows:
             logger.info(f"{total_rows} total rows inserted for {__package__}")
         else:
             logger.warning(
-                f"No rows were inserted for {__package__}. This is likely an "
-                "error. Set the verbose flag with the `--verbose/-v` option "
-                "to enable debug logging."
+                f"No rows were inserted for {__package__}. This could be an error if"
+                " installations were not skipped. Set the verbose flag with the"
+                " `--verbose/-v` option to enable debug logging."
             )
     else:
         logger.info(
             f"Skipping {__package__} installation because no installation "
             "options are provided"
         )
     return total_rows
```

### Comparing `finagg-0.0.0b1/src/finagg/yfinance/api.py` & `finagg-0.1.0/src/finagg/yfinance/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Simple wrappers for `yfinance.Ticker`."""
+"""Simple wrappers for Yahoo! Finance."""
 
 import pandas as pd
 import yfinance as yf
 
 
 def get(
     ticker: str,
@@ -12,34 +12,34 @@
     end: None | str = None,
     interval: str = "1d",
     period: str = "max",
     debug: bool = False,
 ) -> pd.DataFrame:
     """Get a ticker's stock price history.
 
-    Does a simple transform on yfinance's ticker API dataframe result to be
-    a bit more consistent with other API implementations.
+    Does a simple transform on Yahoo! Finance's ticker API dataframe result to
+    be a bit more consistent with other API implementations.
 
     Args:
         ticker: Company ticker to get historical price data for.
         start: Start date for stock price history. Defaults to the first
             recorded date.
         end: End date for stock price history. Defaults to the last recorded
             date.
         interval: Frequency at which stock price history is grabbed.
         period: Time period to get in the past. ``"max"`` returns the full
             stock price history and the default.
-        debug: Debug mode passed to ``yfinance``.
+        debug: Debug mode passed to the Yahoo! Finance scraper.
 
     Returns:
-        :mod:`yfinance` auto-adjusted stock price history with slightly
+        Yahoo! Finance auto-adjusted stock price history with slightly
         different (more normalized) column names.
 
     Examples:
-        >>> finagg.yfinance.api.get("AAPL").head(5)
+        >>> finagg.yfinance.api.get("AAPL").head(5)  # doctest: +SKIP
                  date    open    high     low   close     volume ticker
         0  1980-12-12  0.0997  0.1002  0.0997  0.0997  469033600   AAPL
         1  1980-12-15  0.0950  0.0950  0.0945  0.0945  175884800   AAPL
         2  1980-12-16  0.0880  0.0880  0.0876  0.0876  105728000   AAPL
         3  1980-12-17  0.0897  0.0902  0.0897  0.0897   86441600   AAPL
         4  1980-12-18  0.0924  0.0928  0.0924  0.0924   73449600   AAPL
```

### Comparing `finagg-0.0.0b1/src/finagg.egg-info/PKG-INFO` & `finagg-0.1.0/src/finagg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finagg
-Version: 0.0.0b1
+Version: 0.1.0
 Summary: Data aggregation with popular and free financial APIs.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,15 +201,16 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: repository, https://github.com/theOGognf/finagg
+Project-URL: Repository, https://github.com/theOGognf/finagg
+Project-URL: Documentation, https://theogognf.github.io/finagg/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.10
@@ -227,21 +228,31 @@
 ========================================
 
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
+* **Documentation**: https://theogognf.github.io/finagg/
+* **PyPI**: https://pypi.org/project/finagg/
+* **Repository**: https://github.com/theOGognf/finagg
+
 Quick Start
 ===========
 
 Installation
 ------------
 
-Install **finagg** from GitHub directly.
+Install with pip for the latest (stable) version.
+
+.. code:: console
+
+  pip install finagg
+
+Install from GitHub for the latest (unstable) version.
 
 .. code:: console
 
     git clone https://github.com/theOGognf/finagg.git
     pip install ./finagg/
 
 Optionally install the recommended datasets from 3rd party APIs into a local
@@ -253,26 +264,31 @@
 
 The installation will point you where to get free API keys and write them to a
 local ``.env`` file for storage.
 
 Basic Usage
 -----------
 
+These are just **finagg** usage samples. See the `documentation`_ for all the
+supported APIs and features.
+
 Explore the APIs directly
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
+*These methods require internet access and API keys/user agent declarations.*
+
 Get Bureau of Economic Analysis (BEA) data.
 
 >>> finagg.bea.api.gdp_by_industry.get(year=[2019]).head(5)
-   table_id freq  year quarter industry                         industry_description       value
-0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting  156.300003
-1         1    Q  2019       1    111CA                                        Farms  117.599998
-2         1    Q  2019       1    113FF    Forestry, fishing, and related activities   38.700001
-3         1    Q  2019       1       21                                       Mining  305.700012
-4         1    Q  2019       1      211                       Oil and gas extraction  190.199997
+   table_id freq  year quarter industry                         industry_description ...
+0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting ...
+1         1    Q  2019       1    111CA                                        Farms ...
+2         1    Q  2019       1    113FF    Forestry, fishing, and related activities ...
+3         1    Q  2019       1       21                                       Mining ...
+4         1    Q  2019       1      211                       Oil and gas extraction ...
 
 Get Federal Reserve Economic Data (FRED).
 
 >>> finagg.fred.api.series.observations.get(
 ...   "CPIAUCNS",
 ...   realtime_start=0,
 ...   realtime_end=-1,
@@ -294,69 +310,86 @@
 2  2009-10-16  900678473.0  0001193125-10-012091  2009  FY  10-K/A  2010-01-25 ...
 3  2010-01-15  906794589.0  0001193125-10-012085  2010  Q1    10-Q  2010-01-25 ...
 4  2010-04-09  909938383.0  0001193125-10-088957  2010  Q2    10-Q  2010-04-21 ...
 
 Use installed raw data for exploring the most popular features
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+*These methods require internet access, API keys/user agent declarations, and
+downloading and installing raw data through the* ``finagg install`` *or*
+``finagg <api/subpackage> install`` *commands.*
+
 Get the most popular FRED features all in one dataframe.
 
 >>> finagg.fred.feat.economic.from_raw().head(5)
-            CIVPART_pct_change  CPIAUCNS_pct_change  CSUSHPINSA_pct_change  FEDFUNDS ...
-date                                                                                 ...
-2014-10-06                 0.0                  0.0                    0.0      0.09 ...
-2014-10-08                 0.0                  0.0                    0.0      0.09 ...
-2014-10-13                 0.0                  0.0                    0.0      0.09 ...
-2014-10-15                 0.0                  0.0                    0.0      0.09 ...
-2014-10-20                 0.0                  0.0                    0.0      0.09 ...
+            CIVPART  LOG_CHANGE(CPIAUCNS)  LOG_CHANGE(CSUSHPINSA)  FEDFUNDS ...
+date                                                                        ...
+2014-10-06     62.8                   0.0                     0.0      0.09 ...
+2014-10-08     62.8                   0.0                     0.0      0.09 ...
+2014-10-13     62.8                   0.0                     0.0      0.09 ...
+2014-10-15     62.8                   0.0                     0.0      0.09 ...
+2014-10-20     62.8                   0.0                     0.0      0.09 ...
 
 Get quarterly report features from SEC data.
 
 >>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)
-                    AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-fy   fp filed                                                                   ...
-2010 Q1 2010-01-25                 -0.023398         0.363654              2.54 ...
-     Q2 2010-04-21                  0.000000         0.363654              4.35 ...
-     Q3 2010-07-21                  0.000000         0.363654              6.40 ...
-2011 Q1 2011-01-19                  0.320805         0.433596              3.74 ...
-     Q2 2011-04-21                  0.000000         0.433596              7.12 ...
+                    LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent) ...
+fy   fp filed                                                     ...
+2010 Q1 2010-01-25            0.182629                  -0.023676 ...
+     Q2 2010-04-21            0.000000                   0.000000 ...
+     Q3 2010-07-21            0.000000                   0.000000 ...
+2011 Q1 2011-01-19            0.459174                   0.278241 ...
+     Q2 2011-04-21            0.000000                   0.000000 ...
 
 Get an aggregation of quarterly and daily features for a particular ticker.
 
 >>> finagg.fundam.feat.fundam.from_raw("AAPL").head(5)
+            PriceBookRatio  PriceEarningsRatio
+date
+2010-01-25        0.175061            2.423509
+2010-01-26        0.178035            2.464678
+2010-01-27        0.178813            2.475448
+2010-01-28        0.177154            2.452471
+2010-01-29        0.173825            2.406396
 
 Use installed features for exploring refined aggregations of raw data
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+*These methods require installing refined data through the* ``finagg install``
+*or* ``finagg <api/subpackage> install`` *commands.*
+
 Get a ticker's industry's averaged quarterly report features.
 
 >>> finagg.sec.feat.quarterly.industry.from_refined(ticker="AAPL").head(5)
-                                        avg                                  ...
-name               AssetsCurrent_pct_change DebtEquityRatio EarningsPerShare ...
-fy   fp filed                                                                ...
-2009 Q3 2009-10-30                 0.000000        0.573255         3.065000 ...
-2010 Q1 2010-04-29                -0.012229        0.402497         0.865000 ...
-     Q2 2010-07-30                 0.000000        0.500347         0.538571 ...
-     Q3 2010-11-04                 0.001145        0.456791         1.203750 ...
-2011 Q1 2011-05-05                 0.271624        0.465244         0.992000 ...
+                                 mean                           ...
+name               AssetCoverageRatio BookRatio DebtEquityRatio ...
+fy   fp filed                                                   ...
+2014 Q1 2014-05-15          10.731301  9.448954        0.158318 ...
+     Q2 2014-08-14          10.731301  9.448954        0.158318 ...
+     Q3 2014-11-14          10.731301  9.448954        0.158318 ...
+2015 Q1 2015-05-15          16.738972  9.269250        0.294238 ...
+     Q2 2015-08-13          16.738972  9.269250        0.294238 ...
 
 Get a ticker's industry-averaged quarterly report features.
 
 >>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)
-                    AssetsCurrent_pct_change  DebtEquityRatio  EarningsPerShare ...
-fy   fp filed                                                                   ...
-2010 Q1 2010-01-25                 -0.257265        -0.260642          1.697972 ...
-     Q2 2010-04-21                  0.000000        -0.530932          1.508060 ...
-     Q3 2010-07-21                 -0.377964        -0.348547          1.932276 ...
-2011 Q1 2011-01-19                  0.269259        -0.110688          2.880060 ...
-     Q2 2011-04-21                  0.000000        -0.065501          2.899716 ...
+                    NORM(LOG_CHANGE(Assets))  NORM(LOG_CHANGE(AssetsCurrent)) ...
+fy   fp filed                                                                 ...
+2010 Q2 2010-04-21                  0.000000                         0.000000 ...
+     Q3 2010-07-21                  0.000000                         0.000000 ...
+2011 Q1 2011-01-19                  0.978816                         0.074032 ...
+     Q2 2011-04-21                  0.000000                         0.000000 ...
+     Q3 2011-07-20                 -0.353553                        -0.353553 ...
 
 Get tickers sorted by an industry-averaged quarterly report feature.
 
->>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by("EarningsPerShare", year=2019)[:5]
+>>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by(
+...   "EarningsPerShareBasic",
+...   year=2019
+... )[:5]
 ['XRAY', 'TSLA', 'SYY', 'WHR', 'KMB']
 
 Get tickers sorted by an industry-averaged fundamental feature.
 
 >>> finagg.fundam.feat.fundam.normalized.get_tickers_sorted_by(
 ...   "PriceEarningsRatio",
 ...   date="2019-01-04"
@@ -401,32 +434,35 @@
   ``./findata/finagg.sqlite``.
 
 Dependencies
 ============
 
 * `pandas`_ for fast, flexible, and expressive representations of relational data.
 * `requests`_ for HTTP requests to 3rd party APIs.
-* `requests-cache`_ for caching HTTP requests to avoid getting throttled by 3rd party API servers.
+* `requests-cache`_ for caching HTTP requests to avoid getting throttled by 3rd
+  party API servers.
 * `SQLAlchemy`_ for a SQL Python interface.
 * `yfinance`_ for historical stock data from Yahoo! Finance.
 
 API References
 ==============
 
 * The `BEA API`_ and the `BEA API key registration link`_.
 * The `FRED API`_ and the `FRED API key registration link`_.
 * The `SEC API`_.
 
 Related Projects
 ================
 
-* `FinRL`_ is a collection of financial reinforcement learning environments and tools.
+* `FinRL`_ is a collection of financial reinforcement learning environments
+  and tools.
 * `fredapi`_ is an implementation of the FRED API.
-* `OpenBBTerminal`_ an open-source version of the Bloomberg Terminal.
+* `OpenBBTerminal`_ is an open-source version of the Bloomberg Terminal.
 * `sec-edgar`_ is an implementation of a file-based SEC EDGAR parser.
+* `sec-edgar-api`_ is an implementation of the SEC EDGAR REST API.
 
 Frequently Asked Questions
 ==========================
 
 Where should I start?
 ---------------------
 
@@ -434,14 +470,26 @@
 environments using the implemented data features and SQL tables. This
 project was originally created to make RL environments for financial
 applications but has since focused its purpose to just aggregating financial
 data and features. That being said, all the implemented features are
 defined in such a way to make it very easy to develop financial AI/ML,
 so we encourage you to do just that!
 
+Why aren't features being installed for a specific ticker or economic data series?
+----------------------------------------------------------------------------------
+
+Implemented APIs may be relatively new and simply may not provide data for a
+particular ticker or economic data series. For example, earnings per share may
+not be accessible for all companies through the SEC EDGAR API. In some cases,
+APIs may raise an HTTP error, causing installations to skip the ticker or
+series. Additionally, not all tickers and economic data series contain
+sufficient data for feature normalization. If a ticker or series only has one
+data point, that data point could be dropped when computing a feature (such as
+percent change), causing no data to be installed.
+
 What Python versions are supported?
 -----------------------------------
 
 Python 3.10 and up are supported. We don't plan on supporting lower versions
 because 3.10 introduces some nice quality of life updates that are used
 throughout the package.
 
@@ -452,20 +500,22 @@
 using Linux or WSL in practice. The package performs a good amount of I/O and
 interprocess operations that could result in a noticeable performance
 degradation on Windows.
 
 .. _`BEA API`: https://apps.bea.gov/api/signup/
 .. _`BEA API key registration link`: https://apps.bea.gov/API/signup/
 .. _`BEA API site`: https://apps.bea.gov/API/signup/
+.. _`documentation`: https://theogognf.github.io/finagg/
 .. _`FinRL`: https://github.com/AI4Finance-Foundation/FinRL
 .. _`FRED API`: https://fred.stlouisfed.org/docs/api/fred/
 .. _`FRED API key registration link`: https://fredaccount.stlouisfed.org/login/secure/
 .. _`FRED API site`: https://fredaccount.stlouisfed.org/login/secure/
 .. _`fredapi`: https://github.com/mortada/fredapi
 .. _`OpenBBTerminal`: https://github.com/OpenBB-finance/OpenBBTerminal
 .. _`pandas`: https://pandas.pydata.org/
 .. _`requests`: https://requests.readthedocs.io/en/latest/
 .. _`requests-cache`: https://requests-cache.readthedocs.io/en/stable/
 .. _`SEC API`: https://www.sec.gov/edgar/sec-api-documentation
 .. _`sec-edgar`: https://github.com/sec-edgar/sec-edgar
+.. _`sec-edgar-api`: https://github.com/jadchaar/sec-edgar-api
 .. _`SQLAlchemy`: https://www.sqlalchemy.org/
 .. _`yfinance`: https://github.com/ranaroussi/yfinance
```

### Comparing `finagg-0.0.0b1/src/finagg.egg-info/SOURCES.txt` & `finagg-0.1.0/src/finagg.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.rst
 pyproject.toml
-.github/workflows/python-package.yml
+.github/workflows/build-docs.yml
+.github/workflows/test-and-publish.yml
+.github/workflows/test.yml
+docs/.nojekyll
 docs/Makefile
 docs/cli.rst
 docs/conf.py
 docs/configuration.rst
+docs/conventions.rst
 docs/faq.rst
+docs/index.html
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/references.rst
 docs/requirements.txt
+docs/walkthroughs.rst
 docs/_static/custom.css
 src/finagg/__init__.py
 src/finagg/__main__.py
 src/finagg/backend.py
-src/finagg/feat.py
 src/finagg/frame.py
 src/finagg/portfolio.py
 src/finagg/ratelimit.py
 src/finagg/testing.py
 src/finagg/utils.py
 src/finagg.egg-info/PKG-INFO
 src/finagg.egg-info/SOURCES.txt
@@ -32,41 +37,49 @@
 src/finagg.egg-info/top_level.txt
 src/finagg/bea/__init__.py
 src/finagg/bea/_cli.py
 src/finagg/bea/api.py
 src/finagg/bea/sql.py
 src/finagg/fred/__init__.py
 src/finagg/fred/_cli.py
-src/finagg/fred/feat.py
 src/finagg/fred/sql.py
 src/finagg/fred/api/__init__.py
 src/finagg/fred/api/_api.py
-src/finagg/fred/api/category_.py
-src/finagg/fred/api/release_.py
-src/finagg/fred/api/series_.py
-src/finagg/fred/api/source_.py
-src/finagg/fred/api/tags_.py
+src/finagg/fred/api/_category.py
+src/finagg/fred/api/_release.py
+src/finagg/fred/api/_series.py
+src/finagg/fred/api/_source.py
+src/finagg/fred/api/_tags.py
+src/finagg/fred/feat/__init__.py
+src/finagg/fred/feat/_raw.py
+src/finagg/fred/feat/_refined.py
 src/finagg/fundam/__init__.py
 src/finagg/fundam/_cli.py
 src/finagg/fundam/feat.py
 src/finagg/fundam/sql.py
 src/finagg/indices/__init__.py
 src/finagg/indices/_cli.py
 src/finagg/indices/api.py
 src/finagg/indices/sql.py
 src/finagg/sec/__init__.py
 src/finagg/sec/_cli.py
 src/finagg/sec/api.py
-src/finagg/sec/feat.py
 src/finagg/sec/sql.py
+src/finagg/sec/feat/__init__.py
+src/finagg/sec/feat/_raw.py
+src/finagg/sec/feat/_refined/__init__.py
+src/finagg/sec/feat/_refined/annual.py
+src/finagg/sec/feat/_refined/quarterly.py
 src/finagg/yfinance/__init__.py
 src/finagg/yfinance/_cli.py
 src/finagg/yfinance/api.py
-src/finagg/yfinance/feat.py
 src/finagg/yfinance/sql.py
+src/finagg/yfinance/feat/__init__.py
+src/finagg/yfinance/feat/_raw.py
+src/finagg/yfinance/feat/_refined.py
 tests/__init__.py
 tests/test_frame.py
 tests/test_portfolio.py
 tests/test_ratelimit.py
 tests/test_utils.py
 tests/test_bea/__init__.py
 tests/test_bea/test_api.py
@@ -79,9 +92,8 @@
 tests/test_indices/test_api.py
 tests/test_sec/__init__.py
 tests/test_sec/test_api.py
 tests/test_sec/test_feat.py
 tests/test_sec/test_sql.py
 tests/test_yfinance/__init__.py
 tests/test_yfinance/test_api.py
-tests/test_yfinance/test_feat.py
-tests/test_yfinance/test_sql.py
+tests/test_yfinance/test_feat.py
```

### Comparing `finagg-0.0.0b1/tests/test_frame.py` & `finagg-0.1.0/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `finagg-0.0.0b1/tests/test_fundam/test_feat.py` & `finagg-0.1.0/tests/test_fundam/test_feat.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,31 +9,39 @@
 @pytest.fixture
 def engine() -> Engine:
     yield from finagg.testing.sqlite_engine(
         finagg.backend.database_path, metadata=finagg.fundam.sql.metadata
     )
 
 
-def test_fundam_candidate_ticker_set(engine: Engine) -> None:
+def test_fundam_get_candidate_ticker_set(engine: Engine) -> None:
     finagg.yfinance.feat.prices.install({"AAPL"}, engine=engine)
     finagg.yfinance.feat.daily.install({"AAPL"}, engine=engine)
     finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
     finagg.sec.feat.tags.install({"AAPL"}, engine=engine)
     finagg.sec.feat.quarterly.install({"AAPL"}, engine=engine)
     assert "AAPL" in finagg.fundam.feat.fundam.get_candidate_ticker_set(engine=engine)
 
 
-def test_fundam_ticker_set(engine: Engine) -> None:
+def test_fundam_get_candidate_ticker_set_empty(engine: Engine) -> None:
+    assert len(finagg.fundam.feat.fundam.get_candidate_ticker_set(engine=engine)) == 0
+
+
+def test_fundam_get_ticker_set(engine: Engine) -> None:
     finagg.yfinance.feat.prices.install({"AAPL"}, engine=engine)
     finagg.yfinance.feat.daily.install({"AAPL"}, engine=engine)
     finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
     finagg.sec.feat.tags.install({"AAPL"}, engine=engine)
     finagg.sec.feat.quarterly.install({"AAPL"}, engine=engine)
     finagg.fundam.feat.fundam.install({"AAPL"}, engine=engine)
-    assert "AAPL" in finagg.sec.feat.quarterly.get_ticker_set(engine=engine)
+    assert "AAPL" in finagg.fundam.feat.fundam.get_ticker_set(engine=engine)
+
+
+def test_fundam_get_ticker_set_empty(engine: Engine) -> None:
+    assert len(finagg.fundam.feat.fundam.get_ticker_set(engine=engine)) == 0
 
 
 def test_fundam_to_from_refined(engine: Engine) -> None:
     df1 = finagg.fundam.feat.fundam.from_api("AAPL")
     finagg.fundam.feat.fundam.to_refined(
         "AAPL",
         df1,
```

### Comparing `finagg-0.0.0b1/tests/test_portfolio.py` & `finagg-0.1.0/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `finagg-0.0.0b1/tests/test_ratelimit.py` & `finagg-0.1.0/tests/test_ratelimit.py`

 * *Files identical despite different names*

### Comparing `finagg-0.0.0b1/tests/test_sec/test_feat.py` & `finagg-0.1.0/tests/test_sec/test_sql.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import pandas as pd
 import pytest
 from sqlalchemy.engine import Engine
-from sqlalchemy.exc import IntegrityError
 
 import finagg
 
 
 @pytest.fixture
 def engine() -> Engine:
     yield from finagg.testing.sqlite_engine(
         finagg.backend.database_path, metadata=finagg.sec.sql.metadata
     )
 
 
-def test_quarterly_candidate_ticker_set(engine: Engine) -> None:
+def test_get_cik(engine: Engine) -> None:
     finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
-    finagg.sec.feat.tags.install({"AAPL"}, engine=engine)
-    assert "AAPL" in finagg.sec.sql.get_ticker_set(engine=engine)
-    assert "AAPL" in finagg.sec.feat.quarterly.get_candidate_ticker_set(engine=engine)
+    assert finagg.sec.sql.get_cik("AAPL", engine=engine) == "0000320193"
 
 
-def test_quarterly_ticker_set(engine: Engine) -> None:
+def test_get_metadata(engine: Engine) -> None:
     finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
-    finagg.sec.feat.tags.install({"AAPL"}, engine=engine)
-    finagg.sec.feat.quarterly.install({"AAPL"}, engine=engine)
-    assert "AAPL" in finagg.sec.feat.quarterly.get_candidate_ticker_set(engine=engine)
-    assert "AAPL" in finagg.sec.feat.quarterly.get_ticker_set(engine=engine)
+    assert (
+        finagg.sec.sql.get_metadata(ticker="AAPL", engine=engine)["cik"] == "0000320193"
+    )
+
+
+def test_get_ticker(engine: Engine) -> None:
+    finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
+    assert finagg.sec.sql.get_ticker("0000320193", engine=engine) == "AAPL"
 
 
-def test_quarterly_to_from_refined(engine: Engine) -> None:
+def test_get_ticker_set(engine: Engine) -> None:
     finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
-    df1 = finagg.sec.feat.quarterly.from_api("AAPL")
-    finagg.sec.feat.quarterly.to_refined("AAPL", df1, engine=engine)
-    with pytest.raises(IntegrityError):
-        finagg.sec.feat.quarterly.to_refined("AAPL", df1, engine=engine)
+    finagg.sec.feat.tags.install({"AAPL"}, engine=engine)
+    assert "AAPL" in finagg.sec.feat.tags.get_ticker_set(engine=engine)
+
 
-    df2 = finagg.sec.feat.quarterly.from_refined("AAPL", engine=engine)
-    pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
+def test_get_tickers_in_industry(engine: Engine) -> None:
+    finagg.sec.feat.submissions.install({"HD", "LOW"}, engine=engine)
+    assert "LOW" in finagg.sec.sql.get_tickers_in_industry(ticker="HD", engine=engine)
```

### Comparing `finagg-0.0.0b1/tests/test_sec/test_sql.py` & `finagg-0.1.0/tests/test_fred/test_feat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,41 @@
+import pandas as pd
 import pytest
 from sqlalchemy.engine import Engine
+from sqlalchemy.exc import IntegrityError
 
 import finagg
 
 
 @pytest.fixture
 def engine() -> Engine:
     yield from finagg.testing.sqlite_engine(
-        finagg.backend.database_path, metadata=finagg.sec.sql.metadata
+        finagg.backend.database_path, table=finagg.fred.sql.economic
     )
 
 
-def test_get_cik(engine: Engine) -> None:
-    finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
-    assert finagg.sec.sql.get_cik("AAPL", engine=engine) == "0000320193"
+def test_economic_all_equal(engine: Engine) -> None:
+    finagg.fred.feat.series.install(engine=engine)
+    finagg.fred.feat.economic.install(engine=engine)
+    df1 = finagg.fred.feat.economic.from_api().head(5)
+    df2 = finagg.fred.feat.economic.from_raw(engine=engine).head(5)
+    df3 = finagg.fred.feat.economic.from_refined(engine=engine).head(5)
+    pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
+    pd.testing.assert_frame_equal(df1, df3, rtol=1e-4)
 
 
-def test_get_metadata(engine: Engine) -> None:
-    finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
-    assert (
-        finagg.sec.sql.get_metadata(ticker="AAPL", engine=engine)["cik"] == "0000320193"
+def test_economic_to_from_refined(engine: Engine) -> None:
+    df1 = finagg.fred.feat.economic.from_api()
+    finagg.fred.feat.economic.to_refined(
+        df1,
+        engine=engine,
     )
+    with pytest.raises(IntegrityError):
+        finagg.fred.feat.economic.to_refined(
+            df1,
+            engine=engine,
+        )
 
-
-def test_get_ticker(engine: Engine) -> None:
-    finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
-    assert finagg.sec.sql.get_ticker("0000320193", engine=engine) == "AAPL"
-
-
-def test_get_ticker_set(engine: Engine) -> None:
-    finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
-    finagg.sec.feat.tags.install({"AAPL"}, engine=engine)
-    assert "AAPL" in finagg.sec.sql.get_ticker_set(engine=engine)
-
-
-def test_get_tickers_in_industry(engine: Engine) -> None:
-    finagg.sec.feat.submissions.install({"HD", "LOW"}, engine=engine)
-    assert "LOW" in finagg.sec.sql.get_tickers_in_industry(ticker="HD", engine=engine)
+    df2 = finagg.fred.feat.economic.from_refined(
+        engine=engine,
+    )
+    pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
```

### Comparing `finagg-0.0.0b1/tests/test_yfinance/test_feat.py` & `finagg-0.1.0/tests/test_yfinance/test_feat.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,51 @@
 @pytest.fixture
 def engine() -> Engine:
     yield from finagg.testing.sqlite_engine(
         finagg.backend.database_path, table=finagg.yfinance.sql.daily
     )
 
 
-def test_daily_candidate_ticker_set(engine: Engine) -> None:
+def test_daily_all_equal(engine: Engine) -> None:
     finagg.yfinance.feat.prices.install({"AAPL"}, engine=engine)
-    assert "AAPL" in finagg.yfinance.sql.get_ticker_set(engine=engine)
+    finagg.yfinance.feat.daily.install({"AAPL"}, engine=engine)
+    df1 = finagg.yfinance.feat.daily.from_api("AAPL").head(5)
+    df2 = finagg.yfinance.feat.daily.from_raw("AAPL", engine=engine).head(5)
+    df3 = finagg.yfinance.feat.daily.from_refined("AAPL", engine=engine).head(5)
+    pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
+    pd.testing.assert_frame_equal(df1, df3, rtol=1e-4)
+
+
+def test_daily_get_candidate_ticker_set(engine: Engine) -> None:
+    finagg.yfinance.feat.prices.install({"AAPL"}, engine=engine)
+    assert "AAPL" in finagg.yfinance.feat.prices.get_ticker_set(engine=engine)
     assert "AAPL" in finagg.yfinance.feat.daily.get_candidate_ticker_set(engine=engine)
 
 
-def test_daily_ticker_set(engine: Engine) -> None:
+def test_daily_get_candidate_ticker_set_empty(engine: Engine) -> None:
+    assert len(finagg.yfinance.feat.daily.get_candidate_ticker_set(engine=engine)) == 0
+
+
+def test_daily_get_ticker_set(engine: Engine) -> None:
     finagg.yfinance.feat.prices.install({"AAPL"}, engine=engine)
     finagg.yfinance.feat.daily.install({"AAPL"}, engine=engine)
     assert "AAPL" in finagg.yfinance.feat.daily.get_candidate_ticker_set(engine=engine)
     assert "AAPL" in finagg.yfinance.feat.daily.get_ticker_set(engine=engine)
 
 
+def test_daily_get_ticker_set_empty(engine: Engine) -> None:
+    assert len(finagg.yfinance.feat.daily.get_ticker_set(engine=engine)) == 0
+
+
 def test_daily_to_from_refined(engine: Engine) -> None:
     df1 = finagg.yfinance.feat.daily.from_api("AAPL")
     finagg.yfinance.feat.daily.to_refined("AAPL", df1, engine=engine)
     with pytest.raises(IntegrityError):
         finagg.yfinance.feat.daily.to_refined("AAPL", df1, engine=engine)
 
     df2 = finagg.yfinance.feat.daily.from_refined("AAPL", engine=engine)
     pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
+
+
+def test_prices_get_ticker_set(engine: Engine) -> None:
+    finagg.yfinance.feat.prices.install({"AAPL"}, engine=engine)
+    assert "AAPL" in finagg.yfinance.feat.prices.get_ticker_set(engine=engine)
```

