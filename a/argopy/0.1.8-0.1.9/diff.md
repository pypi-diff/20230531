# Comparing `tmp/argopy-0.1.8.tar.gz` & `tmp/argopy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argopy-0.1.8.tar", last modified: Tue Nov  2 13:55:36 2021, max compression
+gzip compressed data, was "argopy-0.1.9.tar", last modified: Mon Jan 17 09:12:01 2022, max compression
```

## Comparing `argopy-0.1.8.tar` & `argopy-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 13:55:36.534184 argopy-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    10273 2021-11-02 13:55:21.000000 argopy-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-02 13:55:21.000000 argopy-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2021-11-02 13:55:36.534184 argopy-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6655 2021-11-02 13:55:21.000000 argopy-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 13:55:36.530184 argopy-0.1.8/argopy/
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 13:55:36.530184 argopy-0.1.8/argopy/assets/
--rw-r--r--   0 runner    (1001) docker     (121)      959 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/assets/dict_institutions.pickle
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/assets/dict_profilers.pickle
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 13:55:36.530184 argopy-0.1.8/argopy/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16191 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/data_fetchers/argovis_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    23044 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/data_fetchers/erddap_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     9782 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/data_fetchers/erddap_index.py
--rw-r--r--   0 runner    (1001) docker     (121)    21335 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/data_fetchers/localftp_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5739 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/data_fetchers/localftp_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     3134 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/data_fetchers/proto.py
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    28305 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/fetchers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5937 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/options.py
--rw-r--r--   0 runner    (1001) docker     (121)    15590 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 13:55:36.530184 argopy-0.1.8/argopy/stores/
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17717 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/stores/argo_index.py
--rw-r--r--   0 runner    (1001) docker     (121)    26184 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/stores/filesystems.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 13:55:36.534184 argopy-0.1.8/argopy/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6869 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_fetchers_data_argovis.py
--rw-r--r--   0 runner    (1001) docker     (121)    10071 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_fetchers_data_erddap.py
--rw-r--r--   0 runner    (1001) docker     (121)     9044 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_fetchers_data_localftp.py
--rw-r--r--   0 runner    (1001) docker     (121)     9103 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_fetchers_facade_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4101 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_fetchers_facade_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     5587 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_fetchers_index_erddap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4377 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_fetchers_index_localftp.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_fetchers_proto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     7391 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_plotters.py
--rw-r--r--   0 runner    (1001) docker     (121)    11522 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (121)    16195 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     4954 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tests/test_xarray.py
--rw-r--r--   0 runner    (1001) docker     (121)     4796 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (121)    44092 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    36682 2021-11-02 13:55:21.000000 argopy-0.1.8/argopy/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 13:55:36.534184 argopy-0.1.8/argopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-11-02 13:55:36.000000 argopy-0.1.8/argopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-11-02 13:55:21.000000 argopy-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-11-02 13:55:21.000000 argopy-0.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-11-02 13:55:21.000000 argopy-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-02 13:55:36.534184 argopy-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      995 2021-11-02 13:55:21.000000 argopy-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 09:12:01.094407 argopy-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    10273 2022-01-17 09:11:47.000000 argopy-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-01-17 09:11:47.000000 argopy-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7190 2022-01-17 09:12:01.094407 argopy-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6587 2022-01-17 09:11:47.000000 argopy-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 09:12:01.086407 argopy-0.1.9/argopy/
+-rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 09:12:01.086407 argopy-0.1.9/argopy/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)      959 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/assets/dict_institutions.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/assets/dict_profilers.pickle
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 09:12:01.086407 argopy-0.1.9/argopy/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20565 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/data_fetchers/argovis_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23044 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/data_fetchers/erddap_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9782 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/data_fetchers/erddap_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21335 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/data_fetchers/localftp_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5739 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/data_fetchers/localftp_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3134 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/data_fetchers/proto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3025 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30901 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/fetchers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6124 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17321 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 09:12:01.086407 argopy-0.1.9/argopy/stores/
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17717 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/stores/argo_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26184 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/stores/filesystems.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 09:12:01.094407 argopy-0.1.9/argopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     6981 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7607 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_fetchers_data_argovis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10071 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_fetchers_data_erddap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9044 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_fetchers_data_localftp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9395 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_fetchers_facade_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7143 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_fetchers_facade_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5587 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_fetchers_index_erddap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_fetchers_index_localftp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_fetchers_proto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7897 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11522 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18227 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9628 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tests/test_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58247 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    78035 2022-01-17 09:11:47.000000 argopy-0.1.9/argopy/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 09:12:01.094407 argopy-0.1.9/argopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-01-17 09:12:00.000000 argopy-0.1.9/argopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-01-17 09:11:47.000000 argopy-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-01-17 09:11:47.000000 argopy-0.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2022-01-17 09:11:47.000000 argopy-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-17 09:12:01.094407 argopy-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-01-17 09:11:47.000000 argopy-0.1.9/setup.py
```

### Comparing `argopy-0.1.8/LICENSE` & `argopy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/PKG-INFO` & `argopy-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argopy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python library for Argo data beginners and experts
 Home-page: https://github.com/euroargodev/argopy
 Author: argopy Developers
 Author-email: gmaze@ifremer.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
@@ -23,126 +23,117 @@
 |Release|[![](https://img.shields.io/github/release-date/euroargodev/argopy)](//github.com/euroargodev/argopy/releases) [![PyPI](https://img.shields.io/pypi/v/argopy)](//pypi.org/project/argopy/) [![Conda](https://anaconda.org/conda-forge/argopy/badges/version.svg)](//anaconda.org/conda-forge/argopy)|
 |Development|![Github Action Status](https://github.com/euroargodev/argopy/workflows/tests/badge.svg?branch=master) [![Documentation Status](https://readthedocs.org/projects/argopy/badge/?version=latest)](https://argopy.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/gh/euroargodev/argopy/branch/master/graph/badge.svg)](https://codecov.io/gh/euroargodev/argopy)<br>[![lifecycle](https://img.shields.io/badge/lifecycle-maturing-blue.svg)](https://www.tidyverse.org/lifecycle/#maturing)|
 |Data resources|![Erddap status](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/euroargodev/argopy-status/master/argopy_api_status_erddap.json) ![Argovis status](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/euroargodev/argopy-status/master/argopy_api_status_argovis.json) <br>![Profile count](https://img.shields.io/endpoint?label=Number%20of%20Argo%20profiles%3A&style=social&url=https%3A%2F%2Fapi.ifremer.fr%2Fargopy%2Fdata%2FARGO-FULL.json) <br>[![Statuspage](https://img.shields.io/static/v1?label=&message=Check%20all%20monitors&color=blue&logo=statuspage&logoColor=white)](https://argopy.statuspage.io)|
 
 ## Install
 
 
-Install the last release with pip:
+Install the last release with conda:
+```bash
+conda install -c conda-forge argopy
+```
+or pip:
 ```bash
 pip install argopy
 ```
+or conda:
+```bash
+conda install -c conda-forge argopy
+```
 
 But since this is a young library in active development, use direct install from this repo to benefit from the latest version:
 
 ```bash
 pip install git+http://github.com/euroargodev/argopy.git@master
 ```
 
-The ``argopy`` library should work under all OS (Linux, Mac and Windows) and with python versions 3.6, 3.7 and 3.8.
+The ``argopy`` library is tested to work under most OS (Linux, Mac) and with python versions 3.7 and 3.8.
 
 ## Usage
 
-[![badge](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Pangeo+Binder&message=Click+here+to+try+argopy+online+!&color=blue&style=for-the-badge)](https://binder.pangeo.io/v2/gh/euroargodev/argopy/master?urlpath=lab/tree/docs/tryit.ipynb)
+[![badge](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Pangeo+Binder&message=Click+here+to+try+argopy+online+!&color=blue&style=for-the-badge)](https://mybinder.org/v2/gh/euroargodev/argopy/master?labpath=docs/tryit.ipynb)
 
 ### Fetching Argo Data
 
-Init the default data fetcher like:
+Import the data fetcher:
 ```python
 from argopy import DataFetcher as ArgoDataFetcher
-argo_loader = ArgoDataFetcher()
 ```
-and then, request data for a **specific space/time domain**:
+and then, set it up to request data for a **specific space/time domain**:
 ```python
-ds = argo_loader.region([-85,-45,10.,20.,0,10.]).to_xarray()
-ds = argo_loader.region([-85,-45,10.,20.,0,1000.,'2012-01','2012-12']).to_xarray()
+argo_loader = ArgoDataFetcher().region([-85,-45,10.,20.,0,10.])
+argo_loader = ArgoDataFetcher().region([-85,-45,10.,20.,0,1000.,'2012-01','2012-12'])
 ```
 for **profiles of a given float**: 
 ```python
-ds = argo_loader.profile(6902746, 34).to_xarray()
-ds = argo_loader.profile(6902746, np.arange(12,45)).to_xarray()
-ds = argo_loader.profile(6902746, [1,12]).to_xarray()
+argo_loader = ArgoDataFetcher().profile(6902746, 34)
+argo_loader = ArgoDataFetcher().profile(6902746, np.arange(12,45))
+argo_loader = ArgoDataFetcher().profile(6902746, [1,12])
 ```
 or for **one or a collection of floats**:
 ```python
-ds = argo_loader.float(6902746).to_xarray()
-ds = argo_loader.float([6902746, 6902747, 6902757, 6902766]).to_xarray()
+argo_loader = ArgoDataFetcher().float(6902746)
+argo_loader = ArgoDataFetcher().float([6902746, 6902747, 6902757, 6902766])
+```
+
+Once your fetcher is initialized you can trigger fetch/load data like this:
+```python
+ds = argo_loader.to_xarray()  # or:
+ds = argo_loader.load().data
 ```
 By default fetched data are returned in memory as [xarray.DataSet](http://xarray.pydata.org/en/stable/data-structures.html#dataset). 
 From there, it is easy to convert it to other formats like a [Pandas dataframe](https://pandas.pydata.org/pandas-docs/stable/getting_started/dsintro.html#dataframe):
 ```python
-ds = ArgoDataFetcher().profile(6902746, 34).to_xarray()
-df = ds.to_dataframe()
+df = ArgoDataFetcher().profile(6902746, 34).load().data.to_dataframe()
 ```
 
 or to export it to files:
 ```python
-ds = argo_loader.region([-85,-45,10.,20.,0,100.]).to_xarray()
+ds = ArgoDataFetcher().region([-85,-45,10.,20.,0,100.]).to_xarray()
 ds.to_netcdf('my_selection.nc')
 # or by profiles:
 ds.argo.point2profile().to_netcdf('my_selection.nc')
 ```
 
 
-### Argo Index Fetcher
-Index object is returned as a pandas dataframe.
+### Fetching only Argo index
+Argo index are returned as pandas dataframe. Index fetchers works similarly to data fetchers.
 
-Init the fetcher:
+Load the Argo index fetcher:
 ```python
     from argopy import IndexFetcher as ArgoIndexFetcher
-
-    index_loader = ArgoIndexFetcher()
-    index_loader = ArgoIndexFetcher(src='erddap')    
-    #Local ftp backend 
-    #index_loader = ArgoIndexFetcher(src='localftp',path_ftp='/path/to/your/argo/ftp/',index_file='ar_index_global_prof.txt')
 ```
-and then, set the index request index for a domain:
+then, set it up to request index for a **specific space/time domain**:
 ```python
-    idx=index_loader.region([-85,-45,10.,20.])
-    idx=index_loader.region([-85,-45,10.,20.,'2012-01','2014-12'])
+    index_loader = ArgoIndexFetcher().region([-85,-45,10.,20.])
+    index_loader = ArgoIndexFetcher().region([-85,-45,10.,20.,'2012-01','2014-12'])
 ```
-or for a collection of floats:
+or for **one or a collection of floats**:
 ```python
-    idx=index_loader.float(6902746)
-    idx=index_loader.float([6902746, 6902747, 6902757, 6902766])   
+    index_loader = ArgoIndexFetcher().float(6902746)
+    index_loader = ArgoIndexFetcher().float([6902746, 6902747, 6902757, 6902766])   
 ```
-then you can see you index as a pandas dataframe or a xarray dataset :
+Once your fetcher is initialized you can trigger fetch/load index like this:
 ```python
-    idx.to_dataframe()
-    idx.to_xarray()
+    df = index_loader.to_dataframe()  # or
+    df = index_loader.load().index
 ```
-For plottings methods, you'll need `matplotlib`, `cartopy` and `seaborn` installed (they're not in requirements).  
-For plotting the map of your query :
-```python    
-    idx.plot('trajectory')    
+
+Note that like the data fetcher, the index fetcher can use different sources, a local copy of the GDAC ftp for instance:
+```python
+    index_fetcher = ArgoIndexFetcher(src='localftp', path_ftp='/path/to/your/argo/ftp/', index_file='ar_index_global_prof.txt')
 ```
-![index_traj](https://user-images.githubusercontent.com/17851004/78023937-d0c2d580-7357-11ea-9974-70a2aaf30590.png)
 
-For plotting the distribution of DAC or profiler type of the indexed profiles :
+### Visualisation
+For plottings methods, you'll need `matplotlib` and possibly `cartopy` and `seaborn` installed.
+Argo Data and Index fetchers provide direct plotting methods, for instance:
 ```python    
-    idx.plot('dac')    
-    idx.plot('profiler')`
+    ArgoDataFetcher().float([6902745, 6902746]).plot('trajectory')    
 ```
-![dac](https://user-images.githubusercontent.com/17851004/78024137-26977d80-7358-11ea-8557-ef39a88028b2.png)
+![index_traj](https://github.com/euroargodev/argopy/raw/master/docs/_static/trajectory_sample.png)
 
+See the [documentation page for more examples](https://argopy.readthedocs.io/en/latest/visualisation.html).
 
 ## Development roadmap
 
-Our next big steps:
-- [ ] To provide Bio-geochemical variables
-
-We aim to provide high level helper methods to load Argo data and meta-data from:
-- [x] Ifremer erddap
-- [x] local copy of the GDAC ftp folder
-- [x] Index files (local and online)
-- [x] Argovis
-- [ ] Online GDAC ftp
-- [ ] any other useful access point to Argo data ?
-
-We also aim to provide high level helper methods to visualise and plot Argo data and meta-data:
-- [x] Map with trajectories
-- [ ] Waterfall plots
-- [ ] T/S diagram
-- [ ] etc !
-
-
+See milestone here: https://github.com/euroargodev/argopy/milestone/3
```

### Comparing `argopy-0.1.8/README.md` & `argopy-0.1.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,124 +5,116 @@
 |Release|[![](https://img.shields.io/github/release-date/euroargodev/argopy)](//github.com/euroargodev/argopy/releases) [![PyPI](https://img.shields.io/pypi/v/argopy)](//pypi.org/project/argopy/) [![Conda](https://anaconda.org/conda-forge/argopy/badges/version.svg)](//anaconda.org/conda-forge/argopy)|
 |Development|![Github Action Status](https://github.com/euroargodev/argopy/workflows/tests/badge.svg?branch=master) [![Documentation Status](https://readthedocs.org/projects/argopy/badge/?version=latest)](https://argopy.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/gh/euroargodev/argopy/branch/master/graph/badge.svg)](https://codecov.io/gh/euroargodev/argopy)<br>[![lifecycle](https://img.shields.io/badge/lifecycle-maturing-blue.svg)](https://www.tidyverse.org/lifecycle/#maturing)|
 |Data resources|![Erddap status](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/euroargodev/argopy-status/master/argopy_api_status_erddap.json) ![Argovis status](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/euroargodev/argopy-status/master/argopy_api_status_argovis.json) <br>![Profile count](https://img.shields.io/endpoint?label=Number%20of%20Argo%20profiles%3A&style=social&url=https%3A%2F%2Fapi.ifremer.fr%2Fargopy%2Fdata%2FARGO-FULL.json) <br>[![Statuspage](https://img.shields.io/static/v1?label=&message=Check%20all%20monitors&color=blue&logo=statuspage&logoColor=white)](https://argopy.statuspage.io)|
 
 ## Install
 
 
-Install the last release with pip:
+Install the last release with conda:
+```bash
+conda install -c conda-forge argopy
+```
+or pip:
 ```bash
 pip install argopy
 ```
+or conda:
+```bash
+conda install -c conda-forge argopy
+```
 
 But since this is a young library in active development, use direct install from this repo to benefit from the latest version:
 
 ```bash
 pip install git+http://github.com/euroargodev/argopy.git@master
 ```
 
-The ``argopy`` library should work under all OS (Linux, Mac and Windows) and with python versions 3.6, 3.7 and 3.8.
+The ``argopy`` library is tested to work under most OS (Linux, Mac) and with python versions 3.7 and 3.8.
 
 ## Usage
 
-[![badge](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Pangeo+Binder&message=Click+here+to+try+argopy+online+!&color=blue&style=for-the-badge)](https://binder.pangeo.io/v2/gh/euroargodev/argopy/master?urlpath=lab/tree/docs/tryit.ipynb)
+[![badge](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Pangeo+Binder&message=Click+here+to+try+argopy+online+!&color=blue&style=for-the-badge)](https://mybinder.org/v2/gh/euroargodev/argopy/master?labpath=docs/tryit.ipynb)
 
 ### Fetching Argo Data
 
-Init the default data fetcher like:
+Import the data fetcher:
 ```python
 from argopy import DataFetcher as ArgoDataFetcher
-argo_loader = ArgoDataFetcher()
 ```
-and then, request data for a **specific space/time domain**:
+and then, set it up to request data for a **specific space/time domain**:
 ```python
-ds = argo_loader.region([-85,-45,10.,20.,0,10.]).to_xarray()
-ds = argo_loader.region([-85,-45,10.,20.,0,1000.,'2012-01','2012-12']).to_xarray()
+argo_loader = ArgoDataFetcher().region([-85,-45,10.,20.,0,10.])
+argo_loader = ArgoDataFetcher().region([-85,-45,10.,20.,0,1000.,'2012-01','2012-12'])
 ```
 for **profiles of a given float**: 
 ```python
-ds = argo_loader.profile(6902746, 34).to_xarray()
-ds = argo_loader.profile(6902746, np.arange(12,45)).to_xarray()
-ds = argo_loader.profile(6902746, [1,12]).to_xarray()
+argo_loader = ArgoDataFetcher().profile(6902746, 34)
+argo_loader = ArgoDataFetcher().profile(6902746, np.arange(12,45))
+argo_loader = ArgoDataFetcher().profile(6902746, [1,12])
 ```
 or for **one or a collection of floats**:
 ```python
-ds = argo_loader.float(6902746).to_xarray()
-ds = argo_loader.float([6902746, 6902747, 6902757, 6902766]).to_xarray()
+argo_loader = ArgoDataFetcher().float(6902746)
+argo_loader = ArgoDataFetcher().float([6902746, 6902747, 6902757, 6902766])
+```
+
+Once your fetcher is initialized you can trigger fetch/load data like this:
+```python
+ds = argo_loader.to_xarray()  # or:
+ds = argo_loader.load().data
 ```
 By default fetched data are returned in memory as [xarray.DataSet](http://xarray.pydata.org/en/stable/data-structures.html#dataset). 
 From there, it is easy to convert it to other formats like a [Pandas dataframe](https://pandas.pydata.org/pandas-docs/stable/getting_started/dsintro.html#dataframe):
 ```python
-ds = ArgoDataFetcher().profile(6902746, 34).to_xarray()
-df = ds.to_dataframe()
+df = ArgoDataFetcher().profile(6902746, 34).load().data.to_dataframe()
 ```
 
 or to export it to files:
 ```python
-ds = argo_loader.region([-85,-45,10.,20.,0,100.]).to_xarray()
+ds = ArgoDataFetcher().region([-85,-45,10.,20.,0,100.]).to_xarray()
 ds.to_netcdf('my_selection.nc')
 # or by profiles:
 ds.argo.point2profile().to_netcdf('my_selection.nc')
 ```
 
 
-### Argo Index Fetcher
-Index object is returned as a pandas dataframe.
+### Fetching only Argo index
+Argo index are returned as pandas dataframe. Index fetchers works similarly to data fetchers.
 
-Init the fetcher:
+Load the Argo index fetcher:
 ```python
     from argopy import IndexFetcher as ArgoIndexFetcher
-
-    index_loader = ArgoIndexFetcher()
-    index_loader = ArgoIndexFetcher(src='erddap')    
-    #Local ftp backend 
-    #index_loader = ArgoIndexFetcher(src='localftp',path_ftp='/path/to/your/argo/ftp/',index_file='ar_index_global_prof.txt')
 ```
-and then, set the index request index for a domain:
+then, set it up to request index for a **specific space/time domain**:
 ```python
-    idx=index_loader.region([-85,-45,10.,20.])
-    idx=index_loader.region([-85,-45,10.,20.,'2012-01','2014-12'])
+    index_loader = ArgoIndexFetcher().region([-85,-45,10.,20.])
+    index_loader = ArgoIndexFetcher().region([-85,-45,10.,20.,'2012-01','2014-12'])
 ```
-or for a collection of floats:
+or for **one or a collection of floats**:
 ```python
-    idx=index_loader.float(6902746)
-    idx=index_loader.float([6902746, 6902747, 6902757, 6902766])   
+    index_loader = ArgoIndexFetcher().float(6902746)
+    index_loader = ArgoIndexFetcher().float([6902746, 6902747, 6902757, 6902766])   
 ```
-then you can see you index as a pandas dataframe or a xarray dataset :
+Once your fetcher is initialized you can trigger fetch/load index like this:
 ```python
-    idx.to_dataframe()
-    idx.to_xarray()
+    df = index_loader.to_dataframe()  # or
+    df = index_loader.load().index
 ```
-For plottings methods, you'll need `matplotlib`, `cartopy` and `seaborn` installed (they're not in requirements).  
-For plotting the map of your query :
-```python    
-    idx.plot('trajectory')    
+
+Note that like the data fetcher, the index fetcher can use different sources, a local copy of the GDAC ftp for instance:
+```python
+    index_fetcher = ArgoIndexFetcher(src='localftp', path_ftp='/path/to/your/argo/ftp/', index_file='ar_index_global_prof.txt')
 ```
-![index_traj](https://user-images.githubusercontent.com/17851004/78023937-d0c2d580-7357-11ea-9974-70a2aaf30590.png)
 
-For plotting the distribution of DAC or profiler type of the indexed profiles :
+### Visualisation
+For plottings methods, you'll need `matplotlib` and possibly `cartopy` and `seaborn` installed.
+Argo Data and Index fetchers provide direct plotting methods, for instance:
 ```python    
-    idx.plot('dac')    
-    idx.plot('profiler')`
+    ArgoDataFetcher().float([6902745, 6902746]).plot('trajectory')    
 ```
-![dac](https://user-images.githubusercontent.com/17851004/78024137-26977d80-7358-11ea-8557-ef39a88028b2.png)
+![index_traj](https://github.com/euroargodev/argopy/raw/master/docs/_static/trajectory_sample.png)
 
+See the [documentation page for more examples](https://argopy.readthedocs.io/en/latest/visualisation.html).
 
 ## Development roadmap
 
-Our next big steps:
-- [ ] To provide Bio-geochemical variables
-
-We aim to provide high level helper methods to load Argo data and meta-data from:
-- [x] Ifremer erddap
-- [x] local copy of the GDAC ftp folder
-- [x] Index files (local and online)
-- [x] Argovis
-- [ ] Online GDAC ftp
-- [ ] any other useful access point to Argo data ?
-
-We also aim to provide high level helper methods to visualise and plot Argo data and meta-data:
-- [x] Map with trajectories
-- [ ] Waterfall plots
-- [ ] T/S diagram
-- [ ] etc !
-
+See milestone here: https://github.com/euroargodev/argopy/milestone/3
```

### Comparing `argopy-0.1.8/argopy/__init__.py` & `argopy-0.1.9/argopy/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,32 +17,33 @@
 
 from .xarray import ArgoAccessor  # noqa: E402
 from . import tutorial  # noqa: E402
 
 # Other Import
 from . import utilities  # noqa: E402
 from . import stores  # noqa: E402
-from .utilities import show_versions, show_options, clear_cache  # noqa: E402
+from .utilities import show_versions, show_options, clear_cache, TopoFetcher  # noqa: E402
 from .utilities import monitor_status as status  # noqa: E402
 from .options import set_options  # noqa: E402
 from .plotters import open_dashboard as dashboard  # noqa: E402
 
 #
 __all__ = (
     # Classes:
     "DataFetcher",
     "IndexFetcher",
     "ArgoAccessor",
-    # Top-level functions:
+    # Utilities promoted to top-level functions:
     "set_options",
     "show_versions",
     "show_options",
     "dashboard",
     "status",
     "clear_cache",
+    "TopoFetcher",  # Class
     # Sub-packages,
     "utilities",
     "errors",
     "plotters",
     "stores",
     "tutorial",
     # Constants
```

### Comparing `argopy-0.1.8/argopy/assets/dict_institutions.pickle` & `argopy-0.1.9/argopy/assets/dict_institutions.pickle`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/assets/dict_profilers.pickle` & `argopy-0.1.9/argopy/assets/dict_profilers.pickle`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/data_fetchers/argovis_data.py` & `argopy-0.1.9/argopy/data_fetchers/argovis_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import numpy as np
 import pandas as pd
 import getpass
 from .proto import ArgoDataFetcherProto
 from abc import abstractmethod
 import warnings
+import urllib
 
 from argopy.stores import httpstore
 from argopy.options import OPTIONS
 from argopy.utilities import list_standard_variables, format_oneline, Chunker
 from argopy.plotters import open_dashboard
 
 access_points = ['wmo', 'box']
@@ -131,23 +132,132 @@
     def _add_history(self, this, txt):
         if "history" in this.attrs:
             this.attrs["history"] += "; %s" % txt
         else:
             this.attrs["history"] = txt
         return this
 
+    def _add_attributes(self, this):  # noqa: C901
+        """ Add variables attributes not return by erddap requests (csv)
+
+            This is hard coded, but should be retrieved from an API somewhere
+        """
+        for v in this.data_vars:
+            if "TEMP" in v and "_QC" not in v:
+                this[v].attrs = {
+                    "long_name": "SEA TEMPERATURE IN SITU ITS-90 SCALE",
+                    "standard_name": "sea_water_temperature",
+                    "units": "degree_Celsius",
+                    "valid_min": -2.0,
+                    "valid_max": 40.0,
+                    "resolution": 0.001,
+                }
+                if "ERROR" in v:
+                    this[v].attrs["long_name"] = (
+                        "ERROR IN %s" % this[v].attrs["long_name"]
+                    )
+
+        for v in this.data_vars:
+            if "PSAL" in v and "_QC" not in v:
+                this[v].attrs = {
+                    "long_name": "PRACTICAL SALINITY",
+                    "standard_name": "sea_water_salinity",
+                    "units": "psu",
+                    "valid_min": 0.0,
+                    "valid_max": 43.0,
+                    "resolution": 0.001,
+                }
+                if "ERROR" in v:
+                    this[v].attrs["long_name"] = (
+                        "ERROR IN %s" % this[v].attrs["long_name"]
+                    )
+
+        for v in this.data_vars:
+            if "PRES" in v and "_QC" not in v:
+                this[v].attrs = {
+                    "long_name": "Sea Pressure",
+                    "standard_name": "sea_water_pressure",
+                    "units": "decibar",
+                    "valid_min": 0.0,
+                    "valid_max": 12000.0,
+                    "resolution": 0.1,
+                    "axis": "Z",
+                }
+                if "ERROR" in v:
+                    this[v].attrs["long_name"] = (
+                        "ERROR IN %s" % this[v].attrs["long_name"]
+                    )
+
+        for v in this.data_vars:
+            if "DOXY" in v and "_QC" not in v:
+                this[v].attrs = {
+                    "long_name": "Dissolved oxygen",
+                    "standard_name": "moles_of_oxygen_per_unit_mass_in_sea_water",
+                    "units": "micromole/kg",
+                    "valid_min": -5.0,
+                    "valid_max": 600.0,
+                    "resolution": 0.001,
+                }
+                if "ERROR" in v:
+                    this[v].attrs["long_name"] = (
+                        "ERROR IN %s" % this[v].attrs["long_name"]
+                    )
+
+        for v in this.data_vars:
+            if "_QC" in v:
+                attrs = {
+                    "long_name": "Global quality flag of %s profile" % v,
+                    "convention": "Argo reference table 2a",
+                }
+                this[v].attrs = attrs
+
+        if "CYCLE_NUMBER" in this.data_vars:
+            this["CYCLE_NUMBER"].attrs = {
+                "long_name": "Float cycle number",
+                "convention": "0..N, 0 : launch cycle (if exists), 1 : first complete cycle",
+            }
+
+        if "DATA_MODE" in this.data_vars:
+            this["DATA_MODE"].attrs = {
+                "long_name": "Delayed mode or real time data",
+                "convention": "R : real time; D : delayed mode; A : real time with adjustment",
+            }
+
+        if "DIRECTION" in this.data_vars:
+            this["DIRECTION"].attrs = {
+                "long_name": "Direction of the station profiles",
+                "convention": "A: ascending profiles, D: descending profiles",
+            }
+
+        if "PLATFORM_NUMBER" in this.data_vars:
+            this["PLATFORM_NUMBER"].attrs = {
+                "long_name": "Float unique identifier",
+                "convention": "WMO float identifier : A9IIIII",
+            }
+
+        return this
+
     @property
     def cachepath(self):
         """ Return path to cache file for this request """
         return [self.fs.cachepath(url) for url in self.uri]
 
     def cname(self):
         """ Return a unique string defining the constraints """
         return self._cname()
 
+    def url_encode(self, urls):
+        """ Return safely encoded list of urls
+
+            This was made to debug for fsspec caching system not working with cache of profile and region in argovis
+            Not working yet, see: https://github.com/euroargodev/argopy/issues/101
+        """
+        return urls
+        # return [urllib.parse.quote(url, safe='/:?=[]&') for url in urls]
+
     def json2dataframe(self, profiles):
         """ convert json data to Pandas DataFrame """
         # Make sure we deal with a list
         if isinstance(profiles, list):
             data = profiles
         else:
             data = [profiles]
@@ -202,15 +312,17 @@
         ds["N_POINTS"] = ds["N_POINTS"]
         # Convert all coordinate variable names to upper case
         for v in ds.data_vars:
             ds = ds.rename({v: v.upper()})
         ds = ds.set_coords(coords)
 
         # Cast data types and add variable attributes (not available in the csv download):
+        ds['TIME'] = ds['TIME'].astype(np.datetime64)
         ds = ds.argo.cast_types()
+        ds = self._add_attributes(ds)
 
         # Remove argovis file attributes and replace them with argopy ones:
         ds.attrs = {}
         if self.dataset_id == "phy":
             ds.attrs["DATA_ID"] = "ARGO"
         elif self.dataset_id == "ref":
             ds.attrs["DATA_ID"] = "ARGO_Reference"
@@ -314,15 +426,16 @@
             for wmo in wmos:
                 if cycs is None:
                     this.append(self.get_url(wmo))
                 else:
                     this.append(self.get_url(wmo, cycs))
             return this
 
-        return list_bunch(self.WMO, self.CYC)
+        urls = list_bunch(self.WMO, self.CYC)
+        return self.url_encode(urls)
 
     def dashboard(self, **kw):
         if len(self.WMO) == 1:
             return open_dashboard(wmo=self.WMO[0], **kw)
         else:
             warnings.warn("Plot dashboard only available for request with a single float")
 
@@ -385,44 +498,43 @@
         url += "&endDate={}".format(strDate(self.BOX, 7))
         url += "&presRange=[{},{}]".format(self.BOX[4], self.BOX[5])
         url += "&llCorner={}".format(strCorner(self.BOX, [0, 2]))
         url += "&urCorner={}".format(strCorner(self.BOX, [1, 3]))
         return url
 
     def get_url(self):
-        # return self.get_url_shape()
-        return self.get_url_rect()
+        return self.get_url_shape()
+        # return self.get_url_rect()
 
     @property
     def uri(self):
         """ List of URLs to load for a request
 
         Returns
         -------
         list(str)
         """
         Lt = np.timedelta64(pd.to_datetime(self.BOX[7]) - pd.to_datetime(self.BOX[6]), "D")
         MaxLenTime = 90
         MaxLen = np.timedelta64(MaxLenTime, "D")
 
+        urls = []
         if not self.parallel:
             # Check if the time range is not larger than allowed (90 days):
             if Lt > MaxLen:
                 self.Chunker = Chunker(
                     {"box": self.BOX},
                     chunks={"lon": 1, "lat": 1, "dpt": 1, "time": "auto"},
                     chunksize={"time": MaxLenTime},
                 )
                 boxes = self.Chunker.fit_transform()
-                urls = []
                 for box in boxes:
                     urls.append(Fetch_box(box=box, ds=self.dataset_id).get_url())
-                return urls
             else:
-                return [self.get_url()]
+                urls.append(self.get_url())
         else:
             if 'time' not in self.chunks_maxsize:
                 self.chunks_maxsize['time'] = MaxLenTime
             elif self.chunks_maxsize['time'] > MaxLenTime:
                 warnings.warn(("argovis only allows requests of %i days interval, "
                                "modify chunks_maxsize['time'] to %i" % (MaxLenTime, MaxLenTime)))
                 self.chunks_maxsize['time'] = MaxLenTime
@@ -431,16 +543,16 @@
             if Lt > MaxLen and 'time' in self.chunks and self.chunks['time'] not in ['auto']:
                 self.chunks['time'] = 'auto'
 
             self.Chunker = Chunker(
                 {"box": self.BOX}, chunks=self.chunks, chunksize=self.chunks_maxsize
             )
             boxes = self.Chunker.fit_transform()
-            urls = []
             for box in boxes:
                 urls.append(Fetch_box(box=box, ds=self.dataset_id).get_url())
-            return urls
+
+        return self.url_encode(urls)
 
     @property
     def url(self):
-        # return self.get_url_shape()
-        return self.get_url_rect()
+        return self.get_url_shape()
+        # return self.get_url_rect()
```

### Comparing `argopy-0.1.8/argopy/data_fetchers/erddap_data.py` & `argopy-0.1.9/argopy/data_fetchers/erddap_data.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/data_fetchers/erddap_index.py` & `argopy-0.1.9/argopy/data_fetchers/erddap_index.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/data_fetchers/localftp_data.py` & `argopy-0.1.9/argopy/data_fetchers/localftp_data.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/data_fetchers/localftp_index.py` & `argopy-0.1.9/argopy/data_fetchers/localftp_index.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/data_fetchers/proto.py` & `argopy-0.1.9/argopy/data_fetchers/proto.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/errors.py` & `argopy-0.1.9/argopy/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 """
 A bunch of custom errors used in argopy.
 """
 
 
 class DataNotFound(ValueError):
     """ Raise when a data selection returns nothing """
-    pass
+    def __init__(self, path: str = "?"):
+        self.value = "No data found at %s" % path
+        self.path = path
+
+    def __str__(self):
+        return (repr(self.value))
 
 
 class FtpPathError(ValueError):
     """ Raise when the ftp path is not appropriate """
     pass
```

### Comparing `argopy-0.1.8/argopy/fetchers.py` & `argopy-0.1.9/argopy/fetchers.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 Validity of access points parameters (eg: wmo) is made here, not at the data/index source fetcher level
 
 """
 
 import warnings
 import xarray as xr
 import pandas as pd
+import numpy as np
 import logging
 
 from argopy.options import OPTIONS, _VALIDATORS
 from .errors import InvalidFetcherAccessPoint, InvalidFetcher
 from .utilities import list_available_data_src, list_available_index_src, is_box, is_indexbox, check_wmo
-from .plotters import plot_trajectory, bar_plot
+from .plotters import plot_trajectory, bar_plot, open_sat_altim_report
 
 
 AVAILABLE_DATA_SOURCES = list_available_data_src()
 AVAILABLE_INDEX_SOURCES = list_available_index_src()
 
 log = logging.getLogger("argopy.fetchers.facade")
 
@@ -35,34 +36,46 @@
     def wrapper(*args):
         if AccessPoint.__name__ not in args[0].valid_access_points:
             raise InvalidFetcherAccessPoint(
                             "'%s' not available with '%s' src. Available access point(s): %s" %
                             (AccessPoint.__name__, args[0]._src, ", ".join(args[0].Fetchers.keys()))
                         )
         return AccessPoint(*args)
+    wrapper.__name__ = AccessPoint.__name__
+    wrapper.__doc__ = AccessPoint.__doc__
     return wrapper
 
 
 class ArgoDataFetcher:
-    """ Fetcher and post-processor of Argo data (API facade) """
+    """ Fetcher and post-processor of Argo data (API facade)
+
+    Parameters
+    ----------
+    mode: str, optional
+        User mode. Eg: ``standard`` or ``expert``. Set to OPTIONS['mode'] by default if empty.
+    src: str, optional
+         Source of the data to use. Eg: ``erddap``. Set to OPTIONS['src'] by default if empty.
+    ds: str, optional
+        Name of the dataset to load. Eg: ``phy``. Set to OPTIONS['dataset'] by default if empty.
+    **fetcher_kwargs: optional
+        Additional arguments passed on data source fetcher creation of each access points.
+
+    Examples
+    --------
+    >>> from argopy import DataFetcher
+    >>> adf = DataFetcher.region([-75, -65, 10, 20]).load()
+    >>> idx.plot()
+    >>> idx.data
+
+    """
 
     def __init__(self, mode: str = "", src: str = "", ds: str = "", **fetcher_kwargs):
 
         """ Create a fetcher instance
 
-        Parameters
-        ----------
-        mode: str, optional
-            User mode. Eg: ``standard`` or ``expert``. Set to OPTIONS['mode'] by default if empty.
-        src: str, optional
-             Source of the data to use. Eg: ``erddap``. Set to OPTIONS['src'] by default if empty.
-        ds: str, optional
-            Name of the dataset to load. Eg: ``phy``. Set to OPTIONS['dataset'] by default if empty.
-        **fetcher_kwargs: optional
-            Additional arguments passed on data source instance creation of each access points.
 
         Returns
         -------
         :class:`argopy.fetchers.ArgoDataFetcher`
         """
 
         # Facade options:
@@ -152,14 +165,15 @@
         valid_attrs = [
             "Fetchers",
             "fetcher",
             "fetcher_options",
             "postproccessor",
             "data",
             "index",
+            "domain",
             "_loaded",
             "_request"
         ]
         if key not in self.valid_access_points and key not in valid_attrs:
             raise InvalidFetcherAccessPoint("'%s' is not a valid access point" % key)
         pass
 
@@ -168,14 +182,15 @@
         """ List of resources to load for a request
 
         This can be a list of paths or urls, depending on the data source selected.
 
         Returns
         -------
         list(str)
+            List of resources used to fetch data
         """
         if self.fetcher:
             return self.fetcher.uri
         else:
             raise InvalidFetcherAccessPoint(
                 " Initialize an access point (%s) first."
                 % ",".join(self.Fetchers.keys())
@@ -184,33 +199,54 @@
     @property
     def data(self):
         """ Data structure
 
             Returns
             --------
             :class:`xarray.DataArray`
+                Fetched data
         """
         if not isinstance(self._data, xr.Dataset):
             self.load()
         return self._data
 
     @property
     def index(self):
         """ Index structure, as returned by the to_index method
 
             Returns
             --------
-            :class:`pandas.Dataframe`
-
+            :class:`pandas.DataFrame`
+                Argo-like index of fetched data
         """
         if not isinstance(self._index, pd.core.frame.DataFrame):
             self.load()
         return self._index
 
+    @property
+    def domain(self):
+        """" Domain of the dataset
+
+            This is different from a usual ``box`` because dates are already in numpy.datetime64 format.
+        """
+        this_ds = self.data
+        if 'PRES_ADJUSTED' in this_ds.data_vars:
+            Pmin = np.nanmin((np.min(this_ds['PRES'].values), np.min(this_ds['PRES_ADJUSTED'].values)))
+            Pmax = np.nanmax((np.max(this_ds['PRES'].values), np.max(this_ds['PRES_ADJUSTED'].values)))
+        else:
+            Pmin = np.min(this_ds['PRES'].values)
+            Pmax = np.max(this_ds['PRES'].values)
+
+        return [np.min(this_ds['LONGITUDE'].values), np.max(this_ds['LONGITUDE'].values),
+                np.min(this_ds['LATITUDE'].values), np.max(this_ds['LATITUDE'].values),
+                Pmin, Pmax,
+                np.min(this_ds['TIME'].values), np.max(this_ds['TIME'].values)]
+
     def dashboard(self, **kw):
+        """ Open access point dashboard """
         try:
             return self.fetcher.dashboard(**kw)
         except Exception:
             warnings.warn(
                 "dashboard not available for this fetcher access point (%s/%s)"
                 % (self._src, self._AccessPoint)
             )
@@ -284,31 +320,31 @@
 
         return self
 
     @checkAccessPoint
     def region(self, box: list):
         """ Space/time domain data fetcher
 
-        Parameters
-        ----------
-        box: list()
-            Define the domain to load Argo data for. The box list is made of:
-                - lon_min: float, lon_max: float,
-                - lat_min: float, lat_max: float,
-                - dpt_min: float, dpt_max: float,
-                - date_min: str (optional), date_max: str (optional)
-
-            Longitude, latitude and pressure bounds are required, while the two bounding dates are optional.
-            If bounding dates are not specified, the entire time series is fetched.
-            Eg: [-60, -55, 40., 45., 0., 10., '2007-08-01', '2007-09-01']
+            Parameters
+            ----------
+            box: list()
+                Define the domain to load Argo data for. The box list is made of:
+                    - lon_min: float, lon_max: float,
+                    - lat_min: float, lat_max: float,
+                    - dpt_min: float, dpt_max: float,
+                    - date_min: str (optional), date_max: str (optional)
 
-        Returns
-        -------
-        :class:`argopy.fetchers.ArgoDataFetcher`
-            A data source fetcher for a space/time domain
+                Longitude, latitude and pressure bounds are required, while the two bounding dates are optional.
+                If bounding dates are not specified, the entire time series is fetched.
+                Eg: [-60, -55, 40., 45., 0., 10., '2007-08-01', '2007-09-01']
+
+            Returns
+            -------
+            :class:`argopy.fetchers.ArgoDataFetcher`
+                A data source fetcher for a space/time domain
         """
         is_box(box, errors="raise")  # Validate the box definition
         self.fetcher = self.Fetchers["region"](box=box, **self.fetcher_options)
         self._AccessPoint = "region"  # Register the requested access point
         self._AccessPoint_data = {'box': box}  # Register the requested access point data
 
         if self._mode == "standard" and self._dataset_id != "ref":
@@ -320,53 +356,62 @@
             self.postproccessor = postprocessing
 
         return self
 
     def to_xarray(self, **kwargs):
         """ Fetch and return data as xarray.DataSet
 
+            Trigger a fetch of data by the specified source and access point.
+
             Returns
             -------
             :class:`xarray.DataSet`
+                Fetched data
         """
         if not self.fetcher:
             raise InvalidFetcher(
                 " Initialize an access point (%s) first."
                 % ",".join(self.Fetchers.keys())
             )
         xds = self.fetcher.to_xarray(**kwargs)
         xds = self.postproccessor(xds)
         return xds
 
     def to_dataframe(self, **kwargs):
-        """  Fetch and return data as pandas.Dataframe
+        """ Fetch and return data as pandas.Dataframe
+
+            Trigger a fetch of data by the specified source and access point.
 
             Returns
             -------
-            :class:`pandas.Dataframe`
+            :class:`pandas.DataFrame`
+                Fetched data
         """
         if not self.fetcher:
             raise InvalidFetcher(
                 " Initialize an access point (%s) first."
                 % ",".join(self.Fetchers.keys())
             )
         return self.load().data.to_dataframe(**kwargs)
 
     def to_index(self, full: bool = False):
-        """ Create an index of Argo data
+        """ Create an index of Argo data, fetch data if necessary
+
+            Build an Argo-like index of profiles from fetched data.
 
             Parameters
             ----------
             full: bool
                 Should extract a full index, as returned by an IndexFetcher or only a space/time
                 index of fetched profiles (this is the default choice, i.e. full=False).
 
             Returns
             -------
-            :class:`pandas.Dataframe`
+            :class:`pandas.DataFrame`
+                Argo-like index of fetched data
         """
         if not full:
             self.load()
             ds = self.data.argo.point2profile()
             df = (
                 ds.drop_vars(set(ds.data_vars) - set(["PLATFORM_NUMBER"]))
                 .drop_dims("N_LEVELS")
@@ -410,27 +455,27 @@
             # Possibly replace the light index with the full version:
             if not self._loaded or self._request == self.__repr__():
                 self._index = df
 
         return df
 
     def load(self, force: bool = False, **kwargs):
-        """ Load data in memory
+        """ Fetch data (and compute an index) if not already in memory
 
             Apply the default to_xarray() and to_index() methods and store results in memory.
             Access loaded measurements structure with the `data` and `index` properties::
 
                 ds = ArgoDataFetcher().profile(6902746, 34).load().data
                 # or
                 df = ArgoDataFetcher().float(6902746).load().index
 
             Parameters
             ----------
             force: bool
-                Force loading, default is False.
+                Force fetching data if not already in memory, default is False.
 
             Returns
             -------
             :class:`argopy.fetchers.ArgoDataFetcher.float`
                 Data fetcher with `data` and `index` properties in memory
         """
         # Force to load data if the fetcher definition has changed
@@ -457,16 +502,15 @@
         return self.fetcher.clear_cache()
 
     def plot(self, ptype="trajectory", **kwargs):
         """ Create custom plots from data
 
             Parameters
             ----------
-            ptype: str
-                Type of plot to generate. This can be: 'trajectory',' profiler', 'dac'.
+            ptype: {'trajectory',' profiler', 'dac', 'qc_altimetry}, default: 'trajectory'
 
             Returns
             -------
             fig: :class:`matplotlib.figure.Figure`
             ax: :class:`matplotlib.axes.Axes`
         """
         self.load()
@@ -476,45 +520,50 @@
             return bar_plot(self.index, by="institution", **kwargs)
         elif ptype == "profiler":
             if "profiler" not in self.index:
                 self.to_index(full=True)
             return bar_plot(self.index, by="profiler", **kwargs)
         elif ptype == "trajectory":
             return plot_trajectory(self.index, **kwargs)
+        elif ptype == "qc_altimetry":
+            WMOs = np.unique(self.data['PLATFORM_NUMBER'])
+            return open_sat_altim_report(WMOs, **kwargs)
         else:
             raise ValueError(
-                "Type of plot unavailable. Use: 'dac', 'profiler' or 'trajectory' (default)"
+                "Type of plot unavailable. Use: 'trajectory', 'dac', 'profiler', 'qc_altimetry'"
             )
 
 
 class ArgoIndexFetcher:
-    """
-    Specs discussion :
-    https://github.com/euroargodev/argopy/issues/8
-    https://github.com/euroargodev/argopy/pull/6)
-
-    Usage:
-
-    from argopy import ArgoIndexFetcher
-    idx = ArgoIndexFetcher.region([-75, -65, 10, 20])
-    idx.plot.trajectories()
-    idx.load().to_dataframe()
-
-    Fetch and process Argo index.
-
-    Can return metadata from index of :
-        - one or more float(s), defined by WMOs
-        - one or more profile(s), defined for one WMO and one or more CYCLE NUMBER
-        - a space/time rectangular domain, defined by lat/lon/pres/time range
-
-    idx object can also be used as an input :
-     argo_loader = ArgoDataFetcher(index=idx)
-
-    Specify here all options to data_fetchers
+    """ Fetcher and post-processor of Argo index data (API facade)
 
+    Parameters
+    ----------
+    mode: str, optional
+        User mode. Eg: ``standard`` or ``expert``. Set to OPTIONS['mode'] by default if empty.
+    src: str, optional
+         Source of the data to use. Eg: ``erddap``. Set to OPTIONS['src'] by default if empty.
+    ds: str, optional
+        Name of the dataset to load. Eg: ``phy``. Set to OPTIONS['dataset'] by default if empty.
+    **fetcher_kwargs: optional
+        Additional arguments passed on data source fetcher of each access points.
+
+    Notes
+    -----
+    Spec discussions can be found here:
+        https://github.com/euroargodev/argopy/issues/8
+
+        https://github.com/euroargodev/argopy/pull/6
+
+    Examples
+    --------
+    >>> from argopy import IndexFetcher
+    >>> adf = IndexFetcher.region([-75, -65, 10, 20]).load()
+    >>> idx.plot()
+    >>> idx.index
     """
 
     def __init__(self, mode: str = "", src: str = "", ds: str = "", **fetcher_kwargs):
 
         # Facade options:
         self._mode = OPTIONS["mode"] if mode == "" else mode
         self._dataset_id = OPTIONS["dataset"] if ds == "" else ds
@@ -594,15 +643,16 @@
 
     @property
     def index(self):
         """ Index structure
 
             Returns
             --------
-            :class:`pandas.Dataframe`
+            :class:`pandas.DataFrame`
+                Argo-like index of fetched data
         """
         if not isinstance(self._index, pd.core.frame.DataFrame):
             self.load()
         return self._index
 
     @checkAccessPoint
     def float(self, wmo):
@@ -611,16 +661,16 @@
         Parameters
         ----------
         wmo: list(int)
             Define the list of Argo floats to load data for. This is a list of integers with WMO numbers.
 
         Returns
         -------
-        :class:`argopy.fetchers.ArgoIndexFetcher.float`
-            An index source fetcher for all float profiles index
+        :class:`argopy.fetchers.ArgoIndexFetcher`
+            An index fetcher initialised for specific floats
         """
         wmo = check_wmo(wmo)  # Check and return a valid list of WMOs
         self.fetcher = self.Fetchers["float"](WMO=wmo, **self.fetcher_options)
         self._AccessPoint = "float"  # Register the requested access point
         return self
 
     @checkAccessPoint
@@ -634,57 +684,57 @@
                 WMO is the World Meteorological Organization.
             cyc: list(int)
                 Define the list of cycle numbers to load for each Argo floats listed in ``wmo``.
 
             Returns
             -------
             :class:`argopy.fetchers.ArgoIndexFetcher`
-                A index fetcher initialised for specific float profiles
+                An index fetcher initialised for specific float profiles
         """
         wmo = check_wmo(wmo)  # Check and return a valid list of WMOs
         self.fetcher = self.Fetchers["profile"](WMO=wmo, CYC=cyc, **self.fetcher_options)
         self._AccessPoint = "profile"  # Register the requested access point
         return self
 
     @checkAccessPoint
     def region(self, box):
         """ Space/time domain index fetcher
 
-        Parameters
-        ----------
-        box: list()
-            Define the domain to load Argo index for. The box list is made of:
-                - lon_min: float, lon_max: float,
-                - lat_min: float, lat_max: float,
-                - date_min: str (optional), date_max: str (optional)
-
-            Longitude and latitude bounds are required, while the two bounding dates are optional.
-            If bounding dates are not specified, the entire time series is fetched.
-            Eg: [-60, -55, 40., 45., '2007-08-01', '2007-09-01']
+            Parameters
+            ----------
+            box: list()
+                Define the domain to load Argo index for. The box list is made of:
+                    - lon_min: float, lon_max: float,
+                    - lat_min: float, lat_max: float,
+                    - date_min: str (optional), date_max: str (optional)
+
+                Longitude and latitude bounds are required, while the two bounding dates are optional.
+                If bounding dates are not specified, the entire time series is fetched.
+                Eg: [-60, -55, 40., 45., '2007-08-01', '2007-09-01']
 
-        Returns
-        -------
-        :class:`argopy.fetchers.ArgoIndexFetcher`
-            A index fetcher initialised for a space/time domain
+            Returns
+            -------
+            :class:`argopy.fetchers.ArgoIndexFetcher`
+                An index fetcher initialised for a space/time domain
 
-        Warning
-        -------
-        Note that the box option for an index fetcher does not have pressure bounds, contrary to the data fetcher.
+            Warnings
+            --------
+            Note that the box option for an index fetcher does not have pressure bounds, contrary to the data fetcher.
         """
         is_indexbox(box, errors="raise")  # Validate the box definition
         self.fetcher = self.Fetchers["region"](box=box, **self.fetcher_options)
         self._AccessPoint = "region"  # Register the requested access point
         return self
 
     def to_dataframe(self, **kwargs):
         """ Fetch and return index data as pandas Dataframe
 
             Returns
             -------
-            :class:`pandas.Dataframe`
+            :class:`pandas.DataFrame`
         """
         if not self.fetcher:
             raise InvalidFetcher(
                 " Initialize an access point (%s) first."
                 % ",".join(self.Fetchers.keys())
             )
         return self.fetcher.to_dataframe(**kwargs)
@@ -704,15 +754,22 @@
                 % ",".join(self.Fetchers.keys())
             )
         return self.load().index.to_xarray(**kwargs)
 
     def to_csv(self, file: str = "output_file.csv"):
         """ Fetch and save index data as csv in a file
 
-            This is a shortcut to .load().index.to_csv()
+            Notes
+            -----
+            >>> idx.to_csv()
+            is a shortcut to:
+            >>> idx.load().index.to_csv()
+
+            Since the ``index`` property is a :class:`pandas.DataFrame`, this is currently a short
+            cut to :meth:`pandas.DataFrame.to_index`
 
             Returns
             -------
             None
         """
         if self._AccessPoint not in self.valid_access_points:
             raise InvalidFetcherAccessPoint(
@@ -750,30 +807,32 @@
         return self
 
     def plot(self, ptype="trajectory", **kwargs):
         """ Create custom plots from index
 
             Parameters
             ----------
-            ptype: str
-                Type of plot to generate. This can be: 'trajectory',' profiler', 'dac'.
+            ptype: {'trajectory',' profiler', 'dac', 'qc_altimetry}, default: 'trajectory'
 
             Returns
             -------
             fig: :class:`matplotlib.figure.Figure`
             ax: :class:`matplotlib.axes.Axes`
         """
         self.load()
         if ptype in ["dac", "institution"]:
             return bar_plot(self.index, by="institution", **kwargs)
         elif ptype == "profiler":
             return bar_plot(self.index, by="profiler", **kwargs)
         elif ptype == "trajectory":
             return plot_trajectory(self.index.sort_values(["file"]), **kwargs)
+        elif ptype == "qc_altimetry":
+            WMOs = np.unique(self.index['wmo'])
+            return open_sat_altim_report(WMOs, **kwargs)
         else:
             raise ValueError(
-                "Type of plot unavailable. Use: 'dac', 'profiler' or 'trajectory' (default)"
+                "Type of plot unavailable. Use: 'trajectory', 'dac', 'profiler', 'qc_altimetry'"
             )
 
     def clear_cache(self):
         """ Clear fetcher cached data """
         return self.fetcher.clear_cache()
```

### Comparing `argopy-0.1.8/argopy/options.py` & `argopy-0.1.9/argopy/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 # Like always, largely inspired by xarray code:
 # https://github.com/pydata/xarray/blob/cafab46aac8f7a073a32ec5aa47e213a9810ed54/xarray/core/options.py
 """
 import os
 import numpy as np
 from argopy.errors import OptionValueError, FtpPathError
 import warnings
+import logging
+
+
+# Define a logger
+log = logging.getLogger("argopy.options")
 
 # Define option names as seen by users:
 DATA_SOURCE = "src"
 LOCAL_FTP = "local_ftp"
 DATASET = "dataset"
 DATA_CACHE = "cachedir"
 USER_LEVEL = "mode"
 API_TIMEOUT = "api_timeout"
-TRUST_ENV = "trust_env"  # Get proxies information from HTTP_PROXY / HTTPS_PROXY environment variables if the parameter is True (False by default).
-# Get proxy credentials from ~/.netrc file if present.
+TRUST_ENV = "trust_env"
 
 # Define the list of available options and default values:
 OPTIONS = {
     DATA_SOURCE: "erddap",
-    LOCAL_FTP: None,
+    LOCAL_FTP: "-",  # No default value
     DATASET: "phy",
     DATA_CACHE: os.path.expanduser(os.path.sep.join(["~", ".cache", "argopy"])),
     USER_LEVEL: "standard",
     API_TIMEOUT: 60,
     TRUST_ENV: False
 }
 
@@ -36,84 +40,92 @@
 _USER_LEVEL_LIST = frozenset(["standard", "expert"])
 
 
 # Define how to validate options:
 def _positive_integer(value):
     return isinstance(value, int) and value > 0
 
+
 def validate_ftp(this_path):
-    if this_path is not None:
+    if this_path != "-":
         return check_localftp(this_path, errors='raise')
     else:
+        log.debug("OPTIONS['%s'] is not defined" % LOCAL_FTP)
         return False
 
+
 _VALIDATORS = {
     DATA_SOURCE: _DATA_SOURCE_LIST.__contains__,
     LOCAL_FTP: validate_ftp,
     DATASET: _DATASET_LIST.__contains__,
     DATA_CACHE: os.path.exists,
     USER_LEVEL: _USER_LEVEL_LIST.__contains__,
     API_TIMEOUT: lambda x: isinstance(x, int) and x > 0,
     TRUST_ENV: lambda x: isinstance(x, bool)
 }
 
 
 class set_options:
-    """Set options for argopy.
+    """Set options for argopy
 
     List of options:
 
-        - `dataset`: Define the Dataset to work with.
-            Default: `phy`. Possible values: `phy`, `bgc` or `ref`.
-        - `src`: Source of fetched data.
-            Default: `erddap`. Possible values: `erddap`, `localftp`, `argovis`
-        - `local_ftp`: Absolute path to a local GDAC ftp copy.
-            Default: `.`
-        - `cachedir`: Absolute path to a local cache directory.
-            Default: `~/.cache/argopy`
-        - `mode`: User mode.
-            Default: `standard`. Possible values: `standard` or `expert`.
-        - `api_timeout`: Define the time out of internet requests to web API, in seconds.
-            Default: 60
+    - ``dataset``: Define the Dataset to work with.
+        Default: ``phy``.
+        Possible values: ``phy``, ``bgc`` or ``ref``.
+    - ``src``: Source of fetched data.
+        Default: ``erddap``.
+        Possible values: ``erddap``, ``localftp``, ``argovis``
+    - ``local_ftp``: Absolute path to a local GDAC ftp copy.
+        Default: None
+    - ``cachedir``: Absolute path to a local cache directory.
+        Default: ``~/.cache/argopy``
+    - ``mode``: User mode.
+        Default: ``standard``.
+        Possible values: ``standard`` or ``expert``.
+    - ``api_timeout``: Define the time out of internet requests to web API, in seconds.
+        Default: 60
+    - ``trust_env``: Allow for local environment variables to be used by fsspec to connect to the internet.
+        Get proxies information from HTTP_PROXY / HTTPS_PROXY environment variables if this option is True (
+        False by default). Also can get proxy credentials from ~/.netrc file if present.
 
     You can use `set_options` either as a context manager:
+
     >>> import argopy
     >>> with argopy.set_options(src='localftp'):
     >>>    ds = argopy.DataFetcher().float(3901530).to_xarray()
 
     Or to set global options:
+
     >>> argopy.set_options(src='localftp')
 
     """
     def __init__(self, **kwargs):
         self.old = {}
         for k, v in kwargs.items():
             if k not in OPTIONS:
                 raise ValueError(
                     "argument name %r is not in the set of valid options %r"
                     % (k, set(OPTIONS))
                 )
-
             if k in _VALIDATORS and not _VALIDATORS[k](v):
                 raise OptionValueError(f"option {k!r} given an invalid value: {v!r}")
             self.old[k] = OPTIONS[k]
         self._apply_update(kwargs)
 
     def _apply_update(self, options_dict):
-        # for k, v in options_dict.items():
-        #     if k in _SETTERS:
-        #         _SETTERS[k](v)
         OPTIONS.update(options_dict)
 
     def __enter__(self):
         return
 
     def __exit__(self, type, value, traceback):
         self._apply_update(self.old)
 
+
 def check_localftp(path, errors: str = "ignore"):
     """ Check if the path has the expected GDAC ftp structure
 
         Check if the path is structured like:
         .
         └── dac
             ├── aoml
```

### Comparing `argopy-0.1.8/argopy/plotters.py` & `argopy-0.1.9/argopy/plotters.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 
 import numpy as np
 import pandas as pd
 import warnings
 from contextlib import contextmanager
 from argopy.errors import InvalidDashboard
-from argopy.utilities import warnUnless
+from argopy.utilities import warnUnless, check_wmo
 
 
 try:
     with_matplotlib = True
     import matplotlib as mpl
     import matplotlib.pyplot as plt
     import matplotlib.ticker as mticker
@@ -67,54 +67,102 @@
         with sns.axes_style(style):
             yield
     else:  # Otherwise do nothing
         yield
 
 
 def open_dashboard(wmo=None, cyc=None, width="100%", height=1000, url=None, type="ea"):
-    """ Insert in a notebook cell the Euro-Argo dashboard page
+    """ Insert the Euro-Argo dashboard page in a notebook cell
 
         Parameters
         ----------
         wmo: int
             The float WMO to display. By default, this is set to None and will insert the general dashboard.
 
         Returns
         -------
-        IFrame: IPython.lib.display.IFrame
+        :class:`IPython.lib.display.IFrame`
     """
     if type not in ["ea", "eric", "coriolis"]:
         raise InvalidDashboard("Invalid dashboard type")
 
     from IPython.display import IFrame
 
     if url is None:
         if type == "ea" or type == "eric":  # Open Euro-Argo dashboard
             if wmo is None:
                 url = "https://fleetmonitoring.euro-argo.eu"
             else:
-                url = "https://fleetmonitoring.euro-argo.eu/float/{}".format(str(wmo))
+                wmo = check_wmo(wmo)
+                url = "https://fleetmonitoring.euro-argo.eu/float/{}".format(str(wmo[0]))
         elif type == 'coriolis':  # Open Coriolis dashboard
             if wmo is not None:
+                wmo = check_wmo(wmo)
                 url = ("https://co-insitucharts.ifremer.fr/platform/{}/charts").format(
-                    str(wmo)
+                    str(wmo[0])
                 )
 
         # return open_dashboard(url=("https://co-insitucharts.ifremer.fr/platform/{}/charts").format(str(self.WMO[0])), **kw)
 
         # # Note that argovis doesn't allow X-Frame insertion !
         # elif type == 'argovis':
         #     if cyc is None:
         #         url = "https://argovis.colorado.edu/catalog/platforms/{}/page".format(str(wmo))
         #     else:
         #         url = "https://argovis.colorado.edu/catalog/profiles/{}_{}/page".format(str(wmo),str(cyc))
 
     return IFrame(url, width=width, height=height)
 
 
+def open_sat_altim_report(WMO=None, embed='dropdown'):
+    """ Insert the CLS Satellite Altimeter Report figure in notebook cell
+
+        This is the method called when using the facade fetcher methods ``plot``:
+
+        >>> DataFetcher().float(6902745).plot('qc_altimetry')
+
+        Parameters
+        ----------
+        WMO: int or list
+            The float WMO to display. By default, this is set to None and will insert the general dashboard.
+        embed: {'list', 'slide', 'dropdown'}, default: 'dropdown'
+            Set the embedding method. If set to None, simply return the list of urls to figures.
+    """
+    if embed in ['list', 'slide', 'dropdown']:
+        from IPython.display import Image
+    if embed in ['list']:
+        from IPython.display import display
+    if embed in ['slide', 'dropdown']:
+        import ipywidgets as wg
+
+    WMOs = check_wmo(WMO)
+    urls = []
+    urls_dict = {}
+    for this_wmo in WMOs:
+        url = "https://data-argo.ifremer.fr/etc/argo-ast9-item13-AltimeterComparison/figures/%i.png" % this_wmo
+        if embed == 'list':
+            urls.append(Image(url, embed=True))
+        else:
+            urls.append(url)
+            urls_dict[this_wmo] = url
+
+    if embed == 'list':
+        return display(*urls)
+    elif embed == 'slide':
+        def f(Float):
+            return Image(url=urls[Float])
+        return wg.interact(f, Float=wg.IntSlider(min=0, max=len(urls) - 1, step=1))
+    elif embed == 'dropdown':
+        def f(Float):
+            return Image(url=urls_dict[int(Float)])
+        return wg.interact(f, Float=[str(wmo) for wmo in WMOs])
+    else:
+        return urls_dict
+
+
 class discrete_coloring:
     """ Handy class to manage discrete coloring and the associated colorbar
 
     Example
     -------
     This class can be used like this::
```

### Comparing `argopy-0.1.8/argopy/stores/argo_index.py` & `argopy-0.1.9/argopy/stores/argo_index.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/stores/filesystems.py` & `argopy-0.1.9/argopy/stores/filesystems.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,14 @@
 from argopy.errors import FileSystemHasNoCache, CacheFileNotFound, DataNotFound, \
     InvalidMethod
 from abc import ABC, abstractmethod
 
 
 log = logging.getLogger("argopy.stores")
 
-try:
-    from tqdm import tqdm
-except ModuleNotFoundError:
-    log.debug("tqdm not found, argopy needs tqdm installed to display progress bars")
-    tqdm = lambda fct, lst: fct  # noqa: E731
-
 
 def new_fs(protocol: str = '', cache: bool = False, cachedir: str = OPTIONS['cachedir'], **kwargs):
     """ Create a new fsspec file system
 
     Parameters
     ----------
     protocol: str (optional)
@@ -81,15 +75,16 @@
 class argo_store_proto(ABC):
     """ Argo Abstract File System
 
         Provide a prototype for Argo file systems
 
         Should this class inherits from fsspec.spec.AbstractFileSystem ?
     """
-    protocol = ''  # File system name, one in fsspec.registry.known_implementations
+    protocol = ''
+    """str: File system name, one in fsspec.registry.known_implementations"""
 
     def __init__(self,
                  cache: bool = False,
                  cachedir: str = "",
                  **kwargs):
         """ Create a file storage system for Argo data
 
@@ -479,15 +474,15 @@
                 if progress:
                     futures = tqdm(futures, total=len(urls))
 
                 for future in futures:
                     data = None
                     try:
                         data = future.result()
-                    except Exception as e:
+                    except Exception:
                         failed.append(future_to_url[future])
                         if errors == 'ignore':
                             log.debug("Ignored error with this url: %s" % strUrl(future_to_url[future]))
                             # See fsspec.http logger for more
                             pass
                         elif errors == 'silent':
                             pass
@@ -505,15 +500,15 @@
             if progress:
                 urls = tqdm(urls, total=len(urls))
 
             for url in urls:
                 data = None
                 try:
                     data = self._mfprocessor_dataset(url, preprocess=preprocess, *args, **kwargs)
-                except Exception as e:
+                except Exception:
                     failed.append(url)
                     if errors == 'ignore':
                         log.debug("Ignored error with this url: %s" % strUrl(url))  # See fsspec.http logger for more
                         pass
                     elif errors == 'silent':
                         pass
                     else:
@@ -549,15 +544,15 @@
             **kwargs: Arguments passed to :class:`pandas.read_csv`
 
             Returns
             -------
             :class:`pandas.DataFrame`
 
         """
-        log.debug("Reading csv: %s" % url)
+        log.debug("Opening/reading csv: %s" % url)
         with self.open(url) as of:
             df = pd.read_csv(of, **kwargs)
         return df
 
     def open_json(self, url, **kwargs):
         """ Return a json from an url, or verbose errors
 
@@ -567,20 +562,26 @@
 
             Returns
             -------
             json
 
         """
         log.debug("Opening json: %s" % url)
-        try:
-            with self.open(url) as of:
-                js = json.load(of, **kwargs)
-            return js
-        except json.JSONDecodeError:
-            raise
+        # try:
+        #     with self.open(url) as of:
+        #         js = json.load(of, **kwargs)
+        #     return js
+        # except ClientResponseError:
+        #     raise
+        # except json.JSONDecodeError:
+        #     raise
+        data = self.fs.cat_file(url)
+        js = json.loads(data, **kwargs)
+        self.register(url)
+        return js
 
     def _mfprocessor_json(self, url, preprocess=None, *args, **kwargs):
         # Load data
         data = self.open_json(url, **kwargs)
         # Pre-process
         if isinstance(preprocess, types.FunctionType) or isinstance(preprocess, types.MethodType):
             data = preprocess(data)
@@ -642,15 +643,15 @@
                 if progress:
                     futures = tqdm(futures, total=len(urls))
 
                 for future in futures:
                     data = None
                     try:
                         data = future.result()
-                    except Exception as e:
+                    except Exception:
                         failed.append(future_to_url[future])
                         if errors == 'ignore':
                             log.debug("Ignored error with this url: %s" % strUrl(future_to_url[future]))
                             # See fsspec.http logger for more
                             pass
                         elif errors == 'silent':
                             pass
@@ -668,15 +669,15 @@
             if progress:
                 urls = tqdm(urls, total=len(urls))
 
             for url in urls:
                 data = None
                 try:
                     data = self._mfprocessor_json(url, preprocess=preprocess, *args, **kwargs)
-                except Exception as e:
+                except Exception:
                     failed.append(url)
                     if errors == 'ignore':
                         log.debug("Ignored error with this url: %s" % strUrl(url))
                         # See fsspec.http logger for more
                         pass
                     elif errors == 'silent':
                         pass
```

### Comparing `argopy-0.1.8/argopy/tests/__init__.py` & `argopy-0.1.9/argopy/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*coding: UTF-8 -*-
 """
 
 Test suite for argopy continuous integration
 
 """
+import traceback
 import importlib
 import pytest
 import fsspec
 import argopy
 from aiohttp.client_exceptions import ServerDisconnectedError, ClientResponseError
 from packaging import version
 import warnings
@@ -176,20 +177,21 @@
         except ArgovisServerError as e:
             # Test is passed when something goes wrong because of the argovis server
             warnings.warn(
                 "\nSomething happened on argovis server that should not: %s" % str(e.args)
             )
             pass
         except DataNotFound as e:
-            # We make sure that data requested by tests are available from API, so this must be a server side error.
-            warnings.warn("\nSomething happened on server: %s" % str(e.args))
+            # We make sure that data requested by tests are available from API, so this must be a server side error !
+            warnings.warn("\nDataNotFound, Something happened on server side with:\n\t-%s" % "\n\t-".join(list(e.path)))
+            # traceback.print_tb(e.__traceback__)
             pass
         except ServerDisconnectedError as e:
             # We can't do anything about this !
-            warnings.warn("\nWe were disconnected from server !\n%s" % str(e.args))
+            warnings.warn("\n We were disconnected from server !\n%s" % str(e.args))
             pass
         except ClientResponseError as e:
             # The server is sending back an error when creating the response
             warnings.warn("\nAnother server side error:\n%s" % str(e.args))
             pass
         except FileNotFoundError as e:
             warnings.warn("\nServer didn't return the data:\n%s" % str(e.args))
```

### Comparing `argopy-0.1.8/argopy/tests/test_errors.py` & `argopy-0.1.9/argopy/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/tests/test_fetchers_data_argovis.py` & `argopy-0.1.9/argopy/tests/test_fetchers_data_argovis.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 @requires_connected_argovis
 class Test_Backend:
     """ Test main API facade for all available dataset and access points of the ARGOVIS data fetching backend """
 
     src = "argovis"
     requests = {
         "float": [[1901393], [1901393, 6902746]],
-        "profile": [[6902746, 34], [6902746, np.arange(12, 13)], [6902746, [1, 12]]],
+        "profile": [[6902746, 12], [6902746, np.arange(12, 13)], [6902746, [1, 12]]],
         "region": [
-            [-70, -65, 35.0, 40.0, 0, 10.0],
             [-70, -65, 35.0, 40.0, 0, 10.0, "2012-01", "2012-03"],
             [-70, -65, 35.0, 40.0, 0, 10.0, "2012-01", "2012-06"],
         ],
     }
 
     def test_cachepath_notfound(self):
         with tempfile.TemporaryDirectory() as testcachedir:
```

### Comparing `argopy-0.1.8/argopy/tests/test_fetchers_data_erddap.py` & `argopy-0.1.9/argopy/tests/test_fetchers_data_erddap.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/tests/test_fetchers_data_localftp.py` & `argopy-0.1.9/argopy/tests/test_fetchers_data_localftp.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/tests/test_fetchers_facade_data.py` & `argopy-0.1.9/argopy/tests/test_fetchers_facade_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
             assert isinstance(new_fetcher.index, pd.core.frame.DataFrame)
 
     @requires_matplotlib
     def test_plot(self):
         with argopy.set_options(local_ftp=self.local_ftp):
             f, fetcher = self.__get_fetcher(pt='float')
 
+            # Test 'trajectory'
             for ws in [False, has_seaborn]:
                 for wc in [False, has_cartopy]:
                     for legend in [True, False]:
                         fig, ax = fetcher.plot(ptype='trajectory', with_seaborn=ws, with_cartopy=wc, add_legend=legend)
                         assert isinstance(fig, mpl.figure.Figure)
 
                         expected_ax_type = (
@@ -137,23 +138,30 @@
                         assert isinstance(ax, expected_ax_type)
 
                         expected_lg_type = mpl.legend.Legend if legend else type(None)
                         assert isinstance(ax.get_legend(), expected_lg_type)
 
                         mpl.pyplot.close(fig)
 
+            # Test 'dac', 'profiler'
             for ws in [False, has_seaborn]:
                 for by in [
                     "dac",
                     "profiler"
                 ]:
                     fig, ax = fetcher.plot(ptype=by, with_seaborn=ws)
                     assert isinstance(fig, mpl.figure.Figure)
                     mpl.pyplot.close(fig)
 
+            # Test 'qc_altimetry'
+            import IPython
+            dsh = fetcher.plot(ptype='qc_altimetry', embed='slide')
+            assert isinstance(dsh(0), IPython.display.Image)
+
+            # Test invalid plot
             with pytest.raises(ValueError):
                 fetcher.plot(ptype='invalid_cat', with_seaborn=ws)
 
 
 @requires_fetcher
 class Test_DataFetching:
     """ Test main API facade for all available fetching backends and default dataset """
```

### Comparing `argopy-0.1.8/argopy/tests/test_fetchers_index_erddap.py` & `argopy-0.1.9/argopy/tests/test_fetchers_index_erddap.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/tests/test_fetchers_index_localftp.py` & `argopy-0.1.9/argopy/tests/test_fetchers_index_localftp.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/tests/test_fetchers_proto.py` & `argopy-0.1.9/argopy/tests/test_fetchers_proto.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/tests/test_options.py` & `argopy-0.1.9/argopy/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/tests/test_plotters.py` & `argopy-0.1.9/argopy/tests/test_plotters.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     requires_localftp,
     requires_connection,
     requires_matplotlib,
     has_matplotlib,
     has_seaborn,
     has_cartopy,
 )
-from argopy.plotters import bar_plot, plot_trajectory
+from argopy.plotters import bar_plot, plot_trajectory, open_sat_altim_report
 from argopy import IndexFetcher as ArgoIndexFetcher
 from argopy import DataFetcher as ArgoDataFetcher
 
 if has_matplotlib:
     import matplotlib as mpl
 
 if has_cartopy:
@@ -34,14 +34,30 @@
 @requires_connection
 def test_valid_dashboard():
     import IPython
     dsh = argopy.dashboard(wmo=5904797)
     assert isinstance(dsh, IPython.lib.display.IFrame)
 
 
+@requires_connection
+def test_open_sat_altim_report():
+    import IPython
+    dsh = open_sat_altim_report(WMO=5904797, embed='slide')
+    assert isinstance(dsh(0), IPython.display.Image)
+
+    dsh = open_sat_altim_report(WMO=5904797, embed='dropdown')
+    assert isinstance(dsh(5904797), IPython.display.Image)
+
+    open_sat_altim_report(WMO=5904797, embed='list')
+
+    dsh = open_sat_altim_report(WMO=5904797, embed=None)
+    assert isinstance(dsh, dict)
+    assert 5904797 in dsh
+
+
 @requires_localftp
 @requires_matplotlib
 class Test_index_plot:
     src = "localftp"
     local_ftp = argopy.tutorial.open_dataset("localftp")[0]
     requests = {
         "float": [[2901623], [2901623, 6901929, 5906072]],
```

### Comparing `argopy-0.1.8/argopy/tests/test_stores.py` & `argopy-0.1.9/argopy/tests/test_stores.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/tests/test_tutorial.py` & `argopy-0.1.9/argopy/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/tests/test_utilities.py` & `argopy-0.1.9/argopy/tests/test_utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,24 @@
     isAPIconnected,
     erddap_ds_exists,
     linear_interpolation_remap,
     Chunker,
     is_box,
     is_list_of_strings,
     format_oneline, is_indexbox,
-    check_wmo, is_wmo
+    check_wmo, is_wmo,
+    wmo2box,
+    modified_environ,
+    wrap_longitude,
+    toYearFraction, YearFraction_to_datetime,
+    TopoFetcher
 )
 from argopy.errors import InvalidFetcherAccessPoint, FtpPathError
 from argopy import DataFetcher as ArgoDataFetcher
-from . import requires_connection, requires_localftp
+from . import requires_connection, requires_localftp, requires_connection
 
 
 def test_invalid_dictionnary():
     with pytest.raises(ValueError):
         load_dict("invalid_dictionnary")
 
 
@@ -479,7 +484,66 @@
 
 
 def test_check_wmo():
     assert check_wmo(12345) == [12345]
     assert check_wmo([1234567]) == [1234567]
     assert check_wmo([12345, 1234567]) == [12345, 1234567]
     assert check_wmo(np.array((12345, 1234567), dtype='int')) == [12345, 1234567]
+
+
+def test_modified_environ():
+    os.environ["DUMMY_ENV_ARGOPY"] = 'initial'
+    with modified_environ(DUMMY_ENV_ARGOPY='toto'):
+        assert os.environ['DUMMY_ENV_ARGOPY'] == 'toto'
+    assert os.environ['DUMMY_ENV_ARGOPY'] == 'initial'
+    os.environ.pop('DUMMY_ENV_ARGOPY')
+
+
+def test_wmo2box():
+    with pytest.raises(ValueError):
+        wmo2box(12)
+    with pytest.raises(ValueError):
+        wmo2box(8000)
+    with pytest.raises(ValueError):
+        wmo2box(2000)
+
+    def complete_box(b):
+        b2 = b.copy()
+        b2.insert(4, 0.)
+        b2.insert(5, 10000.)
+        return b2
+
+    assert is_box(complete_box(wmo2box(1212)))
+    assert is_box(complete_box(wmo2box(3324)))
+    assert is_box(complete_box(wmo2box(5402)))
+    assert is_box(complete_box(wmo2box(7501)))
+
+
+def test_wrap_longitude():
+    assert wrap_longitude(np.array([-20])) == 340
+    assert wrap_longitude(np.array([40])) == 40
+    assert np.all(np.equal(wrap_longitude(np.array([340, 20])), np.array([340, 380])))
+
+
+def test_toYearFraction():
+    assert toYearFraction(pd.to_datetime('202001010000')) == 2020
+    assert toYearFraction(pd.to_datetime('202001010000', utc=True)) == 2020
+    assert toYearFraction(pd.to_datetime('202001010000')+pd.offsets.DateOffset(years=1)) == 2021
+
+
+def test_YearFraction_to_datetime():
+    assert YearFraction_to_datetime(2020) == pd.to_datetime('202001010000')
+    assert YearFraction_to_datetime(2020+1) == pd.to_datetime('202101010000')
+
+
+@requires_connection
+def test_TopoFetcher():
+    box = [81, 123, -67, -54]
+    fetcher = TopoFetcher(box, ds='gebco', stride=[10, 10], cache=True)
+    ds = fetcher.to_xarray()
+    assert isinstance(ds, xr.Dataset)
+    assert 'elevation' in ds.data_vars
+
+    fetcher = TopoFetcher(box, ds='gebco', stride=[10, 10], cache=False)
+    ds = fetcher.to_xarray()
+    assert isinstance(ds, xr.Dataset)
+    assert 'elevation' in ds.data_vars
```

### Comparing `argopy-0.1.8/argopy/tutorial.py` & `argopy-0.1.9/argopy/tutorial.py`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/argopy/utilities.py` & `argopy-0.1.9/argopy/utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import os
 import sys
 import warnings
 import urllib
 import json
 import collections
+import copy
 from functools import reduce
 from packaging import version
 
 import importlib
 import locale
 import platform
 import struct
@@ -37,14 +38,15 @@
 
 from argopy.options import OPTIONS, set_options
 from argopy.stores import httpstore
 from argopy.errors import (
     FtpPathError,
     InvalidFetcher,
     InvalidFetcherAccessPoint,
+    InvalidOption
 )
 
 try:
     collectionsAbc = collections.abc
 except AttributeError:
     collectionsAbc = collections
 
@@ -92,52 +94,53 @@
         return "Unknown"
     else:
         return Adictionnary[Avalue]
 
 
 def list_available_data_src():
     """ List all available data sources """
-    AVAILABLE_SOURCES = {}
+    sources = {}
     try:
         from .data_fetchers import erddap_data as Erddap_Fetchers
 
-        AVAILABLE_SOURCES["erddap"] = Erddap_Fetchers
+        sources["erddap"] = Erddap_Fetchers
     except Exception:
         warnings.warn(
             "An error occurred while loading the ERDDAP data fetcher, "
             "it will not be available !\n%s\n%s"
             % (sys.exc_info()[0], sys.exc_info()[1])
         )
         pass
 
     try:
         from .data_fetchers import localftp_data as LocalFTP_Fetchers
 
-        AVAILABLE_SOURCES["localftp"] = LocalFTP_Fetchers
+        sources["localftp"] = LocalFTP_Fetchers
     except Exception:
         warnings.warn(
             "An error occurred while loading the local FTP data fetcher, "
             "it will not be available !\n%s\n%s"
             % (sys.exc_info()[0], sys.exc_info()[1])
         )
         pass
 
     try:
         from .data_fetchers import argovis_data as ArgoVis_Fetchers
 
-        AVAILABLE_SOURCES["argovis"] = ArgoVis_Fetchers
+        sources["argovis"] = ArgoVis_Fetchers
     except Exception:
         warnings.warn(
             "An error occurred while loading the ArgoVis data fetcher, "
             "it will not be available !\n%s\n%s"
             % (sys.exc_info()[0], sys.exc_info()[1])
         )
         pass
 
-    return AVAILABLE_SOURCES
+    # return dict(sorted(sources.items()))
+    return sources
 
 
 def list_available_index_src():
     """ List all available index sources """
     AVAILABLE_SOURCES = {}
     try:
         from .data_fetchers import erddap_index as Erddap_Fetchers
@@ -163,15 +166,15 @@
         )
         pass
 
     return AVAILABLE_SOURCES
 
 
 def list_standard_variables():
-    """ Return the list of variables for standard users """
+    """ List of variables for standard users """
     return [
         "DATA_MODE",
         "LATITUDE",
         "LONGITUDE",
         "POSITION_QC",
         "DIRECTION",
         "PLATFORM_NUMBER",
@@ -196,15 +199,15 @@
         "TIME",
         "TIME_QC",
         "CONFIG_MISSION_NUMBER",
     ]
 
 
 def list_multiprofile_file_variables():
-    """ Return the list of variables in a netcdf multiprofile file.
+    """ List of variables in a netcdf multiprofile file.
 
         This is for files created by GDAC under <DAC>/<WMO>/<WMO>_prof.nc
     """
     return [
         "CONFIG_MISSION_NUMBER",
         "CYCLE_NUMBER",
         "DATA_CENTRE",
@@ -506,16 +509,17 @@
     Parameters
     ----------
     file : file-like, optional
         print to the given file-like object. Defaults to sys.stdout.
     """
     print("\nARGOPY OPTIONS", file=file)
     print("--------------", file=file)
-
-    for k, v in OPTIONS.items():
+    opts = copy.deepcopy(OPTIONS)
+    opts = dict(sorted(opts.items()))
+    for k, v in opts.items():
         print(f"{k}: {v}", file=file)
 
 
 def isconnected(host="https://www.ifremer.fr"):
     """ check if we have a live internet connection
 
         Parameters
@@ -550,48 +554,41 @@
             If True check the data fetcher (default), if False, check the index fetcher
 
         Returns
         -------
         bool
     """
     if data:
-        AVAILABLE_SOURCES = list_available_data_src()
+        list_src = list_available_data_src()
     else:
-        AVAILABLE_SOURCES = list_available_index_src()
-    if src in AVAILABLE_SOURCES and getattr(
-        AVAILABLE_SOURCES[src], "api_server_check", None
+        list_src = list_available_index_src()
+
+    if src in list_src and getattr(
+        list_src[src], "api_server_check", None
     ):
         if "localftp" in src:
-            # This is a special case because the source here is a local folder, and the folder validity is checked
-            # when setting the option value of 'local_ftp'
-            # So here, we just need to catch the appropriate error after a call to set_option
-            # opts = {"src": src, "local_ftp": OPTIONS["local_ftp"]}
-            # try:
-            #     set_options(**opts)
-            #     return True
-            # except OptionValueError:
-            #     return False
-            return check_localftp(OPTIONS["local_ftp"])
+            # This is a special case because the source here is a local folder
+            result = check_localftp(OPTIONS["local_ftp"])
         else:
-            with set_options(src=src):
-                return isconnected(AVAILABLE_SOURCES[src].api_server_check)
+            result = isconnected(list_src[src].api_server_check)
+        return result
     else:
         raise InvalidFetcher
 
 
-def erddap_ds_exists(ds: str = "ArgoFloats", erddap: str = 'http://www.ifremer.fr/erddap') -> bool:
+def erddap_ds_exists(ds: str = "ArgoFloats", erddap: str = 'https://www.ifremer.fr/erddap') -> bool:
     """ Check if a dataset exists on a remote erddap server
     return a bool
 
     Parameter
     ---------
     ds: str
         Name of the erddap dataset to check (default: 'ArgoFloats')
     erddap: str
-        Url of the erddap server (default: 'http://www.ifremer.fr/erddap')
+        Url of the erddap server (default: 'https://www.ifremer.fr/erddap')
 
     Return
     ------
     bool
     """
     with httpstore(timeout=OPTIONS['api_timeout']).open("".join([erddap, "/info/index.json"])) as of:
         erddap_index = json.load(of)
@@ -628,23 +625,39 @@
     img = url(urllib.parse.quote(label), urllib.parse.quote(message), color)
     if not insert:
         return img
     else:
         return Image(url=img)
 
 
-def fetch_status(stdout="html", insert=True):
-    """ Fetch and report web API status """
+def fetch_status(stdout: str = "html", insert: bool = True):
+    """ Fetch and report web API status
+
+    Parameters
+    ----------
+    stdout: str
+        Format of the results, default is 'html'. Otherwise a simple string.
+    insert: bool
+        Print or display results directly in stdout format.
+
+    Returns
+    -------
+    IPython.display.HTML or str
+    """
     results = {}
-    for api, mod in list_available_data_src().items():
+    list_src = list_available_data_src()
+    for api, mod in list_src.items():
         if getattr(mod, "api_server_check", None):
             # status = isconnected(mod.api_server_check)
             status = isAPIconnected(api)
-            # message = "up" if status else "down"
-            message = "ok" if status else "offline"
+            if api=='localftp' and OPTIONS['local_ftp'] == '-':
+                message = "ok" if status else "path undefined !"
+            else:
+                # message = "up" if status else "down"
+                message = "ok" if status else "offline"
             results[api] = {"value": status, "message": message}
 
     if "IPython" in sys.modules and stdout == "html":
         cols = []
         for api in sorted(results.keys()):
             color = "green" if results[api]["value"] else "orange"
             if isconnected():
@@ -835,23 +848,27 @@
 
         Allow to easily split an access point request into chunks
 
         Parameters
         ----------
         request: dict
             Access point request to be chunked. One of the following:
-            {'box': [lon_min, lon_max, lat_min, lat_max, dpt_min, dpt_max, time_min, time_max]}
-            {'box': [lon_min, lon_max, lat_min, lat_max, dpt_min, dpt_max]}
-            {'wmo': [wmo1, wmo2, ...], 'cyc': [0,1, ...]}
+
+            - {'box': [lon_min, lon_max, lat_min, lat_max, dpt_min, dpt_max, time_min, time_max]}
+            - {'box': [lon_min, lon_max, lat_min, lat_max, dpt_min, dpt_max]}
+            - {'wmo': [wmo1, wmo2, ...], 'cyc': [0,1, ...]}
         chunks: 'auto' or dict
             Dictionary with request access point as keys and number of chunks to create as values.
+
             Eg: {'wmo':10} will create a maximum of 10 chunks along WMOs.
         chunksize: dict, optional
             Dictionary with request access point as keys and chunk size as values (used as maximum values in
-            'auto' chunking). Eg: {'wmo': 5} will create chunks with as many as 5 WMOs each.
+            'auto' chunking).
+
+            Eg: {'wmo': 5} will create chunks with as many as 5 WMOs each.
 
         """
         self.request = request
 
         if "box" in self.request:
             is_box(self.request["box"])
             if len(self.request["box"]) == 8:
@@ -1166,30 +1183,30 @@
     #     print(box)
     # Formats:
     tests["box must be a list"] = lambda b: isinstance(b, list)
     tests["box must be a list with 6 or 8 elements"] = lambda b: len(b) in [6, 8]
 
     # Types:
     tests["lon_min must be numeric"] = lambda b: (
-        isinstance(b[0], int) or isinstance(b[0], float)
+        isinstance(b[0], int) or isinstance(b[0], (np.floating, float))
     )
     tests["lon_max must be numeric"] = lambda b: (
-        isinstance(b[1], int) or isinstance(b[1], float)
+        isinstance(b[1], int) or isinstance(b[1], (np.floating, float))
     )
     tests["lat_min must be numeric"] = lambda b: (
-        isinstance(b[2], int) or isinstance(b[2], float)
+        isinstance(b[2], int) or isinstance(b[2], (np.floating, float))
     )
     tests["lat_max must be numeric"] = lambda b: (
-        isinstance(b[3], int) or isinstance(b[3], float)
+        isinstance(b[3], int) or isinstance(b[3], (np.floating, float))
     )
     tests["pres_min must be numeric"] = lambda b: (
-        isinstance(b[4], int) or isinstance(b[4], float)
+        isinstance(b[4], int) or isinstance(b[4], (np.floating, float))
     )
     tests["pres_max must be numeric"] = lambda b: (
-        isinstance(b[5], int) or isinstance(b[5], float)
+        isinstance(b[5], int) or isinstance(b[5], (np.floating, float))
     )
     if len(box) == 8:
         tests[
             "datetim_min must be a string convertible to a Pandas datetime"
         ] = lambda b: isinstance(b[-2], str) and is_dateconvertible(b[-2])
         tests[
             "datetim_max must be a string convertible to a Pandas datetime"
@@ -1238,16 +1255,21 @@
     return all(isinstance(x, dict) for x in lst)
 
 
 def is_list_of_datasets(lst):
     return all(isinstance(x, xr.Dataset) for x in lst)
 
 
+def is_list_equal(lst1, lst2):
+    """ Return true if 2 lists contain same elements"""
+    return len(lst1) == len(lst2) and len(lst1) == sum([1 for i, j in zip(lst1, lst2) if i == j])
+
+
 def check_wmo(lst):
-    """ Check a WMO option and returned it as a list of integers
+    """ Validate a WMO option and returned it as a list of integers
 
     Parameters
     ----------
     wmo: int
         WMO must be an integer or an iterable with elements that can be casted as integers
     errors: 'raise'
 
@@ -1265,15 +1287,15 @@
             lst = [lst]
 
     # Then cast list elements as integers
     return [abs(int(x)) for x in lst]
 
 
 def is_wmo(lst, errors="raise"):  # noqa: C901
-    """ Assess validity of a WMO option value
+    """ Check if a WMO is valid
 
     Parameters
     ----------
     wmo: int, list(int), array(int)
         WMO must be a single or a list of 5/7 digit positive numbers
     errors: 'raise'
         Possibly raises a ValueError exception, otherwise fails silently.
@@ -1380,8 +1402,408 @@
 
     try:
         env.update(update)
         [env.pop(k, None) for k in remove]
         yield
     finally:
         env.update(update_after)
-        [env.pop(k) for k in remove_after]
+        [env.pop(k) for k in remove_after]
+
+
+def toYearFraction(this_date: pd._libs.tslibs.timestamps.Timestamp = pd.to_datetime('now')):
+    """ Compute decimal year, robust to leap years, precision to the second
+
+    Compute the fraction of the year a given timestamp corresponds to.
+    The "fraction of the year" goes:
+    - from 0 on 01-01T00:00:00.000 of the year
+    - to 1 on the 01-01T00:00:00.000 of the following year
+
+    1 second corresponds to the number of days in the year times 86400.
+    The faction of the year is rounded to 10-digits in order to have a "second" precision.
+
+    See discussion here: https://github.com/euroargodev/argodmqc_owc/issues/35
+
+    Parameters
+    ----------
+    pd._libs.tslibs.timestamps.Timestamp
+
+    Returns
+    -------
+    float
+    """
+    if "UTC" in [this_date.tzname() if not this_date.tzinfo is None else ""]:
+        startOfThisYear = pd.to_datetime("%i-01-01T00:00:00.000" % this_date.year, utc=True)
+    else:
+        startOfThisYear = pd.to_datetime("%i-01-01T00:00:00.000" % this_date.year)
+    yearDuration_sec = (startOfThisYear + pd.offsets.DateOffset(years=1) - startOfThisYear).total_seconds()
+
+    yearElapsed_sec = (this_date - startOfThisYear).total_seconds()
+    fraction = yearElapsed_sec / yearDuration_sec
+    fraction = np.round(fraction, 10)
+    return this_date.year + fraction
+
+
+def YearFraction_to_datetime(yf: float):
+    """ Compute datetime from year fraction
+
+    Inverse the toYearFraction() function
+
+    Parameters
+    ----------
+    float
+
+    Returns
+    -------
+    pd._libs.tslibs.timestamps.Timestamp
+    """
+    year = np.int32(yf)
+    fraction = yf - year
+    fraction = np.round(fraction, 10)
+
+    startOfThisYear = pd.to_datetime("%i-01-01T00:00:00" % year)
+    yearDuration_sec = (startOfThisYear + pd.offsets.DateOffset(years=1) - startOfThisYear).total_seconds()
+    yearElapsed_sec = pd.Timedelta(fraction * yearDuration_sec, unit='s')
+    return pd.to_datetime(startOfThisYear + yearElapsed_sec, unit='s')
+
+
+def wrap_longitude(grid_long):
+    """ Allows longitude (0-360) to wrap beyond the 360 mark, for mapping purposes.
+        Makes sure that, if the longitude is near the boundary (0 or 360) that we
+        wrap the values beyond
+        360 so it appears nicely on a map
+        This is a refactor between get_region_data and get_region_hist_locations to
+        avoid duplicate code
+
+        source: https://github.com/euroargodev/argodmqc_owc/blob/e174f4538fdae1534c9740491398972b1ffec3ca/pyowc/utilities.py#L80
+
+        Parameters
+        ----------
+        grid_long: array of longitude values
+
+        Returns
+        -------
+        array of longitude values that can extend past 360
+    """
+    neg_long = np.argwhere(grid_long < 0)
+    grid_long[neg_long] = grid_long[neg_long] + 360
+
+    # if we have data close to upper boundary (360), then wrap some of the data round
+    # so it appears on the map
+    top_long = np.argwhere(grid_long >= 320)
+    if top_long.__len__() != 0:
+        bottom_long = np.argwhere(grid_long <= 40)
+        grid_long[bottom_long] = 360 + grid_long[bottom_long]
+
+    return grid_long
+
+
+def wmo2box(wmo_id: int):
+    """ Convert WMO square box number into a latitude/longitude box
+
+    See:
+    https://en.wikipedia.org/wiki/World_Meteorological_Organization_squares
+    https://commons.wikimedia.org/wiki/File:WMO-squares-global.gif
+
+    Parameters
+    ----------
+    wmo_id: int
+        WMO square number, must be between 1000 and 7817
+
+    Returns
+    -------
+    box: list(int)
+        [lon_min, lon_max, lat_min, lat_max] bounds to the WMO square number
+    """
+    if wmo_id < 1000 or wmo_id > 7817:
+        raise ValueError("Invalid WMO square number, must be between 1000 and 7817.")
+    wmo_id = str(wmo_id)
+
+    # "global quadrant" numbers where 1=NE, 3=SE, 5=SW, 7=NW
+    quadrant = int(wmo_id[0])
+    if quadrant not in [1, 3, 5 ,7]:
+        raise ValueError("Invalid WMO square number, 1st digit must be 1, 3, 5 or 7.")
+
+    # 'minimum' Latitude square boundary, nearest to the Equator
+    nearest_to_the_Equator_latitude = int(wmo_id[1])
+
+    # 'minimum' Longitude square boundary, nearest to the Prime Meridian
+    nearest_to_the_Prime_Meridian = int(wmo_id[2:4])
+
+    #
+    dd = 10
+    if quadrant in [1, 3]:
+        lon_min = nearest_to_the_Prime_Meridian*dd
+        lon_max = nearest_to_the_Prime_Meridian*dd+dd
+    elif quadrant in [5, 7]:
+        lon_min = -nearest_to_the_Prime_Meridian*dd-dd
+        lon_max = -nearest_to_the_Prime_Meridian*dd
+
+    if quadrant in [1, 7]:
+        lat_min = nearest_to_the_Equator_latitude*dd
+        lat_max = nearest_to_the_Equator_latitude*dd+dd
+    elif quadrant in [3, 5]:
+        lat_min = -nearest_to_the_Equator_latitude*dd-dd
+        lat_max = -nearest_to_the_Equator_latitude*dd
+
+    box = [lon_min, lon_max, lat_min, lat_max]
+    return box
+
+
+def groupby_remap(z, data, z_regridded, z_dim=None, z_regridded_dim="regridded", output_dim="remapped", select='deep', right=False):
+    """ todo: Need a docstring here !"""
+
+    # sub-sampling called in xarray ufunc
+    def _subsample_bins(x, y, target_values):
+        # remove all nans from input x and y
+        idx = np.logical_or(np.isnan(x), np.isnan(y))
+        x = x[~idx]
+        y = y[~idx]
+
+        ifound = np.digitize(x, target_values, right=right)  # ``bins[i-1] <= x < bins[i]``
+        ifound -= 1  # Because digitize returns a 1-based indexing, we need to remove 1
+        y_binned = np.ones_like(target_values) * np.nan
+
+        for ib, this_ibin in enumerate(np.unique(ifound)):
+            ix = np.where(ifound == this_ibin)
+            iselect = ix[-1]
+
+            # Map to y value at specific x index in the bin:
+            if select == 'shallow':
+                iselect = iselect[0]  # min/shallow
+                mapped_value = y[iselect]
+            elif select == 'deep':
+                iselect = iselect[-1]  # max/deep
+                mapped_value = y[iselect]
+            elif select == 'middle':
+                iselect = iselect[np.where(x[iselect] >= np.median(x[iselect]))[0][0]]  # median/middle
+                mapped_value = y[iselect]
+            elif select == 'random':
+                iselect = iselect[np.random.randint(len(iselect))]
+                mapped_value = y[iselect]
+
+            # or Map to y statistics in the bin:
+            elif select == 'mean':
+                mapped_value = np.nanmean(y[iselect])
+            elif select == 'min':
+                mapped_value = np.nanmin(y[iselect])
+            elif select == 'max':
+                mapped_value = np.nanmax(y[iselect])
+            elif select == 'median':
+                mapped_value = np.median(y[iselect])
+
+            else:
+                raise InvalidOption("`select` option has invalid value (%s)" % select)
+
+            y_binned[this_ibin] = mapped_value
+
+        return y_binned
+
+    # infer dim from input
+    if z_dim is None:
+        if len(z.dims) != 1:
+            raise RuntimeError("if z_dim is not specified, x must be a 1D array.")
+        dim = z.dims[0]
+    else:
+        dim = z_dim
+
+    # if dataset is passed drop all data_vars that dont contain dim
+    if isinstance(data, xr.Dataset):
+        raise ValueError("Dataset input is not supported yet")
+        # TODO: for a dataset input just apply the function for each appropriate array
+
+    if version.parse(xr.__version__) > version.parse("0.15.0"):
+        kwargs = dict(
+            input_core_dims=[[dim], [dim], [z_regridded_dim]],
+            output_core_dims=[[output_dim]],
+            vectorize=True,
+            dask="parallelized",
+            output_dtypes=[data.dtype],
+            dask_gufunc_kwargs={'output_sizes': {output_dim: len(z_regridded[z_regridded_dim])}},
+        )
+    else:
+        kwargs = dict(
+            input_core_dims=[[dim], [dim], [z_regridded_dim]],
+            output_core_dims=[[output_dim]],
+            vectorize=True,
+            dask="parallelized",
+            output_dtypes=[data.dtype],
+            output_sizes={output_dim: len(z_regridded[z_regridded_dim])},
+        )
+    remapped = xr.apply_ufunc(_subsample_bins, z, data, z_regridded, **kwargs)
+
+    remapped.coords[output_dim] = z_regridded.rename({z_regridded_dim: output_dim}).coords[output_dim]
+    return remapped
+
+
+class TopoFetcher():
+    """ Fetch topographic data through an ERDDAP server for an ocean rectangle
+
+    Example:
+        >>> from argopy import TopoFetcher
+        >>> box = [-75, -45, 20, 30]  # Lon_min, lon_max, lat_min, lat_max
+        >>> ds = TopoFetcher(box).to_xarray()
+        >>> ds = TopoFetcher(box, ds='gebco', stride=[10, 10], cache=True).to_xarray()
+
+    """
+
+    class ERDDAP():
+        def __init__(self, server: str, protocol: str = 'tabledap'):
+            self.server = server
+            self.protocol = protocol
+            self.response = 'nc'
+            self.dataset_id = ''
+            self.constraints = ''
+
+    def __init__(
+            self,
+            box: list,
+            ds: str = "gebco",
+            cache: bool = False,
+            cachedir: str = "",
+            api_timeout: int = 0,
+            stride: list = [1, 1],
+            **kwargs,
+    ):
+        """ Instantiate an ERDDAP topo data fetcher
+
+        Parameters
+        ----------
+        ds: str (optional), default: 'gebco'
+            Dataset to load:
+
+            - 'gebco' will load the GEBCO_2020 Grid, a continuous terrain model for oceans and land at 15 arc-second intervals
+        stride: list, default [1, 1]
+            Strides along longitude and latitude. This allows to change the output resolution
+        cache: bool (optional)
+            Cache data or not (default: False)
+        cachedir: str (optional)
+            Path to cache folder
+        api_timeout: int (optional)
+            Erddap request time out in seconds. Set to OPTIONS['api_timeout'] by default.
+        """
+        timeout = OPTIONS["api_timeout"] if api_timeout == 0 else api_timeout
+        self.fs = httpstore(cache=cache, cachedir=cachedir, timeout=timeout, size_policy='head')
+        self.definition = "Erddap topographic data fetcher"
+
+        self.BOX = box
+        self.stride = stride
+        if ds == "gebco":
+            self.definition = "NOAA erddap gebco data fetcher for a space region"
+            self.server = 'https://coastwatch.pfeg.noaa.gov/erddap'
+            self.server_name = 'NOAA'
+            self.dataset_id = 'gebco'
+
+        self._init_erddap()
+
+    def _init_erddap(self):
+        # Init erddap
+        self.erddap = self.ERDDAP(server=self.server, protocol="griddap")
+        self.erddap.response = (
+            "nc"
+        )
+
+        if self.dataset_id == "gebco":
+            self.erddap.dataset_id = "GEBCO_2020"
+        else:
+            raise ValueError(
+                "Invalid database short name for %s erddap" % self.server_name
+            )
+        return self
+
+    def _cname(self) -> str:
+        """ Fetcher one line string definition helper """
+        cname = "?"
+
+        if hasattr(self, "BOX"):
+            BOX = self.BOX
+            cname = ("[x=%0.2f/%0.2f; y=%0.2f/%0.2f]") % (
+                BOX[0],
+                BOX[1],
+                BOX[2],
+                BOX[3],
+            )
+        return cname
+
+    def __repr__(self):
+        summary = ["<topofetcher.erddap>"]
+        summary.append("Name: %s" % self.definition)
+        summary.append("API: %s" % self.server)
+        summary.append("Domain: %s" % format_oneline(self.cname()))
+        return "\n".join(summary)
+
+    def cname(self):
+        """ Return a unique string defining the constraints """
+        return self._cname()
+
+    @property
+    def cachepath(self):
+        """ Return path to cached file(s) for this request
+
+        Returns
+        -------
+        list(str)
+        """
+        return [self.fs.cachepath(uri) for uri in self.uri]
+
+    def define_constraints(self):
+        """ Define request constraints """
+        #        Eg: https://coastwatch.pfeg.noaa.gov/erddap/griddap/GEBCO_2020.nc?elevation%5B(34):5:(42)%5D%5B(-21):7:(-12)%5D
+        self.erddap.constraints = "%s(%0.2f):%i:(%0.2f)%s%s(%0.2f):%i:(%0.2f)%s" % (
+        "%5B", self.BOX[2], self.stride[1], self.BOX[3], "%5D",
+        "%5B", self.BOX[0], self.stride[0], self.BOX[1], "%5D")
+        return None
+
+    #     @property
+    #     def _minimal_vlist(self):
+    #         """ Return the minimal list of variables to retrieve """
+    #         vlist = list()
+    #         vlist.append("latitude")
+    #         vlist.append("longitude")
+    #         vlist.append("elevation")
+    #         return vlist
+
+    def get_url(self):
+        """ Return the URL to download data requested
+
+        Returns
+        -------
+        str
+        """
+        # First part of the URL:
+        protocol = self.erddap.protocol
+        dataset_id = self.erddap.dataset_id
+        response = self.erddap.response
+        url = f"{self.erddap.server}/{protocol}/{dataset_id}.{response}?"
+
+        # Add variables to retrieve:
+        variables = ["elevation"]
+        variables = ",".join(variables)
+        url += f"{variables}"
+
+        # Add constraints:
+        self.define_constraints()  # Define constraint to select this box of data (affect self.erddap.constraints)
+        url += f"{self.erddap.constraints}"
+
+        return url
+
+    @property
+    def uri(self):
+        """ List of files to load for a request
+
+        Returns
+        -------
+        list(str)
+        """
+        return [self.get_url()]
+
+    def to_xarray(self, errors: str = 'ignore'):
+        """ Load Topographic data and return a xarray.DataSet """
+
+        # Download data
+        if len(self.uri) == 1:
+            ds = self.fs.open_dataset(self.uri[0])
+
+        return ds
+
+    def load(self, errors: str = 'ignore'):
+        """ Load Topographic data and return a xarray.DataSet """
+        return self.to_xarray(errors=errors)
```

### Comparing `argopy-0.1.8/argopy.egg-info/SOURCES.txt` & `argopy-0.1.9/argopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argopy-0.1.8/setup.py` & `argopy-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name='argopy',
-    version='0.1.8',
+    version='0.1.9',
     author="argopy Developers",
     author_email="gmaze@ifremer.fr",
     description="A python library for Argo data beginners and experts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/euroargodev/argopy",
     packages=setuptools.find_packages(),
```

