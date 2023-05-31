# Comparing `tmp/regionmask-0.8.0.tar.gz` & `tmp/regionmask-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regionmask-0.8.0.tar", last modified: Wed Sep  8 19:48:10 2021, max compression
+gzip compressed data, was "regionmask-0.9.0.tar", last modified: Wed Mar  2 20:58:31 2022, max compression
```

## Comparing `regionmask-0.8.0.tar` & `regionmask-0.9.0.tar`

### file list

```diff
@@ -1,102 +1,105 @@
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.937778 regionmask-0.8.0/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      190 2021-07-28 12:03:42.000000 regionmask-0.8.0/.codecov.yml
--rw-rw-r--   0 mathause  (1000) mathause  (1000)       24 2021-09-06 06:33:50.000000 regionmask-0.8.0/.git_archival.txt
--rw-rw-r--   0 mathause  (1000) mathause  (1000)       69 2021-09-06 06:33:50.000000 regionmask-0.8.0/.gitattributes
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.929778 regionmask-0.8.0/.github/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      212 2021-07-28 12:03:42.000000 regionmask-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.929778 regionmask-0.8.0/.github/workflows/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2893 2021-09-08 19:24:42.000000 regionmask-0.8.0/.github/workflows/ci-additional.yaml
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2617 2021-09-08 19:24:42.000000 regionmask-0.8.0/.github/workflows/ci.yaml
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2138 2021-07-28 12:03:42.000000 regionmask-0.8.0/.github/workflows/linting.yaml
--rw-r--r--   0 mathause  (1000) mathause  (1000)      431 2020-04-06 15:04:44.000000 regionmask-0.8.0/.gitignore
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     3461 2021-09-06 06:33:50.000000 regionmask-0.8.0/HOW_TO_RELEASE.md
--rw-r--r--   0 mathause  (1000) mathause  (1000)     1070 2019-10-05 07:31:56.000000 regionmask-0.8.0/LICENSE
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1048 2021-09-08 19:48:10.937778 regionmask-0.8.0/PKG-INFO
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1217 2021-09-08 19:25:02.000000 regionmask-0.8.0/README.rst
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.933778 regionmask-0.8.0/ci/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     7082 2021-09-08 19:24:42.000000 regionmask-0.8.0/ci/min_deps_check.py
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.933778 regionmask-0.8.0/ci/requirements/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      840 2021-09-08 19:24:42.000000 regionmask-0.8.0/ci/requirements/docs.yml
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      268 2021-09-08 19:24:42.000000 regionmask-0.8.0/ci/requirements/environment.yml
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      247 2021-09-08 19:24:42.000000 regionmask-0.8.0/ci/requirements/py36-bare-minimum.yml
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      335 2021-09-08 19:24:42.000000 regionmask-0.8.0/ci/requirements/py36-min-all-deps.yml
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.933778 regionmask-0.8.0/data/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)   109303 2020-08-19 21:32:03.000000 regionmask-0.8.0/data/IPCC-WGI-reference-regions-v1.zip
--rw-rw-r--   0 mathause  (1000) mathause  (1000)   117037 2020-08-19 21:32:03.000000 regionmask-0.8.0/data/IPCC-WGI-reference-regions-v4.zip
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1227 2020-07-30 20:01:48.000000 regionmask-0.8.0/data/README.md
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1334 2021-07-28 12:03:42.000000 regionmask-0.8.0/data/regions_remote_catalog.yaml
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.933778 regionmask-0.8.0/docs/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)       99 2021-07-28 12:03:42.000000 regionmask-0.8.0/docs/.gitignore
--rw-r--r--   0 mathause  (1000) mathause  (1000)     7158 2020-04-06 15:04:44.000000 regionmask-0.8.0/docs/Makefile
--rw-r--r--   0 mathause  (1000) mathause  (1000)     1117 2019-10-05 07:31:56.000000 regionmask-0.8.0/docs/README_ipynp_for_RTD
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1585 2021-07-28 12:03:42.000000 regionmask-0.8.0/docs/api.rst
--rwxr-xr-x   0 mathause  (1000) mathause  (1000)      116 2020-04-06 15:04:44.000000 regionmask-0.8.0/docs/clean_notebooks
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     8022 2021-09-08 19:24:42.000000 regionmask-0.8.0/docs/conf.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1707 2020-07-30 20:01:48.000000 regionmask-0.8.0/docs/defined_countries.rst
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1123 2021-07-28 12:03:42.000000 regionmask-0.8.0/docs/defined_landmask.rst
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1417 2020-07-30 20:01:48.000000 regionmask-0.8.0/docs/defined_ocean_basins.rst
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     3072 2021-08-09 14:58:44.000000 regionmask-0.8.0/docs/defined_scientific.rst
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2638 2021-07-28 12:03:42.000000 regionmask-0.8.0/docs/index.rst
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1744 2021-09-08 19:24:42.000000 regionmask-0.8.0/docs/installation.rst
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2883 2021-07-28 12:03:42.000000 regionmask-0.8.0/docs/intake_regionmask.rst
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.933778 regionmask-0.8.0/docs/logo/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    15406 2021-07-28 12:03:42.000000 regionmask-0.8.0/docs/logo/favicon.ico
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     5192 2021-09-08 19:24:42.000000 regionmask-0.8.0/docs/logo/logo.ipynb
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    36492 2021-07-28 12:03:42.000000 regionmask-0.8.0/docs/logo/logo.png
--rw-r--r--   0 mathause  (1000) mathause  (1000)     6709 2019-10-05 07:31:56.000000 regionmask-0.8.0/docs/make.bat
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.933778 regionmask-0.8.0/docs/notebooks/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     7188 2021-09-08 19:24:42.000000 regionmask-0.8.0/docs/notebooks/create_own_regions.ipynb
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     7844 2021-09-08 19:24:42.000000 regionmask-0.8.0/docs/notebooks/geopandas.ipynb
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    15449 2021-09-08 19:24:42.000000 regionmask-0.8.0/docs/notebooks/mask_2D.ipynb
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    14583 2021-07-28 12:03:42.000000 regionmask-0.8.0/docs/notebooks/mask_3D.ipynb
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    17916 2021-09-08 19:25:02.000000 regionmask-0.8.0/docs/notebooks/method.ipynb
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     5092 2021-09-08 19:24:42.000000 regionmask-0.8.0/docs/notebooks/plotting.ipynb
--rw-r--r--   0 mathause  (1000) mathause  (1000)     2104 2020-04-06 15:04:44.000000 regionmask-0.8.0/docs/notebooks/tutorial_rst.tpl
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    19892 2021-09-08 19:46:26.000000 regionmask-0.8.0/docs/whats_new.rst
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.937778 regionmask-0.8.0/licences/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    18658 2020-07-30 20:01:48.000000 regionmask-0.8.0/licences/AR6_REGIONS_LICENSE
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    10273 2020-07-30 20:01:48.000000 regionmask-0.8.0/licences/XARRAY_LICENSE
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      220 2021-09-06 06:33:50.000000 regionmask-0.8.0/pyproject.toml
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      302 2021-09-06 06:33:50.000000 regionmask-0.8.0/readthedocs.yml
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.937778 regionmask-0.8.0/regionmask/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      467 2021-09-06 06:33:50.000000 regionmask-0.8.0/regionmask/__init__.py
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.937778 regionmask-0.8.0/regionmask/core/
--rw-r--r--   0 mathause  (1000) mathause  (1000)        0 2019-10-05 07:31:56.000000 regionmask-0.8.0/regionmask/core/__init__.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     6168 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/core/_geopandas.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2252 2021-07-28 12:03:42.000000 regionmask-0.8.0/regionmask/core/formatting.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    16101 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/core/mask.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    12205 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/core/plot.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    13496 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/core/regions.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     5962 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/core/utils.py
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.937778 regionmask-0.8.0/regionmask/defined_regions/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      237 2021-08-09 14:58:44.000000 regionmask-0.8.0/regionmask/defined_regions/__init__.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1936 2021-07-28 12:03:42.000000 regionmask-0.8.0/regionmask/defined_regions/_ar6.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     4711 2021-07-28 12:03:42.000000 regionmask-0.8.0/regionmask/defined_regions/_ar6_pre_revisions.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      833 2021-07-28 12:03:42.000000 regionmask-0.8.0/regionmask/defined_regions/_ressources.py
--rw-r--r--   0 mathause  (1000) mathause  (1000)     2880 2020-04-06 15:04:44.000000 regionmask-0.8.0/regionmask/defined_regions/giorgi.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     8958 2021-07-28 12:03:42.000000 regionmask-0.8.0/regionmask/defined_regions/natural_earth.py
--rw-r--r--   0 mathause  (1000) mathause  (1000)     4797 2020-04-06 15:04:44.000000 regionmask-0.8.0/regionmask/defined_regions/srex.py
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.937778 regionmask-0.8.0/regionmask/tests/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      464 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/tests/__init__.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2583 2021-07-28 12:03:42.000000 regionmask-0.8.0/regionmask/tests/test_OneRegion.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     8619 2021-07-28 12:03:42.000000 regionmask-0.8.0/regionmask/tests/test_Regions.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2187 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/tests/test_defined_regions.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1610 2021-07-28 12:03:42.000000 regionmask-0.8.0/regionmask/tests/test_formatting.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    11006 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/tests/test_geopandas.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    24756 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/tests/test_mask.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1786 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/tests/test_mask_defined_regions.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)    21039 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/tests/test_plot.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      961 2021-07-28 12:03:42.000000 regionmask-0.8.0/regionmask/tests/test_save_utils.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     6168 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/tests/test_utils.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1703 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/tests/test_wrapAngle.py
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2674 2021-09-08 19:24:42.000000 regionmask-0.8.0/regionmask/tests/utils.py
-drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2021-09-08 19:48:10.937778 regionmask-0.8.0/regionmask.egg-info/
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1048 2021-09-08 19:48:10.000000 regionmask-0.8.0/regionmask.egg-info/PKG-INFO
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     2349 2021-09-08 19:48:10.000000 regionmask-0.8.0/regionmask.egg-info/SOURCES.txt
--rw-rw-r--   0 mathause  (1000) mathause  (1000)        1 2021-09-08 19:48:10.000000 regionmask-0.8.0/regionmask.egg-info/dependency_links.txt
--rw-rw-r--   0 mathause  (1000) mathause  (1000)        1 2021-09-08 19:48:10.000000 regionmask-0.8.0/regionmask.egg-info/not-zip-safe
--rw-rw-r--   0 mathause  (1000) mathause  (1000)       95 2021-09-08 19:48:10.000000 regionmask-0.8.0/regionmask.egg-info/requires.txt
--rw-rw-r--   0 mathause  (1000) mathause  (1000)       11 2021-09-08 19:48:10.000000 regionmask-0.8.0/regionmask.egg-info/top_level.txt
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      322 2021-09-06 06:33:50.000000 regionmask-0.8.0/requirements.txt
--rw-rw-r--   0 mathause  (1000) mathause  (1000)     1806 2021-09-08 19:48:10.937778 regionmask-0.8.0/setup.cfg
--rw-rw-r--   0 mathause  (1000) mathause  (1000)      103 2021-09-06 06:33:50.000000 regionmask-0.8.0/setup.py
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.278232 regionmask-0.9.0/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      190 2021-07-28 12:03:42.000000 regionmask-0.9.0/.codecov.yml
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)       24 2021-09-08 19:49:50.000000 regionmask-0.9.0/.git_archival.txt
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)       69 2021-09-08 19:49:50.000000 regionmask-0.9.0/.gitattributes
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.266231 regionmask-0.9.0/.github/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      212 2021-07-28 12:03:42.000000 regionmask-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.266231 regionmask-0.9.0/.github/workflows/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     3200 2022-02-07 14:09:21.000000 regionmask-0.9.0/.github/workflows/ci-additional.yaml
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2682 2022-02-07 14:09:21.000000 regionmask-0.9.0/.github/workflows/ci.yaml
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2340 2022-02-07 14:09:21.000000 regionmask-0.9.0/.github/workflows/linting.yaml
+-rw-r--r--   0 mathause  (1000) mathause  (1000)      431 2020-04-06 15:04:44.000000 regionmask-0.9.0/.gitignore
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     3263 2022-03-01 22:51:49.000000 regionmask-0.9.0/HOW_TO_RELEASE.md
+-rw-r--r--   0 mathause  (1000) mathause  (1000)     1070 2019-10-05 07:31:56.000000 regionmask-0.9.0/LICENSE
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1049 2022-03-02 20:58:31.278232 regionmask-0.9.0/PKG-INFO
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1363 2022-02-07 14:09:21.000000 regionmask-0.9.0/README.rst
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.266231 regionmask-0.9.0/ci/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     7010 2022-02-07 14:09:21.000000 regionmask-0.9.0/ci/min_deps_check.py
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.266231 regionmask-0.9.0/ci/requirements/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      695 2022-03-01 22:51:49.000000 regionmask-0.9.0/ci/requirements/docs.yml
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      282 2022-02-07 14:09:21.000000 regionmask-0.9.0/ci/requirements/environment.yml
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      254 2022-02-07 14:09:21.000000 regionmask-0.9.0/ci/requirements/py37-bare-minimum.yml
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      354 2022-02-07 14:09:21.000000 regionmask-0.9.0/ci/requirements/py37-min-all-deps.yml
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.270232 regionmask-0.9.0/data/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)   109303 2020-08-19 21:32:03.000000 regionmask-0.9.0/data/IPCC-WGI-reference-regions-v1.zip
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)   117037 2020-08-19 21:32:03.000000 regionmask-0.9.0/data/IPCC-WGI-reference-regions-v4.zip
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1227 2020-07-30 20:01:48.000000 regionmask-0.9.0/data/README.md
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1334 2021-07-28 12:03:42.000000 regionmask-0.9.0/data/regions_remote_catalog.yaml
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.270232 regionmask-0.9.0/docs/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)       99 2021-07-28 12:03:42.000000 regionmask-0.9.0/docs/.gitignore
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     7157 2022-02-09 23:06:56.000000 regionmask-0.9.0/docs/Makefile
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1116 2022-03-01 22:51:49.000000 regionmask-0.9.0/docs/README_ipynp_for_RTD
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1717 2022-03-01 23:21:57.000000 regionmask-0.9.0/docs/api.rst
+-rwxrwxr-x   0 mathause  (1000) mathause  (1000)      114 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/clean_notebooks
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     8047 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/conf.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1737 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/defined_countries.rst
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1115 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/defined_landmask.rst
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1444 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/defined_ocean_basins.rst
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     4340 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/defined_scientific.rst
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2625 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/index.rst
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1822 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/installation.rst
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2883 2022-01-19 22:59:39.000000 regionmask-0.9.0/docs/intake_regionmask.rst
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.274232 regionmask-0.9.0/docs/logo/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    15406 2021-07-28 12:03:42.000000 regionmask-0.9.0/docs/logo/favicon.ico
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     5192 2021-09-08 19:49:50.000000 regionmask-0.9.0/docs/logo/logo.ipynb
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    36492 2021-07-28 12:03:42.000000 regionmask-0.9.0/docs/logo/logo.png
+-rw-r--r--   0 mathause  (1000) mathause  (1000)     6709 2022-01-19 22:59:41.000000 regionmask-0.9.0/docs/make.bat
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.274232 regionmask-0.9.0/docs/notebooks/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     6733 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/notebooks/create_own_regions.ipynb
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     8595 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/notebooks/geopandas.ipynb
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    15863 2022-03-01 22:51:49.000000 regionmask-0.9.0/docs/notebooks/mask_2D.ipynb
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    14950 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/notebooks/mask_3D.ipynb
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    17585 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/notebooks/method.ipynb
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    10344 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/notebooks/overlap.ipynb
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     5143 2022-03-01 22:51:49.000000 regionmask-0.9.0/docs/notebooks/plotting.ipynb
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2125 2022-02-07 14:09:21.000000 regionmask-0.9.0/docs/notebooks/tutorial_rst.tpl
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    25106 2022-03-02 20:52:50.000000 regionmask-0.9.0/docs/whats_new.rst
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.274232 regionmask-0.9.0/licences/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    18658 2020-07-30 20:01:48.000000 regionmask-0.9.0/licences/AR6_REGIONS_LICENSE
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    10273 2020-07-30 20:01:48.000000 regionmask-0.9.0/licences/XARRAY_LICENSE
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      252 2022-02-07 14:09:21.000000 regionmask-0.9.0/pyproject.toml
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      195 2022-02-07 14:09:21.000000 regionmask-0.9.0/readthedocs.yml
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.274232 regionmask-0.9.0/regionmask/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      692 2022-02-11 10:43:21.000000 regionmask-0.9.0/regionmask/__init__.py
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.278232 regionmask-0.9.0/regionmask/core/
+-rw-r--r--   0 mathause  (1000) mathause  (1000)        0 2019-10-05 07:31:56.000000 regionmask-0.9.0/regionmask/core/__init__.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     7563 2022-03-01 23:21:57.000000 regionmask-0.9.0/regionmask/core/_geopandas.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2213 2022-03-01 23:21:57.000000 regionmask-0.9.0/regionmask/core/formatting.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    18823 2022-03-01 22:51:49.000000 regionmask-0.9.0/regionmask/core/mask.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    15061 2022-03-02 19:57:44.000000 regionmask-0.9.0/regionmask/core/plot.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    17438 2022-03-02 19:57:44.000000 regionmask-0.9.0/regionmask/core/regions.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     6265 2022-02-11 10:43:21.000000 regionmask-0.9.0/regionmask/core/utils.py
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.278232 regionmask-0.9.0/regionmask/defined_regions/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      298 2022-02-07 14:09:21.000000 regionmask-0.9.0/regionmask/defined_regions/__init__.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2029 2022-02-07 14:09:21.000000 regionmask-0.9.0/regionmask/defined_regions/_ar6.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     5150 2022-02-11 10:43:21.000000 regionmask-0.9.0/regionmask/defined_regions/_ar6_pre_revisions.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    13768 2022-03-02 19:57:44.000000 regionmask-0.9.0/regionmask/defined_regions/_natural_earth.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      833 2022-02-11 10:43:21.000000 regionmask-0.9.0/regionmask/defined_regions/_ressources.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2899 2022-02-07 14:09:21.000000 regionmask-0.9.0/regionmask/defined_regions/giorgi.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1586 2022-02-07 14:09:21.000000 regionmask-0.9.0/regionmask/defined_regions/prudence.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     4816 2022-02-07 14:09:21.000000 regionmask-0.9.0/regionmask/defined_regions/srex.py
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.278232 regionmask-0.9.0/regionmask/tests/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      964 2022-03-01 22:51:49.000000 regionmask-0.9.0/regionmask/tests/__init__.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2439 2022-03-01 22:51:49.000000 regionmask-0.9.0/regionmask/tests/test_OneRegion.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    11249 2022-03-01 23:21:57.000000 regionmask-0.9.0/regionmask/tests/test_Regions.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     5556 2022-02-11 10:43:21.000000 regionmask-0.9.0/regionmask/tests/test_create_dataarray.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     3966 2022-02-07 14:09:21.000000 regionmask-0.9.0/regionmask/tests/test_defined_regions.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1693 2022-02-07 14:09:21.000000 regionmask-0.9.0/regionmask/tests/test_formatting.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    11369 2022-03-01 23:21:57.000000 regionmask-0.9.0/regionmask/tests/test_geopandas.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    25149 2022-03-01 22:51:49.000000 regionmask-0.9.0/regionmask/tests/test_mask.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1501 2022-02-07 14:09:21.000000 regionmask-0.9.0/regionmask/tests/test_mask_defined_regions.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)    23431 2022-03-01 22:51:49.000000 regionmask-0.9.0/regionmask/tests/test_plot.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2681 2022-03-01 22:51:49.000000 regionmask-0.9.0/regionmask/tests/test_segmentize.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     8650 2022-02-07 14:09:21.000000 regionmask-0.9.0/regionmask/tests/test_utils.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1703 2021-09-08 19:49:50.000000 regionmask-0.9.0/regionmask/tests/test_wrapAngle.py
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     5096 2022-03-01 22:51:49.000000 regionmask-0.9.0/regionmask/tests/utils.py
+drwxrwxr-x   0 mathause  (1000) mathause  (1000)        0 2022-03-02 20:58:31.274232 regionmask-0.9.0/regionmask.egg-info/
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1049 2022-03-02 20:58:31.000000 regionmask-0.9.0/regionmask.egg-info/PKG-INFO
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     2460 2022-03-02 20:58:31.000000 regionmask-0.9.0/regionmask.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)        1 2022-03-02 20:58:31.000000 regionmask-0.9.0/regionmask.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)        1 2022-03-02 20:58:31.000000 regionmask-0.9.0/regionmask.egg-info/not-zip-safe
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      111 2022-03-02 20:58:31.000000 regionmask-0.9.0/regionmask.egg-info/requires.txt
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)       11 2022-03-02 20:58:31.000000 regionmask-0.9.0/regionmask.egg-info/top_level.txt
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      340 2022-02-07 14:09:21.000000 regionmask-0.9.0/requirements.txt
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)     1826 2022-03-02 20:58:31.278232 regionmask-0.9.0/setup.cfg
+-rw-rw-r--   0 mathause  (1000) mathause  (1000)      103 2021-09-08 19:49:50.000000 regionmask-0.9.0/setup.py
```

### Comparing `regionmask-0.8.0/.github/workflows/ci-additional.yaml` & `regionmask-0.9.0/.github/workflows/ci-additional.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -3,59 +3,66 @@
   push:
     branches:
       - "*"
   pull_request:
     branches:
       - "*"
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   test:
-    name: ${{ matrix.env }}
+    name: py${{ matrix.python-version }}-${{ matrix.env }}
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"]
         env:
           [
-            "py36-bare-minimum",
-            "py36-min-all-deps",
+            "bare-minimum",
+            "min-all-deps",
           ]
+        python-version: ["3.7"]
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0 # Fetch all history for all branches and tags.
 
       - name: Set environment variables
         run: |
-            echo "CONDA_ENV_FILE=ci/requirements/${{ matrix.env }}.yml" >> $GITHUB_ENV
+            PY=${{ matrix.python-version }}
+            # replace "." in matrix.python-version
+            PY=${PY//./}
+            echo "CONDA_ENV_FILE=ci/requirements/py${PY}-${{ matrix.env }}.yml" >> $GITHUB_ENV
       - name: Cache conda
         uses: actions/cache@v2
         with:
           path: |
             ~/conda_pkgs_dir
             ~/.cache/regionmask/
-            ~/.local/share/cartopy/
           key:
-            ${{ runner.os }}-conda-${{ matrix.env }}-${{ hashFiles('ci/requirements/**.yml') }}
+            ${{ runner.os }}-conda-py${{ matrix.python-version }}-${{ matrix.env }}-${{ hashFiles('ci/requirements/**.yml') }}
           restore-keys: |
-            ${{ runner.os }}-conda-${{ matrix.env }}
+            ${{ runner.os }}-conda-py${{ matrix.python-version }}-
             ${{ runner.os }}-
 
       - uses: conda-incubator/setup-miniconda@v2
         with:
           channels: conda-forge
           channel-priority: strict
           mamba-version: "*"
           activate-environment: regionmask-tests
           auto-update-conda: false
-          python-version: 3.6
+          python-version: ${{ matrix.python-version }}
           use-only-tar-bz2: true
 
       - name: Install conda dependencies
         run: |
           mamba env update -f $CONDA_ENV_FILE
 
       - name: Install regionmask
@@ -66,22 +73,22 @@
         run: |
           conda info -a
           conda list
       - name: Import regionmask
         run: |
           python -c "import regionmask"
       - name: Run tests
-        timeout-minutes: 5
+        timeout-minutes: 15
         run: python -u -m pytest
           --cov=regionmask
           --cov-report=xml
           $PYTEST_EXTRA_FLAGS
 
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v1
+        uses: codecov/codecov-action@v2
         with:
           file: ./coverage.xml
           flags: unittests,${{ matrix.env }}
           env_vars: RUNNER_OS
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -102,8 +109,8 @@
           mamba-version: "*"
           auto-update-conda: false
           python-version: "3.8"
 
       - name: minimum versions policy
         run: |
           mamba install -y pyyaml conda python-dateutil
-          python ci/min_deps_check.py ci/requirements/py36-min-all-deps.yml
+          python ci/min_deps_check.py ci/requirements/py37-min-all-deps.yml
```

### Comparing `regionmask-0.8.0/.github/workflows/ci.yaml` & `regionmask-0.9.0/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,31 @@
   push:
     branches:
       - "*"
   pull_request:
     branches:
       - "*"
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   test:
     name: py${{ matrix.python-version }}
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"]
         # Bookend python versions
-        python-version: ["3.7", "3.8", "3.9"]
+        python-version: ["3.7", "3.8", "3.9", "3.10"]
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0 # Fetch all history for all branches and tags.
       - name: Set environment variables
         run: |
           echo "CONDA_ENV_FILE=ci/requirements/environment.yml" >> $GITHUB_ENV
@@ -31,18 +35,17 @@
 
       - name: Cache conda
         uses: actions/cache@v2
         with:
           path: |
             ~/conda_pkgs_dir
             ~/.cache/regionmask/
-            ~/.local/share/cartopy/
           key: ${{ runner.os }}-conda-py${{ matrix.python-version }}-${{ hashFiles('ci/requirements/**.yml') }}
           restore-keys: |
-            ${{ runner.os }}-conda-${{ matrix.python-version }}-
+            ${{ runner.os }}-conda-py${{ matrix.python-version }}-
             ${{ runner.os }}-
       - uses: conda-incubator/setup-miniconda@v2
         with:
           channels: conda-forge
           channel-priority: strict
           mamba-version: "*"
           activate-environment: regionmask-tests
@@ -76,14 +79,14 @@
         if: always()
         uses: actions/upload-artifact@v2
         with:
           name: Test results for ${{ runner.os }}-${{ matrix.python-version }}
           path: test-results/${{ runner.os }}-${{ matrix.python-version }}.xml
 
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v1
+        uses: codecov/codecov-action@v2
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS,PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `regionmask-0.8.0/.github/workflows/linting.yaml` & `regionmask-0.9.0/.github/workflows/linting.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,18 @@
   push:
     branches:
       - "*"
   pull_request:
     branches:
       - "*"
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   test:
     name: linting
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash -l {0}
@@ -29,16 +33,18 @@
           echo "CONDA_ENV_FILE=ci/requirements/environment.yml" >> $GITHUB_ENV
           echo "PYTHON_VERSION=${{ matrix.python-version }}" >> $GITHUB_ENV
 
       - name: Cache conda
         uses: actions/cache@v2
         with:
           path: ~/conda_pkgs_dir
-          key: ${{ runner.os }}-conda-py${{ matrix.python-version }}-${{
-            hashFiles('ci/requirements/**.yml') }}
+          key: ${{ runner.os }}-conda-py${{ matrix.python-version }}-${{ hashFiles('ci/requirements/**.yml') }}
+          restore-keys: |
+            ${{ runner.os }}-conda-py${{ matrix.python-version }}-
+            ${{ runner.os }}-
       - uses: conda-incubator/setup-miniconda@v2
         with:
           channels: conda-forge
           channel-priority: strict
           mamba-version: "*"
           activate-environment: regionmask-tests
           auto-update-conda: false
```

### Comparing `regionmask-0.8.0/HOW_TO_RELEASE.md` & `regionmask-0.9.0/HOW_TO_RELEASE.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
      ```sh
      git switch master
      git pull upstream master
      ```
  2. Maybe write a release summary: ~50 words describing the high level features.
  3. Look over whats-new.rst and the docs. Make sure "What's New" is complete
     (check the date!) and add the release summary at the top.
- 4. Open a PR with the release summary and whatsnew changes.
+ 4. Open a PR with the release summary and what's new changes.
  5. After merging, again ensure your master branch is synced to upstream:
      ```sh
      git pull upstream master
      ```
  7. Check that the tests and ReadTheDocs build is passing!
  8. Tag the release (remove the curly braces):
       ```sh
@@ -29,14 +29,17 @@
       ```sh
       mamba update pip
       python -m pip install setuptools setuptools-scm wheel twine check-manifest
       ```
 10. Build source and binary wheels for PyPI:
       ```sh
       git clean -xdfn  # This removes any untracked files! - Dry run -
+      ```
+      For real
+      ```sh
       git clean -xdf  # This removes any untracked files!
       git status # check for tracked files
       git restore -SW .  # This removes any tracked changes!
       python setup.py bdist_wheel sdist
       ```
 11. Use twine to check the package build:
       ```sh
@@ -50,23 +53,15 @@
     You will need to be listed as a package owner at
     <https://pypi.python.org/pypi/regionmask> for this to work.
 13. Push your changes to master:
       ```sh
       git push upstream master
       git push upstream --tags
       ```
-14. Update the stable branch (used by ReadTheDocs) and switch back to master:
-     ```sh
-      git switch stable
-      git rebase master
-      git push --force upstream stable
-      git switch master
-     ```
-    It's OK to force push to `stable` if necessary.
-15. Add a section for the next release {0.X.Y+1} to doc/whats-new.rst:
+14. Add a section for the next release {0.X.Y+1} to doc/whats-new.rst:
      ```rst
      .. _whats-new.{0.X.Y+1}:
 
      v{0.X.Y+1} (unreleased)
      ---------------------
 
      Breaking Changes
@@ -87,23 +82,24 @@
      Docs
      ~~~~
 
      Internal Changes
      ~~~~~~~~~~~~~~~~
 
      ```
-16. Commit your changes and push to master again:
+15. Commit your changes and push to master again:
       ```sh
       git commit -am 'New whatsnew section'
       git push upstream master
       ```
     You're done pushing to master!
-17. Issue the release on GitHub. Click on "Draft a new release" at
+16. Issue the release on GitHub. Click on "Draft a new release" at
     <https://github.com/regionmask/regionmask/releases>. Type in the version number
     and paste the release summary in the notes.
+17. Update zenodo link.
 18. Update the docs. Login to <https://readthedocs.org/projects/regionmask/versions/>
     and switch your new release tag (at the bottom) from "Inactive" to "Active".
     It should now build automatically.
 19. Release regionmask on conda - also update the requirements in meta.yaml <https://github.com/conda-forge/regionmask-feedstock>
 
 <!-- markdownlint-enable MD013 -->
```

### Comparing `regionmask-0.8.0/LICENSE` & `regionmask-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/PKG-INFO` & `regionmask-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: regionmask
-Version: 0.8.0
+Version: 0.9.0
 Summary: plotting and creation of masks for spatial regions
 Home-page: https://github.com/regionmask/regionmask
 Author: regionmask Developers
 Author-email: mathias.hauser@env.ethz.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 See https://regionmask.readthedocs.io
```

### Comparing `regionmask-0.8.0/README.rst` & `regionmask-0.9.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,19 @@
    :target: https://regionmask.readthedocs.io
 .. image:: https://img.shields.io/pypi/v/regionmask.svg
    :target: https://pypi.python.org/pypi/regionmask/
 .. image:: https://anaconda.org/conda-forge/regionmask/badges/installer/conda.svg
    :target: https://conda.anaconda.org/conda-forge
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/ambv/black
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3585543.svg
-   :target: https://doi.org/10.5281/zenodo.3585543
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5532848.svg
+   :target: https://doi.org/10.5281/zenodo.5532848
 
+Create *masks* of geographical *regions* for arbitrary longitude and latitude grids.
 
 Documentation
 -------------
-See the `documentation <http://regionmask.readthedocs.io/>`_  (on readthedocs).
+See the `documentation <http://regionmask.readthedocs.io/>`_ (on readthedocs).
+
+License
+-------
+regionmask is published under a MIT license.
```

### Comparing `regionmask-0.8.0/ci/min_deps_check.py` & `regionmask-0.9.0/ci/min_deps_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,14 @@
     # The conda metadata is malformed for setuptools < 38.4 (Jan 2018)
     # (it's missing a timestamp which prevents this tool from working).
     # setuptools < 40.4 (Sep 2018) from conda-forge cannot be installed into a py37
     # environment
     # TODO remove this special case and the matching note in installing.rst
     #      after March 2022.
     "setuptools": (40, 4),
-    # cannot install pygeos=0.7 alongside shapely
-    "pygeos": (0, 9),
 }
 has_errors = False
 
 
 def error(msg: str) -> None:
     global has_errors
     has_errors = True
```

### Comparing `regionmask-0.8.0/ci/requirements/docs.yml` & `regionmask-0.9.0/ci/requirements/docs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 channels:
   - conda-forge
   - nodefaults
 
 dependencies:
   - python
 # regionmask dependencies
-  # https://github.com/SciTools/cartopy/pull/1646
-  - cartopy=0.19
+  - cartopy
   - geopandas
-  # related to the cartopy issue
-  - matplotlib-base=3.4
+  - matplotlib-base
   - numpy
   - pooch
+  - packaging
   - pygeos
   - rasterio
   - xarray
-# depencies for the examples
+# dependencies for the examples
   - cftime
   - netcdf4
 # for regionmask intake example
   - aiohttp
   - fsspec==0.8.7
   - intake
   - requests
 # dependencies to build the docu
-  # https://github.com/readthedocs/sphinx_rtd_theme/issues/1115
-  - docutils==0.16
+  - docutils
   - ipykernel
   - nbconvert
   - numpydoc
   - pillow
   - pip
   - sphinx_rtd_theme
   - sphinx
```

### Comparing `regionmask-0.8.0/data/IPCC-WGI-reference-regions-v1.zip` & `regionmask-0.9.0/data/IPCC-WGI-reference-regions-v1.zip`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/data/IPCC-WGI-reference-regions-v4.zip` & `regionmask-0.9.0/data/IPCC-WGI-reference-regions-v4.zip`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/data/README.md` & `regionmask-0.9.0/data/README.md`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/data/regions_remote_catalog.yaml` & `regionmask-0.9.0/data/regions_remote_catalog.yaml`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/docs/Makefile` & `regionmask-0.9.0/docs/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 	rm -rf $(BUILDDIR)/*
 
 html: 	# ${TUTORIALS}
 	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) $(BUILDDIR)/html
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
 
-dirhtml: 
+dirhtml:
 	$(SPHINXBUILD) -b dirhtml $(ALLSPHINXOPTS) $(BUILDDIR)/dirhtml
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/dirhtml."
 
 singlehtml:
 	$(SPHINXBUILD) -b singlehtml $(ALLSPHINXOPTS) $(BUILDDIR)/singlehtml
 	@echo
```

### Comparing `regionmask-0.8.0/docs/README_ipynp_for_RTD` & `regionmask-0.9.0/docs/README_ipynp_for_RTD`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 Create iPython Notebooks to use ase tutorials for documenting things.
 This is very handy...
 
-Stolen from: 
+Stolen from:
 http://sphinx-ipynb.readthedocs.io/en/latest/howto.html
 https://github.com/dfm/george/tree/1.0-dev
 
 The idea is to automatically invoke `ipython nbconvert` to convert the .ipynb to .rst.
 Therefore changes to the Makefile have to be made.
 
 NOTE: The ipynb need at least one markdown field with a #Title!
@@ -16,18 +16,18 @@
 template: ./tutorial/tutorial_rst.tpl
 target directory of the .rst file: ./tutorial/
 
 Changes to Makefile
 # define targets
 TUTORIALS = tutorials/plotting.rst tutorials/mask_numpy.rst tutorials/mask_xarray.rst
 
-# recipie to create targets
+# recipe to create targets
 tutorials/%.rst: _static/notebooks/%.ipynb
         cd tutorials;ipython nbconvert --template tutorial_rst --to rst ../$<
 
 # add `${TUTORIALS}` to the documentation you want to create.
 
 # probably readthedocs executes `dirhtml`
 dirhtml: ${TUTORIALS}
         $(SPHINXBUILD) -b dirhtml $(ALLSPHINXOPTS) $(BUILDDIR)/dirhtml
         @echo
-        @echo "Build finished. The HTML pages are in $(BUILDDIR)/dirhtml."
+        @echo "Build finished. The HTML pages are in $(BUILDDIR)/dirhtml."
```

### Comparing `regionmask-0.8.0/docs/api.rst` & `regionmask-0.9.0/docs/api.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .. currentmodule:: regionmask
 
-#############
 API reference
 #############
 
 This page provides an auto-generated summary of regionmask's API.
 
 
 Top-level functions
@@ -62,14 +61,25 @@
 
 .. autosummary::
    :toctree: generated/
 
    Regions.mask
    Regions.mask_3D
 
+Conversion
+----------
+
+.. autosummary::
+   :toctree: generated/
+
+   Regions.to_dataframe
+   Regions.to_geodataframe
+   Regions.to_geoseries
+   Regions.from_geodataframe
+
 
 Attributes
 ----------
 
 .. autosummary::
    :toctree: generated/
 
@@ -80,16 +90,14 @@
    Regions.coords
    Regions.polygons
    Regions.centroids
    Regions.bounds
    Regions.bounds_global
    Regions.lon_180
    Regions.lon_360
-   Regions._is_polygon
-
 
 _OneRegion
 ==========
 
 
 Creating one Region
 -------------------
```

### Comparing `regionmask-0.8.0/docs/conf.py` & `regionmask-0.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,15 @@
 
 notebooks = (
     "notebooks/method",
     "notebooks/plotting",
     "notebooks/mask_2D",
     "notebooks/mask_3D",
     "notebooks/geopandas",
+    "notebooks/overlap",
     "notebooks/create_own_regions",
 )
 
 print("\nBuilding notebooks:")
 for nb in notebooks:
 
     # only render notebooks if necessary
```

### Comparing `regionmask-0.8.0/docs/defined_countries.rst` & `regionmask-0.9.0/docs/defined_ocean_basins.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,61 @@
-################################
-Countries/ States (NaturalEarth)
-################################
+Marine Areas/ Ocean Basins (NaturalEarth)
+#########################################
 
-The outline of the countries are obtained from
+The outline of the marine areas are obtained from
 `Natural Earth <http://www.naturalearthdata.com/>`_.
-They are automatically downloaded on-the-fly (but only once) with cartopy and opened with geopandas.
-The following countries and regions are defined in regionmask.
+They are automatically downloaded, cached and opened with geopandas.
+The following marine regions are defined in regionmask:
 
-* Countries 1:110m
-* Countries 1:50m
-* US States 1:50m
-* US States 1:10m
-
-.. note::
-   A mask obtained with a fine resolution dataset is not necessarily better.
-   Always check your mask!
+* Marine Areas 1:50m
+
+
+.. warning::
+   ``regionmask.defined_regions.natural_earth`` is deprecated.
+   Please use ``natural_earth_v4_1_0`` or ``natural_earth_v5_0_0`` instead.
+
+   Be careful when working with the different versions of NaturalEarth regions. Some
+   polygons and regions have changed and the numbering of the regions may be different.
 
 .. ipython:: python
     :suppress:
 
-    # Use defaults so we don't get gridlines in generated docs
     import matplotlib as mpl
-    mpl.rcdefaults()
-    mpl.use('Agg')
 
     # cut border when saving (for maps)
     mpl.rcParams["savefig.bbox"] = "tight"
 
-The following imports are necessary for the examples.
+Import regionmask:
 
 .. ipython:: python
 
     import regionmask
-    import matplotlib.pyplot as plt
 
-Countries
-=========
+Ocean Basins
+============
 
 .. ipython:: python
 
-    regionmask.defined_regions.natural_earth.countries_110.plot(add_label=False);
-
-    @savefig plotting_countries.png width=100%
-    plt.tight_layout()
-
-US States
-=========
+    basins = regionmask.defined_regions.natural_earth_v5_0_0.ocean_basins_50
+    basins
 
 .. ipython:: python
 
-    states = regionmask.defined_regions.natural_earth.us_states_50
-
-    states.plot(add_label=False);
+    @savefig plotting_basins.png width=100%
+    basins.plot(add_label=False);
 
-    @savefig plotting_states.png width=100%
-    plt.tight_layout()
-
-Also create a mask for a 1° grid over the US:
+Also create a mask for a 1° grid globally:
 
 .. ipython:: python
 
     import numpy as np
 
     # create a grid
-    lon = np.arange(200.5, 325)
-    lat = np.arange(74.5, 14, -1)
-
-    mask = states.mask(lon, lat)
+    lon = np.arange(0.5, 360)
+    lat = np.arange(89.5, -90, -1)
 
-    states.plot(add_label=False);
-    mask.plot(add_colorbar=False)
+    mask = basins.mask(lon, lat)
 
-    @savefig plotting_states_mask.png width=100%
-    plt.tight_layout()
+    basins.plot(add_label=False);
 
+    @savefig plotting_basins_mask.png width=100%
+    mask.plot(add_colorbar=False);
```

### Comparing `regionmask-0.8.0/docs/defined_ocean_basins.rst` & `regionmask-0.9.0/docs/defined_countries.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,72 @@
-#########################################
-Marine Areas/ Ocean Basins (NaturalEarth)
-#########################################
+Countries/ States (NaturalEarth)
+################################
 
-The outline of the marine areas are obtained from
+The outline of the countries are obtained from
 `Natural Earth <http://www.naturalearthdata.com/>`_.
-They are automatically downloaded on-the-fly (but only once) with cartopy and opened with geopandas.
-The following marine regions are defined in regionmask:
+They are automatically downloaded, cached and opened with geopandas.
+The following countries and regions are defined in regionmask.
 
-* Marine Areas 1:50m
+* Countries 1:110m
+* Countries 1:50m
+* US States 1:50m
+* US States 1:10m
+
+.. warning::
+   ``regionmask.defined_regions.natural_earth`` is deprecated.
+   Please use ``natural_earth_v4_1_0`` or ``natural_earth_v5_0_0`` instead.
+
+   Be careful when working with the different versions of NaturalEarth regions. Some
+   polygons and regions have changed and the numbering of the regions may be different.
+
+.. note::
+   A mask obtained with a fine resolution dataset is not necessarily better.
+   Always check your mask!
 
 .. ipython:: python
     :suppress:
 
-    # Use defaults so we don't get gridlines in generated docs
     import matplotlib as mpl
-    mpl.rcdefaults()
-    mpl.use('Agg')
 
     # cut border when saving (for maps)
     mpl.rcParams["savefig.bbox"] = "tight"
 
-The following imports are necessary for the examples.
+Import regionmask:
 
 .. ipython:: python
 
     import regionmask
-    import matplotlib.pyplot as plt
 
-Ocean Basins
-============
+Countries
+=========
 
 .. ipython:: python
 
-    basins = regionmask.defined_regions.natural_earth.ocean_basins_50
+    @savefig plotting_countries.png width=100%
+    regionmask.defined_regions.natural_earth_v5_0_0.countries_110.plot(add_label=False);
 
-    basins.plot(add_label=False);
+US States
+=========
 
-    @savefig plotting_basins.png width=100%
-    plt.tight_layout()
+.. ipython:: python
 
-Also create a mask for a 1° grid globally:
+    states = regionmask.defined_regions.natural_earth_v5_0_0.us_states_50
 
-.. ipython:: python
+    @savefig plotting_states.png width=100%
+    states.plot(add_label=False);
 
-    import numpy as np
 
-    # create a grid
-    lon = np.arange(0.5, 360)
-    lat = np.arange(89.5, -90, -1)
+Also create a mask for a 1° grid over the US:
 
-    mask = basins.mask(lon, lat)
+.. ipython:: python
 
-    basins.plot(add_label=False, add_ocean=False);
+    import numpy as np
 
-     # plot using xarray
-     mask.plot(add_colorbar=False);
+    # create a grid
+    lon = np.arange(200.5, 325)
+    lat = np.arange(74.5, 14, -1)
 
-    @savefig plotting_basins_mask.png width=100%
-    plt.tight_layout()
+    mask = states.mask(lon, lat)
 
+    states.plot(add_label=False);
+    @savefig plotting_states_mask.png width=100%
+    mask.plot(add_colorbar=False)
```

### Comparing `regionmask-0.8.0/docs/installation.rst` & `regionmask-0.9.0/docs/installation.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Installation
 ============
 
 Required dependencies
 ---------------------
 
-- Python (3.6 or later)
-- `geopandas <http://geopandas.org/>`__ (0.6 or later)
+- Python (3.7 or later)
+- `geopandas <http://geopandas.org/>`__ (0.7 or later)
 - `numpy <http://www.numpy.org/>`__ (1.17 or later)
-- `pooch <https://www.fatiando.org/pooch/latest/>`__ (1.0 or later)
-- `rasterio <https://rasterio.readthedocs.io/>`__ (1.0 or later)
-- `shapely <http://toblerity.org/shapely/>`__ (1.6 or later)
+- `packaging <https://packaging.pypa.io/en/latest/>`__ (20.0 or later)
+- `pooch <https://www.fatiando.org/pooch/latest/>`__ (1.2 or later)
+- `rasterio <https://rasterio.readthedocs.io/>`__ (1.1 or later)
+- `shapely <http://toblerity.org/shapely/>`__ (1.7 or later)
 - `xarray <http://xarray.pydata.org/>`__ (0.15 or later)
 
 Optional dependencies
 ---------------------
 
 For plotting
 ~~~~~~~~~~~~
 
-- `matplotlib <http://matplotlib.org/>`__ is required to create any plots.
-- `cartopy <http://scitools.org.uk/cartopy/>`__ for plotting on geographical maps and
-  for downloading natural earth data.
+- `matplotlib <http://matplotlib.org/>`__ (3.2 or later) is required to create any plots.
+- `cartopy <http://scitools.org.uk/cartopy/>`__ (0.17 or later) for plotting on
+  geographical maps.
 
 For faster masking
 ~~~~~~~~~~~~~~~~~~
 
-- `pygeos <https://pygeos.readthedocs.io/en/stable/>`__ enables faster mask creations for
+- `pygeos <https://pygeos.readthedocs.io/en/stable/>`__ (0.9 or later) enables faster mask creations for
   irregular and 2D grids.
 
 Instructions
 ------------
 
 regionmask itself is a pure Python package, but its dependencies are not. The
 easiest way to get them installed is to use conda_. The package is available
```

### Comparing `regionmask-0.8.0/docs/intake_regionmask.rst` & `regionmask-0.9.0/docs/intake_regionmask.rst`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/docs/logo/favicon.ico` & `regionmask-0.9.0/docs/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/docs/logo/logo.ipynb` & `regionmask-0.9.0/docs/logo/logo.ipynb`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/docs/logo/logo.png` & `regionmask-0.9.0/docs/logo/logo.png`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/docs/make.bat` & `regionmask-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/docs/notebooks/create_own_regions.ipynb` & `regionmask-0.9.0/docs/notebooks/create_own_regions.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745126382876382%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(0, 'import cartopy.crs as ccrs\\n'), (1, 'import numpy as "*

 * *            "np\\n'), (2, 'import matplotlib.pyplot as plt\\n'), (3, '\\n')]}}, 11: {'source': "*

 * *            "{delete: [3, 2, 1]}}, 13: {'source': {delete: [8, 7, 6, 5]}}, 14: {'source': {insert: "*

 * *            '[(2, \'h = mask.plot(\\n\'), (4, \'    cmap="Paired",\\n\'), (5, \'    '*

 * *            "add_colorbar=False,\\n'), (6, '    vmax=12,\\n')], delete: [12, 10, 9, 8, 7, 5, 4, 3, "*

 * *            "1, 0]}}, 15: {' […]*

```diff
@@ -26,59 +26,40 @@
                 "# Create your own region"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "% comment: leave next cell as RawNBConvert -> else the warning mesage is not correctly displayed"
-            ]
-        },
-        {
-            "cell_type": "raw",
-            "metadata": {},
-            "source": [
-                ".. note:: In version 0.5 the ``Regions_cls`` has been renamed to ``Regions`` and it's call signature has changed. All arguments (except ``outlines``) are now optional."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "Creating own regions is straightforward. Import regionmask and check the version:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import cartopy.crs as ccrs\n",
+                "import numpy as np\n",
+                "import matplotlib.pyplot as plt\n",
+                "\n",
                 "import regionmask\n",
                 "\n",
                 "regionmask.__version__"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Import numpy"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import numpy as np"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Assume you have two custom regions in the US, you can easily use these to create `Regions`:"
             ]
         },
         {
@@ -90,14 +71,21 @@
                 "US1 = np.array([[-100.0, 30], [-100, 40], [-120, 35]])\n",
                 "US2 = np.array([[-100.0, 30], [-80, 30], [-80, 40], [-100, 40]])\n",
                 "\n",
                 "regionmask.Regions([US1, US2])"
             ]
         },
         {
+            "cell_type": "raw",
+            "metadata": {},
+            "source": [
+                ".. note:: Set ``overlap=True`` if some of the regions overlap. See the tutorial on :doc:`overlapping regions<overlap>` for details."
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If you want to set the `names` and `abbrevs` yourself you can still do that:"
             ]
         },
         {
@@ -124,17 +112,14 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ax = USregions.plot(label=\"abbrev\")\n",
                 "\n",
-                "# load cartopy\n",
-                "import cartopy.crs as ccrs\n",
-                "\n",
                 "# fine tune the extent\n",
                 "ax.set_extent([225, 300, 25, 45], crs=ccrs.PlateCarree())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -150,40 +135,30 @@
             "source": [
                 "import numpy as np\n",
                 "\n",
                 "# define lat/ lon grid\n",
                 "lon = np.arange(200.5, 330, 1)\n",
                 "lat = np.arange(74.5, 15, -1)\n",
                 "\n",
-                "# for the plotting\n",
-                "lon_edges = np.arange(200, 331, 1)\n",
-                "lat_edges = np.arange(75, 14, -1)\n",
-                "\n",
                 "mask = USregions.mask(lon, lat)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import matplotlib.pyplot as plt\n",
-                "\n",
                 "ax = plt.subplot(111, projection=ccrs.PlateCarree())\n",
                 "\n",
-                "# pcolormesh does not handle NaNs, requires masked array\n",
-                "mask_ma = np.ma.masked_invalid(mask)\n",
-                "\n",
-                "h = ax.pcolormesh(\n",
-                "    lon_edges,\n",
-                "    lat_edges,\n",
-                "    mask_ma,\n",
+                "h = mask.plot(\n",
                 "    transform=ccrs.PlateCarree(),\n",
-                "    cmap=\"viridis\",\n",
+                "    cmap=\"Paired\",\n",
+                "    add_colorbar=False,\n",
+                "    vmax=12,\n",
                 ")\n",
                 "\n",
                 "ax.coastlines()\n",
                 "\n",
                 "# add the outlines of the regions\n",
                 "USregions.plot_regions(ax=ax, add_label=False)\n",
                 "\n",
@@ -192,15 +167,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Use shapely Polygon\n",
                 "\n",
-                "If you have the region defined as a shapely polygon, this also works:"
+                "You can also define the region with shapely polygons (see [geopandas tutorial](geopandas.html) how to work with shapefiles)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -302,33 +277,36 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ax = plt.subplot(111, projection=ccrs.PlateCarree())\n",
                 "\n",
                 "mask.plot(transform=ccrs.PlateCarree(), add_colorbar=False)\n",
                 "\n",
-                "ax.coastlines();"
+                "ax.coastlines()\n",
+                "\n",
+                "# fine tune the extent\n",
+                "ax.set_extent([225, 300, 25, 45], crs=ccrs.PlateCarree())"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.6"
+            "version": "3.10.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `regionmask-0.8.0/docs/notebooks/geopandas.ipynb` & `regionmask-0.9.0/docs/notebooks/geopandas.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.987832079614487%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, 'regionmask includes support for regions defined as "*

 * *            'geopandas GeoDataFrame. These are often shapefiles, which can be opened in the '*

 * *            'formats `.zip`, `.shp`, `.geojson` etc. with '*

 * *            "`geopandas.read_file(url_or_path).`\\n')], delete: [0]}}, 3: {'source': {insert: [(3, "*

 * *            "'import matplotlib.patheffects as pe\\n')]}}, 21: {'source': ['text_kws = dict(\\n', "*

 * *            '\'    bbox=dict(color="none"),\\n\', \'    path_ […]*

```diff
@@ -32,15 +32,15 @@
                 "# Working with geopandas (shapefiles)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "regionmask includes support for regions defined as geopandas GeoDataFrame. These are often shapefiles, which can be opened in the formats `.zip` or `.shp` with `geopandas.read_file(url_or_path).`\n",
+                "regionmask includes support for regions defined as geopandas GeoDataFrame. These are often shapefiles, which can be opened in the formats `.zip`, `.shp`, `.geojson` etc. with `geopandas.read_file(url_or_path).`\n",
                 "\n",
                 "There are two possibilities:\n",
                 "\n",
                 "1. Directly create a mask from a geopandas GeoDataFrame or GeoSeries using `mask_geopandas` or `mask_3D_geopandas`. \n",
                 "2. Convert a GeoDataFrame to a `Regions` object (regionmask's internal data container) using `from_geopandas`.\n",
                 "\n",
                 "As always, start with the imports:"
@@ -51,14 +51,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import cartopy.crs as ccrs\n",
                 "import geopandas as gp\n",
                 "import matplotlib.pyplot as plt\n",
+                "import matplotlib.patheffects as pe\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import pooch\n",
                 "\n",
                 "import regionmask\n",
                 "\n",
                 "regionmask.__version__"
@@ -174,14 +175,21 @@
                 "    cmap=cmap1,\n",
                 ")\n",
                 "\n",
                 "ax.coastlines(color=\"0.1\");"
             ]
         },
         {
+            "cell_type": "raw",
+            "metadata": {},
+            "source": [
+                ".. note:: Set ``regionmask.mask_3D_geopandas(..., overlap=True)`` if some of the regions overlap. See the tutorial on :doc:`overlapping regions<overlap>` for details."
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 2. Convert GeoDataFrame to a Regions object\n",
                 "\n",
                 "Creating a `Regions` object with `regionmask.from_geopandas` requires a GeoDataFrame:"
             ]
@@ -214,27 +222,41 @@
                 "continents_regions = regionmask.from_geopandas(\n",
                 "    continents, names=\"CONTINENT\", abbrevs=\"_from_name\", name=\"continent\"\n",
                 ")\n",
                 "continents_regions"
             ]
         },
         {
+            "cell_type": "raw",
+            "metadata": {},
+            "source": [
+                ".. note:: Set ``overlap=True`` if some of the regions overlap. See the tutorial on :doc:`overlapping regions<overlap>` for details."
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As usual the newly created `Regions` object can be plotted on a world map:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "continents_regions.plot(label=\"name\", add_coastlines=False);"
+                "text_kws = dict(\n",
+                "    bbox=dict(color=\"none\"),\n",
+                "    path_effects=[pe.withStroke(linewidth=2, foreground=\"w\")],\n",
+                "    color=\"#67000d\",\n",
+                "    fontsize=9,\n",
+                ")\n",
+                "\n",
+                "continents_regions.plot(label=\"name\", add_coastlines=False, text_kws=text_kws);"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "And to create mask a mask for arbitrary latitude/ longitude grids:"
@@ -305,13 +327,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.10.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `regionmask-0.8.0/docs/notebooks/mask_2D.ipynb` & `regionmask-0.9.0/docs/notebooks/mask_2D.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9938523884396526%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(1, '   2D masks are good for plotting. However, to "*

 * *            'calculate weighted regional averages 3D boolean masks are more convenient. See the '*

 * *            ':doc:`tutorial on 3D masks<mask_3D>`. See :issue:`226` how *weighted* regional '*

 * *            'averages can be calculated with 2D integer mask (this may also offer some speed '*

 * *            "gains).')], delete: [1]}}, 6: {'source': {insert: [(1, 'import numpy as np\\n'), (2, "*

 * *            '\'\\n\'), (3, \'xr.s […]*

```diff
@@ -29,15 +29,15 @@
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
                 ".. note::\n",
-                "   2D masks are good for plotting. However, to calculate weighted regional averages 3D boolean masks are more convenient. See the :doc:`tutorial on 3D masks<mask_3D>`."
+                "   2D masks are good for plotting. However, to calculate weighted regional averages 3D boolean masks are more convenient. See the :doc:`tutorial on 3D masks<mask_3D>`. See :issue:`226` how *weighted* regional averages can be calculated with 2D integer mask (this may also offer some speed gains)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Import regionmask and check the version:"
@@ -64,15 +64,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import xarray as xr\n",
-                "import numpy as np"
+                "import numpy as np\n",
+                "\n",
+                "xr.set_options(display_style=\"text\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating a mask\n",
@@ -106,15 +108,15 @@
                 "regionmask.defined_regions.srex"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The function `mask` determines which gripoints lie within the polygon making up the each region:"
+                "The function `mask` determines which gridpoints lie within the polygon making up the each region:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -140,15 +142,19 @@
             "source": [
                 "import cartopy.crs as ccrs\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "f, ax = plt.subplots(subplot_kw=dict(projection=ccrs.PlateCarree()))\n",
                 "ax.coastlines()\n",
                 "\n",
-                "mask.plot(ax=ax, transform=ccrs.PlateCarree(), add_colorbar=False);"
+                "regionmask.defined_regions.srex.plot(\n",
+                "    ax=ax, add_label=False, line_kws=dict(lw=0.5, color=\"0.5\")\n",
+                ")\n",
+                "\n",
+                "mask.plot(ax=ax, transform=ccrs.PlateCarree(), add_colorbar=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Working with a mask\n",
@@ -188,15 +194,15 @@
                 "ax.coastlines();"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Conviniently we can directly pass an xarray object to the `mask` function. It gets the longitude and latitude from the `DataArray`/ `Dataset` and creates the `mask`. If the longitude and latitude in the xarray object are not called `\"lon\"` and `\"lat\"`, respectively; you can pass their name via the `lon_name` and `lat_name` keyword."
+                "Conveniently we can directly pass an xarray object to the `mask` function. It gets the longitude and latitude from the `DataArray`/ `Dataset` and creates the `mask`. Per default regionmask assumes the longitude and latitude are called `\"lon\"` and `\"lat\"`. If they have another name, you can pass them individually, e.g. `region.mask(ds.longitude, ds.latitude)`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -204,15 +210,15 @@
                 "mask = regionmask.defined_regions.srex.mask(airtemps)"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
-                ".. note:: From version 0.5 ``regionmask`` automatically detects wether the longitude needs to be wrapped around, i.e. if the regions extend from -180\u00b0 E to 180\u00b0 W, while the grid goes from 0\u00b0 to 360\u00b0 W as in our example:"
+                ".. note:: ``regionmask`` automatically detects whether the longitude needs to be wrapped around, i.e. if the regions extend from -180\u00b0 E to 180\u00b0 W, while the grid goes from 0\u00b0 to 360\u00b0 W as in our example:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -290,15 +296,15 @@
                 "### Mask out a region"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`xarray` provides the handy `where` function:"
+                "`xarray` provides the handy `where` method ([documentation](https://xarray.pydata.org/en/stable/generated/xarray.DataArray.where.html)), that filters elements from this object according to a condition:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -343,15 +349,15 @@
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
                 ".. note::\n",
-                "   It is better to use a model's original grid cell area (e.g. areacella). ``cos(lat)`` works reasonably well for regular lat/ lon grids. For irregular grids (regional models, ocean models, ...) it is not appropriate."
+                "   It is better to use a model's original grid cell area (e.g. ``areacella``). ``cos(lat)`` works reasonably well for regular lat/ lon grids. For irregular grids (regional models, ocean models, ...) it is not appropriate."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -394,17 +400,16 @@
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
                 ".. warning::\n",
-                "   Using ``groupby`` offers some convenience and is faster than using ``where`` and a loop. However, it cannot\n",
-                "   currently be combinded with ``weighted`` (xarray `GH3937 <https://github.com/pydata/xarray/issues/3937>`_).\n",
-                "   Therefore, I recommend working with a :doc:`3D mask<mask_3D>`."
+                "   Using ``groupby`` offers some convenience and is faster than using ``where`` and a loop. However, xarray does currently not natively support to combine ``groupby`` with ``weighted`` (`pydata/xarray#3937 <https://github.com/pydata/xarray/issues/3937>`_), see :issue:`226` for a workaround.\n",
+                "   Overall, I recommend working with a :doc:`3D mask<mask_3D>`. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -414,15 +419,15 @@
                 "airtemps_all"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "However, `groupby` is the way to go when calculating a regional median:"
+                "However, `groupby` is the way to go when calculating a (unweighted) regional median:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -467,18 +472,16 @@
             "source": [
                 "# choose a projection\n",
                 "proj = ccrs.NorthPolarStereo()\n",
                 "\n",
                 "ax = plt.subplot(111, projection=proj)\n",
                 "ax.set_global()\n",
                 "\n",
-                "# `shading=\"flat\"` is a workaround for matplotlib 3.3 and 3.4\n",
-                "# until SciTools/cartopy#1646 is merged\n",
                 "rasm.isel(time=1).Tair.plot.pcolormesh(\n",
-                "    ax=ax, x=\"xc\", y=\"yc\", transform=ccrs.PlateCarree(), shading=\"flat\"\n",
+                "    ax=ax, x=\"xc\", y=\"yc\", transform=ccrs.PlateCarree()\n",
                 ")\n",
                 "\n",
                 "# add the abbreviation of the regions\n",
                 "regionmask.defined_regions.srex[[1, 2, 11, 12, 18]].plot(\n",
                 "    ax=ax, add_coastlines=False, label=\"abbrev\"\n",
                 ")\n",
                 "\n",
@@ -487,24 +490,24 @@
                 "ax.coastlines();"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Again we pass the xarray object to regionmask. We have to specify `\"xc\"` and `\"yc\"` as the longitude and latitude coordinates of the array:"
+                "Again we pass the xarray object to regionmask. We have to pass `rasm.xc` and `rasm.yc` as the longitude and latitude coordinates of the array:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "mask = regionmask.defined_regions.srex.mask(rasm, lon_name=\"xc\", lat_name=\"yc\")\n",
+                "mask = regionmask.defined_regions.srex.mask(rasm.xc, rasm.yc)\n",
                 "mask"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -560,15 +563,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## References\n",
                 "\n",
-                "* Special Report on Managing the Risks of Extreme Events and Disasters to Advance Climate Change Adaptation (SREX, Seneviratne et al., 2012: https://www.ipcc.ch/site/assets/uploads/2018/03/SREX-Ch3-Supplement_FINAL-1.pdf)"
+                "* Special Report on Managing the Risks of Extreme Events and Disasters to Advance Climate Change Adaptation (SREX, Seneviratne et al., [2012](https://www.ipcc.ch/site/assets/uploads/2018/03/SREX-Ch3-Supplement_FINAL-1.pdf))"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -580,13 +583,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.10.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `regionmask-0.8.0/docs/notebooks/mask_3D.ipynb` & `regionmask-0.9.0/docs/notebooks/mask_3D.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9887801434676434%*

 * *Differences: {"'cells'": '{6: {\'source\': {insert: [(4, \'xr.set_options(display_style="text", '*

 * *            "display_expand_data=False)')], delete: [4]}}, 20: {'metadata': {replace: "*

 * *            'OrderedDict()}}, 35: {\'source\': {insert: [(1, "   It is better to use a model\'s '*

 * *            'original grid cell area (e.g. ``areacella``). ``cos(lat)`` works reasonably well for '*

 * *            'regular lat/ lon grids. For irregular grids (regional models, ocean models, ...) it '*

 * *            'is not appropriate.")], delet […]*

```diff
@@ -27,14 +27,22 @@
                 "\n",
                 "In this tutorial we will show how to create 3D boolean masks for arbitrary latitude and longitude grids. It uses the same algorithm to determine if a gridpoint is in a region as for the 2D mask. However, it returns a `xarray.Dataset` with shape `region x lat x lon`, gridpoints that do not fall in a region are `False`, the gridpoints that fall in a region are `True`.\n",
                 "\n",
                 "3D masks are convenient as they can be used to directly calculate weighted regional means (over all regions) using xarray v0.15.1 or later. Further, the mask includes the region names and abbreviations as non-dimension coordinates."
             ]
         },
         {
+            "cell_type": "raw",
+            "metadata": {},
+            "source": [
+                ".. note::\n",
+                "   3D boolean masks are more convenient to work with but :doc:`2D masks<mask_2D>` may offer some speed gains when calculating regional means. See :issue:`226` how *weighted* regional averages can be calculated with 2D integer mask."
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Import regionmask and check the version:"
             ]
         },
         {
@@ -61,15 +69,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import xarray as xr\n",
                 "import numpy as np\n",
                 "\n",
                 "# don't expand data\n",
-                "xr.set_options(display_expand_data=False)"
+                "xr.set_options(display_style=\"text\", display_expand_data=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating a mask\n",
@@ -203,17 +211,15 @@
             "source": [
                 "The example data is a temperature field over North America. Let's plot the first time step:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "scrolled": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "# choose a good projection for regional maps\n",
                 "proj = ccrs.LambertConformal(central_longitude=-100)\n",
                 "\n",
                 "ax = plt.subplot(111, projection=proj)\n",
                 "\n",
@@ -358,15 +364,15 @@
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
                 ".. note::\n",
-                "   It is better to use a model's original grid cell area (e.g. areacella). ``cos(lat)`` works reasonably well for regular lat/ lon grids. For irregular grids (regional models, ocean models, ...) it is not appropriate."
+                "   It is better to use a model's original grid cell area (e.g. ``areacella``). ``cos(lat)`` works reasonably well for regular lat/ lon grids. For irregular grids (regional models, ocean models, ...) it is not appropriate."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -410,23 +416,23 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Restrict the mask to land points\n",
                 "\n",
-                "Combining the mask of the regions with a land-sea mask we can create a land-only mask using the `natural_earth.land_110` regions."
+                "Combining the mask of the regions with a land-sea mask we can create a land-only mask using the `land_110` region from NaturalEarth."
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
                 ".. warning::\n",
-                "   It is better to use a model's original land/ sea mask (e.g. sftlf). Many CMIP models treat the Antarctic ice shelves and the Caspian Sea as land, while it is classified as 'water' in ``natural_earth.land_110``."
+                "   It is better to use a model's original land/ sea mask (e.g. ``sftlf``). Many CMIP models treat the Antarctic ice shelves and the Caspian Sea as land, while it is classified as 'water' in ``natural_earth_v5_0_0.land_110``."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "With this caveat in mind we can create the land-sea mask:"
@@ -434,15 +440,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "land_110 = regionmask.defined_regions.natural_earth.land_110\n",
+                "land_110 = regionmask.defined_regions.natural_earth_v5_0_0.land_110\n",
                 "\n",
                 "land_mask = land_110.mask_3D(airtemps)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -517,33 +523,33 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## References\n",
                 "\n",
-                "* Special Report on Managing the Risks of Extreme Events and Disasters to Advance Climate Change Adaptation (SREX, Seneviratne et al., 2012: https://www.ipcc.ch/site/assets/uploads/2018/03/SREX-Ch3-Supplement_FINAL-1.pdf)"
+                "* Special Report on Managing the Risks of Extreme Events and Disasters to Advance Climate Change Adaptation (SREX, Seneviratne et al., [2012](https://www.ipcc.ch/site/assets/uploads/2018/03/SREX-Ch3-Supplement_FINAL-1.pdf))"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.8"
+            "version": "3.10.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `regionmask-0.8.0/docs/notebooks/method.ipynb` & `regionmask-0.9.0/docs/notebooks/method.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960886150957968%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(6, 'cmap3 = mplc.ListedColormap([color3])\\n'), (7, '\\n'), "*

 * *            "(8, 'cmap12 = mplc.ListedColormap([color1, color2])')], delete: [6]}}, 8: {'source': "*

 * *            '{insert: [(8, "All methods use the `lon` and `lat` coordinates to determine if a grid '*

 * *            'cell is in a region. `lon` and `lat` are assumed to indicate the *center* of the grid '*

 * *            "cell. All methods have the same edge behavior and consider 'holes' in the regions. "*

 * *            […]*

```diff
@@ -88,30 +88,32 @@
             "source": [
                 "color1 = \"#9ecae1\"\n",
                 "color2 = \"#fc9272\"\n",
                 "color3 = \"#cab2d6\"\n",
                 "\n",
                 "cmap1 = mplc.ListedColormap([color1])\n",
                 "cmap2 = mplc.ListedColormap([color2])\n",
-                "cmap3 = mplc.ListedColormap([color3])"
+                "cmap3 = mplc.ListedColormap([color3])\n",
+                "\n",
+                "cmap12 = mplc.ListedColormap([color1, color2])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Methods\n",
                 "\n",
                 "Regionmask offers three \"methods\"* to rasterize regions\n",
                 "\n",
                 "1. `rasterize`: fastest but only for equally-spaced grid, uses `rasterio.features.rasterize` internally.\n",
                 "2. `shapely`: for irregular grids, uses `shapely.vectorized.contains` internally.\n",
                 "3. `pygeos`: a faster alternative for irregular grids. This is method is preferred over (2) if the optional dependency pygeos is installed. Uses `pygeos.STRtree` internally.\n",
                 "\n",
-                "All methods use the `lon` and `lat` coordinates to determine if a grid cell is in a region. `lon` and `lat` are assumed to indicate the *center* of the grid cell. Methods (1) and (2) have the same edge behavior and consider 'holes' in the regions. `regionmask` automatically determines which `method` to use.\n",
+                "All methods use the `lon` and `lat` coordinates to determine if a grid cell is in a region. `lon` and `lat` are assumed to indicate the *center* of the grid cell. All methods have the same edge behavior and consider 'holes' in the regions. `regionmask` automatically determines which `method` to use.\n",
                 "\n",
                 "(2) and (3) subtract a tiny offset from `lon` and `lat` to achieve a edge behaviour consistent with (1). Due to [mapbox/rasterio#1844](https://github.com/mapbox/rasterio/issues/1844) this is unfortunately also necessary for (1).\n",
                 "\n",
                 "\n",
                 "\\*Note that all \"methods\" yield the same results."
             ]
         },
@@ -317,20 +319,21 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "outline_global = np.array(\n",
-                "    [[-180.0, 90.0], [-180.0, -90.0], [180.0, -90.0], [180.0, 90.0]]\n",
-                ")\n",
+                "# almost 360 to avoid wrap-around for the plot\n",
+                "lon_max = 360.0 - 1e-10\n",
+                "outline_global = np.array([[0, 90], [0, -90], [lon_max, -90], [lon_max, 90]])\n",
+                "\n",
                 "region_global = regionmask.Regions([outline_global])\n",
                 "\n",
-                "lon = np.arange(-180, 180, 30)\n",
+                "lon = np.arange(0, 360, 30)\n",
                 "lat = np.arange(90, -91, -30)\n",
                 "\n",
                 "LON, LAT = np.meshgrid(lon, lat)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -342,17 +345,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# setting `wrap_lon=False` turns this feature off\n",
-                "mask_global_nontreat = region_global.mask(lon, lat, wrap_lon=False)\n",
+                "mask_global_nontreat = region_global.mask(LON, LAT, wrap_lon=False)\n",
                 "\n",
-                "mask_global = region_global.mask(lon, lat)"
+                "mask_global = region_global.mask(LON, LAT)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "And illustrate the issue:"
@@ -360,54 +363,49 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "f, axes = plt.subplots(1, 2, subplot_kw=dict(projection=ccrs.PlateCarree()))\n",
+                "proj = ccrs.PlateCarree(central_longitude=180)\n",
+                "f, axes = plt.subplots(1, 2, subplot_kw=dict(projection=proj))\n",
                 "f.subplots_adjust(wspace=0.05)\n",
                 "\n",
-                "opt = dict(add_colorbar=False, ec=\"0.3\", lw=0.5, transform=ccrs.PlateCarree())\n",
+                "opt = dict(add_colorbar=False, ec=\"0.2\", lw=0.25, transform=ccrs.PlateCarree())\n",
                 "\n",
                 "ax = axes[0]\n",
-                "# work around for SciTools/cartopy/issues/1845\n",
-                "mask_global_nontreat = mask_global_nontreat.fillna(1)\n",
-                "mask_global_nontreat.plot(ax=ax, colors=[color1, \"none\"], levels=2, **opt)\n",
-                "\n",
-                "# only for the gridlines\n",
-                "mask_global.plot(ax=ax, colors=[\"none\"], levels=1, **opt)\n",
+                "mask_global_nontreat.plot(ax=ax, cmap=cmap1, x=\"lon\", y=\"lat\", **opt)\n",
                 "\n",
-                "ax.set_title(\"Not treating points at -180\u00b0E and -90\u00b0N\", size=6)\n",
+                "ax.set_title(\"Not treating points at 0\u00b0E and -90\u00b0N\", size=6)\n",
                 "ax.set_title(\"(a)\", loc=\"left\", size=6)\n",
                 "\n",
                 "ax = axes[1]\n",
-                "mask_global.plot(ax=ax, cmap=cmap1, **opt)\n",
+                "mask_global.plot(ax=ax, cmap=cmap1, x=\"lon\", y=\"lat\", **opt)\n",
                 "\n",
-                "ax.set_title(\"Treating points at -180\u00b0E and -90\u00b0N\", size=6)\n",
+                "ax.set_title(\"Treating points at 0\u00b0E and -90\u00b0N\", size=6)\n",
                 "ax.set_title(\"(b)\", loc=\"left\", size=6)\n",
                 "\n",
                 "\n",
                 "for ax in axes:\n",
                 "\n",
                 "    ax = region_global.plot(\n",
                 "        ax=ax,\n",
                 "        line_kws=dict(lw=2, color=\"#b15928\"),\n",
                 "        add_label=False,\n",
                 "    )\n",
                 "    ax.plot(LON, LAT, \"o\", color=\"0.3\", ms=1, transform=ccrs.PlateCarree(), zorder=5)\n",
-                "\n",
                 "    ax.outline_patch.set_visible(False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In the example the region spans the whole globe and there are gridpoints at -180\u00b0E and -90\u00b0N. Just applying the approach above leads to gridpoints that are not assigned to any region even though the region is global (as shown in a). Therefore, points at -180\u00b0E (or 0\u00b0E) and -90\u00b0N are treated specially (b):\n",
+                "In the example the region spans the whole globe and there are gridpoints at 0\u00b0E and -90\u00b0N. Just applying the approach above leads to gridpoints that are not assigned to any region even though the region is global (as shown in a). Therefore, points at -180\u00b0E (or 0\u00b0E) and -90\u00b0N are treated specially (b):\n",
                 "\n",
                 "Points at -180\u00b0E (0\u00b0E) are mapped to 180\u00b0E (360\u00b0E). Points at -90\u00b0N are slightly shifted northwards (by 1 * 10 ** -10). Then it is tested if the shifted points belong to any region\n",
                 "\n",
                 "This means that (i) a point at -180\u00b0E is part of the region that is present at 180\u00b0E and not the one at -180\u00b0E (this is consistent with assigning points to the polygon *left* from it) and (ii) only the points at -90\u00b0N get assigned to the region above.\n",
                 "\n",
                 "This is illustrated in the figure below:"
             ]
@@ -429,37 +427,34 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ax = region_global_2.plot(\n",
-                "    line_kws=dict(color=\"#b15928\", zorder=3, lw=1),\n",
+                "    line_kws=dict(color=\"#b15928\", zorder=3, lw=1.5),\n",
                 "    add_label=False,\n",
                 ")\n",
                 "\n",
-                "ax.plot(LON, LAT, \"o\", color=\"0.3\", ms=2, transform=ccrs.PlateCarree(), zorder=5)\n",
-                "\n",
-                "# work around for SciTools/cartopy/issues/1845\n",
-                "mask_global_2regions = mask_global_2regions.fillna(2)\n",
-                "mask_global_2regions.plot(ax=ax, colors=[color1, color2, \"none\"], levels=3, **opt)\n",
-                "# only for the gridlines\n",
-                "mask_global.plot(ax=ax, colors=[\"none\"], levels=1, **opt)\n",
+                "ax.plot(\n",
+                "    LON, LAT, \"o\", color=\"0.3\", lw=0.25, ms=2, transform=ccrs.PlateCarree(), zorder=5\n",
+                ")\n",
+                "mask_global_2regions.plot(ax=ax, cmap=cmap12, **opt)\n",
                 "\n",
                 "ax.set_title(\"Points at -180\u00b0E are mapped to 180\u00b0E\", size=6)\n",
                 "\n",
-                "ax.outline_patch.set_lw(0.5)\n",
+                "ax.outline_patch.set_lw(0.25)\n",
                 "ax.outline_patch.set_zorder(1);"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
-                ".. note:: This only applies if the border of the region falls *exactly* on the point. One way to avoid the problem is to calculate the `fractional overlap <https://github.com/regionmask/regionmask/issues/38>`_ of each gridpoint with the regions (which is not yet implemented)."
+                ".. note:: This only applies if the border of the region falls *exactly* on the point. One way to avoid the problem is to calculate the fractional overlap (see :issue:`38`) of each gridpoint with the regions (which is not yet implemented)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Polygon interiors\n",
@@ -550,15 +545,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "land110 = regionmask.defined_regions.natural_earth.land_110\n",
+                "land110 = regionmask.defined_regions.natural_earth_v5_0_0.land_110\n",
                 "\n",
                 "mask_land110 = land110.mask(ds_GLOB)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -596,13 +591,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.10.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `regionmask-0.8.0/docs/notebooks/plotting.ipynb` & `regionmask-0.9.0/docs/notebooks/plotting.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963330123716153%*

 * *Differences: {"'cells'": "{11: {'source': {insert: [(11, '    text_kws=text_kws,\\n')]}}, 15: {'source': ['To "*

 * *            "achieve this, you need to explicitly create the axes: ']}, 16: {'source': {insert: "*

 * *            "[(4, 'srex.plot_regions(ax=ax, line_kws=dict(lw=1), text_kws=text_kws)\\n')], delete: "*

 * *            '[4]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.2'}}"}*

```diff
@@ -138,14 +138,15 @@
                 "proj = ccrs.LambertConformal(central_longitude=15)\n",
                 "\n",
                 "ax = srex[regions].plot(\n",
                 "    add_ocean=True,\n",
                 "    resolution=\"50m\",\n",
                 "    proj=proj,\n",
                 "    label=\"abbrev\",\n",
+                "    text_kws=text_kws,\n",
                 ")\n",
                 "\n",
                 "# fine tune the extent\n",
                 "ax.set_extent([-15, 45, 28, 76], crs=ccrs.PlateCarree())"
             ]
         },
         {
@@ -171,28 +172,28 @@
                 ".. note:: This does *not* create a cartopy GeoAxes."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To achieve this, you need to explicitely create the axes: "
+                "To achieve this, you need to explicitly create the axes: "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "f, ax = plt.subplots(subplot_kw=dict(projection=ccrs.Robinson()))\n",
                 "\n",
-                "srex.plot_regions(ax=ax, line_kws=dict(lw=1))\n",
+                "srex.plot_regions(ax=ax, line_kws=dict(lw=1), text_kws=text_kws)\n",
                 "\n",
                 "ax.coastlines()\n",
                 "ax.set_global()"
             ]
         }
     ],
     "metadata": {
@@ -207,13 +208,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.10.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `regionmask-0.8.0/docs/notebooks/tutorial_rst.tpl` & `regionmask-0.9.0/docs/notebooks/tutorial_rst.tpl`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {%- extends 'display_priority.tpl' -%}
 
 {% block header %}
 
-.. note:: This tutorial was generated from an IPython notebook that can be
-          downloaded `here <../../notebooks/{{ resources.metadata.name }}.ipynb>`_.
+.. note:: This tutorial was generated from an IPython notebook that can be accessed from
+          `github <https://github.com/regionmask/regionmask/tree/master/docs/notebooks>`_.
 
 .. _{{resources.metadata.name}}:
 {% endblock %}
 
 {% block in_prompt %}
 {% endblock in_prompt %}
```

### Comparing `regionmask-0.8.0/docs/whats_new.rst` & `regionmask-0.9.0/docs/whats_new.rst`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,131 @@
 ==========
 
 .. ipython:: python
    :suppress:
 
     import regionmask
 
-.. _whats-new.0.8.0:
+.. _whats-new.0.9.0:
+
+v0.9.0 (02.03.2022)
+-------------------
+
+Version 0.9.0 contains some exiting improvements: overlapping regions and unstructured
+grids can now be masked correctly. Further, :py:class:`Regions` can now be round-tripped
+to :py:class:`geopandas.GeoDataFrame` objects. The new version also adds PRUDENCE
+regions and a more stable handling of naturalearth regions.
+
+Many thanks to the contributors to the v0.9.0 release: Aaron Spring, Mathias Hauser, and
+Ruth Lorenz!
+
+Breaking Changes
+~~~~~~~~~~~~~~~~
+
+- Removed support for Python 3.6 (:pull:`288`).
+- The ``xarray.DataArray`` mask returned by all masking functions (e.g. :py:meth:`Regions.mask`)
+  was renamed from `region` to `mask`. The former was ambiguous with respect to the `region` dimension
+  of 3D masks (:pull:`318`).
+- The minimum versions of some dependencies were changed (:pull:`311`, :pull:`312`):
+
+  ============ ===== =====
+  Package      Old   New
+  ============ ===== =====
+  geopandas    0.6   0.7
+  matplotlib   3.1   3.2
+  pooch        1.0   1.2
+  rasterio     1.0   1.1
+  shapely      1.6   1.7
+  ============ ===== =====
+
+- ``regionmask.defined_regions.natural_earth`` is deprecated. ``defined_regions.natural_earth`` used
+  cartopy to download natural_earth data and it was unclear which version of the regions
+  is available. This is problematic because some regions change between the versions.
+  Please use ``defined_regions.natural_earth_v4_1_0`` or ``defined_regions.natural_earth_v5_0_0``
+  instead (:issue:`306`, :pull:`311`).
+- Passing coordinates with different type to :py:meth:`Regions.mask` and :py:meth:`Regions.mask_3D`
+  is no longer supported, i.e. can no longer pass lon as numpy array and lat as
+  DataArray (:pull:`294`).
+- The mask no longer has dimension coordinates when 2D numpy arrays are passed as lat and
+  lon coords (:pull:`294`).
+
+Enhancements
+~~~~~~~~~~~~
+
+- regionmask does now correctly treat overlapping regions if ``overlap=True`` is set in
+  the constructor (:issue:`228`, :pull:`318`).
+
+  Per default regionmask assumes non-overlapping regions. In this case grid points of
+  overlapping polygons will silently be assigned to the region with the higher number.
+  This may change in a future version.
+
+- :py:meth:`Regions.mask` and :py:meth:`Regions.mask_3D` now work with unstructured 1D
+  grids such as:
+
+  - `ICON <https://code.mpimet.mpg.de/projects/iconpublic>`_
+  - `FESOM <https://fesom.de/>`_
+  - `MPAS <https://mpas-dev.github.io/>`_
+
+  with 1-dimensional coordinates of the form ``lon(cell)`` and ``lat(cell)``.
+  Note that only xarray arrays can be detected as unstructured grids.
+  (:issue:`278`, :pull:`280`). By `Aaron Spring <https://github.com/aaronspring>`_.
+
+- Add methods to convert :py:class:`Regions` to (geo)pandas objects, namely :py:meth:`Regions.to_geodataframe`,
+  :py:meth:`Regions.to_geoseries`, :py:meth:`Regions.to_dataframe`). The geopandas.GeoDataFrame
+  can be converted back (round-tripped) using :py:meth:`Regions.from_geodataframe`
+  (:issue:`50`, :pull:`298`).
+
+- The plotting methods (:py:meth:`Regions.plot` and :py:meth:`Regions.plot_regions`) now
+  use a more sophisticated logic to subsample lines on GeoAxes plots. The new method is
+  based on the euclidean distance of each segment. Per default the maximum distance of
+  each segment is 1 for lat/ lon coords - see the ``tolerance`` keyword of the plotting
+  methods. The ``subsample`` keyword is deprecated (:issue:`109`, :pull:`292`).
+- The download of the natural_earth regions is now done in regionmask (using pooch) and no
+  longer relies on cartopy (:issue:`306`, :pull:`311`).
+
+Deprecations
+~~~~~~~~~~~~
+
+- The ``regionmask.defined_regions._ar6_pre_revisions`` regions are deprecated. The
+  ``regionmask.defined_regions.ar6`` regions should be used instead (:issue:`314`, :pull:`320`).
+
+New regions
+~~~~~~~~~~~
+
+- Added :py:attr:`prudence` regions for Europe from `Christensen and Christensen, 2007,
+  <https://link.springer.com/article/10.1007/s10584-006-9210-7>`_ (:pull:`283`).
+  By `Ruth Lorenz <https://github.com/ruthlorenz>`_.
+
+Bug Fixes
+~~~~~~~~~
+
+- The name of lon and lat coordinates when passed as single elements is now respected when
+  creating masks i.e. for ``region.mask(ds.longitude, ds.longitude)`` (:issue:`129`,
+  :pull:`294`).
+- Ensure :py:meth:`Regions.plot` uses the current axes (``plt.gca()``) if possible and
+  error if a non-cartopy GeoAxes is passed (:issue:`316`, :pull:`321`).
+
+Docs
+~~~~
+
+- Went over the documentation, improved some sections, unpinned some packages, modernized
+  some aspects (:pull:`313`).
+
+Internal Changes
+~~~~~~~~~~~~~~~~
+
+- Fix compatibility with shapely 1.8 (:pull:`291`).
+- Fix downloading naturalearth regions part 2 (see :pull:`261`): Monkeypatch the correct
+  download URL and catch all ``URLError``, not only timeouts (:pull:`289`).
+- Rewrote the function to create the mask `DataArray` (:issue:`168`, :pull:`294`).
+- Follow up to :pull:`294` - fix wrong dimension order for certain conditions (:issue:`295`).
+- Refactor `test_mask` - make use of ``xr.testing.assert_equal`` and simplify some
+  elements (:pull:`297`).
+- Add `packaging` as a dependency (:issue:`324`, :pull:`328`).
+- Add python 3.10 to list of supported versions (:pull:`330`).
 
 v0.8.0 (08.09.2021)
 -------------------
 
 Version 0.8.0 contains an important bugfix, improves the handling of wrapped longitudes,
 can create masks for coordinates and regions that do not have a lat/ lon coordinate
 reference system and masks for irregular and 2D grids are created faster if the optional
@@ -22,15 +138,15 @@
 ~~~~~~~~~~~~~~~~
 
 - Points at *exactly* -180°E (or 0°E) and -90°N are no longer special cased if
   ``wrap_lon=False`` when creating a mask - see :doc:`methods<notebooks/method>` for
   details (:issue:`151`).
 - Updates to :py:meth:`Regions.plot` and :py:meth:`Regions.plot_regions` (:pull:`246`):
 
-  - Deprecated all positional arguments (keword arguments only).
+  - Deprecated all positional arguments (keyword arguments only).
   - The ``regions`` keyword was deprecated. Subset regions before plotting, i.e.
     use ``r[regions].plot()`` instead of ``r.plot(regions=regions)``. This will allow
     to remove a argument from the methods.
 - Updates to :py:meth:`Regions.plot` (:pull:`246`):
 
   - Added ``lw=0`` to the default ``ocean_kws`` and ``land_kws`` to avoid overlap with
     the coastlines.
@@ -74,18 +190,18 @@
 Docs
 ~~~~
 
 - Updated the plotting tutorial (:pull:`246`).
 - Install `regionmask` via `ci/requirements/docs.yml` on RTD using pip and update the
   packages: don't require jupyter (but ipykernel, which leads to a smaller environment),
   use new versions of sphinx and sphinx_rtd_theme (:pull:`248`).
-- Pin cartopy to version 0.19 and matplotlib to version 3.4 and use a (temorary) fix for
+- Pin cartopy to version 0.19 and matplotlib to version 3.4 and use a (temporary) fix for
   :issue:`165`. This allows to make use of `conda-forge/cartopy-feedstock#116
   <https://github.com/conda-forge/cartopy-feedstock/pull/116>`__ such that natural_earth
-  shapefiles can be donwloaded again. Also added some other minor doc updates
+  shapefiles can be downloaded again. Also added some other minor doc updates
   (:pull:`269`).
 
 Internal Changes
 ~~~~~~~~~~~~~~~~
 
 - Updated setup configuration and automated version numbering:
 
@@ -259,15 +375,15 @@
 
 New regions
 ~~~~~~~~~~~
 
 - Added the AR6 reference regions described in `Iturbide et al., (2000)
   <https://essd.copernicus.org/preprints/essd-2019-258/>`_ (:pull:`61`).
 - New marine regions from natural earth added as :py:attr:`natural_earth.ocean_basins_50`
-  (:pull:`63` by `Julius Busecke <https://github.com/jbusecke>`_).
+  (:pull:`91` by `Julius Busecke <https://github.com/jbusecke>`_).
 
 Bug Fixes
 ~~~~~~~~~
 
 - The natural earth shapefiles are now loaded with ``encoding="utf8"`` (:issue:`95`).
 - Explicitly check that the numbers are numeric and raise an informative error (:issue:`130`).
 - Do not subset coords with more than 10 vertices when plotting regions as this
```

### Comparing `regionmask-0.8.0/licences/AR6_REGIONS_LICENSE` & `regionmask-0.9.0/licences/AR6_REGIONS_LICENSE`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/licences/XARRAY_LICENSE` & `regionmask-0.9.0/licences/XARRAY_LICENSE`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/regionmask/core/_geopandas.py` & `regionmask-0.9.0/regionmask/core/_geopandas.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import warnings
+
 import numpy as np
 
-from ..defined_regions.natural_earth import _maybe_get_column
+from ..defined_regions._natural_earth import _maybe_get_column
 from .mask import _inject_mask_docstring, _mask_2D, _mask_3D
 from .regions import Regions
 
 
 def _check_duplicates(data, name):
     """Checks if `data` has duplicates.
 
@@ -53,48 +55,103 @@
     names = names.str.replace("[/-]", " ", regex=True)
     abbrevs = names.str.split(" ").map(lambda x: "".join([y[:3] for y in x]))
     abbrevs = _enumerate_duplicates(abbrevs)
     return abbrevs
 
 
 def from_geopandas(
-    geodataframe, numbers=None, names=None, abbrevs=None, name="unnamed", source=None
+    geodataframe,
+    numbers=None,
+    names=None,
+    abbrevs=None,
+    name="unnamed",
+    source=None,
+    overlap=False,
 ):
     """
-    Create ``regionmask.Region`` from ``geopandas.geodataframe.GeoDataFrame``.
+    Create ``regionmask.Regions`` from a ``geopandas.GeoDataFrame``.
 
     Parameters
     ----------
-    geodataframe : geopandas.geodataframe.GeoDataFrame
+    geodataframe : geopandas.GeoDataFrame
         GeoDataFrame to be transformed to a Regions class.
+
     numbers : str, optional
         Name of the column in geodataframe that gives each region its number.
         This column must not have duplicates. If None (default), takes
         ``geodataframe.index.values``.
+
     names : str, optional
         Name of the column in shapefile that names a region. Breaks for duplicates.
         If None (default) uses "Region0", .., "RegionN".
+
     abbrevs : str, optional
         Name of the column in shapefile that five a region its abbreviation.
         Breaks for duplicates. If ``_from_name``, a combination of the first letters
         of region name is taken. If None (default) uses "r0", .., "rN".
+
     name : str, optional
         name of the ``regionmask.Region`` instance created
+
     source : str, optional
         source of the shapefile
 
+    overlap : bool, default: False
+        Indicates if (some of) the regions overlap. If True ``mask_3D`` will ensure
+        overlapping regions are correctly assigned to grid points while ``mask`` will
+        error (because overlapping regions cannot be represented by a 2D mask).
+
+        If False (default) assumes non-overlapping regions. Grid points will
+        silently be assigned to the region with the higher number (this may change
+        in a future version).
+
+        There is (currently) no automatic detection of overlapping regions.
+
     Returns
     -------
     regionmask.core.regions.Regions
 
+    See Also
+    --------
+    Regions.to_dataframe, Regions.to_geodataframe, Regions.to_geoseries, Regions.from_geodataframe
     """
+
     from geopandas import GeoDataFrame
 
     if not isinstance(geodataframe, (GeoDataFrame)):
-        raise TypeError("`geodataframe` must be a geopandas 'GeoDataFrame'")
+        raise TypeError(
+            "`geodataframe` must be a geopandas 'GeoDataFrame',"
+            f" found {type(geodataframe)}"
+        )
+
+    if any(x in geodataframe.attrs for x in ["name", "source", "overlap"]):
+        warnings.warn(
+            "Use ``regionmask.Regions.from_geodataframe`` to round-trip ``Regions``"
+        )
+
+    return _from_geopandas(
+        geodataframe,
+        numbers=numbers,
+        names=names,
+        abbrevs=abbrevs,
+        name=name,
+        source=source,
+        overlap=overlap,
+    )
+
+
+def _from_geopandas(
+    geodataframe,
+    numbers=None,
+    names=None,
+    abbrevs=None,
+    name="unnamed",
+    source=None,
+    overlap=False,
+):
 
     if numbers is not None:
         # sort, otherwise breaks
         geodataframe = geodataframe.sort_values(numbers)
         numbers = _maybe_get_column(geodataframe, numbers)
         _check_missing(numbers, "numbers")
         _check_duplicates(numbers, "numbers")
@@ -121,14 +178,15 @@
     return Regions(
         outlines,
         numbers=numbers,
         names=names,
         abbrevs=abbrevs,
         name=name,
         source=source,
+        overlap=overlap,
     )
 
 
 def _prepare_gdf_for_mask(geodataframe, method, numbers):
 
     from geopandas import GeoDataFrame, GeoSeries
 
@@ -188,14 +246,15 @@
     lat=None,
     drop=True,
     lon_name="lon",
     lat_name="lat",
     numbers=None,
     method=None,
     wrap_lon=None,
+    overlap=False,
 ):
 
     polygons, lon_bounds, numbers = _prepare_gdf_for_mask(
         geodataframe, method=method, numbers=numbers
     )
 
     mask_3D = _mask_3D(
@@ -205,13 +264,14 @@
         lon_or_obj=lon_or_obj,
         lat=lat,
         drop=drop,
         lon_name=lon_name,
         lat_name=lat_name,
         method=method,
         wrap_lon=wrap_lon,
+        as_3D=overlap,
     )
 
     return mask_3D
 
 
 mask_3D_geopandas.__doc__ = _inject_mask_docstring(is_3D=True, gp_method=True)
```

### Comparing `regionmask-0.8.0/regionmask/core/formatting.py` & `regionmask-0.9.0/regionmask/core/formatting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """String formatting routines for __repr__."""
 
-import geopandas as gp
+
 from pandas.io.formats import console
 
 
 def pretty_print(x, numchars, right=True):
     """Given an object `x`, call `str(x)` and format the returned string so
     that it is numchars long, padding with trailing spaces or truncating with
     ellipses as necessary
@@ -25,39 +25,35 @@
 
     s = str(obj)
     if len(s) > maxlen:
         s = s[: (maxlen - 3)] + "..."
     return s
 
 
-def _display_metadata(name, source, max_width=80):
+def _display_metadata(name, source, overlap, max_width=80):
     pad = 10
 
     name = pretty_print("Name:", pad) + maybe_truncate(name, max_width - pad)
     summary = [name]
 
     if source is not None:
         source = pretty_print("Source:", pad) + maybe_truncate(source, max_width - pad)
         summary.append(source)
 
+    overlap = pretty_print("overlap:", pad) + f"{overlap}"
+    summary.append(overlap)
+
     return summary
 
 
 def _display_regions_gp(self, max_rows, max_width, max_colwidth):  # pragma: no cover
     summary = ["Regions:"]
 
-    data = dict(
-        numbers=self.numbers,
-        abbrevs=self.abbrevs,
-        names=self.names,
-        # __repr__ of polygons can be slow
-        # geometry=self.polygons,
-    )
-
-    df = gp.GeoDataFrame.from_dict(data)
+    # __repr__ of polygons can be slow -> use pd.DataFrame
+    df = self.to_dataframe().reset_index()
 
     summary.append(
         df.to_string(
             columns=["numbers", "abbrevs", "names"],
             max_rows=max_rows,
             max_cols=0,
             line_width=max_width,
@@ -69,23 +65,25 @@
     )
 
     return summary
 
 
 def _display(self, max_rows=10, max_width=None, max_colwidth=50):
 
-    summary = ["<regionmask.{}>".format(type(self).__name__)]
+    summary = [f"<regionmask.{type(self).__name__}>"]
 
     if max_rows is None:
         max_rows = len(self)
 
     if max_width is None:
         max_width, _ = console.get_console_size()
 
-    summary += _display_metadata(self.name, self.source, max_width=max_width)
+    summary += _display_metadata(
+        self.name, self.source, self.overlap, max_width=max_width
+    )
     summary.append("")
     summary += _display_regions_gp(self, max_rows, max_width, max_colwidth)
 
     summary.append("")
-    summary.append("[{:d} regions]".format(len(self)))
+    summary.append(f"[{len(self):d} regions]")
 
     return "\n".join(summary)
```

### Comparing `regionmask-0.8.0/regionmask/core/mask.py` & `regionmask-0.9.0/regionmask/core/mask.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 create a {nd} {dtype} mask of a set of regions for the given lat/ lon grid
 
 Parameters
 ----------
 {gp_doc}lon_or_obj : object or array_like
     Can either be a longitude array and then ``lat`` needs to be
     given. Or an object where the longitude and latitude can be
-    retrived as: ``lon = lon_or_obj[lon_name]`` and
-    ``lat = lon_or_obj[lat_name]``
+    retrieved as: ``lon = lon_or_obj[lon_name]`` and
+    ``lat = lon_or_obj[lat_name]``.
 lat : array_like, optional
     If ``lon_or_obj`` is a longitude array, the latitude needs to be
     specified here.
 {drop_doc}lon_name : str, optional
     Name of longitude in ``lon_or_obj``, default: "lon".
 lat_name : str, optional
     Name of latgitude in ``lon_or_obj``, default: "lat"
@@ -50,15 +50,15 @@
     - ``None``: autodetects whether the longitude needs to be wrapped
     - ``False``: nothing is done. This is useful when working with coordinates that are
       not in lat/ lon format.
     - ``True``: longitude data is wrapped to `[0, 360[` if its minimum is smaller than 0
       and wrapped to `[-180, 180[` if its maximum is larger than 180.
     - ``180``: Wraps longitude coordinates to `[-180, 180[`
     - ``360``: Wraps longitude coordinates to `[0, 360[`
-
+{overlap}
 
 Returns
 -------
 mask_{nd} : {dtype} xarray.DataArray
 
 References
 ----------
@@ -81,25 +81,42 @@
 _DROP_DOCSTRING = """\
 drop : boolean, default: True
     If True (default) drops slices where all elements are False (i.e no
     gridpoints are contained in a region). If False returns one slice per
     region.
 """
 
+_OVERLAP_DOCSTRING = """\
+overlap : bool, default: False
+    Indicates if (some of) the regions overlap. If True ``mask_3D_geopandas`` will
+    ensure overlapping regions are correctly assigned to grid points.
+
+    If False (default) assumes non-overlapping regions. Grid points will silently be
+    assigned to the region with the higher number (this may change in a future version).
+
+    There is (currently) no automatic detection of overlapping regions.
+"""
+
 
 def _inject_mask_docstring(is_3D, gp_method):
 
     dtype = "float" if is_3D else "boolean"
     nd = "3D" if is_3D else "2D"
     drop_doc = _DROP_DOCSTRING if is_3D else ""
     numbers_doc = _NUMBERS_DOCSTRING if gp_method else ""
     gp_doc = _GP_DOCSTRING if gp_method else ""
+    overlap = _OVERLAP_DOCSTRING if (gp_method and is_3D) else ""
 
     mask_docstring = _MASK_DOCSTRING_TEMPLATE.format(
-        dtype=dtype, nd=nd, drop_doc=drop_doc, numbers_doc=numbers_doc, gp_doc=gp_doc
+        dtype=dtype,
+        nd=nd,
+        drop_doc=drop_doc,
+        numbers_doc=numbers_doc,
+        gp_doc=gp_doc,
+        overlap=overlap,
     )
 
     return mask_docstring
 
 
 def _mask(
     outlines,
@@ -107,41 +124,48 @@
     numbers,
     lon_or_obj,
     lat=None,
     lon_name="lon",
     lat_name="lat",
     method=None,
     wrap_lon=None,
+    as_3D=False,
 ):
     """
     internal function to create a mask
     """
 
     if not _is_numeric(numbers):
         raise ValueError("'numbers' must be numeric")
 
     lat_orig = lat
-
     lon, lat = _extract_lon_lat(lon_or_obj, lat, lon_name, lat_name)
 
+    # determine whether unstructured grid
+    # have to do this before np.asarray
+    is_unstructured = False
+    if isinstance(lon, xr.DataArray) and isinstance(lat, xr.DataArray):
+        if len(lon.dims) == 1 and len(lat.dims) == 1:
+            if lon.name != lon.dims[0] and lat.name != lat.dims[0]:
+                is_unstructured = True
+
     lon = np.asarray(lon)
     lat = np.asarray(lat)
 
     # automatically detect whether wrapping is necessary
     if wrap_lon is None:
         msg_add = "Set `wrap_lon=False` to skip this check."
         regions_is_180 = _is_180(*lon_bounds, msg_add=msg_add)
 
         wrap_lon_ = 180 if regions_is_180 else 360
     else:
         wrap_lon_ = wrap_lon
 
-    lon_orig = lon.copy()
     if wrap_lon_:
-        lon = _wrapAngle(lon, wrap_lon_)
+        lon = _wrapAngle(lon, wrap_lon_, is_unstructured=is_unstructured)
 
     if method not in (None, "rasterize", "shapely", "pygeos"):
         msg = "Method must be None or one of 'rasterize', 'shapely' and 'pygeos'."
         raise ValueError(msg)
 
     if method is None:
         method = _determine_method(lon, lat)
@@ -149,37 +173,54 @@
         method = _determine_method(lon, lat)
         if "rasterize" not in method:
             msg = "`lat` and `lon` must be equally spaced to use `method='rasterize'`"
             raise ValueError(msg)
     elif method == "pygeos" and not has_pygeos:
         raise ModuleNotFoundError("No module named 'pygeos'")
 
+    kwargs = {}
     if method == "rasterize":
-        mask = _mask_rasterize(lon, lat, outlines, numbers=numbers)
+        mask_func = _mask_rasterize
     elif method == "rasterize_flip":
-        mask = _mask_rasterize_flip(lon, lat, outlines, numbers=numbers)
+        mask_func = _mask_rasterize_flip
     elif method == "rasterize_split":
-        mask = _mask_rasterize_split(lon, lat, outlines, numbers=numbers)
+        mask_func = _mask_rasterize_split
     elif method == "pygeos":
-        mask = _mask_pygeos(lon, lat, outlines, numbers=numbers)
+        mask_func = _mask_pygeos
+        kwargs = {"is_unstructured": is_unstructured}
     elif method == "shapely":
-        mask = _mask_shapely(lon, lat, outlines, numbers=numbers)
+        mask_func = _mask_shapely
+        kwargs = {"is_unstructured": is_unstructured}
+
+    if as_3D:
+        masks = list()
+        for outline, number in zip(outlines, numbers):
+            mask = mask_func(lon, lat, [outline], numbers=[number], **kwargs)
+
+            # not False required
+            if wrap_lon is not False:
+                # treat the points at -180°E/0°E and -90°N
+                mask = _mask_edgepoints_shapely(
+                    mask, lon, lat, [outline], [number], is_unstructured=is_unstructured
+                )
+            masks.append(mask == number)
+
+        mask = np.stack(masks, axis=0)
 
-    # not False required
-    if wrap_lon is not False:
-        # treat the points at -180°E/0°E and -90°N
-        mask = _mask_edgepoints_shapely(mask, lon, lat, outlines, numbers)
-
-    # create an xr.DataArray
-    if lon.ndim == 1:
-        mask = _create_xarray(mask, lon_orig, lat, lon_name, lat_name)
     else:
-        mask = _create_xarray_2D(mask, lon_or_obj, lat_orig, lon_name, lat_name)
+        mask = mask_func(lon, lat, outlines, numbers=numbers, **kwargs)
 
-    return mask
+        # not False required
+        if wrap_lon is not False:
+            # treat the points at -180°E/0°E and -90°N
+            mask = _mask_edgepoints_shapely(
+                mask, lon, lat, outlines, numbers, is_unstructured=is_unstructured
+            )
+
+    return mask_to_dataarray(mask, lon_or_obj, lat_orig, lon_name, lat_name)
 
 
 def _mask_2D(
     outlines,
     lon_bounds,
     numbers,
     lon_or_obj,
@@ -216,43 +257,56 @@
     lon_or_obj,
     lat=None,
     drop=True,
     lon_name="lon",
     lat_name="lat",
     method=None,
     wrap_lon=None,
+    as_3D=False,
 ):
 
     mask = _mask(
         outlines=outlines,
         lon_bounds=lon_bounds,
         numbers=numbers,
         lon_or_obj=lon_or_obj,
         lat=lat,
         lon_name=lon_name,
         lat_name=lat_name,
         method=method,
         wrap_lon=wrap_lon,
+        as_3D=as_3D,
     )
 
+    if as_3D:
+        mask_3D = _unpack_3D_mask(mask, numbers, drop)
+    else:
+        mask_3D = _unpack_2D_mask(mask, numbers, drop)
+
+    return mask_3D
+
+
+def _unpack_2D_mask(mask, numbers, drop):
+
     isnan = np.isnan(mask.values)
 
     if drop:
         numbers = np.unique(mask.values[~isnan])
         numbers = numbers.astype(int)
 
     # if no regions are found return a 0 x lat x lon mask
     if len(numbers) == 0:
-        mask = mask.expand_dims("region", axis=0).sel(region=slice(0, 0))
+        mask_3D = mask.expand_dims("region", axis=0).sel(region=slice(0, 0))
+        mask_3D = mask_3D.assign_coords(region=("region", numbers))
         msg = (
             "No gridpoint belongs to any region. Returning an empty mask"
-            " with shape {}".format(mask.shape)
+            f" with shape {mask.shape}"
         )
         warnings.warn(msg, UserWarning, stacklevel=3)
-        return mask
+        return mask_3D
 
     mask_3D = list()
     for num in numbers:
         mask_3D.append(mask == num)
 
     mask_3D = xr.concat(mask_3D, dim="region", compat="override", coords="minimal")
     mask_3D = mask_3D.assign_coords(region=("region", numbers))
@@ -260,14 +314,42 @@
     if np.all(isnan):
         msg = "No gridpoint belongs to any region. Returning an all-False mask."
         warnings.warn(msg, UserWarning, stacklevel=3)
 
     return mask_3D
 
 
+def _unpack_3D_mask(mask_3D, numbers, drop):
+
+    any_masked = mask_3D.any(mask_3D.dims[1:])
+
+    if drop:
+        mask_3D = mask_3D.isel(region=any_masked)
+
+        numbers = np.asarray(numbers)[any_masked.values]
+
+    if len(numbers) == 0:
+
+        mask_3D = mask_3D.assign_coords(region=("region", numbers))
+        msg = (
+            "No gridpoint belongs to any region. Returning an empty mask"
+            f" with shape {mask_3D.shape}"
+        )
+        warnings.warn(msg, UserWarning, stacklevel=3)
+        return mask_3D
+
+    mask_3D = mask_3D.assign_coords(region=("region", numbers))
+
+    if not np.any(any_masked):
+        msg = "No gridpoint belongs to any region. Returning an all-False mask."
+        warnings.warn(msg, UserWarning, stacklevel=3)
+
+    return mask_3D
+
+
 def _determine_method(lon, lat):
     """find method to be used -> prefers faster methods"""
 
     if equally_spaced(lon, lat):
         return "rasterize"
 
     if _equally_spaced_on_split_lon(lon) and equally_spaced(lat):
@@ -293,65 +375,63 @@
         lat = lon_or_obj[lat_name]
     else:
         lon = lon_or_obj
 
     return lon, lat
 
 
-def _create_xarray(mask, lon, lat, lon_name, lat_name):
-    """create an xarray DataArray"""
+def mask_to_dataarray(mask, lon_or_obj, lat=None, lon_name="lon", lat_name="lat"):
 
-    # create the xarray output
-    coords = {lat_name: lat, lon_name: lon}
-    mask = xr.DataArray(mask, coords=coords, dims=(lat_name, lon_name), name="region")
+    lon, lat = _extract_lon_lat(lon_or_obj, lat, lon_name, lat_name)
 
-    return mask
+    if sum(isinstance(c, xr.DataArray) for c in (lon, lat)) == 1:
+        raise ValueError("Cannot handle coordinates with mixed types!")
 
+    if not isinstance(lon, xr.DataArray) or not isinstance(lat, xr.DataArray):
+        lon, lat = _numpy_coords_to_dataarray(lon, lat, lon_name, lat_name)
 
-def _create_xarray_2D(mask, lon_or_obj, lat, lon_name, lat_name):
-    """create an xarray DataArray for 2D fields"""
+    ds = lat.coords.merge(lon.coords)
 
-    lon2D, lat2D = _extract_lon_lat(lon_or_obj, lat, lon_name, lat_name)
+    dims = xr.core.variable.broadcast_variables(lat.variable, lon.variable)[0].dims
 
-    if isinstance(lon2D, xr.DataArray):
-        dim1D_names = lon2D.dims
-        dim1D_0 = lon2D[dim1D_names[0]]
-        dim1D_1 = lon2D[dim1D_names[1]]
-    else:
-        dim1D_names = (lon_name + "_idx", lat_name + "_idx")
-        dim1D_0 = np.arange(np.array(lon2D).shape[0])
-        dim1D_1 = np.arange(np.array(lon2D).shape[1])
-
-    # dict with the coordinates
-    coords = {
-        dim1D_names[0]: dim1D_0.data,
-        dim1D_names[1]: dim1D_1.data,
-        lat_name: (
-            dim1D_names,
-            lat2D.data if isinstance(lat2D, xr.DataArray) else lat2D,
-        ),
-        lon_name: (
-            dim1D_names,
-            lon2D.data if isinstance(lon2D, xr.DataArray) else lon2D,
-        ),
-    }
+    # unstructured grids are 1D
+    if mask.ndim - 1 == len(dims):
+        dims = ("region",) + dims
 
-    mask = xr.DataArray(mask, coords=coords, dims=dim1D_names)
+    return ds.assign(mask=(dims, mask)).mask
 
-    return mask
+
+def _numpy_coords_to_dataarray(lon, lat, lon_name, lat_name):
+    # TODO: simplify if passing lon_name and lat_name is no longer supported
+
+    dims2D = (f"{lat_name}_idx", f"{lon_name}_idx")
+
+    lon = np.asarray(lon)
+    dims = dims2D if lon.ndim == 2 else lon_name
+    lon = xr.Dataset(coords={lon_name: (dims, lon)})[lon_name]
+
+    lat = np.asarray(lat)
+    dims = dims2D if lat.ndim == 2 else lat_name
+    lat = xr.Dataset(coords={lat_name: (dims, lat)})[lat_name]
+
+    return lon, lat
 
 
-def _mask_edgepoints_shapely(mask, lon, lat, polygons, numbers, fill=np.NaN):
+def _mask_edgepoints_shapely(
+    mask, lon, lat, polygons, numbers, fill=np.NaN, is_unstructured=False
+):
 
     import shapely.vectorized as shp_vect
 
     # not sure if this is really necessary
-    lon, lat, numbers = _parse_input(lon, lat, polygons, fill, numbers)
+    lon, lat = _parse_input(lon, lat, polygons, fill, numbers)
 
-    LON, LAT, out, shape = _get_LON_LAT_out_shape(lon, lat, fill)
+    LON, LAT, out, shape = _get_LON_LAT_out_shape(
+        lon, lat, fill, is_unstructured=is_unstructured
+    )
 
     mask = mask.flatten()
     mask_unassigned = np.isnan(mask)
 
     # find points at -180°E/0°E
     if lon.min() < 0:
         LON_180W_or_0E = np.isclose(LON, -180.0) & mask_unassigned
@@ -364,68 +444,72 @@
     borderpoints = LON_180W_or_0E | LAT_90S
 
     # return if there are no unassigned gridpoints at -180°E/0°E and -90°N
     if not borderpoints.any():
         return mask.reshape(shape)
 
     # add a tiny offset to get a consistent edge behaviour
-    LON = LON[borderpoints] - 1 * 10 ** -8
-    LAT = LAT[borderpoints] - 1 * 10 ** -10
+    LON = LON[borderpoints] - 1 * 10**-8
+    LAT = LAT[borderpoints] - 1 * 10**-10
 
     # wrap points LON_180W_or_0E: -180°E -> 180°E and 0°E -> 360°E
     LON[LON_180W_or_0E[borderpoints]] += 360
     # shift points at -90°N to -89.99...°N
-    LAT[LAT_90S[borderpoints]] = -90 + 1 * 10 ** -10
+    LAT[LAT_90S[borderpoints]] = -90 + 1 * 10**-10
 
     # "mask[borderpoints][sel] = number" does not work, need to use np.where
     idx = np.where(borderpoints)[0]
     for i, polygon in enumerate(polygons):
         sel = shp_vect.contains(polygon, LON, LAT)
         mask[idx[sel]] = numbers[i]
 
     return mask.reshape(shape)
 
 
-def _mask_pygeos(lon, lat, polygons, numbers, fill=np.NaN):
+def _mask_pygeos(lon, lat, polygons, numbers, fill=np.NaN, is_unstructured=False):
     """create a mask using pygeos.STRtree"""
 
-    lon, lat, numbers = _parse_input(lon, lat, polygons, fill, numbers)
+    lon, lat = _parse_input(lon, lat, polygons, fill, numbers)
 
-    LON, LAT, out, shape = _get_LON_LAT_out_shape(lon, lat, fill)
+    LON, LAT, out, shape = _get_LON_LAT_out_shape(
+        lon, lat, fill, is_unstructured=is_unstructured
+    )
 
     # add a tiny offset to get a consistent edge behaviour
-    LON = LON - 1 * 10 ** -8
-    LAT = LAT - 1 * 10 ** -10
+    LON = LON - 1 * 10**-8
+    LAT = LAT - 1 * 10**-10
 
     # convert shapely points to pygeos
     poly_pygeos = pygeos.from_shapely(polygons)
     points_pygeos = pygeos.points(LON, LAT)
 
     tree = pygeos.STRtree(points_pygeos)
     a, b = tree.query_bulk(poly_pygeos, predicate="contains")
 
-    for i, (polygon, number) in enumerate(zip(poly_pygeos, numbers)):
+    for i, number in enumerate(numbers):
 
         out[b[a == i]] = number
 
     return out.reshape(shape)
 
 
-def _mask_shapely(lon, lat, polygons, numbers, fill=np.NaN):
+def _mask_shapely(lon, lat, polygons, numbers, fill=np.NaN, is_unstructured=False):
     """create a mask using shapely.vectorized.contains"""
 
     import shapely.vectorized as shp_vect
 
-    lon, lat, numbers = _parse_input(lon, lat, polygons, fill, numbers)
+    lon, lat = _parse_input(lon, lat, polygons, fill, numbers)
 
-    LON, LAT, out, shape = _get_LON_LAT_out_shape(lon, lat, fill)
+    LON, LAT, out, shape = _get_LON_LAT_out_shape(
+        lon, lat, fill, is_unstructured=is_unstructured
+    )
 
     # add a tiny offset to get a consistent edge behaviour
-    LON = LON - 1 * 10 ** -8
-    LAT = LAT - 1 * 10 ** -10
+    LON = LON - 1 * 10**-8
+    LAT = LAT - 1 * 10**-10
 
     for i, polygon in enumerate(polygons):
         sel = shp_vect.contains(polygon, LON, LAT)
         out[sel] = numbers[i]
 
     return out.reshape(shape)
 
@@ -433,27 +517,24 @@
 def _parse_input(lon, lat, coords, fill, numbers):
 
     lon = np.asarray(lon)
     lat = np.asarray(lat)
 
     n_coords = len(coords)
 
-    if numbers is None:
-        numbers = range(n_coords)
-    else:
-        if len(numbers) != n_coords:
-            raise ValueError("`numbers` and `coords` must have the same length.")
+    if len(numbers) != n_coords:
+        raise ValueError("`numbers` and `coords` must have the same length.")
 
     if fill in numbers:
         raise ValueError("The fill value should not be one of the region numbers.")
 
-    return lon, lat, numbers
+    return lon, lat
 
 
-def _get_LON_LAT_out_shape(lon, lat, fill):
+def _get_LON_LAT_out_shape(lon, lat, fill, is_unstructured=False):
 
     if lon.ndim != lat.ndim:
         raise ValueError(
             f"Equal number of dimensions required, found "
             f"lon.ndim={lon.ndim} & lat.ndim={lat.ndim}."
         )
 
@@ -461,15 +542,17 @@
 
     if ndim == 2 and lon.shape != lat.shape:
         raise ValueError(
             "2D lon and lat coordinates need to have the same shape, found "
             f"lon.shape={lon.shape} & lat.shape={lat.shape}."
         )
 
-    if ndim == 1:
+    if is_unstructured:
+        LON, LAT = lon, lat
+    elif ndim == 1:
         LON, LAT = np.meshgrid(lon, lat)
     elif ndim == 2:
         LON, LAT = lon, lat
     else:
         raise ValueError(
             f"1D or 2D data required - found {ndim} dimensions. Use `squeeze` to remove"
             " axes of length 1 - e.g. `mask(lon.squeeze(), lat.squeeze())`."
@@ -483,15 +566,15 @@
     out = np.empty(shape=np.prod(shape))
     out.fill(fill)
 
     return LON, LAT, out, shape
 
 
 def _transform_from_latlon(lon, lat):
-    """perform an affine tranformation to the latitude/longitude coordinates"""
+    """perform an affine transformation to the latitude/longitude coordinates"""
 
     from affine import Affine
 
     lat = np.asarray(lat)
     lon = np.asarray(lon)
 
     d_lon = lon[1] - lon[0]
@@ -503,49 +586,52 @@
 
 
 def _mask_rasterize_flip(lon, lat, polygons, numbers, fill=np.NaN, **kwargs):
 
     split_point = _find_splitpoint(lon)
     flipped_lon = np.hstack((lon[split_point:], lon[:split_point]))
 
-    mask = _mask_rasterize(flipped_lon, lat, polygons, numbers=numbers)
+    mask = _mask_rasterize(flipped_lon, lat, polygons, numbers=numbers, **kwargs)
 
     # revert the mask
     return np.hstack((mask[:, -split_point:], mask[:, :-split_point]))
 
 
 def _mask_rasterize_split(lon, lat, polygons, numbers, fill=np.NaN, **kwargs):
 
     split_point = _find_splitpoint(lon)
     lon_l, lon_r = lon[:split_point], lon[split_point:]
 
-    mask_l = _mask_rasterize(lon_l, lat, polygons, numbers=numbers)
-    mask_r = _mask_rasterize(lon_r, lat, polygons, numbers=numbers)
+    mask_l = _mask_rasterize(lon_l, lat, polygons, numbers=numbers, **kwargs)
+    mask_r = _mask_rasterize(lon_r, lat, polygons, numbers=numbers, **kwargs)
 
     return np.hstack((mask_l, mask_r))
 
 
 def _mask_rasterize(lon, lat, polygons, numbers, fill=np.NaN, **kwargs):
     """Rasterize a list of (geometry, fill_value) tuples onto the given coordinates.
 
-    This only works for 1D lat and lon arrays.
-
-    for internal use: does not check valitity of input
+    This only works for regularly spaced 1D lat and lon arrays.
     """
+
+    lon, lat = _parse_input(lon, lat, polygons, fill, numbers)
+
     # subtract a tiny offset: https://github.com/mapbox/rasterio/issues/1844
-    lon = np.asarray(lon) - 1 * 10 ** -8
-    lat = np.asarray(lat) - 1 * 10 ** -10
+    lon = lon - 1 * 10**-8
+    lat = lat - 1 * 10**-10
 
     return _mask_rasterize_no_offset(lon, lat, polygons, numbers, fill, **kwargs)
 
 
-def _mask_rasterize_no_offset(lon, lat, polygons, numbers, fill=np.NaN, **kwargs):
+def _mask_rasterize_no_offset(
+    lon, lat, polygons, numbers, fill=np.NaN, dtype=float, **kwargs
+):
     """Rasterize a list of (geometry, fill_value) tuples onto the given coordinates.
 
-    This only works for 1D lat and lon arrays.
+    This only works for regularly spaced 1D lat and lon arrays.
 
     for internal use: does not check valitity of input
     """
     # TODO: use only this function once https://github.com/mapbox/rasterio/issues/1844
     # is resolved
 
     from rasterio import features
@@ -556,12 +642,12 @@
     out_shape = (len(lat), len(lon))
 
     raster = features.rasterize(
         shapes,
         out_shape=out_shape,
         fill=fill,
         transform=transform,
-        dtype=float,
+        dtype=dtype,
         **kwargs,
     )
 
     return raster
```

### Comparing `regionmask-0.8.0/regionmask/core/plot.py` & `regionmask-0.9.0/regionmask/core/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,63 +5,121 @@
 from .utils import _deprecate_positional, _flatten_polygons
 
 
 def _polygons_coords(polygons):
 
     coords = []
     for p in polygons:
-        coords += [np.asarray(p.exterior)[:, :2]] + [
-            np.asarray(i)[:, :2] for i in p.interiors
+        coords += [np.asarray(p.exterior.coords)[:, :2]] + [
+            np.asarray(i.coords)[:, :2] for i in p.interiors
         ]
 
     return coords
 
 
-def _draw_poly(ax, polygons, subsample=False, **kwargs):
+def _get_tolerance(coords):
+
+    mx = np.max(np.abs(coords))
+    return 1 if mx == 0 else max(10 ** (int(np.log10(mx)) - 2), 1)
+
+
+def _draw_poly(ax, polygons, tolerance=None, **kwargs):
     """
     draw the outline of the regions
 
     """
 
     from matplotlib.collections import LineCollection
 
     polygons = _flatten_polygons(polygons)
     coords = _polygons_coords(polygons)
 
-    if subsample:
-        coords = [_subsample(coord) if len(coord) < 10 else coord for coord in coords]
+    if tolerance == "auto":
+        tolerance = _get_tolerance(np.concatenate(coords, 0))
+
+    if tolerance is not None:
+        coords = [segmentize(coord, tolerance) for coord in coords]
 
     color = kwargs.pop("color", "0.1")
 
     lc = LineCollection(coords, color=color, **kwargs)
     ax.add_collection(lc)
     ax.autoscale_view()
 
     # from matplotlib.path import Path
     # import matplotlib.patches as patches
     # paths = [Path(coord) for coord in coords]
-    # patchs = [patches.PathPatch(path, facecolor='none', **kwargs) for path in paths]
-    # [ax.add_patch(patch) for patch in patchs]
+    # patches = [patches.PathPatch(path, facecolor='none', **kwargs) for path in paths]
+    # [ax.add_patch(patch) for patch in patches]
     # ax.autoscale_view()
 
 
-def _subsample(outl, num=50):
-    # assumes outl is closed - i.e outl[:-1] == outl[0]
-    out = np.linspace(outl[:-1], outl[1:], num=num, endpoint=False, axis=1)
-    out = out.reshape(-1, 2)
-    return np.vstack([out, outl[-1]])
+def segmentize(coords, tolerance):
+    """Adds vertices to line segments based on tolerance.
+
+    Additional vertices will be added to every line segment in input coordinates
+    so that segments are no greater than tolerance. New vertices will evenly
+    subdivide each segment.
+
+    Parameters
+    ----------
+    coords : ndarray
+        2D coordinate array of shape N x 2
+    tolerance : float
+        Additional vertices will be added so that all line segments are no
+        greater than this value. Must be greater than 0.
+
+    See Also
+    --------
+    pygeos.segmentize
+    """
+
+    coords = np.asarray(coords)
+    dist = np.sqrt(np.sum((coords[1:] - coords[:-1]) ** 2, axis=1))
+    num = np.ceil(dist / tolerance).astype(int)
+
+    if (num == 1).all():
+        return coords
+
+    out = list()
+    for i in range(len(coords) - 1):
+        if num[i] > 1:
+            out.append(
+                np.linspace(coords[i, :], coords[i + 1, :], num=num[i], endpoint=False)
+            )
+        else:
+            out.append(coords[i : i + 1, :])
+
+    out.append(coords[-1:, :])
+
+    return np.concatenate(out, 0)
 
 
 def _check_unused_kws(add, kws, feature_name, kws_name):
     if (kws is not None) and (not add):
         warnings.warn(
             f"'{kws_name}' are passed but '{feature_name}' is False.", RuntimeWarning
         )
 
 
+def _maybe_gca(**kwargs):
+
+    import matplotlib.pyplot as plt
+
+    # can call gcf unconditionally: either it exists or would be created by plt.axes
+    f = plt.gcf()
+
+    # only call gca if an active axes exists
+    if f.axes:
+        # can not pass kwargs to active axes
+        return plt.gca()
+
+    return plt.axes(**kwargs)
+
+
 @_deprecate_positional
 def _plot(
     self,
     ax=None,
     projection=None,
     regions=None,
     add_label=True,
@@ -73,70 +131,91 @@
     resolution="110m",
     subsample=None,
     add_land=False,
     coastline_kws=None,
     ocean_kws=None,
     land_kws=None,
     label_multipolygon="largest",
+    tolerance="auto",
     **kwargs,
 ):
     """
     plot map with with region outlines
 
     Parameters
     ----------
     ax : axes handle, optional
-        If given uses existing axes (needs to be a cartopy axes). If not
-        given, creates a new axes with the specified projection.
+        If given uses existing axes (needs to be a cartopy GeoAxes). If not given,
+        uses the current axes or creates a new axes with the specified projection.
+
     projection : cartopy projection, default: None
         Defines the projection of the map. If None uses 'PlateCarree'.
         See cartopy home page.
+
     regions : list of int or str | 'all', default: 'all'
         Deprecated - subset regions before plotting, i.e. use `r[regions].plot()`
         instead of `r.plot(regions=regions)`.
         Select the regions (by number, abbrev or name, can be mixed)
         that should be drawn.
+
     add_label : bool, default: True
         If true labels the regions.
+
     label : 'number' | 'name' | 'abbrev', default: 'number'
         If 'number' labels the regions with numbers, if 'name' uses
         the long name of the regions, if 'short_name' uses
         abbreviations of the regions.
+
     add_coastlines : bool, default: None
         If None or true plots coastlines. See coastline_kws.
+
     add_ocean : bool,  default: False
         If true adds the ocean feature. See ocean_kws.
+
     line_kws : dict, default: None
         Arguments passed to plot.
+
     text_kws : dict, default, None
         Arguments passed to the labels (ax.text).
+
     resolution : '110m' | '50m' | '10m', default: '110m'
         Specify the resolution of the coastline and the ocean dataset.
         See cartopy for details.
+
     subsample : None or bool, default: None
-        If True subsamples the outline of the coords to make better
-        looking plots on certain maps. If False does not subsample.
-        If None, infers the subsampling -> if the input is given as
-        array subsamples if it is given as (Multi)Polygons does not
-        subsample.
+        Deprecated, use tolerance.
+
     add_land : bool, default: False
         If true adds the land feature. See land_kws.
+
     coastline_kws : dict, default: None
         Arguments passed to ``ax.coastlines()``. If None uses ``color="0.4"`` and
         ``lw=0.5``.
+
     ocean_kws : dict, default: None
         Arguments passed to ``ax.add_feature(OCEAN)``. Per default uses the cartopy
         ocean color and ``zorder=0.9, lw=0``.
+
     land_kws : dict, default: None
         Arguments passed to ``ax.add_feature(LAND)``. Per default uses the cartopy
         land color and ``zorder=0.9, lw=0``.
+
     label_multipolygon : 'largest' | 'all', default: 'largest'.
         If 'largest' only adds a text label for the largest Polygon of a
         MultiPolygon. If 'all' adds text labels to all of them.
 
+    tolerance : None | 'auto' | float, default: 'auto'.
+        Maximum length of drawn line segments. Can lead to better looking plots on
+        certain maps.
+
+        - None: draw original coordinates
+        - float > 0: the maximum (euclidean) length of each line segment.
+        - 'auto': The tolerance is automatically determined based on the log10 of the
+          largest absolute coordinate. Defaults to 1 for lat/ lon coordinates.
+
     Returns
     -------
     ax : axes handle
 
     Notes
     -----
     plot internally calls :py:func:`Regions.plot_regions`.
@@ -166,30 +245,42 @@
 
     # set add_coastlines=True in the fcn signature after the deprecation period
     if add_coastlines is None:
         add_coastlines = True
 
     import cartopy.crs as ccrs
     import cartopy.feature as cfeature
-    import matplotlib.pyplot as plt
+    from cartopy.mpl import geoaxes
 
     NEF = cfeature.NaturalEarthFeature
 
     if label_multipolygon not in ["all", "largest"]:
         raise ValueError("'label_multipolygon' must be one of 'all' and 'largest'")
 
     _check_unused_kws(add_coastlines, coastline_kws, "add_coastlines", "coastline_kws")
     _check_unused_kws(add_ocean, ocean_kws, "add_ocean", "ocean_kws")
     _check_unused_kws(add_land, land_kws, "add_land", "land_kws")
 
     if projection is None:
         projection = ccrs.PlateCarree()
 
+    if ax is not None and not isinstance(ax, geoaxes.GeoAxes):
+        raise TypeError(
+            "The passed axes (``ax``) is not a cartopy GeoAxes. "
+            "Either provide a GeoAxes or use ``plot_region``"
+        )
+
     if ax is None:
-        ax = plt.axes(projection=projection)
+        ax = _maybe_gca(projection=projection)
+
+    if not isinstance(ax, geoaxes.GeoAxes):
+        raise TypeError(
+            "The current axes (``plt.gca()``) is not a cartopy GeoAxes. "
+            "Either provide a GeoAxes or use ``plot_region``"
+        )
 
     if ocean_kws is None:
         ocean_kws = dict(color=cfeature.COLORS["water"], zorder=0.9, lw=0)
 
     if land_kws is None:
         land_kws = dict(color=cfeature.COLORS["land"], zorder=0.9, lw=0)
 
@@ -214,14 +305,15 @@
         regions=regions,
         add_label=add_label,
         label=label,
         line_kws=line_kws,
         text_kws=text_kws,
         subsample=subsample,
         label_multipolygon=label_multipolygon,
+        tolerance=tolerance,
     )
 
     return ax
 
 
 @_deprecate_positional
 def _plot_regions(
@@ -230,49 +322,63 @@
     regions=None,
     add_label=True,
     label="number",
     line_kws=None,
     text_kws=None,
     subsample=None,
     label_multipolygon="largest",
+    tolerance="auto",
 ):
     """
     plot map with with srex regions
 
     Parameters
     ----------
     ax : axes handle, optional
-        If given, uses existing axes. If not given, creates a new axes.
-        Note: in contrast to plot this does not create a cartopy axes.
+        If given, uses existing axes. If not given, uses the current axes or creates new
+        axes. In contrast to plot this does not create a cartopy axes.
+
     regions : list of int or str | 'all', default: "all"
         Deprecated - subset regions before plotting, i.e. use `r[regions].plot()`
         instead of `r.plot(regions=regions)`.
         Select the regions (by number, abbrev or name, can be mixed)
         that should be drawn.
+
     add_label : bool
         If true labels the regions. Optional, default True.
+
     label : 'number' | 'name' | 'abbrev', optional
         If 'number' labels the regions with numbers, if 'name' uses
         the long name of the regions, if 'short_name' uses
         abbreviations of the regions. Default 'number'.
+
     line_kws : dict, optional
         Arguments passed to plot.
+
     text_kws : dict, optional
         Arguments passed to the labels (ax.text).
+
     subsample : None or bool, optional
-        If True subsamples the outline of the coords to make better
-        looking plots on certain maps. If False does not subsample.
-        If None, infers the subsampling -> if the input is given as
-        array subsamples if it is given as (Multi)Polygons does not
-        subsample.
+        Deprecated, use tolerance.
+
     label_multipolygon : 'largest' | 'all', optional
         If 'largest' only adds a text label for the largest Polygon of a
         MultiPolygon. If 'all' adds text labels to all of them. Default:
         'largest'.
 
+    tolerance : None | 'auto' | float, default: 'auto'.
+        Maximum length of drawn line segments. Can lead to better looking plots on
+        certain maps.
+
+        - None: draw original coordinates
+        - float > 0: the maximum (euclidean) length of each line segment.
+        - 'auto': None if a matplotlib axes is passed. If a cartopy GeoAxes is passed
+          the tolerance is automatically determined based on the log10 of the
+          largest absolute coordinate. Defaults to 1 for lat/ lon coordinates.
+
     Returns
     -------
     ax : axes handle
 
     """
 
     if regions is not None:
@@ -280,57 +386,64 @@
             "The 'regions' keyword has been deprecated. Subset regions before plotting,"
             " i.e. use `r[regions].plot()` instead of `r.plot(regions=regions)`.",
             FutureWarning,
         )
     else:
         regions = "all"
 
+    if subsample is not None:
+        warnings.warn(
+            "The 'subsample' keyword has been deprecated. Use ``tolerance`` instead.",
+            FutureWarning,
+        )
+
     import matplotlib.pyplot as plt
 
+    is_geoaxes = False
     try:
         import cartopy.crs as ccrs
         from cartopy.mpl import geoaxes
 
-        has_cartopy = True
+        is_geoaxes = isinstance(ax, geoaxes.GeoAxes)
     except ImportError:
-        has_cartopy = False
+        pass
 
     if label_multipolygon not in ["all", "largest"]:
         raise ValueError("'label_multipolygon' must be one of 'all' and 'largest'")
 
     _check_unused_kws(add_label, text_kws, "add_label", "text_kws")
 
     if ax is None:
         ax = plt.gca()
 
-    if has_cartopy and isinstance(ax, geoaxes.GeoAxes):
+    if is_geoaxes:
         trans = ccrs.PlateCarree()
     else:
         trans = ax.transData
 
     if regions == "all":
         regions = self.numbers
     else:
         regions = self.map_keys(regions)
 
     if np.isscalar(regions):
         regions = [regions]
 
-    if subsample is None:
-        subsample = not self._is_polygon
-
     if line_kws is None:
         line_kws = dict()
 
     if text_kws is None:
         text_kws = dict()
 
+    if tolerance == "auto" and not is_geoaxes:
+        tolerance = None
+
     # draw the outlines
     polygons = [self[i].polygon for i in regions]
-    _draw_poly(ax, polygons, subsample=subsample, transform=trans, **line_kws)
+    _draw_poly(ax, polygons, tolerance=tolerance, transform=trans, **line_kws)
 
     if add_label:
 
         va = text_kws.pop("va", "center")
         ha = text_kws.pop("ha", "center")
         col = text_kws.pop("backgroundcolor", "0.85")
         clip_on = text_kws.pop("clip_on", True)
@@ -387,14 +500,20 @@
 
     if not mask_3D.ndim == 3:
         raise ValueError(f"``mask_3D`` must have 3 dimensions, found {mask_3D.ndim}")
 
     if "region" not in mask_3D.coords:
         raise ValueError("``mask_3D`` must contain the dimension 'region'")
 
+    if (mask_3D.sum("region") > 1).any():
+        warnings.warn(
+            "Found overlapping regions which cannot correctly be displayed on a 2D map",
+            RuntimeWarning,
+        )
+
     # flatten the mask
     mask_2D = (mask_3D * mask_3D.region).sum("region")
 
     # mask all gridpoints not belonging to any region
     mask_2D = mask_2D.where(mask_3D.any("region"))
 
     return mask_2D.plot.pcolormesh(**kwargs)
```

### Comparing `regionmask-0.8.0/regionmask/core/regions.py` & `regionmask-0.9.0/regionmask/core/regions.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,88 +2,99 @@
 
 # Author: Mathias Hauser
 # Date:
 
 import copy
 from collections import OrderedDict
 
+import geopandas as gp
 import numpy as np
+import pandas as pd
 from shapely.geometry import MultiPolygon, Polygon
 
 from .formatting import _display
 from .mask import _inject_mask_docstring, _mask_2D, _mask_3D
 from .plot import _plot, _plot_regions
 from .utils import _is_180, _is_numeric, _maybe_to_dict, _sanitize_names_abbrevs
 
 
 class Regions:
     """
     class for plotting regions and creating region masks
+
+    Parameters
+    ----------
+    outlines : iterable or dict of: Nx2 array of vertices, Polygon or MultiPolygon
+        List of the coordinates of the vertices (outline) of the region as
+        shapely Polygon/ MultiPolygon or list.
+    numbers : iterable of int, optional
+        List of numerical indices for every region. Default: range(0, len(outlines))
+    names : iterable or dict of string, optional
+        Long name of each region. Default: ["Region0", .., "RegionN"]
+    abbrevs : iterable or dict of string, optional
+        Abbreviations of each region. Default: ["r0", ..., "rN"]
+    name : string, optional
+        Name of the collection of regions. Default: "unnamed"
+    source : string, optional
+        Source of the region definitions. Default: "".
+    overlap : bool, default: False
+        Indicates if (some of) the regions overlap. If True ``mask_3D`` will ensure
+        overlapping regions are correctly assigned to grid points while ``mask`` will
+        error (because overlapping regions cannot be represented by a 2D mask).
+
+        If False (default) assumes non-overlapping regions. Grid points will
+        silently be assigned to the region with the higher number (this may change
+        in a future version of regionmask).
+
+        There is (currently) no automatic detection of overlapping regions.
+
+    Examples
+    --------
+    Create your own ``Regions``::
+
+        from regionmask import Regions
+
+        name = 'Example'
+        numbers = [0, 1]
+        names = ['Unit Square1', 'Unit Square2']
+        abbrevs = ['uSq1', 'uSq2']
+
+        outl1 = ((0, 0), (0, 1), (1, 1.), (1, 0))
+        outl2 = ((0, 1), (0, 2), (1, 2.), (1, 1))
+        outlines = [outl1, outl2]
+
+        r = Regions(outlines, numbers, names, abbrevs, name)
+
+    It's also possible to pass shapely Poylgons::
+
+        from shapely.geometry import Polygon
+
+        numbers = [1, 2]
+        names = {1:'Unit Square1', 2: 'Unit Square2'}
+        abbrevs = {1:'uSq1', 2:'uSq2'}
+        poly = {1: Polygon(outl1), 2: Polygon(outl2)}
+
+        r = Regions(outlines, numbers, names, abbrevs, name)
+
+        # arguments are now optional
+        r = Regions(outlines)
+
     """
 
     def __init__(
         self,
         outlines,
         numbers=None,
         names=None,
         abbrevs=None,
         name="unnamed",
         source=None,
+        overlap=False,
     ):
 
-        """
-        Parameters
-        ----------
-        outlines : iterable or dict of: Nx2 array of vertices, Polygon or MultiPolygon
-            List of the coordinates of the vertices (outline) of the region as
-            shapely Polygon/ MultiPolygon or list.
-        numbers : iterable of int, optional
-            List of numerical indices for every region. Default: range(0, len(outlines))
-        names : iterable or dict of string, optional
-            Long name of each region. Default: ["Region0", .., "RegionN"]
-        abbrevs : iterable or dict of string, optional
-            Abbreviations of each region. Default: ["r0", ..., "rN"]
-        name : string, optional
-            Name of the collection of regions. Default: "unnamed"
-        source : string, optional
-            Source of the region definitions. Default: "".
-
-        Examples
-        --------
-        Create your own ``Regions``::
-
-            from regionmask import Regions
-
-            name = 'Example'
-            numbers = [0, 1]
-            names = ['Unit Square1', 'Unit Square2']
-            abbrevs = ['uSq1', 'uSq2']
-
-            outl1 = ((0, 0), (0, 1), (1, 1.), (1, 0))
-            outl2 = ((0, 1), (0, 2), (1, 2.), (1, 1))
-            outlines = [outl1, outl2]
-
-            r = Regions(outlines, numbers, names, abbrevs, name)
-
-        It's also possible to pass shapely Poylgons::
-
-            from shapely.geometry import Polygon
-
-            numbers = [1, 2]
-            names = {1:'Unit Square1', 2: 'Unit Square2'}
-            abbrevs = {1:'uSq1', 2:'uSq2'}
-            poly = {1: Polygon(outl1), 2: Polygon(outl2)}
-
-            r = Regions(outlines, numbers, names, abbrevs, name)
-
-            # arguments are now optional
-            r = Regions(outlines)
-
-        """
-
         if numbers is None:
             numbers = range(len(outlines))
 
         if not _is_numeric(numbers):
             raise ValueError("'numbers' must be numeric")
 
         outlines = _maybe_to_dict(numbers, outlines)
@@ -95,14 +106,15 @@
 
         for n in sorted(numbers):
             regions[n] = _OneRegion(n, names[n], abbrevs[n], outlines[n])
 
         self.regions = regions
         self.name = name
         self.source = source
+        self.overlap = overlap
 
     def __getitem__(self, key):
         """subset of Regions or Region
 
         Parameters
         ----------
         key : (list of) int or string
@@ -212,19 +224,14 @@
 
     @property
     def centroids(self):
         """list of the center of mass of the regions"""
         return self.combiner("centroid")
 
     @property
-    def _is_polygon(self):
-        """is there at least one region was passed as (Multi)Polygon"""
-        return np.any(np.array(self.combiner("_is_polygon")))
-
-    @property
     def bounds(self):
         """list of the bounds of the regions (min_lon, min_lat, max_lon, max_lat)"""
         return self.combiner("bounds")
 
     @property
     def bounds_global(self):
         """global bounds over all regions (min_lon, min_lat, max_lon, max_lat)"""
@@ -282,14 +289,20 @@
         lat=None,
         lon_name="lon",
         lat_name="lat",
         method=None,
         wrap_lon=None,
     ):
 
+        if self.overlap:
+            raise ValueError(
+                "Creating a 2D mask with overlapping regions yields wrong results. "
+                "Set ``region.overlap = False`` to create a 2D mask anyway."
+            )
+
         return _mask_2D(
             outlines=self.polygons,
             lon_bounds=self.bounds_global[::2],
             numbers=self.numbers,
             lon_or_obj=lon_or_obj,
             lat=lat,
             lon_name=lon_name,
@@ -318,116 +331,237 @@
             lon_or_obj=lon_or_obj,
             lat=lat,
             drop=drop,
             lon_name=lon_name,
             lat_name=lat_name,
             method=method,
             wrap_lon=wrap_lon,
+            as_3D=self.overlap,
         )
 
         numbers = mask_3D.region.values
         abbrevs = self[numbers].abbrevs
         names = self[numbers].names
 
         mask_3D = mask_3D.assign_coords(
             abbrevs=("region", abbrevs), names=("region", names)
         )
 
         return mask_3D
 
     mask_3D.__doc__ = _inject_mask_docstring(is_3D=True, gp_method=False)
 
+    def to_dataframe(self):
+        """Convert this region into a pandas.DataFrame, excluding polygons.
+
+        See Also
+        --------
+        from_geopandas, Regions.to_geodataframe, Regions.to_geoseries, Regions.from_geodataframe
+
+        """
+
+        data = dict(
+            numbers=self.numbers,
+            abbrevs=self.abbrevs,
+            names=self.names,
+        )
+
+        df = pd.DataFrame.from_dict(data).set_index("numbers")
+        return df
+
+    def to_geodataframe(self):
+        """Convert this region into a geopandas.GeoDataFrame.
+
+        Use ``Regions.from_geodataframe`` to round-trip a geodataframe created with
+        this method.
+
+        See Also
+        --------
+        from_geopandas, Regions.to_dataframe, Regions.to_geoseries, Regions.from_geodataframe
+
+        """
+
+        data = dict(
+            numbers=self.numbers,
+            abbrevs=self.abbrevs,
+            names=self.names,
+            geometry=self.polygons,
+        )
+
+        df = gp.GeoDataFrame.from_dict(data).set_index("numbers")
+        df.attrs["name"] = self.name
+        df.attrs["source"] = self.source
+        df.attrs["overlap"] = self.overlap
+
+        return df
+
+    def to_geoseries(self):
+        """Convert this region into a geopandas.GeoSeries.
+
+        See Also
+        --------
+        from_geopandas, Regions.to_dataframe, Regions.to_geodataframe, Regions.from_geodataframe
+
+        """
+
+        df = gp.GeoSeries(self.polygons, index=self.numbers)
+        df.attrs["name"] = self.name
+        df.attrs["source"] = self.source
+        df.attrs["overlap"] = self.overlap
+
+        return df
+
+    @classmethod
+    def from_geodataframe(cls, df, *, name=None, source=None, overlap=None):
+        """
+        Convert a  ``geopandas.GeoDataFrame`` created with ``to_geodataframe`` back to
+        ``regionmask.Region`` (round trip)
+
+        Parameters
+        ----------
+        df : geopandas.GeoDataFrame
+            GeoDataFrame to be transformed to a Regions class.
+
+        name : str, optional
+            name of the Regions. If None uses ``df.attrs.get("name", "unnamed")``.
+
+        source : str, optional
+            Source of the shapefile.  If None uses ``df.attrs.get("source")``.
+
+        overlap : bool, default: None
+            Indicates if (some of) the regions overlap. If None uses
+            ``df.attrs.get("overlap")``. If True ``mask_3D`` will ensure
+            overlapping regions are correctly assigned to grid points while ``mask``
+            will error (because overlapping regions cannot be represented by a 2D mask).
+
+            If False assumes non-overlapping regions. Grid points will silently be
+            assigned to the region with the higher number (this may change in a future
+            version).
+
+            There is (currently) no automatic detection of overlapping regions.
+
+        Returns
+        -------
+        regionmask.core.regions.Regions
+
+        See Also
+        --------
+        from_geopandas, Regions.to_dataframe, Regions.to_geodataframe, Regions.to_geoseries
+        """
+
+        from regionmask.core._geopandas import _from_geopandas
+
+        if name is None:
+            name = df.attrs.get("name", "unnamed")
+
+        if source is None:
+            source = df.attrs.get("source")
+
+        if overlap is None:
+            overlap = df.attrs.get("overlap", False)
+
+        return _from_geopandas(
+            df,
+            numbers=None,
+            names="names",
+            abbrevs="abbrevs",
+            name=name,
+            source=source,
+            overlap=overlap,
+        )
+
 
 # add the plotting methods
 Regions.plot = _plot
 Regions.plot_regions = _plot_regions
 
 
 # =============================================================================
 
 
 class _OneRegion:
     """a single Region, used as member of 'Regions'"""
 
-    def __init__(self, number, name, abbrev, outline, centroid=None):
+    def __init__(self, number, name, abbrev, outline):
         """
         Parameters
         ----------
         number : int
             Number of this region.
         name : string
             Long name of this region.
         abbrev : string
             Abbreviation of this region.
         outline : Nx2 array of vertices, Polygon or MultiPolygon
             Coordinates/ outline of the region as shapely Polygon/
             MultiPolygon or list.
-        centroid : 1x2 iterable, optional.
-            Center of mass of this region. If not provided is calculated
-            as (Multi)Polygon.centroid. Position of the label on map plots.
 
         Examples
         --------
         ``_OneRegion`` can be created with numpy-style outlines::
 
             outl = ((0, 0), (0, 1), (1, 1.), (1, 0))
             r = _OneRegion(1, 'Unit Square', 'USq', outl)
 
         or by passing shapely Polygons::
 
             from shapely.geometry import Polygon
 
             poly = Polygon(outl)
-            r = _OneRegion(1, 'Unit Square', 'USq', poly, centroid=[0.5, 0.75])
+            r = _OneRegion(1, 'Unit Square', 'USq', poly)
         """
 
         self.number = number
         self.name = name
         self.abbrev = abbrev
+        self._centroid = None
+        self._bounds = None
 
-        self._is_polygon = isinstance(outline, (Polygon, MultiPolygon))
-
-        if self._is_polygon:
+        if isinstance(outline, (Polygon, MultiPolygon)):
             self._polygon = outline
             self._coords = None
         else:
             self._polygon = None
             outline = np.asarray(outline)
 
             if outline.ndim != 2:
                 raise ValueError("Outline must be 2D")
 
             if outline.shape[1] != 2:
                 raise ValueError("Outline must have Nx2 elements")
 
             self._coords = np.array(outline)
 
+    def __repr__(self):
+
+        klass = type(self).__name__
+        return f"<regionmask.{klass}: {self.name} ({self.abbrev} / {self.number})>"
+
+    @property
+    def centroid(self):
+
         # the Polygon Centroid is much stabler
-        if centroid is None:
+        if self._centroid is None:
             poly = self.polygon
             if isinstance(poly, MultiPolygon):
                 # find the polygon with the largest area and assig as centroid
                 area = 0
-                for p in poly:
+                for p in poly.geoms:
                     if p.area > area:
                         centroid = np.array(p.centroid.coords).squeeze()
                         area = p.area
 
                 # another possibility; errors on self-intersecting polygon
                 # centroid = np.array(poly.representative_point().coords).squeeze()
             else:
                 centroid = np.array(poly.centroid.coords).squeeze()
 
-        self.centroid = centroid
+            self._centroid = centroid
 
-        self._bounds = None
-
-    def __repr__(self):
-        msg = "Region: {} ({} / {})\ncenter: {}"
-        return msg.format(self.name, self.abbrev, self.number, self.centroid)
+        return self._centroid
 
     @property
     def polygon(self):
         """shapely Polygon or MultiPolygon of the region"""
 
         if self._polygon is None:
             self._polygon = Polygon(self.coords)
@@ -439,21 +573,19 @@
 
         if self._coords is None:
 
             # make an array of polygons
             if isinstance(self._polygon, Polygon):
                 polys = [self._polygon]
             else:
-                polys = list(self._polygon)
+                polys = list(self._polygon.geoms)
 
             # separate the single polygons with NaNs
-            nan = np.ones(shape=(1, 2)) * np.nan
-            lst = list()
-            for poly in polys:
-                lst.append(np.vstack((np.array(poly.exterior.coords), nan)))
+            nan = np.full((1, 2), np.nan)
+            lst = [np.vstack((np.array(poly.exterior.coords), nan)) for poly in polys]
 
             # remove the very last NaN
             self._coords = np.vstack(lst)[:-1, :]
 
         return self._coords
 
     @property
```

### Comparing `regionmask-0.8.0/regionmask/core/utils.py` & `regionmask-0.9.0/regionmask/core/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     if error not in ["raise", "skip"]:
         raise ValueError("'error' must be one of 'raise' and 'skip'")
 
     polys = []
     for p in polygons:
         if isinstance(p, MultiPolygon):
-            polys += list(p)
+            polys += list(p.geoms)
         elif isinstance(p, Polygon):
             polys += [p]
         else:
             if error == "raise":
                 msg = f"Expected 'Polygon' or 'MultiPolygon', found {type(p)}"
                 raise TypeError(msg)
 
@@ -51,35 +51,29 @@
             raise ValueError("`numbers` and `values` do not have the same length.")
 
         values = _maybe_to_dict(numbers, values)
 
     return values
 
 
-# -----------------------------------------------------------------------------
-
-
 def _wrapAngle360(lon):
     """wrap angle to `[0, 360[`."""
     lon = np.array(lon)
     return np.mod(lon, 360)
 
 
-# -----------------------------------------------------------------------------
-
-
 def _wrapAngle180(lon):
     """wrap angle to `[-180, 180[`."""
     lon = np.array(lon)
     sel = (lon < -180) | (180 <= lon)
     lon[sel] = _wrapAngle360(lon[sel] + 180) - 180
     return lon
 
 
-def _wrapAngle(lon, wrap_lon=True):
+def _wrapAngle(lon, wrap_lon=True, is_unstructured=False):
     """wrap the angle to the other base
 
     If lon is from -180 to 180 wraps them to 0..360
     If lon is from 0 to 360 wraps them to -180..180
     """
 
     if np.isscalar(lon):
@@ -96,24 +90,21 @@
     if wl == 180 or (wl != 360 and lon.max() > 180):
         new_lon = _wrapAngle180(lon.copy())
 
     if wl == 360 or (wl != 180 and lon.min() < 0):
         new_lon = _wrapAngle360(lon.copy())
 
     # check if they are still unique
-    if new_lon.ndim == 1:
+    if new_lon.ndim == 1 and not is_unstructured:
         if new_lon.shape != np.unique(new_lon).shape:
             raise ValueError("There are equal longitude coordinates (when wrapped)!")
 
     return new_lon
 
 
-# -----------------------------------------------------------------------------
-
-
 def _is_180(lon_min, lon_max, msg_add=""):
 
     lon_min = np.round(lon_min, 6)
     lon_max = np.round(lon_max, 6)
 
     if (lon_min < 0) and (lon_max > 180):
         msg = "lon has both data that is larger than 180 and smaller than 0. " + msg_add
@@ -236,7 +227,21 @@
                 "passing positional arguments will result in an error",
                 FutureWarning,
             )
 
         return func(*args, **kwargs)
 
     return _inner
+
+
+def unpackbits(numbers, num_bits):
+    "Unpacks elements of a array into a binary-valued output array."
+
+    # after https://stackoverflow.com/a/51509307/3010700
+
+    if np.issubdtype(numbers.dtype, np.floating):
+        raise ValueError("numpy data type needs to be int-like")
+    shape = numbers.shape + (num_bits,)
+
+    numbers = numbers.reshape([-1, 1])
+    mask = 2 ** np.arange(num_bits, dtype=numbers.dtype).reshape([1, num_bits])
+    return (numbers & mask).astype(bool).reshape(shape)
```

### Comparing `regionmask-0.8.0/regionmask/defined_regions/_ar6.py` & `regionmask-0.9.0/regionmask/defined_regions/_ar6.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         if self._all is None:
             self._all = from_geopandas(
                 self.df,
                 names="Name",
                 abbrevs="Acronym",
                 name=self._name,
                 source=self._source,
+                overlap=False,
             )
 
         return self._all
 
     @property
     def land(self):
         if self._land is None:
@@ -59,14 +60,15 @@
 
             self._land = from_geopandas(
                 self.df.loc[land],
                 names="Name",
                 abbrevs="Acronym",
                 name=self._name + " (land only)",
                 source=self._source,
+                overlap=False,
             )
 
         return self._land
 
     @property
     def ocean(self):
         if self._ocean is None:
@@ -75,14 +77,15 @@
 
             self._ocean = from_geopandas(
                 self.df.loc[ocean],
                 names="Name",
                 abbrevs="Acronym",
                 name=self._name + " (ocean only)",
                 source=self._source,
+                overlap=False,
             )
 
         return self._ocean
 
     def __repr__(self):  # pragma: no cover
         return REPR
```

### Comparing `regionmask-0.8.0/regionmask/defined_regions/_ar6_pre_revisions.py` & `regionmask-0.9.0/regionmask/defined_regions/_ar6_pre_revisions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 import geopandas as gp
 from shapely import geometry
 
 from ..core._geopandas import _enumerate_duplicates, from_geopandas
 from ._ressources import read_remote_shapefile
 
 REPR = """
@@ -34,14 +36,19 @@
 Note
 ----
 The region numbers for ``all``, ``land``, and ``ocean`` are consistent. The
 region numbers for ``separate_pacific`` and all others are not.
 
 """
 
+DEPRECATION = (
+    "The ``_ar6_pre_revisions`` regions are deprecated and will be removed in a future "
+    "release."
+)
+
 
 def _combine_to_multipolygon(df, column, *names):
 
     all_poly = [df[df[column] == name].geometry.values[0] for name in names]
 
     combined_poly = geometry.MultiPolygon(all_poly)
 
@@ -155,55 +162,64 @@
 
             self.__df_combined = _df_combined
 
         return self.__df_combined
 
     @property
     def all(self):
+        warnings.warn(DEPRECATION, FutureWarning)
         if self._all is None:
 
             self._all = from_geopandas(
                 self._df_combined,
                 names="V2",
                 abbrevs="V3",
                 name=self._name,
                 source=self._source,
+                overlap=False,
             )
 
         return self._all
 
     @property
     def land(self):
         if self._land is None:
             r = self.all[land]
             r.name = self._name + " (land only)"
             self._land = r
+        else:
+            warnings.warn(DEPRECATION, FutureWarning)
+
         return self._land
 
     @property
     def ocean(self):
         if self._ocean is None:
             r = self.all[ocean]
             r.name = self._name + " (ocean only)"
             self._ocean = r
+        else:
+            warnings.warn(DEPRECATION, FutureWarning)
         return self._ocean
 
     @property
     def separate_pacific(self):
+        warnings.warn(DEPRECATION, FutureWarning)
         if self._separate_pacific is None:
             # need to fix the duplicates
             df = self._df.copy()
             df["V2"] = _enumerate_duplicates(df["V2"])
 
             self._separate_pacific = from_geopandas(
                 df,
                 names="V2",
                 abbrevs="V3",
                 name=self._name + "(separate Pacific regions)",
                 source=self._source,
+                overlap=False,
             )
 
         return self._separate_pacific
 
     def __repr__(self):  # pragma: no cover
         return REPR
```

### Comparing `regionmask-0.8.0/regionmask/defined_regions/_ressources.py` & `regionmask-0.9.0/regionmask/defined_regions/_ressources.py`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/regionmask/defined_regions/giorgi.py` & `regionmask-0.9.0/regionmask/defined_regions/giorgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,8 +84,9 @@
 giorgi = Regions(
     outlines,
     numbers=numbers,
     names=names,
     abbrevs=abbrevs,
     name="Giorgi",
     source=source,
+    overlap=False,
 )
```

### Comparing `regionmask-0.8.0/regionmask/defined_regions/srex.py` & `regionmask-0.9.0/regionmask/defined_regions/srex.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,8 +233,9 @@
 srex = Regions(
     outlines,
     numbers=numbers,
     names=names,
     abbrevs=short_names,
     name="SREX",
     source=source,
+    overlap=False,
 )
```

### Comparing `regionmask-0.8.0/regionmask/tests/test_OneRegion.py` & `regionmask-0.9.0/regionmask/tests/test_OneRegion.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,19 +56,14 @@
 
     outl = ((0, 0), (0, 1), (1, 1.0), (1, 0))
 
     # normal
     r = _OneRegion(1, "Unit Square", "USq", outl)
     assert np.allclose(r.centroid, (0.5, 0.5))
 
-    # user defined centroid
-    c = (1, 1)
-    r = _OneRegion(1, "Unit Square", "USq", outl, centroid=c)
-    assert np.allclose(r.centroid, c)
-
     # superfluous point -> center should still be at (0.5, 0.5)
     outl = ((0, 0), (0, 0.5), (0, 1), (1, 1.0), (1, 0))
     r = _OneRegion(1, "Unit Square", "USq", outl)
     assert np.allclose(r.centroid, (0.5, 0.5))
 
 
 def test_bounds():
```

### Comparing `regionmask-0.8.0/regionmask/tests/test_formatting.py` & `regionmask-0.9.0/regionmask/tests/test_formatting.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     pytest.importorskip("pandas", minversion="1.2")
 
     result = srex.__repr__()
 
     expected = """<regionmask.Regions>
 Name:     SREX
 Source:   Seneviratne et al., 2012 (https://www.ipcc.ch/site/assets/uploads/2...
+overlap:  False
 
 Regions:
  1 ALA       Alaska/N.W. Canada
  2 CGI     Canada/Greenl./Icel.
  3 WNA         W. North America
  4 CNA         C. North America
  5 ENA         E. North America
@@ -42,18 +43,18 @@
 [26 regions]"""
 
     assert result == expected
 
 
 def test_display_metadata():
 
-    expected = ["Name:     name"]
-    result = formatting._display_metadata("name", None)
+    expected = ["Name:     name", "overlap:  False"]
+    result = formatting._display_metadata("name", None, False)
     assert result == expected
 
-    expected = ["Name:     name", "Source:   source"]
-    result = formatting._display_metadata("name", "source")
+    expected = ["Name:     name", "Source:   source", "overlap:  True"]
+    result = formatting._display_metadata("name", "source", True)
     assert result == expected
 
-    expected = ["Name:     na..."]
-    result = formatting._display_metadata("name of regions", source=None, max_width=15)
+    expected = ["Name:     na...", "overlap:  None"]
+    result = formatting._display_metadata("name of regions", None, None, max_width=15)
     assert result == expected
```

### Comparing `regionmask-0.8.0/regionmask/tests/test_geopandas.py` & `regionmask-0.9.0/regionmask/tests/test_geopandas.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,60 +9,72 @@
 from regionmask.core._geopandas import (
     _check_duplicates,
     _construct_abbrevs,
     _enumerate_duplicates,
 )
 
 from .utils import (
-    dummy_lat,
-    dummy_ll_dict,
-    dummy_lon,
-    dummy_outlines_poly,
+    dummy_ds,
+    dummy_region,
+    dummy_region_overlap,
     expected_mask_2D,
     expected_mask_3D,
 )
 
 
 @pytest.fixture
 def geodataframe_clean():
 
-    numbers = [1, 2, 3]
+    numbers = [0, 1, 2]
     names = ["Unit Square1", "Unit Square2", "Unit Square3"]
     abbrevs = ["uSq1", "uSq2", "uSq3"]
 
     d = dict(
-        names=names, abbrevs=abbrevs, numbers=numbers, geometry=dummy_outlines_poly
+        names=names, abbrevs=abbrevs, numbers=numbers, geometry=dummy_region.polygons
+    )
+
+    return gp.GeoDataFrame.from_dict(d)
+
+
+@pytest.fixture
+def geodataframe_clean_overlap():
+
+    d = dict(
+        names=dummy_region_overlap.names,
+        abbrevs=dummy_region_overlap.abbrevs,
+        numbers=dummy_region_overlap.numbers,
+        geometry=dummy_region_overlap.polygons,
     )
 
     return gp.GeoDataFrame.from_dict(d)
 
 
 @pytest.fixture
 def geodataframe_missing():
 
     numbers = [1, None, None]
     names = ["Unit Square1", None, None]
     abbrevs = ["uSq1", None, None]
 
     d = dict(
-        names=names, abbrevs=abbrevs, numbers=numbers, geometry=dummy_outlines_poly
+        names=names, abbrevs=abbrevs, numbers=numbers, geometry=dummy_region.polygons
     )
 
     return gp.GeoDataFrame.from_dict(d)
 
 
 @pytest.fixture
 def geodataframe_duplicates():
 
     numbers = [1, 1, 1]
     names = ["Unit Square", "Unit Square", "Unit Square"]
     abbrevs = ["uSq", "uSq", "uSq"]
 
     d = dict(
-        names=names, abbrevs=abbrevs, numbers=numbers, geometry=dummy_outlines_poly
+        names=names, abbrevs=abbrevs, numbers=numbers, geometry=dummy_region.polygons
     )
 
     return gp.GeoDataFrame.from_dict(d)
 
 
 def test_from_geopandas_wrong_input():
     with pytest.raises(
@@ -80,33 +92,45 @@
         abbrevs="abbrevs",
         name="name",
         source="source",
     )
 
     assert isinstance(result, Regions)
 
-    assert result.polygons[0].equals(dummy_outlines_poly[0])
-    assert result.polygons[1].equals(dummy_outlines_poly[1])
-    assert result.polygons[2].equals(dummy_outlines_poly[2])
-    assert result.numbers == [1, 2, 3]
+    assert result.polygons[0].equals(dummy_region.polygons[0])
+    assert result.polygons[1].equals(dummy_region.polygons[1])
+    assert result.polygons[2].equals(dummy_region.polygons[2])
+    assert result.numbers == [0, 1, 2]
     assert result.names == ["Unit Square1", "Unit Square2", "Unit Square3"]
     assert result.abbrevs == ["uSq1", "uSq2", "uSq3"]
     assert result.name == "name"
     assert result.source == "source"
 
 
+@pytest.mark.parametrize("attr", ["name", "source", "overlap"])
+def test_from_geopandas_not_roundtrip_warning(attr, geodataframe_clean):
+
+    geodataframe_clean.attrs = {attr: "x"}
+
+    with pytest.warns(
+        UserWarning,
+        match="Use ``regionmask.Regions.from_geodataframe`` to round-trip ``Regions``",
+    ):
+        from_geopandas(geodataframe_clean)
+
+
 def test_from_geopandas_default(geodataframe_clean):
 
     result = from_geopandas(geodataframe_clean)
 
     assert isinstance(result, Regions)
 
-    assert result.polygons[0].equals(dummy_outlines_poly[0])
-    assert result.polygons[1].equals(dummy_outlines_poly[1])
-    assert result.polygons[2].equals(dummy_outlines_poly[2])
+    assert result.polygons[0].equals(dummy_region.polygons[0])
+    assert result.polygons[1].equals(dummy_region.polygons[1])
+    assert result.polygons[2].equals(dummy_region.polygons[2])
     assert result.numbers == [0, 1, 2]
     assert result.names == ["Region0", "Region1", "Region2"]
     assert result.abbrevs == ["r0", "r1", "r2"]
     assert result.name == "unnamed"
     assert result.source is None
 
 
@@ -183,108 +207,109 @@
         assert result[i] == expected[i]
 
 
 # ==============================================================================
 # uses the same function as `Regions.mask` - only do minimal tests here
 
 
-@pytest.mark.parametrize("lon_lat", [(dummy_lon, dummy_lat), (dummy_ll_dict, None)])
+@pytest.mark.parametrize("lon_lat", [(dummy_ds.lon, dummy_ds.lat), (dummy_ds, None)])
 @pytest.mark.parametrize("method", ["rasterize", "shapely"])
 def test_mask_geopandas(geodataframe_clean, lon_lat, method):
 
     lon, lat = lon_lat
     result = mask_geopandas(geodataframe_clean, lon, lat, method=method)
     expected = expected_mask_2D()
 
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat.values, dummy_lat))
-    assert np.all(np.equal(result.lon.values, dummy_lon))
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("drop", [True, False])
-@pytest.mark.parametrize("lon_lat", [(dummy_lon, dummy_lat), (dummy_ll_dict, None)])
+@pytest.mark.parametrize("lon_lat", [(dummy_ds.lon, dummy_ds.lat), (dummy_ds, None)])
 @pytest.mark.parametrize("method", ["rasterize", "shapely"])
 def test_mask_3D_geopandas(geodataframe_clean, drop, lon_lat, method):
 
     lon, lat = lon_lat
     result = mask_3D_geopandas(geodataframe_clean, lon, lat, drop=drop, method=method)
-    expected = expected_mask_3D(drop=drop)
+    expected = expected_mask_3D(drop=drop).drop_vars(["names", "abbrevs"])
 
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat.values, dummy_lat))
-    assert np.all(np.equal(result.lon.values, dummy_lon))
-
-    numbers = [0, 1] if drop else [0, 1, 2]
-    assert np.all(np.equal(result.region.values, numbers))
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("method", ["rasterize", "shapely"])
 def test_mask_geopandas_numbers(geodataframe_clean, method):
 
     result = mask_geopandas(
-        geodataframe_clean, dummy_lon, dummy_lat, method=method, numbers="numbers"
+        geodataframe_clean, dummy_ds.lon, dummy_ds.lat, method=method, numbers="numbers"
     )
-    expected = expected_mask_2D(1, 2)
+    expected = expected_mask_2D()
 
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat.values, dummy_lat))
-    assert np.all(np.equal(result.lon.values, dummy_lon))
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("method", ["rasterize", "shapely"])
 def test_mask_geopandas_warns_empty(geodataframe_clean, method):
 
+    lon = lat = [10, 11]
     with pytest.warns(UserWarning, match="No gridpoint belongs to any region."):
         result = mask_geopandas(
-            geodataframe_clean, [10, 11], [10, 11], method=method, numbers="numbers"
+            geodataframe_clean, lon, lat, method=method, numbers="numbers"
         )
 
-    assert isinstance(result, xr.DataArray)
-    assert result.isnull().all()
-    assert np.all(np.equal(result.lat.values, [10, 11]))
-    assert np.all(np.equal(result.lon.values, [10, 11]))
+    expected = expected_mask_2D(coords={"lon": lon, "lat": lat})
+
+    xr.testing.assert_equal(result, expected * np.NaN)
 
 
 @pytest.mark.parametrize("drop", [True, False])
 @pytest.mark.parametrize("method", ["rasterize", "shapely"])
 def test_mask_3D_geopandas_numbers(geodataframe_clean, drop, method):
 
-    expected = expected_mask_3D(drop)
+    expected = expected_mask_3D(drop).drop_vars(["names", "abbrevs"])
     result = mask_3D_geopandas(
         geodataframe_clean,
-        dummy_lon,
-        dummy_lat,
+        dummy_ds.lon,
+        dummy_ds.lat,
         drop=drop,
         method=method,
         numbers="numbers",
     )
 
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat.values, dummy_lat))
-    assert np.all(np.equal(result.lon.values, dummy_lon))
+    xr.testing.assert_equal(result, expected)
+
+
+@pytest.mark.parametrize("drop", [True, False])
+@pytest.mark.parametrize("method", ["rasterize", "shapely"])
+def test_mask_3D_overlap_geopandas_numbers(geodataframe_clean_overlap, drop, method):
+
+    expected = expected_mask_3D(drop, overlap=True).drop_vars(["names", "abbrevs"])
+    result = mask_3D_geopandas(
+        geodataframe_clean_overlap,
+        dummy_ds.lon,
+        dummy_ds.lat,
+        drop=drop,
+        method=method,
+        numbers="numbers",
+        overlap=True,
+    )
 
-    numbers = geodataframe_clean.numbers[:2] if drop else geodataframe_clean.numbers
-    assert np.all(np.equal(result.region.values, numbers))
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("drop", [True, False])
 def test_mask_3D_geopandas_warns_empty(geodataframe_clean, drop):
 
+    lon = lat = [10, 11]
     with pytest.warns(UserWarning, match="No gridpoint belongs to any region."):
-        result = mask_3D_geopandas(geodataframe_clean, [10], [10], drop=drop)
+        result = mask_3D_geopandas(geodataframe_clean, lon, lat, drop=drop)
+
+    coords = {"lat": lat, "lon": lon}
+    expected = expected_mask_3D(False, coords=coords).drop_vars(["names", "abbrevs"])
+    expected = expected.isel(region=slice(0, 0)) if drop else expected
 
-    assert isinstance(result, xr.DataArray)
-    shape = (0, 1, 1) if drop else (3, 1, 1)
-    assert result.shape == shape
-    assert np.all(np.equal(result.lat.values, [10]))
-    assert np.all(np.equal(result.lon.values, [10]))
+    xr.testing.assert_equal(result, expected * False)
 
 
 @pytest.mark.parametrize("func", [mask_geopandas, mask_3D_geopandas])
 def test_wrap_lon_maybe_error(func):
 
     # regions that exceed 360° longitude
     p = shapely.geometry.Polygon([[-180, 0], [-180, 10], [360, 10], [360, 0]])
@@ -304,36 +329,36 @@
         func(gs, lon, lat)
 
 
 @pytest.mark.parametrize("func", [mask_geopandas, mask_3D_geopandas])
 def test_mask_geopandas_wrong_input(func):
 
     with pytest.raises(TypeError, match="'GeoDataFrame' or 'GeoSeries'"):
-        func(None, dummy_lon, dummy_lat)
+        func(None, dummy_ds.lon, dummy_ds.lat)
 
 
 @pytest.mark.parametrize("func", [mask_geopandas, mask_3D_geopandas])
 def test_mask_geopandas_wrong_numbers(geodataframe_clean, func):
 
     with pytest.raises(KeyError):
-        func(geodataframe_clean, dummy_lon, dummy_lat, numbers="not_a_column")
+        func(geodataframe_clean, dummy_ds.lon, dummy_ds.lat, numbers="not_a_column")
 
 
 @pytest.mark.parametrize("func", [mask_geopandas, mask_3D_geopandas])
 def test_mask_geopandas_missing_error(geodataframe_missing, func):
 
     with pytest.raises(ValueError, match="cannot contain missing values"):
-        func(geodataframe_missing, dummy_lon, dummy_lat, numbers="numbers")
+        func(geodataframe_missing, dummy_ds.lon, dummy_ds.lat, numbers="numbers")
 
 
 @pytest.mark.parametrize("func", [mask_geopandas, mask_3D_geopandas])
 def test_mask_geopandas_duplicates_error(geodataframe_duplicates, func):
 
     with pytest.raises(ValueError, match="cannot contain duplicate values"):
-        func(geodataframe_duplicates, dummy_lon, dummy_lat, numbers="numbers")
+        func(geodataframe_duplicates, dummy_ds.lon, dummy_ds.lat, numbers="numbers")
 
 
 @pytest.mark.parametrize("func", [mask_geopandas, mask_3D_geopandas])
 def test_raise_on_non_numeric_numbers(geodataframe_clean, func):
 
     with pytest.raises(ValueError, match="'numbers' must be numeric"):
-        func(geodataframe_clean, dummy_lon, dummy_lat, numbers="abbrevs")
+        func(geodataframe_clean, dummy_ds.lon, dummy_ds.lat, numbers="abbrevs")
```

### Comparing `regionmask-0.8.0/regionmask/tests/test_mask.py` & `regionmask-0.9.0/regionmask/tests/test_mask.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import copy
+
 import numpy as np
 import pytest
 import xarray as xr
 from affine import Affine
 from shapely.geometry import Polygon
 
 from regionmask import Regions
@@ -14,19 +16,17 @@
     _mask_shapely,
     _transform_from_latlon,
 )
 from regionmask.core.utils import _wrapAngle, create_lon_lat_dataarray_from_bounds
 
 from . import has_pygeos, requires_pygeos
 from .utils import (
-    dummy_lat,
-    dummy_lon,
-    dummy_outlines,
-    dummy_outlines_poly,
+    dummy_ds,
     dummy_region,
+    dummy_region_overlap,
     expected_mask_2D,
     expected_mask_3D,
 )
 
 MASK_FUNCS = [
     _mask_rasterize,
     _mask_shapely,
@@ -48,96 +48,88 @@
 # =============================================================================
 
 
 @pytest.mark.parametrize("func", MASK_FUNCS)
 def test_mask_func(func):
 
     # standard
-    result = func(dummy_lon, dummy_lat, dummy_outlines_poly, numbers=[0, 1, 2])
+    result = func(dummy_ds.lon, dummy_ds.lat, dummy_region.polygons, numbers=[0, 1, 2])
     expected = expected_mask_2D()
-    assert np.allclose(result, expected, equal_nan=True)
+    np.testing.assert_equal(result, expected)
 
-    result = func(dummy_lon, dummy_lat, dummy_outlines_poly, numbers=[0, 1, 2], fill=5)
+    result = func(
+        dummy_ds.lon, dummy_ds.lat, dummy_region.polygons, numbers=[0, 1, 2], fill=5
+    )
     expected = expected_mask_2D(fill=5)
-    assert np.allclose(result, expected, equal_nan=True)
+    np.testing.assert_equal(result, expected)
 
-    result = func(dummy_lon, dummy_lat, dummy_outlines_poly, numbers=[5, 6, 7])
+    result = func(dummy_ds.lon, dummy_ds.lat, dummy_region.polygons, numbers=[5, 6, 7])
     expected = expected_mask_2D(a=5, b=6)
-    assert np.allclose(result, expected, equal_nan=True)
+    np.testing.assert_equal(result, expected)
 
 
-@pytest.mark.parametrize(
-    "func",
-    [
-        pytest.param(_mask_rasterize, marks=pytest.mark.xfail),
-        _mask_shapely,
-        pytest.param(_mask_pygeos, marks=requires_pygeos),
-    ],
-)
+@pytest.mark.parametrize("func", MASK_FUNCS)
 def test_mask_wrong_number_fill(func):
 
     with pytest.raises(ValueError, match="The fill value should not"):
-        _mask_shapely(
-            dummy_lon, dummy_lat, dummy_outlines_poly, numbers=[0, 1, 2], fill=0
+        func(
+            dummy_ds.lon, dummy_ds.lat, dummy_region.polygons, numbers=[0, 1, 2], fill=0
         )
 
     with pytest.raises(ValueError, match="`numbers` and `coords` must have"):
-        _mask_shapely(dummy_lon, dummy_lat, dummy_outlines, numbers=[5])
+        func(dummy_ds.lon, dummy_ds.lat, dummy_region.coords, numbers=[5])
 
 
 @pytest.mark.parametrize("method", MASK_METHODS)
 def test_mask(method):
 
     expected = expected_mask_2D()
-    result = dummy_region.mask(dummy_lon, dummy_lat, method=method).values
-    assert np.allclose(result, expected, equal_nan=True)
+    result = dummy_region.mask(dummy_ds.lon, dummy_ds.lat, method=method)
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.skipif(has_pygeos, reason="Only errors if pygeos is missing")
 def test_missing_pygeos_error():
 
     with pytest.raises(ModuleNotFoundError, match="No module named 'pygeos'"):
-        dummy_region.mask(dummy_lon, dummy_lat, method="pygeos")
+        dummy_region.mask(dummy_ds.lon, dummy_ds.lat, method="pygeos")
 
 
 @pytest.mark.parametrize("method", MASK_METHODS)
-def test_mask_xarray(method):
+def test_mask_xr_keep_name(method):
 
-    expected = expected_mask_2D()
-    result = dummy_region.mask(dummy_lon, dummy_lat, method=method)
+    ds = xr.Dataset(
+        coords={"longitude": dummy_ds.lon.values, "latitude": dummy_ds.lat.values}
+    )
 
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat.values, dummy_lat))
-    assert np.all(np.equal(result.lon.values, dummy_lon))
+    expected = expected_mask_2D().rename(lat="latitude", lon="longitude")
+
+    result = dummy_region.mask(ds.longitude, ds.latitude, method=method)
+
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("method", MASK_METHODS)
 def test_mask_poly_z_value(method):
 
     outl1 = Polygon(((0, 0, 1), (0, 1, 1), (1, 1.0, 1), (1, 0, 1)))
     outl2 = Polygon(((0, 1, 1), (0, 2, 1), (1, 2.0, 1), (1, 1, 1)))
-    outlines = [outl1, outl2]
-
-    r_z = Regions(outlines)
+    r_z = Regions([outl1, outl2])
 
     expected = expected_mask_2D()
-    result = r_z.mask(dummy_lon, dummy_lat, method=method)
+    result = r_z.mask(dummy_ds, method=method)
 
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat.values, dummy_lat))
-    assert np.all(np.equal(result.lon.values, dummy_lon))
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("method", MASK_METHODS)
 def test_mask_xarray_name(method):
 
-    msk = dummy_region.mask(dummy_lon, dummy_lat, method=method)
-    assert msk.name == "region"
+    msk = dummy_region.mask(dummy_ds, method=method)
+    assert msk.name == "mask"
 
 
 @pytest.mark.parametrize("ndims", [(2, 1), (1, 2)])
 def test_mask_unequal_ndim(ndims):
 
     lon = np.arange(ndims[0] * 2).reshape(ndims[0] * (2,))
     lat = np.arange(ndims[1] * 2).reshape(ndims[1] * (2,))
@@ -168,22 +160,20 @@
 
 
 @pytest.mark.parametrize("lon_name", ["lon", "longitude"])
 @pytest.mark.parametrize("lat_name", ["lat", "latitude"])
 @pytest.mark.parametrize("method", MASK_METHODS)
 def test_mask_obj(lon_name, lat_name, method):
 
-    expected = expected_mask_2D()
+    expected = expected_mask_2D().rename(lat=lat_name, lon=lon_name)
 
-    obj = {lon_name: dummy_lon, lat_name: dummy_lat}
-    result = dummy_region.mask(
-        obj, method=method, lon_name=lon_name, lat_name=lat_name
-    ).values
+    obj = {lon_name: dummy_ds.lon.values, lat_name: dummy_ds.lat.values}
+    result = dummy_region.mask(obj, method=method, lon_name=lon_name, lat_name=lat_name)
 
-    assert np.allclose(result, expected, equal_nan=True)
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.filterwarnings("ignore:No gridpoint belongs to any region.")
 @pytest.mark.parametrize("method", MASK_METHODS)
 def test_mask_wrap(method):
 
     # create a test case where the outlines and the lon coordinates
@@ -196,30 +186,30 @@
 
     r = Regions(outlines)
 
     # lon -180..179.9
     lon = [-1.5, -0.5]
     lat = [0.5, 1.5]
 
-    result = r.mask(lon, lat, method=method, wrap_lon=False).values
-    assert np.all(np.isnan(result))
+    result = r.mask(lon, lat, method=method, wrap_lon=False)
+    assert result.isnull().all()
 
     # this is the wrong wrapping
-    result = r.mask(lon, lat, method=method, wrap_lon=180).values
-    assert np.all(np.isnan(result))
+    result = r.mask(lon, lat, method=method, wrap_lon=180)
+    assert result.isnull().all()
 
-    expected = expected_mask_2D()
+    expected = expected_mask_2D(coords={"lon": lon, "lat": lat})
 
     # determine the wrap automatically
-    result = r.mask(lon, lat, method=method, wrap_lon=True).values
-    assert np.allclose(result, expected, equal_nan=True)
+    result = r.mask(lon, lat, method=method, wrap_lon=True)
+    xr.testing.assert_equal(result, expected)
 
     # determine the wrap by hand
-    result = r.mask(lon, lat, method=method, wrap_lon=360).values
-    assert np.allclose(result, expected, equal_nan=True)
+    result = r.mask(lon, lat, method=method, wrap_lon=360)
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.filterwarnings("ignore:No gridpoint belongs to any region.")
 @pytest.mark.parametrize("meth", ["mask", "mask_3D"])
 def test_wrap_lon_no_error_wrap_lon_false(meth):
 
     # regions that exceed 360° longitude
@@ -255,96 +245,115 @@
     lat = np.arange(10, 1, -3)
 
     with pytest.raises(ValueError, match="Set `wrap_lon=False` to skip this check."):
         getattr(r, meth)(lon, lat)
 
 
 @pytest.mark.parametrize("method", MASK_METHODS)
-def test_mask_autowrap(method):
-
-    expected = expected_mask_2D()
+@pytest.mark.parametrize(
+    "lon, extent",
+    (
+        ([358.5, 359.5], (-180, -1)),
+        ([-1.5, -0.5], (-180, -1)),
+        ([-1.5, -0.5], (359, 0)),
+        ([358.5, 359.5], (359, 0)),
+    ),
+)
+def test_mask_autowrap(method, lon, extent):
 
-    # create a test case where the outlines and the lon coordinates
-    # are different - or the same - should work either way
+    # outlines and lon are different - or the same - should work either way
 
-    # 1. -180..180 regions and -180..180 lon
-    lon = [0.5, 1.5]
     lat = [0.5, 1.5]
-    result = dummy_region.mask(lon, lat, method=method).values
-    assert np.allclose(result, expected, equal_nan=True)
 
-    # 2. -180..180 regions and 0..360 lon
-    # outline -180..180
-    outl1 = ((-180, 0), (-180, 1), (-1, 1.0), (-1, 0))
-    outl2 = ((-180, 1), (-180, 2), (-1, 2.0), (-1, 1))
-    outlines = [outl1, outl2]
+    r_from, r_to = extent
+    outl1 = ((r_from, 0), (r_from, 1), (r_to, 1.0), (r_to, 0))
+    outl2 = ((r_from, 1), (r_from, 2), (r_to, 2.0), (r_to, 1))
+    r = Regions([outl1, outl2])
 
-    r = Regions(outlines)
+    expected = expected_mask_2D(coords={"lon": lon, "lat": lat})
 
-    # lon -180..179.9
-    lon = [358.5, 359.5]
-    lat = [0.5, 1.5]
+    result = r.mask(lon, lat, method=method)
+    xr.testing.assert_equal(result, expected)
 
-    result = r.mask(lon, lat, method=method).values
-    assert np.allclose(result, expected, equal_nan=True)
 
-    # 3. 0..360 regions and -180..180 lon
+def test_mask_wrong_method():
 
-    # outline 0..359.9
-    outl1 = ((359, 0), (359, 1), (0, 1.0), (0, 0))
-    outl2 = ((359, 1), (359, 2), (0, 2.0), (0, 1))
-    outlines = [outl1, outl2]
+    msg = "Method must be None or one of 'rasterize', 'shapely' and 'pygeos'."
+    with pytest.raises(ValueError, match=msg):
+        dummy_region.mask(dummy_ds, method="wrong")
 
-    r = Regions(outlines)
 
-    # lon -180..179.9
-    lon = [-1.5, -0.5]
-    lat = [0.5, 1.5]
+@pytest.mark.parametrize("method", MASK_METHODS)
+def test_mask_2D_overlap_error(method):
 
-    result = r.mask(lon, lat, method=method).values
-    assert np.allclose(result, expected, equal_nan=True)
+    # make a copy to ensure dummy_region_overlap.overlap is not overwritten
+    region = copy.copy(dummy_region_overlap)
+    expected = expected_mask_2D(a=1, b=2)
 
-    # 3. 0..360 regions and 0..360 lon
+    match = "Creating a 2D mask with overlapping regions yields wrong results"
+    with pytest.raises(ValueError, match=match):
+        region.mask(dummy_ds, method=method)
 
-    # lon 0..359.9
-    lon = [0.5, 359.5]
-    lat = [0.5, 1.5]
+    region.overlap = False
+    result = region.mask(dummy_ds, method=method)
 
-    result = r.mask(lon, lat, method=method).values
-    assert np.allclose(result, expected, equal_nan=True)
+    xr.testing.assert_equal(result, expected)
 
 
-def test_mask_wrong_method():
+@pytest.mark.parametrize("drop", [True, False])
+@pytest.mark.parametrize("method", MASK_METHODS)
+def test_mask_3D_overlap(drop, method):
 
-    msg = "Method must be None or one of 'rasterize', 'shapely' and 'pygeos'."
-    with pytest.raises(ValueError, match=msg):
-        dummy_region.mask(dummy_lon, dummy_lat, method="wrong")
+    expected = expected_mask_3D(drop=drop, overlap=True)
+    result = dummy_region_overlap.mask_3D(dummy_ds, drop=drop, method=method)
+
+    xr.testing.assert_equal(result, expected)
+
+
+@pytest.mark.parametrize("method", MASK_METHODS)
+def test_mask_3D_overlap_empty(method):
+
+    match = "No gridpoint belongs to any region. "
+
+    lon = lat = [10, 11]
+    with pytest.warns(UserWarning, match=match + "Returning an empty mask"):
+        result = dummy_region_overlap.mask_3D(lon, lat, drop=True, method=method)
+
+    coords = {"lat": lat, "lon": lon}
+    expected = expected_mask_3D(False, coords=coords, overlap=True).isel(
+        region=slice(0, 0)
+    )
+
+    assert result.shape == (0, 2, 2)
+    xr.testing.assert_equal(result, expected)
+
+    with pytest.warns(UserWarning, match=match + "Returning an all-False mask."):
+        result = dummy_region_overlap.mask_3D(lon, lat, drop=False, method=method)
+
+    assert result.shape == (4, 2, 2)
+    assert not result.any()
 
 
 # ======================================================================
 
 # test 2D array
 lon_2D = [[0.5, 1.5], [0.5, 1.5]]
 lat_2D = [[0.5, 0.5], [1.5, 1.5]]
 
 
 @pytest.mark.parametrize("method", MASK_METHODS_IRREGULAR)
 def test_mask_2D(method):
 
-    expected = expected_mask_2D()
-    result = dummy_region.mask(lon_2D, lat_2D, method=method)
+    dims = ("lat_idx", "lon_idx")
+    coords = {"lat": (dims, lat_2D), "lon": (dims, lon_2D)}
 
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-
-    assert np.all(np.equal(result.lat.values, lat_2D))
-    assert np.all(np.equal(result.lon.values, lon_2D))
+    expected = expected_mask_2D(coords=coords, dims=dims)
+    result = dummy_region.mask(lon_2D, lat_2D, method=method)
 
-    assert np.all(np.equal(result.lat_idx.values, [0, 1]))
-    assert np.all(np.equal(result.lon_idx.values, [0, 1]))
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("lon", [lon_2D, [0, 1, 3], 0])
 @pytest.mark.parametrize("lat", [lat_2D, [0, 1, 3], 0])
 def test_mask_rasterize_irregular(lon, lat):
 
     with pytest.raises(ValueError, match="`lat` and `lon` must be equally spaced"):
@@ -358,30 +367,20 @@
     coords = {
         "lat_1D": [1, 2],
         "lon_1D": [1, 2],
         "lat_2D": (("lat_1D", "lon_1D"), lat_2D),
         "lon_2D": (("lat_1D", "lon_1D"), lon_2D),
     }
 
-    d = np.random.rand(2, 2)
+    data = xr.Dataset(coords=coords)
 
-    data = xr.DataArray(d, coords=coords, dims=("lat_1D", "lon_1D"))
+    expected = expected_mask_2D(coords=coords, dims=("lat_1D", "lon_1D"))
+    result = dummy_region.mask(data.lon_2D, data.lat_2D, method=method)
 
-    expected = expected_mask_2D()
-    result = dummy_region.mask(
-        data, lon_name="lon_2D", lat_name="lat_2D", method=method
-    )
-
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat_2D.values, lat_2D))
-    assert np.all(np.equal(result.lon_2D.values, lon_2D))
-
-    assert np.all(np.equal(result.lat_1D.values, [1, 2]))
-    assert np.all(np.equal(result.lon_1D.values, [1, 2]))
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("lon_start", [0, 1, -5])
 @pytest.mark.parametrize("dlon", [1, 2])
 @pytest.mark.parametrize("lat_start", [0, 1, -5])
 @pytest.mark.parametrize("dlat", [1, 2])
 def test_transform_from_latlon(lon_start, dlon, lat_start, dlat):
@@ -403,95 +402,103 @@
 @pytest.mark.parametrize("a, b", [(0, 1), (4, 5)])
 @pytest.mark.parametrize("fill", [np.NaN, 3])
 def test_rasterize(a, b, fill):
 
     expected = expected_mask_2D(a=a, b=b, fill=fill)
 
     result = _mask_rasterize(
-        dummy_lon, dummy_lat, dummy_outlines_poly, numbers=[a, b], fill=fill
+        dummy_ds.lon, dummy_ds.lat, dummy_region.polygons, numbers=[a, b, -1], fill=fill
     )
 
-    assert np.allclose(result, expected, equal_nan=True)
+    np.testing.assert_equal(result, expected)
 
 
-def test_mask_empty():
+@pytest.mark.parametrize("method", MASK_METHODS)
+def test_mask_empty(method):
 
+    lon = lat = [10, 11]
     with pytest.warns(UserWarning, match="No gridpoint belongs to any region."):
-        result = dummy_region.mask([10, 11], [10, 11], method="shapely")
+        result = dummy_region.mask(lon, lat, method=method)
 
-    assert isinstance(result, xr.DataArray)
-    assert result.shape == (2, 2)
-    assert result.isnull().all()
-    assert np.all(np.equal(result.lon.values, [10, 11]))
-    assert np.all(np.equal(result.lat.values, [10, 11]))
+    expected = expected_mask_2D(coords={"lon": lon, "lat": lat})
+
+    xr.testing.assert_equal(result, expected * np.NaN)
+
+
+# =============================================================================
+# =============================================================================
+# test unstructured
+
+
+@pytest.mark.parametrize("method", MASK_METHODS_IRREGULAR)
+def test_mask_unstructured(method):
+    """Test for unstructured output."""
+    lat = [0.5, 0.5, 1.5, 1.5]
+    lon = [0.5, 1.5, 0.5, 1.5]
+
+    coords = {"lon": ("cells", lon), "lat": ("cells", lat)}
+    grid = xr.Dataset(coords=coords)
+
+    result = dummy_region.mask(grid, method=method)
+    expected = expected_mask_2D(flatten=True, coords=coords, dims="cells")
+
+    xr.testing.assert_equal(result, expected)
 
 
 # =============================================================================
 # =============================================================================
 # test mask_3D: only basics (same algorithm as mask)
 
 
 @pytest.mark.parametrize("drop", [True, False])
 @pytest.mark.parametrize("method", MASK_METHODS)
 def test_mask_3D(drop, method):
 
     expected = expected_mask_3D(drop)
-    result = dummy_region.mask_3D(dummy_lon, dummy_lat, drop=drop, method=method)
+    result = dummy_region.mask_3D(dummy_ds.lon, dummy_ds.lat, drop=drop, method=method)
 
-    assert isinstance(result, xr.DataArray)
-    assert result.shape == expected.shape
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat.values, dummy_lat))
-    assert np.all(np.equal(result.lon.values, dummy_lon))
-
-    _dr = dummy_region[[0, 1]] if drop else dummy_region
-
-    assert np.all(np.equal(result.region.values, _dr.numbers))
-    assert np.all(result.abbrevs.values == _dr.abbrevs)
-    assert np.all(result.names.values == _dr.names)
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("method", MASK_METHODS)
 def test_mask_3D_empty(method):
 
-    with pytest.warns(UserWarning, match="No gridpoint belongs to any region."):
-        result = dummy_region.mask_3D([10, 11], [10, 11], drop=True, method=method)
+    match = "No gridpoint belongs to any region. "
+
+    lon = lat = [10, 11]
+    with pytest.warns(UserWarning, match=match + "Returning an empty mask"):
+        result = dummy_region.mask_3D(lon, lat, drop=True, method=method)
+
+    coords = {"lat": lat, "lon": lon}
+    expected = expected_mask_3D(False, coords=coords).isel(region=slice(0, 0))
 
-    assert isinstance(result, xr.DataArray)
     assert result.shape == (0, 2, 2)
-    assert np.all(np.equal(result.lon.values, [10, 11]))
-    assert np.all(np.equal(result.lat.values, [10, 11]))
+    xr.testing.assert_equal(result, expected)
+
+    with pytest.warns(UserWarning, match=match + "Returning an all-False mask."):
+        result = dummy_region.mask_3D(lon, lat, drop=False, method=method)
+
+    assert result.shape == (3, 2, 2)
+    assert not result.any()
 
 
 @pytest.mark.parametrize("lon_name", ["lon", "longitude"])
 @pytest.mark.parametrize("lat_name", ["lat", "latitude"])
 @pytest.mark.parametrize("drop", [True, False])
 @pytest.mark.parametrize("method", MASK_METHODS)
 def test_mask_3D_obj(lon_name, lat_name, drop, method):
 
-    expected = expected_mask_3D(drop)
+    expected = expected_mask_3D(drop).rename(lon=lon_name, lat=lat_name)
 
-    obj = {lon_name: dummy_lon, lat_name: dummy_lat}
+    obj = dummy_ds.rename(lon=lon_name, lat=lat_name)
     result = dummy_region.mask_3D(
         obj, method=method, drop=drop, lon_name=lon_name, lat_name=lat_name
     )
 
-    assert isinstance(result, xr.DataArray)
-
-    assert result.shape == expected.shape
-    assert np.allclose(result, expected, equal_nan=True)
-
-    assert np.all(np.equal(result[lat_name].values, dummy_lat))
-    assert np.all(np.equal(result[lon_name].values, dummy_lon))
-
-    _dr = dummy_region[[0, 1]] if drop else dummy_region
-
-    assert np.all(np.equal(result.region.values, _dr.numbers))
-    assert np.all(result.abbrevs.values == _dr.abbrevs)
-    assert np.all(result.names.values == _dr.names)
+    xr.testing.assert_equal(result, expected)
 
 
 # =============================================================================
 # =============================================================================
 # =============================================================================
 
 # create a region such that the edge falls exactly on the lat/ lon coordinates
@@ -546,76 +553,74 @@
 
     expected = _expected_rectangle(ds, -100, -80, 28, 50, is_360)
 
     # set number and fill value
     expected = expected.where(expected, fill)
     expected = expected.where(expected != 1, number)
 
+    coords = {"lat": ds.lat, "lon": ds.lon}
+    expected = xr.DataArray(expected, dims=("lat", "lon"), coords=coords)
     return expected
 
 
 def expected_mask_interior_and_edge(ds, is_360, number=0, fill=np.NaN):
 
     expected_outerior = _expected_rectangle(ds, -100, -80, 28, 50, is_360)
     expected_interior = _expected_rectangle(ds, -94, -86, 34, 44, is_360)
 
     expected = expected_outerior & ~expected_interior
 
     # set number and fill value
     expected = expected.where(expected, fill)
     expected = expected.where(expected != 1, number)
 
+    coords = {"lat": ds.lat, "lon": ds.lon}
+    expected = xr.DataArray(expected, dims=("lat", "lon"), coords=coords)
     return expected
 
 
 @pytest.mark.parametrize("method", MASK_METHODS)
 @pytest.mark.parametrize(
     "regions", [r_US_180_ccw, r_US_180_cw, r_US_360_ccw, r_US_360_cw]
 )
 @pytest.mark.parametrize("ds_US, is_360", [(ds_US_180, False), (ds_US_360, True)])
 def test_mask_edge(method, regions, ds_US, is_360):
 
     expected = expected_mask_edge(ds_US, is_360)
     result = regions.mask(ds_US, method=method)
 
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat, ds_US.lat))
-    assert np.all(np.equal(result.lon, ds_US.lon))
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.parametrize("method", MASK_METHODS)
 @pytest.mark.parametrize(
     "regions",
     [r_US_hole_180_cw, r_US_hole_180_ccw, r_US_hole_360_cw, r_US_hole_360_ccw],
 )
 @pytest.mark.parametrize("ds_US, is_360", [(ds_US_180, False), (ds_US_360, True)])
 def test_mask_interior_and_edge(method, regions, ds_US, is_360):
 
     expected = expected_mask_interior_and_edge(ds_US, is_360)
     result = regions.mask(ds_US, method=method)
 
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat.values, ds_US.lat))
-    assert np.all(np.equal(result.lon.values, ds_US.lon))
+    xr.testing.assert_equal(result, expected)
 
 
 @pytest.mark.xfail(
     raises=AssertionError, reason="https://github.com/mapbox/rasterio/issues/1844"
 )
 def test_rasterize_edge():
 
     lon = ds_US_180.lon
     lat = ds_US_180.lat
 
     expected = expected_mask_edge(ds_US_180, is_360=False)
     result = _mask_rasterize_no_offset(lon, lat, r_US_180_ccw.polygons, numbers=[0])
 
-    assert np.allclose(result, expected, equal_nan=True)
+    np.testing.assert_equal(result, expected)
 
 
 ds_for_45_deg = create_lon_lat_dataarray_from_bounds(*(-0.5, 16, 1), *(10.5, -0.5, -1))
 
 # add a small offset to y to avoid https://github.com/mapbox/rasterio/issues/1844
 outline_45_deg = np.array([[0, 10.1], [0, 0.1], [5.1, 0.1], [15.1, 10.1]])
 
@@ -644,15 +649,15 @@
     polygons = regions.polygons
     lon = ds_for_45_deg.lon
     lat = ds_for_45_deg.lat
 
     result_no_offset = _mask_rasterize_no_offset(lon, lat, polygons, numbers=[0])
     result_offset = _mask_rasterize(lon, lat, polygons, numbers=[0])
 
-    assert np.allclose(result_no_offset, result_offset, equal_nan=True)
+    np.testing.assert_equal(result_no_offset, result_offset)
 
 
 # =============================================================================
 
 # the whole globe -> can be re-arranged (_mask_rasterize_flip)
 ds_GLOB_360 = create_lon_lat_dataarray_from_bounds(*(0, 360, 2), *(75, 13, -2))
 # not all lon -> must be masked twice (_mask_rasterize_split)
@@ -665,18 +670,15 @@
     # https://github.com/regionmask/regionmask/issues/127
 
     # using regions_180 and ds_360 lon must be wrapped, making it
     # NOT equally_spaced
     result = regions_180.mask(ds_360, method="rasterize")
 
     expected = expected_mask_edge(ds_360, is_360=True)
-    assert isinstance(result, xr.DataArray)
-    assert np.allclose(result, expected, equal_nan=True)
-    assert np.all(np.equal(result.lat, expected.lat))
-    assert np.all(np.equal(result.lon, expected.lon))
+    xr.testing.assert_equal(result, expected)
 
     expected_shapely = regions_180.mask(ds_360, method="shapely")
     xr.testing.assert_equal(result, expected_shapely)
 
 
 def test_rasterize_on_split_lon_asymmetric():
     # https://github.com/regionmask/regionmask/issues/266
@@ -700,15 +702,15 @@
     2: "rasterize_split",
     3: METHOD_IRREGULAR,
 }
 
 equal = np.arange(0.5, 360)
 grid_2D = np.arange(10).reshape(2, 5)
 un_equal = [0, 1, 2, 4, 5, 6.1]
-close_to_equal = equal + np.random.randn(*equal.shape) * 10 ** -6
+close_to_equal = equal + np.random.randn(*equal.shape) * 10**-6
 
 
 @pytest.mark.parametrize(
     "lon, m_lon",
     [
         (equal, 0),
         (close_to_equal, 0),
@@ -730,15 +732,15 @@
     assert _determine_method(lon, lat) == expected
 
 
 # =============================================================================
 # =============================================================================
 # =============================================================================
 
-# ensure a global region incudes all gridpoints - also the ones at
+# ensure a global region includes all gridpoints - also the ones at
 # 0°E/ -180°E and -90°N (#GH159)
 
 outline_GLOB_180 = np.array(
     [[-180.0, 90.0], [-180.0, -90.0], [180.0, -90.0], [180.0, 90.0]]
 )
 outline_GLOB_360 = outline_GLOB_180 + [180, 0]
 
@@ -772,22 +774,40 @@
     lat = np.arange(90, -91, -2.5)
     lon = np.arange(-300, 60, 2.5)
     mask = regions.mask(lon, lat, method=method)
 
     assert (mask == 0).all()
 
 
+@pytest.mark.parametrize("method", MASK_METHODS)
+@pytest.mark.parametrize("outline", [outline_GLOB_180, outline_GLOB_360])
+@pytest.mark.parametrize("lon", [lon180, lon360])
+def test_mask_whole_grid_overlap(method, outline, lon):
+
+    regions = Regions([outline, outline], overlap=True)
+
+    lat = np.arange(90, -91, -10)
+    mask = regions.mask_3D(lon, lat, method=method)
+    assert mask.all()
+
+    # with wrap_lon=False the edges are not masked
+    mask = regions.mask_3D(lon, lat, method=method, wrap_lon=False)
+    assert not mask.sel(lat=-90).any()
+
+
 def test_inject_mask_docstring():
 
     result = _inject_mask_docstring(True, True)
 
     assert "3D" in result
     assert "2D" not in result
     assert "drop :" in result
     assert "geodataframe" in result
+    assert "overlap" in result
 
     result = _inject_mask_docstring(False, False)
 
     assert "2D" in result
     assert "3D" not in result
     assert "drop :" not in result
     assert "geodataframe" not in result
+    assert "overlap" not in result
```

### Comparing `regionmask-0.8.0/regionmask/tests/test_mask_defined_regions.py` & `regionmask-0.9.0/regionmask/tests/test_mask_defined_regions.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,52 +2,44 @@
 
 import numpy as np
 import pytest
 
 from regionmask import defined_regions
 from regionmask.core.utils import create_lon_lat_dataarray_from_bounds
 
-from . import has_pygeos, requires_cartopy
-from .utils import REGIONS, REGIONS_REQUIRING_CARTOPY, get_naturalearth_region_or_skip
+from . import has_pygeos
+from .utils import REGIONS
 
 # =============================================================================
 
 ds_glob_1 = create_lon_lat_dataarray_from_bounds(*(-180, 181, 1), *(90, -91, -1))
 ds_glob_2 = create_lon_lat_dataarray_from_bounds(*(-180, 181, 2), *(90, -91, -2))
 # for _mask_rasterize_flip
 ds_glob_360_2 = create_lon_lat_dataarray_from_bounds(*(0, 361, 2), *(90, -91, -2))
 # for _mask_rasterize_split
 ds_glob_360_2_part = create_lon_lat_dataarray_from_bounds(*(0, 220, 2), *(90, -91, -2))
 
 DATASETS = [ds_glob_1, ds_glob_2, ds_glob_360_2, ds_glob_360_2_part]
 
 
-def _test_mask_equal_defined_regions(region, ds):
+def _test_mask_equal_defined_regions(region, ds, mask_method):
 
-    rasterize = region.mask(ds, method="rasterize")
-    shapely = region.mask(ds, method="shapely")
+    mask = getattr(region, mask_method)
+
+    rasterize = mask(ds, method="rasterize")
+    shapely = mask(ds, method="shapely")
 
     assert np.allclose(rasterize, shapely, equal_nan=True)
 
     if has_pygeos:
-        pygeos = region.mask(ds, method="pygeos")
+        pygeos = mask(ds, method="pygeos")
 
         assert np.allclose(rasterize, pygeos, equal_nan=True)
 
 
-@pytest.mark.parametrize("region_name", REGIONS.keys())
+@pytest.mark.parametrize("defined_region", REGIONS)
 @pytest.mark.parametrize("ds", DATASETS)
-def test_mask_equal_defined_regions(region_name, ds):
-
-    region = attrgetter(region_name)(defined_regions)
-
-    _test_mask_equal_defined_regions(region, ds)
-
-
-@requires_cartopy
-@pytest.mark.parametrize("region_name", REGIONS_REQUIRING_CARTOPY.keys())
-@pytest.mark.parametrize("ds", DATASETS)
-def test_mask_equal_defined_regions_cartopy(monkeypatch, region_name, ds):
-
-    region = get_naturalearth_region_or_skip(monkeypatch, region_name)
+def test_mask_equal_defined_regions(defined_region, ds):
 
-    _test_mask_equal_defined_regions(region, ds)
+    region = attrgetter(defined_region.region_name)(defined_regions)
+    mask_method = "mask_3D" if defined_region.overlap else "mask"
+    _test_mask_equal_defined_regions(region, ds, mask_method)
```

### Comparing `regionmask-0.8.0/regionmask/tests/test_plot.py` & `regionmask-0.9.0/regionmask/tests/test_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from shapely.geometry import MultiPolygon, Point, Polygon
 
 import regionmask
 from regionmask import Regions, plot_3D_mask
 from regionmask.core.plot import (
     _check_unused_kws,
     _flatten_polygons,
+    _maybe_gca,
     _polygons_coords,
-    _subsample,
 )
 
-from . import requires_cartopy, requires_matplotlib
+from . import assert_no_warnings, requires_cartopy, requires_matplotlib
 
 # =============================================================================
 
 # set up the testing regions
 
 name = "Example"
 numbers = [0, 1]
@@ -55,14 +55,17 @@
 poly = {1: poly1, 2: poly2}
 
 r2 = Regions(name=name, numbers=numbers, names=names, abbrevs=abbrevs, outlines=poly)
 
 multipoly = MultiPolygon([poly1, poly2])
 r3 = Regions([multipoly])
 
+# a region with segments longer than 1, use Polygon to close the coords
+r_large = regionmask.Regions([Polygon(c * 10) for c in r1.coords])
+
 # create a polygon with a hole
 interior1_closed = ((0.2, 0.2), (0.2, 0.45), (0.45, 0.45), (0.45, 0.2), (0.2, 0.2))
 interior2_closed = ((0.55, 0.55), (0.55, 0.8), (0.8, 0.8), (0.8, 0.55), (0.55, 0.55))
 poly1_interior1 = Polygon(outl1, [interior1_closed])
 poly1_interior2 = Polygon(outl1, [interior1_closed, interior2_closed])
 
 point = Point(1, 2)
@@ -85,38 +88,14 @@
     "plot_regions",
 ]
 
 
 # =============================================================================
 
 
-def test_subsample():
-
-    result = _subsample([[0, 1], [1, 0]])
-    expected = np.vstack((np.arange(0, 1.01, 0.02), np.arange(1, -0.01, -0.02))).T
-
-    assert np.allclose(expected, result)
-
-    result = _subsample(outl1_closed, num=2)
-
-    expected = [
-        [0, 0],
-        [0, 0.5],
-        [0, 1],
-        [0.5, 1],
-        [1, 1.0],
-        [1, 0.5],
-        [1, 0],
-        [0.5, 0],
-        [0, 0],
-    ]
-
-    assert np.allclose(expected, result)
-
-
 def test_flatten_polygons():
     # TODO: move to test_utils.py
 
     result = _flatten_polygons([poly1])
     assert len(result) == 1
     assert result[0].equals(poly1)
 
@@ -166,75 +145,135 @@
     assert np.allclose(interior1_closed, result[1])
     assert np.allclose(interior2_closed, result[2])
 
 
 # =============================================================================
 
 
+@requires_matplotlib
+def test_maybe_gca():
+
+    with figure_context():
+        ax = _maybe_gca(aspect=1)
+
+        assert isinstance(ax, mpl.axes.Axes)
+        assert ax.get_aspect() == 1
+
+    with figure_context():
+
+        # create figure without axes
+        plt.figure()
+        ax = _maybe_gca(aspect=1)
+
+        assert isinstance(ax, mpl.axes.Axes)
+        assert ax.get_aspect() == 1
+
+    with figure_context():
+        existing_axes = plt.axes()
+        ax = _maybe_gca(aspect=1)
+
+        # re-uses the existing axes
+        assert existing_axes == ax
+        # kwargs are ignored when reusing axes
+        assert ax.get_aspect() == "auto"
+
+
 @requires_cartopy
-@pytest.mark.filterwarnings("ignore:numpy.dtype size changed")
-@pytest.mark.filterwarnings("ignore:numpy.ufunc size changed")
 def test_plot_projection():
 
     # default is PlateCarree
     with figure_context():
-        ax = r1.plot(subsample=False)
+        ax = r1.plot(tolerance=None)
         assert isinstance(ax.projection, ccrs.PlateCarree)
 
-    # make sure the proj keword is respected
+    # make sure the proj keyword is respected
     with figure_context():
-        ax = r1.plot(subsample=False, projection=ccrs.Miller())
+        ax = r1.plot(tolerance=None, projection=ccrs.Miller())
         assert isinstance(ax.projection, ccrs.Miller)
 
     # projection given with axes is respected
     with figure_context() as f:
         ax = f.subplots(subplot_kw=dict(projection=ccrs.Mollweide()))
-        ax = r1.plot(subsample=False, ax=ax)
+        ax = r1.plot(tolerance=None, ax=ax)
         assert isinstance(ax.projection, ccrs.Mollweide)
 
 
 @requires_cartopy
+def test_plot_gca():
+
+    with figure_context() as f:
+        axs = f.subplots(1, 2, subplot_kw=dict(projection=ccrs.Robinson()))
+
+        ax = r1.plot(tolerance=None)
+        assert ax is axs[1]
+
+    with figure_context() as f:
+        ax = f.subplots()
+
+        match = "current axes .* is not a cartopy GeoAxes"
+        with pytest.raises(TypeError, match=match):
+            r1.plot(tolerance=None)
+
+    with figure_context() as f:
+        ax = f.subplots()
+
+        match = "passed axes .* is not a cartopy GeoAxes"
+        with pytest.raises(TypeError, match=match):
+            r1.plot(tolerance=None, ax=ax)
+
+
+@requires_cartopy
+def test_plot_regions_gca():
+
+    with figure_context() as f:
+        axs = f.subplots(1, 2)
+
+        ax = r1.plot_regions(tolerance=None)
+        assert ax is axs[1]
+
+
+@requires_cartopy
 def test_plot_deprecated_proj():
 
     proj = ccrs.PlateCarree()
     with pytest.warns(FutureWarning, match="'proj' has been renamed to 'projection'"):
         with figure_context():
-            ax = r1.plot(subsample=False, proj=proj)
+            ax = r1.plot(tolerance=None, proj=proj)
             assert isinstance(ax.projection, ccrs.PlateCarree)
 
     with pytest.raises(TypeError, match="Cannot set 'proj' and 'projection'"):
-        r1.plot(subsample=False, proj=proj, projection=proj)
+        r1.plot(tolerance=None, proj=proj, projection=proj)
 
 
 @requires_cartopy
 def test_plot_regions_projection():
 
     # if none is given -> no projection
     with figure_context():
-        ax = r1.plot_regions(subsample=False)
+        ax = r1.plot_regions(tolerance=None)
         assert not hasattr(ax, "projection")
 
     # projection given with axes is respected
     with figure_context() as f:
         ax = f.subplots(subplot_kw=dict(projection=ccrs.Mollweide()))
-        ax = r1.plot_regions(subsample=False, ax=ax)
+        ax = r1.plot_regions(tolerance=None, ax=ax)
         assert isinstance(ax.projection, ccrs.Mollweide)
 
 
 # -----------------------------------------------------------------------------
 
 
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
 def test_plot_lines(plotfunc):
 
     func = getattr(r1, plotfunc)
 
     with figure_context():
-        ax = func(subsample=False)
+        ax = func(tolerance=None)
 
         lines = ax.collections[0].get_segments()
 
         assert len(lines) == 2
         assert np.allclose(lines[0], outl1_closed)
         assert np.allclose(lines[1], outl2_closed)
 
@@ -244,15 +283,15 @@
 def test_plot_lines_multipoly(plotfunc):
     """regression of 47: because multipolygons were concatenated
     they did not look closed"""
 
     func = getattr(r3, plotfunc)
 
     with figure_context():
-        ax = func(subsample=False)
+        ax = func(tolerance=None)
 
         lines = ax.collections[0].get_segments()
         assert len(lines) == 2
         assert np.allclose(lines[0], outl1_closed)
         assert np.allclose(lines[1], outl2_closed)
 
 
@@ -263,69 +302,69 @@
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
 @pytest.mark.filterwarnings("ignore:The 'regions' keyword has been deprecated")
 def test_plot_lines_selection(plotfunc):
 
     func = getattr(r1, plotfunc)
 
     with figure_context():
-        ax = func(subsample=False, regions=[0, 1])
+        ax = func(tolerance=None, regions=[0, 1])
         lines = ax.collections[0].get_segments()
         assert len(lines) == 2
         assert np.allclose(lines[0], outl1_closed)
         assert np.allclose(lines[1], outl2_closed)
 
     # select a single number
     with figure_context():
-        ax = func(subsample=False, regions=0)
+        ax = func(tolerance=None, regions=0)
         lines = ax.collections[0].get_segments()
         assert len(lines) == 1
         assert np.allclose(lines[0], outl1_closed)
 
     # select by number
     with figure_context():
-        ax = func(subsample=False, regions=[0])
+        ax = func(tolerance=None, regions=[0])
         lines = ax.collections[0].get_segments()
         assert len(lines) == 1
         assert np.allclose(lines[0], outl1_closed)
 
     # select by long_name
     with figure_context():
-        ax = func(subsample=False, regions=["Unit Square1"])
+        ax = func(tolerance=None, regions=["Unit Square1"])
         lines = ax.collections[0].get_segments()
         assert len(lines) == 1
         assert np.allclose(lines[0], outl1_closed)
 
     # select by abbreviation
     with figure_context():
-        ax = func(subsample=False, regions=["uSq1"])
+        ax = func(tolerance=None, regions=["uSq1"])
         lines = ax.collections[0].get_segments()
         assert len(lines) == 1
         assert np.allclose(lines[0], outl1_closed)
 
 
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
 def test_plot_regions_kw_deprecated(plotfunc):
 
     func = getattr(r1, plotfunc)
 
     with pytest.warns(FutureWarning, match="The 'regions' keyword has been deprecated"):
         with figure_context():
-            func(subsample=False, regions=[0, 1])
+            func(tolerance=None, regions=[0, 1])
 
     with pytest.warns(FutureWarning, match="The 'regions' keyword has been deprecated"):
         with figure_context():
-            func(subsample=False, regions="all")
+            func(tolerance=None, regions="all")
 
 
 @requires_matplotlib
 @requires_cartopy
 def test_error_extra_kwarg():
     # manual TypeError for extra kwargs
-    # remove test after coastlines and proj kewords are removed
+    # remove test after coastlines and proj keywords are removed
 
     with pytest.raises(TypeError, match="got an unexpected keyword argument 'bar'"):
         with figure_context():
             r1.plot(bar=5)
 
 
 # -----------------------------------------------------------------------------
@@ -342,45 +381,83 @@
     ):
         with figure_context():
             func(None)
 
 
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
-def test_plot_lines_subsample(plotfunc):
+def test_plot_lines_tolerance(plotfunc):
 
     func = getattr(r1, plotfunc)
 
     with figure_context():
-        ax = func(subsample=True)
+        ax = func(tolerance=1 / 50)
         lines = ax.collections[0].get_paths()
 
         assert len(lines) == 2
         assert np.allclose(lines[0].vertices.shape, (201, 2))
 
 
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
-@pytest.mark.parametrize("n, expected", [(9, (9 - 1) * 50 + 1), (10, 10)])
-def test_plot_lines_maybe_subsample(plotfunc, n, expected):
-    """only subset non-polygons if they have less than 10 elements GH153
-    should eventually be superseeded by GH109"""
-
-    # create closed coordinates with n points
-    coords = np.linspace(interior1_closed[0], interior1_closed[1], num=n - 4)
-    coords = np.vstack((coords, interior1_closed[1:]))
-    r = Regions([coords])
+def test_plot_lines_tolerance_None(plotfunc):
+
+    func = getattr(r_large, plotfunc)
 
-    func = getattr(r, plotfunc)
     with figure_context():
-        ax = func(subsample=True)
+        ax = func(tolerance=None)
         lines = ax.collections[0].get_paths()
 
-        assert len(lines) == 1
-        assert np.allclose(lines[0].vertices.shape, (expected, 2))
+        np.testing.assert_allclose(lines[0].vertices, r_large.coords[0])
+        np.testing.assert_allclose(lines[1].vertices, r_large.coords[1])
+
+
+@requires_matplotlib
+@pytest.mark.parametrize("plotfunc", PLOTFUNCS)
+@pytest.mark.parametrize("kwargs", ({}, {"tolerance": "auto"}))
+def test_plot_lines_tolerance_auto(plotfunc, kwargs):
+
+    func = getattr(r_large, plotfunc)
+
+    expected = (41, 2) if plotfunc == "plot" else (5, 2)
+
+    with figure_context():
+        ax = func(**kwargs)
+
+        lines = ax.collections[0].get_paths()
+        np.testing.assert_allclose(lines[0].vertices.shape, expected)
+        np.testing.assert_allclose(lines[1].vertices.shape, expected)
+
+
+@requires_cartopy
+def test_plot_regions_lines_tolerance_cartopy_axes():
+
+    expected = (41, 2)
+
+    # when passing GeoAxes -> auto segmentizes lines
+    with figure_context():
+        ax = r_large.plot_regions(ax=plt.axes(projection=ccrs.PlateCarree()))
+
+        lines = ax.collections[0].get_paths()
+        np.testing.assert_allclose(lines[0].vertices.shape, expected)
+        np.testing.assert_allclose(lines[1].vertices.shape, expected)
+
+
+@requires_matplotlib
+@pytest.mark.parametrize("plotfunc", PLOTFUNCS)
+@pytest.mark.parametrize("subsample", [True, False])
+def test_plot_lines_subsample_deprecated(plotfunc, subsample):
+
+    func = getattr(r1, plotfunc)
+
+    with pytest.warns(
+        FutureWarning, match="The 'subsample' keyword has been deprecated."
+    ):
+        with figure_context():
+            func(subsample=subsample)
 
 
 # -----------------------------------------------------------------------------
 
 
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
@@ -403,15 +480,15 @@
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
 def test_plot_line_prop(plotfunc):
 
     func = getattr(r1, plotfunc)
 
     with figure_context():
-        ax = func(subsample=False, line_kws=dict(lw=2, color="g"))
+        ax = func(tolerance=None, line_kws=dict(lw=2, color="g"))
 
         collection = ax.collections[0]
 
         assert collection.get_linewidth() == 2
         np.testing.assert_equal(collection.get_color(), mpl.colors.to_rgba_array("g"))
 
 
@@ -421,56 +498,56 @@
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
 def test_plot_label_defaults(plotfunc):
 
     func = getattr(r1, plotfunc)
 
     with figure_context():
-        ax = func(subsample=False)
+        ax = func(tolerance=None)
         texts = ax.texts
         assert len(texts) == 2
 
 
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
 def test_plot_label(plotfunc):
 
     func = getattr(r1, plotfunc)
 
     with figure_context():
-        ax = func(subsample=False, add_label=True)
+        ax = func(tolerance=None, add_label=True)
         texts = ax.texts
 
         # default text is the number
         assert len(texts) == 2
         assert texts[0].get_text() == "0"
         assert texts[1].get_text() == "1"
 
         # they are at the centroid
         assert np.allclose(texts[0].get_position(), (0.5, 0.5))
         assert np.allclose(texts[1].get_position(), (0.5, 1.5))
 
     # no label
     with figure_context():
-        ax = func(subsample=False, add_label=False)
+        ax = func(tolerance=None, add_label=False)
         texts = ax.texts
         assert len(texts) == 0
 
     # label: abbrev
     with figure_context():
-        ax = func(subsample=False, add_label=True, label="abbrev")
+        ax = func(tolerance=None, add_label=True, label="abbrev")
         texts = ax.texts
 
         assert len(texts) == 2
         assert texts[0].get_text() == "uSq1"
         assert texts[1].get_text() == "uSq2"
 
     # label: name
     with figure_context():
-        ax = func(subsample=False, add_label=True, label="name")
+        ax = func(tolerance=None, add_label=True, label="name")
         texts = ax.texts
 
         assert len(texts) == 2
         assert texts[0].get_text() == "Unit Square1"
         assert texts[1].get_text() == "Unit Square2"
 
 
@@ -482,38 +559,38 @@
 
     with pytest.raises(
         ValueError, match="'label_multipolygon' must be one of 'all' and 'largest'"
     ):
         func(label_multipolygon=None)
 
     with figure_context():
-        ax = func(subsample=False, add_label=True, label_multipolygon="all")
+        ax = func(tolerance=None, add_label=True, label_multipolygon="all")
         texts = ax.texts
 
         assert len(texts) == 2
         assert texts[0].get_text() == "0"
         assert texts[1].get_text() == "0"
 
     with figure_context():
-        ax = func(subsample=False, add_label=True, label_multipolygon="largest")
+        ax = func(tolerance=None, add_label=True, label_multipolygon="largest")
         texts = ax.texts
 
         assert len(texts) == 1
         assert texts[0].get_text() == "0"
 
 
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
 def test_plot_text_prop(plotfunc):
 
     func = getattr(r1, plotfunc)
 
     with figure_context():
 
-        ax = func(subsample=False, add_label=True, text_kws=dict(fontsize=15))
+        ax = func(tolerance=None, add_label=True, text_kws=dict(fontsize=15))
 
         texts = ax.texts
 
         assert texts[0].get_fontsize() == 15
         assert texts[1].get_fontsize() == 15
 
         assert texts[0].get_va() == "center"
@@ -527,37 +604,37 @@
 def test_plot_text_clip(plotfunc):
     """test fix for #157"""
 
     func = getattr(r1, plotfunc)
 
     with figure_context():
 
-        ax = func(subsample=False, add_label=True)
+        ax = func(tolerance=None, add_label=True)
 
         texts = ax.texts
 
         for text in texts:
             assert text.get_clip_on() is True
             assert text.get_clip_box() == ax.bbox
 
     with figure_context():
 
-        ax = func(subsample=False, add_label=True, text_kws=dict(clip_on=False))
+        ax = func(tolerance=None, add_label=True, text_kws=dict(clip_on=False))
 
         texts = ax.texts
 
         for text in texts:
             assert text.get_clip_on() is False
 
 
 @requires_matplotlib
 @requires_cartopy
 def test_plot_ocean():
 
-    kwargs = dict(subsample=False, add_label=False, add_coastlines=False)
+    kwargs = dict(tolerance=None, add_label=False, add_coastlines=False)
 
     # no ocean per default
     with figure_context():
         ax = r1.plot(**kwargs)
         assert len(ax.artists) == 0
 
     with figure_context():
@@ -583,15 +660,15 @@
         assert art.get_zorder() == 1
 
 
 @requires_matplotlib
 @requires_cartopy
 def test_plot_land():
 
-    kwargs = dict(subsample=False, add_label=False, add_coastlines=False)
+    kwargs = dict(tolerance=None, add_label=False, add_coastlines=False)
 
     # no land per default
     with figure_context():
         ax = r1.plot(**kwargs)
         assert len(ax.artists) == 0
 
     with figure_context():
@@ -615,15 +692,15 @@
         assert art.get_zorder() == 1
 
 
 @requires_matplotlib
 @requires_cartopy
 def test_plot_add_coastlines():
 
-    kwargs = dict(subsample=False, add_label=False)
+    kwargs = dict(tolerance=None, add_label=False)
 
     # coastlines are added per default
     with figure_context():
         ax = r1.plot(**kwargs)
         assert len(ax.artists) == 1
 
     with figure_context():
@@ -643,15 +720,15 @@
         assert art._kwargs == {"edgecolor": "black", "facecolor": "none"}
 
 
 @requires_matplotlib
 @requires_cartopy
 def test_plot_coastlines_deprecated():
 
-    kwargs = dict(subsample=False, add_label=False)
+    kwargs = dict(tolerance=None, add_label=False)
 
     with pytest.warns(FutureWarning, match="'coastlines' has been renamed"):
         with figure_context():
             ax = r1.plot(coastlines=True, **kwargs)
             assert len(ax.artists) == 1
 
     with pytest.raises(TypeError, match="Cannot set 'coastlines' and 'add_coastlines'"):
@@ -684,46 +761,60 @@
         assert np.ma.allequal(expected, h.get_array())
 
         # ensure kwargs are passed through
         assert h.get_zorder() == 3
 
 
 @requires_matplotlib
+def test_plot_3D_mask_overlap():
+
+    lon = np.arange(-180, 180, 2)
+    lat = np.arange(90, -91, -2)
+
+    outline_GLOB = np.array(
+        [[-180.0, 90.0], [-180.0, -90.0], [180.0, -90.0], [180.0, 90.0]]
+    )
+    region = regionmask.Regions([outline_GLOB, outline_GLOB], overlap=True)
+
+    mask_3D = region.mask_3D(lon, lat)
+
+    with pytest.warns(RuntimeWarning, match="overlapping regions"):
+        plot_3D_mask(mask_3D)
+
+
+@requires_matplotlib
 @requires_cartopy
 def test_check_unused_kws():
 
     # ensure no warning is raised
-    with pytest.warns(None) as record:
+    with assert_no_warnings():
         _check_unused_kws(True, None, "feature_name", "kws_name")
-    assert not record
 
-    with pytest.warns(None) as record:
+    with assert_no_warnings():
         _check_unused_kws(True, {}, "feature_name", "kws_name")
-    assert not record
 
-    with pytest.warns(None) as record:
+    with assert_no_warnings():
         _check_unused_kws(False, None, "feature_name", "kws_name")
-    assert not record
 
     with pytest.warns(
         RuntimeWarning, match="'kws_name' are passed but 'feature_name' is False"
     ):
         _check_unused_kws(False, {}, "feature_name", "kws_name")
 
 
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
 def test_plot_no_warning_default(plotfunc):
+    # ensure no warning is raised on default
 
     func = getattr(r1, plotfunc)
 
-    # ensure no warning is raised on default
-    with pytest.warns(None) as record:
-        func()
-    assert not record
+    with figure_context():
+        with assert_no_warnings():
+            func()
 
 
 @requires_matplotlib
 @pytest.mark.parametrize("plotfunc", PLOTFUNCS)
 def test_plot_unused_text_kws(plotfunc):
 
     func = getattr(r1, plotfunc)
```

### Comparing `regionmask-0.8.0/regionmask/tests/test_wrapAngle.py` & `regionmask-0.9.0/regionmask/tests/test_wrapAngle.py`

 * *Files identical despite different names*

### Comparing `regionmask-0.8.0/regionmask.egg-info/PKG-INFO` & `regionmask-0.9.0/regionmask.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: regionmask
-Version: 0.8.0
+Version: 0.9.0
 Summary: plotting and creation of masks for spatial regions
 Home-page: https://github.com/regionmask/regionmask
 Author: regionmask Developers
 Author-email: mathias.hauser@env.ethz.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 See https://regionmask.readthedocs.io
```

### Comparing `regionmask-0.8.0/regionmask.egg-info/SOURCES.txt` & `regionmask-0.9.0/regionmask.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/ci-additional.yaml
 .github/workflows/ci.yaml
 .github/workflows/linting.yaml
 ci/min_deps_check.py
 ci/requirements/docs.yml
 ci/requirements/environment.yml
-ci/requirements/py36-bare-minimum.yml
-ci/requirements/py36-min-all-deps.yml
+ci/requirements/py37-bare-minimum.yml
+ci/requirements/py37-min-all-deps.yml
 data/IPCC-WGI-reference-regions-v1.zip
 data/IPCC-WGI-reference-regions-v4.zip
 data/README.md
 data/regions_remote_catalog.yaml
 docs/.gitignore
 docs/Makefile
 docs/README_ipynp_for_RTD
@@ -42,14 +42,15 @@
 docs/logo/logo.ipynb
 docs/logo/logo.png
 docs/notebooks/create_own_regions.ipynb
 docs/notebooks/geopandas.ipynb
 docs/notebooks/mask_2D.ipynb
 docs/notebooks/mask_3D.ipynb
 docs/notebooks/method.ipynb
+docs/notebooks/overlap.ipynb
 docs/notebooks/plotting.ipynb
 docs/notebooks/tutorial_rst.tpl
 licences/AR6_REGIONS_LICENSE
 licences/XARRAY_LICENSE
 regionmask/__init__.py
 regionmask.egg-info/PKG-INFO
 regionmask.egg-info/SOURCES.txt
@@ -63,24 +64,26 @@
 regionmask/core/mask.py
 regionmask/core/plot.py
 regionmask/core/regions.py
 regionmask/core/utils.py
 regionmask/defined_regions/__init__.py
 regionmask/defined_regions/_ar6.py
 regionmask/defined_regions/_ar6_pre_revisions.py
+regionmask/defined_regions/_natural_earth.py
 regionmask/defined_regions/_ressources.py
 regionmask/defined_regions/giorgi.py
-regionmask/defined_regions/natural_earth.py
+regionmask/defined_regions/prudence.py
 regionmask/defined_regions/srex.py
 regionmask/tests/__init__.py
 regionmask/tests/test_OneRegion.py
 regionmask/tests/test_Regions.py
+regionmask/tests/test_create_dataarray.py
 regionmask/tests/test_defined_regions.py
 regionmask/tests/test_formatting.py
 regionmask/tests/test_geopandas.py
 regionmask/tests/test_mask.py
 regionmask/tests/test_mask_defined_regions.py
 regionmask/tests/test_plot.py
-regionmask/tests/test_save_utils.py
+regionmask/tests/test_segmentize.py
 regionmask/tests/test_utils.py
 regionmask/tests/test_wrapAngle.py
 regionmask/tests/utils.py
```

### Comparing `regionmask-0.8.0/setup.cfg` & `regionmask-0.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Intended Audience :: Science/Research
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Atmospheric Science
 	Topic :: Scientific/Engineering :: GIS
 
 [options]
 packages = find:
 zip_safe = False  # https://mypy.readthedocs.io/en/latest/installed_packages.html
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
-	geopandas >= 0.6
+	geopandas >= 0.7
 	numpy >= 1.17
-	pooch >= 1.0
-	rasterio >= 1.0
+	pooch >= 1.2
+	rasterio >= 1.1
+	packaging >= 20.0
 	setuptools >= 40.4  # for pkg_resources
-	shapely >= 1.6
+	shapely >= 1.7
 	xarray >= 0.15
 
 [tool:pytest]
 python_files = test_*.py
 testpaths = regionmask/tests
 filterwarnings = 
 	ignore:numpy.ufunc size changed, may indicate binary incompatibility.:RuntimeWarning
```

