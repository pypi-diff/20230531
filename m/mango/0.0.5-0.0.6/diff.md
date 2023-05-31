# Comparing `tmp/mango-0.0.5.tar.gz` & `tmp/mango-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-0.0.5.tar", last modified: Wed Apr 26 11:38:15 2023, max compression
+gzip compressed data, was "mango-0.0.6.tar", last modified: Wed May 31 09:25:02 2023, max compression
```

## Comparing `mango-0.0.5.tar` & `mango-0.0.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.674650 mango-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-26 11:38:07.000000 mango-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 11:38:07.000000 mango-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 11:38:15.674650 mango-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 11:38:07.000000 mango-0.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 11:38:07.000000 mango-0.0.5/mango/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/email_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/google_cloud_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/config/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 11:38:07.000000 mango-0.0.5/mango/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-26 11:38:07.000000 mango-0.0.5/mango/config/base_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/data/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 11:38:07.000000 mango-0.0.5/mango/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-04-26 11:38:07.000000 mango-0.0.5/mango/data/ts_dataset.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:07.000000 mango-0.0.5/mango/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-26 11:38:07.000000 mango-0.0.5/mango/images/images_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 11:38:07.000000 mango-0.0.5/mango/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-26 11:38:07.000000 mango-0.0.5/mango/logging/chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-26 11:38:07.000000 mango-0.0.5/mango/logging/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-26 11:38:07.000000 mango-0.0.5/mango/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/models/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 11:38:07.000000 mango-0.0.5/mango/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-26 11:38:07.000000 mango-0.0.5/mango/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 11:38:07.000000 mango-0.0.5/mango/models/neural_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:07.000000 mango-0.0.5/mango/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-26 11:38:07.000000 mango-0.0.5/mango/plots/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/processing_time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 11:38:07.000000 mango-0.0.5/mango/schemas/location.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 11:38:07.000000 mango-0.0.5/mango/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-26 11:38:07.000000 mango-0.0.5/mango/shared/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-26 11:38:07.000000 mango-0.0.5/mango/shared/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 11:38:07.000000 mango-0.0.5/mango/shared/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/table/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 11:38:07.000000 mango-0.0.5/mango/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-04-26 11:38:07.000000 mango-0.0.5/mango/table/pytups_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    25317 2023-04-26 11:38:07.000000 mango-0.0.5/mango/table/pytups_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-26 11:38:07.000000 mango-0.0.5/mango/table/table_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.674650 mango-0.0.5/mango/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/json_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test_bad_type.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test_bad_value.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test_good.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_arcgis_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_processing_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    42962 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:38:15.674650 mango-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-26 11:38:07.000000 mango-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.633232 mango-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-31 09:24:57.000000 mango-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-31 09:24:57.000000 mango-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-31 09:25:02.633232 mango-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-31 09:24:57.000000 mango-0.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.621231 mango-0.0.6/mango/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 09:24:57.000000 mango-0.0.6/mango/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.625232 mango-0.0.6/mango/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:24:57.000000 mango-0.0.6/mango/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-31 09:24:57.000000 mango-0.0.6/mango/clients/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-31 09:24:57.000000 mango-0.0.6/mango/clients/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-31 09:24:57.000000 mango-0.0.6/mango/clients/email_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-31 09:24:57.000000 mango-0.0.6/mango/clients/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-31 09:24:57.000000 mango-0.0.6/mango/clients/google_cloud_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.625232 mango-0.0.6/mango/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 09:24:57.000000 mango-0.0.6/mango/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-31 09:24:57.000000 mango-0.0.6/mango/config/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.625232 mango-0.0.6/mango/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-31 09:24:57.000000 mango-0.0.6/mango/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-05-31 09:24:57.000000 mango-0.0.6/mango/data/ts_dataset.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.625232 mango-0.0.6/mango/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:24:57.000000 mango-0.0.6/mango/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-05-31 09:24:57.000000 mango-0.0.6/mango/images/images_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.625232 mango-0.0.6/mango/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 09:24:57.000000 mango-0.0.6/mango/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-31 09:24:57.000000 mango-0.0.6/mango/logging/chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-31 09:24:57.000000 mango-0.0.6/mango/logging/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-31 09:24:57.000000 mango-0.0.6/mango/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.629232 mango-0.0.6/mango/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-31 09:24:57.000000 mango-0.0.6/mango/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-31 09:24:57.000000 mango-0.0.6/mango/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-31 09:24:57.000000 mango-0.0.6/mango/models/neural_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.629232 mango-0.0.6/mango/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:24:57.000000 mango-0.0.6/mango/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-31 09:24:57.000000 mango-0.0.6/mango/plots/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.629232 mango-0.0.6/mango/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-31 09:24:57.000000 mango-0.0.6/mango/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-31 09:24:57.000000 mango-0.0.6/mango/processing/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-31 09:24:57.000000 mango-0.0.6/mango/processing/file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-31 09:24:57.000000 mango-0.0.6/mango/processing/object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-31 09:24:57.000000 mango-0.0.6/mango/processing/processing_time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.629232 mango-0.0.6/mango/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-31 09:24:57.000000 mango-0.0.6/mango/schemas/location.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.629232 mango-0.0.6/mango/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 09:24:57.000000 mango-0.0.6/mango/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-31 09:24:57.000000 mango-0.0.6/mango/shared/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-31 09:24:57.000000 mango-0.0.6/mango/shared/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-31 09:24:57.000000 mango-0.0.6/mango/shared/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.629232 mango-0.0.6/mango/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 09:24:57.000000 mango-0.0.6/mango/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-05-31 09:24:57.000000 mango-0.0.6/mango/table/pytups_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26941 2023-05-31 09:24:57.000000 mango-0.0.6/mango/table/pytups_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-31 09:24:57.000000 mango-0.0.6/mango/table/table_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.633232 mango-0.0.6/mango/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.633232 mango-0.0.6/mango/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/data/json_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/data/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/data/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/data/test.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/data/test_bad_type.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/data/test_bad_value.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/data/test_good.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_arcgis_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_processing_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46624 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-31 09:24:57.000000 mango-0.0.6/mango/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:25:02.625232 mango-0.0.6/mango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-31 09:25:02.000000 mango-0.0.6/mango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-31 09:25:02.000000 mango-0.0.6/mango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:25:02.000000 mango-0.0.6/mango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-31 09:25:02.000000 mango-0.0.6/mango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 09:25:02.000000 mango-0.0.6/mango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:25:02.633232 mango-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-31 09:24:57.000000 mango-0.0.6/setup.py
```

### Comparing `mango-0.0.5/LICENSE` & `mango-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/PKG-INFO` & `mango-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
```

### Comparing `mango-0.0.5/mango/clients/arcgis.py` & `mango-0.0.6/mango/clients/arcgis.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/clients/email_downloader.py` & `mango-0.0.6/mango/clients/email_downloader.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/clients/email_sender.py` & `mango-0.0.6/mango/clients/email_sender.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/clients/google_cloud_storage.py` & `mango-0.0.6/mango/clients/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/config/base_config.py` & `mango-0.0.6/mango/config/base_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/data/ts_dataset.pkl` & `mango-0.0.6/mango/data/ts_dataset.pkl`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/images/images_functions.py` & `mango-0.0.6/mango/images/images_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/logging/chrono.py` & `mango-0.0.6/mango/logging/chrono.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/logging/decorators.py` & `mango-0.0.6/mango/logging/decorators.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/logging/logger.py` & `mango-0.0.6/mango/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/models/neural_networks.py` & `mango-0.0.6/mango/models/neural_networks.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/plots/plots.py` & `mango-0.0.6/mango/plots/plots.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/processing/__init__.py` & `mango-0.0.6/mango/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/processing/date_functions.py` & `mango-0.0.6/mango/processing/date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/processing/file_functions.py` & `mango-0.0.6/mango/processing/file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/processing/object_functions.py` & `mango-0.0.6/mango/processing/object_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/processing/processing_time_series.py` & `mango-0.0.6/mango/processing/processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/shared/const.py` & `mango-0.0.6/mango/shared/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/shared/decorators.py` & `mango-0.0.6/mango/shared/decorators.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/table/pytups_table.py` & `mango-0.0.6/mango/table/pytups_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     lag_col,
     replace_nan,
     group_mutate,
     to_dictlist,
     distinct,
     order_by,
     drop_nested,
-    group_by, auto_join,
+    group_by,
+    auto_join,
 )
 from .table_tools import is_subset
 from mango.processing import load_json, write_json, as_list
 
 
 class Table(TupList):
     def __init__(self, data=None, check=False):
@@ -86,14 +87,18 @@
 
     def sorted(self, **kwargs) -> "Table":
         raise NotImplementedError(
             "A list of dict cannot be sorted. Use order_by instead"
         )
 
     def take(self, indices, use_numpy=False) -> TupList:
+        indices = as_list(indices)
+        if len(indices) == 1:
+            indices = indices[0]
+
         return TupList(self).take(indices, use_numpy)
 
     # New or modified methods
     def __str__(self):
         if self.len():
             if not isinstance(self[0], dict):
                 return super.__str__(self)
@@ -133,17 +138,17 @@
         Show the first, middle and last n rows of the table.
 
         :param n: number of rows to show in each part.
         :param name: name or message to print with the table
         :return: the printed string
         """
         if name is None:
-            name=""
+            name = ""
         else:
-            name = name +": "
+            name = name + ": "
         if self.len() < 3 * n:
             print(f"{name}{self}")
             return self
         else:
             middle = (self.len() - n) // 2
             message = (
                 f"{name}Table ({self.len()} rows, , {len(self[0])} columns):\n"
@@ -303,14 +308,17 @@
     def filter(self, func) -> "Table":
         """
         Filter a table.
 
         :param func: function to use to filter
         :return: the filtered table.
         """
+        if not self.len():
+            return self
+
         return Table(self.vfilter(func))
 
     def get_col_names(self) -> "Table":
         """
         Get the names of the column of the table.
 
         :return: a list of keys
@@ -321,16 +329,16 @@
         """
         Create a dict with a list of values for each column of the table.
 
         :return: a dict
         """
         if self.len() == 0:
             return SuperDict()
-
-        return SuperDict({col: self.take(col) for col in self.get_col_names()})
+        table = self.replace_empty(None)
+        return SuperDict({col: table.take(col) for col in self.get_col_names()})
 
     @staticmethod
     def from_columns(dct) -> "Table":
         """
         Create a table from a dict of list (columns)
 
         Example:
@@ -343,15 +351,15 @@
         """
         return Table(to_dictlist(dct))
 
     def get_index(self, cond) -> "list":
         """
         Get row number for rows which respect a condition.
 
-        :param cond: codition/filter to apply to the rows
+        :param cond: condition/filter to apply to the rows
         :return: a list of row numbers
         """
         return [i for i, v in enumerate(self) if cond(v)]
 
     def replace(self, replacement=None, to_replace=None) -> "Table":
         """
         Fill missing values of a tuplist.
@@ -494,14 +502,17 @@
         Create a dict with the given columns as keys and values.
 
         :param keys: columns to use as keys.
         :param value: column to use as values.
         :param is_list: True if the values are a list instead of a single value.
         :return: a superdict indexed by the given keys.
         """
+        if not self.len():
+            return SuperDict()
+
         table_col = set(self[0].keys())
         if not is_subset(keys, table_col):
             raise KeyError(f"key(s) {keys} are not in table.")
         if not is_list and not self.is_unique(keys):
             raise ValueError(
                 "There are duplicate values for keys {keys}."
                 + " Method to_param with is_list=False expect a single value for each keys."
@@ -525,14 +536,23 @@
 
         :param kwargs: values of the column in the format column_name=value
         :return: the table with added row.
         """
         result = self + [{**kwargs}]
         return result.replace(replacement=None, to_replace=None)
 
+    def rbind(self, table: TupList):
+        """
+        Bind two tables by rows.
+
+        :param table: another table
+        :return: the complete table.
+        """
+        return (self + Table(table)).replace(replacement=None, to_replace=None)
+
     @staticmethod
     def format_dataset(dataset):
         """
         Format an entire data instance applying Table() to every table.
         Leave dict as they are.
 
         :param dataset: a data instance in dict/json format.
@@ -631,7 +651,19 @@
         """
         Create a table from a json file.
 
         :param path: path to json file
         :return: a Table containing the data.
         """
         return Table(load_json(path))
+
+    def apply(self, func: Callable, *args, **kwargs):
+        """
+        Apply a function to the entire table.
+        Useful to chain varius functions applied to the entire table.
+
+        :param func: a function which take the table as a first argument.
+        :param args: args of the function
+        :param kwargs: kwargs of the function
+        :return: what the function returns.
+        """
+        return func(self, *args, **kwargs)
```

### Comparing `mango-0.0.5/mango/table/pytups_tools.py` & `mango-0.0.6/mango/table/pytups_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,16 @@
      - a list with all the values of the column. ex: b=[4,5,6]
      - a function to apply to the row. ex: c=lambda v: v["a"]+v["b"]
     :return: a TupList
     """
     assert isinstance(table, TupList)
 
     if len(table) == 0:
-        print("Warning: applying mutate on an empty table")
+        # TODO: put that in a debug log
+        # print("Warning: applying mutate on an empty table")
         return table
 
     # Copy deep of table has been removed.
     table2 = table
 
     # Transform TupList in list of dict
     if isinstance(table2[0], tuple):
@@ -66,15 +67,15 @@
     :param group_by: name of the columns to group.
     :return: a table (TupList of dict)
     """
     assert isinstance(table, TupList)
     if len(table) == 0:
         return table
     if group_by is None:
-        group_by=[]
+        group_by = []
 
     return (
         table.to_dict(indices=group_by, result_col=None, is_list=True)
         .vapply(lambda v: invert_dict_list(v, unique=False))
         .vapply(lambda v: {k: sum(v[k]) if k not in group_by else v[k][0] for k in v})
         .values_tl()
     )
@@ -108,15 +109,15 @@
     :return: a table (TupList of dict).
     """
     assert isinstance(table, TupList)
     # todo: should it create an error?
     if len(table) == 0:
         return table
     if group_by is None:
-        group_by=[]
+        group_by = []
     if default is not None:
         apply_func = {k: default for k in table[0] if k not in group_by}
     else:
         apply_func = {}
     apply_func.update(dict(**func))
     return (
         table.to_dict(indices=group_by, result_col=None, is_list=True)
@@ -176,15 +177,16 @@
     :param table: a table
     :param args: names of the columns to select
     :return: a table (TupList) with the selected columns.
     """
     assert isinstance(table, TupList)
 
     if not len(table):
-        print("Warning: applying select on an empty table")
+        # TODO: put that in a debug log
+        # print("Warning: applying select on an empty table")
         return TupList()
 
     keep = as_list(args)
     missing = [k for k in keep if k not in get_col_names(table)]
     if len(missing):
         raise ValueError("Column %s not found" % missing)
     return table.vapply(lambda v: {k: v[k] for k in keep})
@@ -198,15 +200,15 @@
     :param args: names of the columns to drop
     :return: a table (TupList) without the selected columns.
     """
     assert isinstance(table, TupList)
 
     remove = as_list(args)
     keep = [k for k in get_col_names(table) if k not in remove]
-    return table.vapply(lambda v: {k: v[k] for k in keep})
+    return table.vapply(lambda v: {k: v[k] for k in keep if k in v})
 
 
 def rename(table, **kwargs):
     """
     Rename columns from a table
 
     :param table: a table
@@ -336,21 +338,59 @@
     elif jtype == "right":
         join_keys = [k for k in tab2.keys()]
     elif jtype == "inner":
         join_keys = [k for k in tab1.keys() if k in tab2.keys()]
     else:
         raise ValueError("jtype must be full, inner, right or left")
 
-    result = TupList(join_keys).unique2()
-    result.sort()
+    result = (
+        TupList(join_keys)
+        .vfilter(lambda v: all(i is not None for i in as_list(v)))
+        .unique2()
+        .sorted()
+    )
+    return result
+
+
+def manage_join_none(tab1, tab2, empty, t1_keys, t2_keys, by, jtype):
+    """
+    None values should never join with other None.
+    Depending on the type of join, return the relevant rows with None values in keys.
+    TODO: there should be a simpler way to do that.
+    :param tab1:
+    :param tab2:
+    :param empty:
+    :param t1_keys:
+    :param t2_keys:
+    :param by:
+    :param jtype:
+    :return:
+    """
+    result = []
+    if jtype == "left":
+        for i in tab1:
+            if any(v is None for v in as_list(i)):
+                tab2[i] = [{k: empty for k in t2_keys if k not in by}]
+                result += [{**d1, **d2} for d1 in tab1[i] for d2 in tab2[i]]
+    elif jtype == "right":
+        result = manage_join_none(tab2, tab1, empty, t2_keys, t1_keys, by, jtype="left")
+    elif jtype == "full":
+        result = manage_join_none(
+            tab1, tab2, empty, t1_keys, t2_keys, by, jtype="left"
+        ) + manage_join_none(tab1, tab2, empty, t1_keys, t2_keys, by, jtype="right")
+    elif jtype == "inner":
+        return TupList()
+    else:
+        raise ValueError("jtype must be full, inner, right or left")
+
     return result
 
 
 def join(
-    table1, table2, by=None, suffix=None, jtype="full", empty=None, drop_if_nested=True
+    table1, table2, by=None, suffix=None, jtype="full", empty=None, drop_if_nested=False
 ):
     """
     Join to tables.
     Inspired by R dplyr join functions.
 
     :param table1: 1st table (TupList with dict)
     :param table2: 2nd table (TupList with dict)
@@ -433,15 +473,17 @@
     for i in join_keys:
         if i not in tab1:
             tab1[i] = [{k: empty for k in t1_keys if k not in by}]
         if i not in tab2:
             tab2[i] = [{k: empty for k in t2_keys if k not in by}]
         result += [{**d1, **d2} for d1 in tab1[i] for d2 in tab2[i]]
 
-    return TupList(result)
+    return TupList(result) + manage_join_none(
+        tab1, tab2, empty, t1_keys, t2_keys, by, jtype
+    )
 
 
 def auto_join(table, by=None, suffix=None, empty=None):
     """
     Join a table with itself.
     Useful to create combinations of values from columns of a table.
 
@@ -483,26 +525,34 @@
 
     :param tl: a tuplist
     :param replacement: a single value or a dict of columns and values to use as replacement.
     :param to_replace: a single value or a dict of columns and values to replace.
 
     :return: a tuplist with missing values filled.
     """
-    if not isinstance(replacement, dict):
+    apply_to_col = []
+    if isinstance(replacement, dict):
+        apply_to_col += [i for i in replacement.keys()]
+    else:
         replacement = {k: replacement for k in get_col_names(tl)}
-    if to_replace is None or not isinstance(to_replace, dict):
+    if isinstance(to_replace, dict):
+        apply_to_col += [i for i in to_replace.keys()]
+    else:
         to_replace = {k: to_replace for k in get_col_names(tl)}
+    if not len(apply_to_col):
+        apply_to_col = get_col_names(tl)
+
     return TupList(
         [
             {
                 **replacement,
                 **{
                     k: v
                     for k, v in dic.items()
-                    if not k in to_replace or v != to_replace[k]
+                    if k not in apply_to_col or v != to_replace[k]
                 },
             }
             for dic in tl
         ]
     )
```

### Comparing `mango-0.0.5/mango/table/table_tools.py` & `mango-0.0.6/mango/table/table_tools.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/const.py` & `mango-0.0.6/mango/tests/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/data/json_dataset.json` & `mango-0.0.6/mango/tests/data/json_dataset.json`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/data/test.xlsx` & `mango-0.0.6/mango/tests/data/test.xlsx`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_arcgis_client.py` & `mango-0.0.6/mango/tests/test_arcgis_client.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_config.py` & `mango-0.0.6/mango/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_date_functions.py` & `mango-0.0.6/mango/tests/test_date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_file_functions.py` & `mango-0.0.6/mango/tests/test_file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_images.py` & `mango-0.0.6/mango/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_logging.py` & `mango-0.0.6/mango/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_models.py` & `mango-0.0.6/mango/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_object_functions.py` & `mango-0.0.6/mango/tests/test_object_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_processing_time_series.py` & `mango-0.0.6/mango/tests/test_processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_table.py` & `mango-0.0.6/mango/tests/test_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import io
 import numpy as np
 import pandas as pd
-from pytups import TupList
+from pytups import TupList, SuperDict
 from unittest import TestCase, mock
 from mango.table.pytups_table import Table
 from mango.table.table_tools import mean
 from mango.processing import row_number
 from mango.tests.const import normalize_path
 
 
@@ -93,14 +93,22 @@
         result = Table(self.default_data).take(["Name", "Age"])
         expected = TupList(
             [("Albert", 20), ("Bernard", 25), ("Charlie", 30), ("Daniel", 35)]
         )
         self.assertIsInstance(result, TupList, msg="take create a TupList")
         self.assertEqual(result, expected, msg="take works as expected")
 
+    def test_take_tup(self):
+        result = Table(self.default_data).take(("Name", "Age"))
+        expected = TupList(
+            [("Albert", 20), ("Bernard", 25), ("Charlie", 30), ("Daniel", 35)]
+        )
+        self.assertIsInstance(result, TupList, msg="take create a TupList")
+        self.assertEqual(result, expected, msg="take works as expected")
+
     def test_mutate_on_tuplist(self):
         msg = "mutate transform a list of tuple into a list of dict"
         result = Table([(1, 2), (3, 4), (5, 6)]).mutate(a=5)
         expected = [{0: 1, 1: 2, "a": 5}, {0: 3, 1: 4, "a": 5}, {0: 5, 1: 6, "a": 5}]
         self.assertEqual(result, expected, msg=msg)
 
     def test_mutate_constant(self):
@@ -240,17 +248,15 @@
         self.assertEqual(df, expected, msg=msg)
 
     def test_summarise_group_by_none(self):
         msg = "summarise with group_by = None"
         df = Table(self.default_data2).summarise(
             group_by=None, Points=sum, default=None
         )
-        expected = Table(
-            [{"Points": 23}]
-        )
+        expected = Table([{"Points": 23}])
         self.assertEqual(df, expected, msg=msg)
 
     def test_select(self):
         msg = "select 2 columns"
         df = Table(self.default_data2).select("Name", "Points")
         expected = Table(
             [
@@ -266,34 +272,38 @@
         msg = "unknown column raise error"
 
         def try_select():
             return Table(self.default_data2).select("unknown", "Points")
 
         self.assertRaises(ValueError, try_select)
 
-
     def test_select_empty(self):
         msg = "select on empty table return empty table"
         df = Table().select("Name")
         self.assertEqual(df, Table())
 
-
     def test_drop(self):
         msg = "drop 3 columns"
         df = Table(self.default_data2).drop("Under_25", "Points", "Male")
         expected = Table(
             [
                 {"Name": "Albert", "Age": 20},
                 {"Name": "Bernard", "Age": 25},
                 {"Name": "Charlie", "Age": 30},
                 {"Name": "Daniel", "Age": 35},
             ]
         )
         self.assertEqual(df, expected, msg=msg)
 
+    def test_drop_empty_table(self):
+        msg = "drop on empty table"
+        df = Table().drop("Under_25", "Points", "Male")
+
+        self.assertEqual(df, Table(), msg=msg)
+
     def test_rename(self):
         msg = "rename a column"
         col_names = Table(self.default_data2).rename(Points="Value").get_col_names()
         expected = ["Name", "Age", "Male", "Value", "Under_25"]
         self.assertEqual(col_names, expected, msg=msg)
 
     def test_join_jtype_left(self):
@@ -311,15 +321,15 @@
         self.assertEqual(df, expected, msg=msg)
 
     def test_join_wrong_jtype(self):
         msg = "wrong jtype creates an error"
         df_id = Table(self.df_id)
 
         def try_join():
-            return  Table(self.default_data2).join(df_id, jtype="up")
+            return Table(self.default_data2).join(df_id, jtype="up")
 
         self.assertRaises(ValueError, try_join)
 
     def test_left_join(self):
         msg = "left join with other table"
         df_id = Table(self.df_id)
         df = Table(self.default_data2).left_join(df_id).select("Name", "Id")
@@ -346,15 +356,15 @@
     def test_left_join_wrong_by(self):
         msg = "error when left join with wrong by value"
         df_id = Table(self.df_id)
 
         def try_left_join():
             return Table(self.default_data2).left_join(df_id, by="Id")
 
-        self.assertRaises(ValueError,try_left_join)
+        self.assertRaises(ValueError, try_left_join)
 
     def test_left_join2(self):
         msg = "left join with a repeated value"
         df_id = Table(self.df_id + [{"Name": "Albert", "Id": 5}])
         df = Table(self.default_data2).left_join(df_id).select("Name", "Id")
         expected = Table(
             [
@@ -396,16 +406,36 @@
                 {"Name": "Bernard", "Id": 2},
                 {"Name": "Charlie", "Id": 3},
                 {"Name": "Daniel", "Id": 0},
             ]
         )
         self.assertEqual(df, expected, msg=msg)
 
+    def test_left_join_none(self):
+        msg = "left join with None values as keys"
+        df_id = Table(self.df_id).add_row(Name=None, Id=5)
+        df = (
+            Table(self.default_data2)
+            .add_row(Name=None)
+            .left_join(df_id, by="Name")
+            .select("Name", "Id")
+        )
+        expected = Table(
+            [
+                {"Name": "Albert", "Id": 1},
+                {"Name": "Bernard", "Id": 2},
+                {"Name": "Charlie", "Id": 3},
+                {"Name": "Daniel", "Id": None},
+                {"Name": None, "Id": None},
+            ]
+        )
+        self.assertEqual(expected, df, msg=msg)
+
     def test_right_join(self):
-        msg = "right join with toher table"
+        msg = "right join with other table"
         df_id = Table(self.df_id)
         df = Table(self.default_data2).right_join(df_id).select("Name", "Id")
         expected = Table(
             [
                 {"Name": "Albert", "Id": 1},
                 {"Name": "Bernard", "Id": 2},
                 {"Name": "Charlie", "Id": 3},
@@ -561,26 +591,65 @@
             {"Name": "Bernard", "Age": 25},
             {"Name": "Charlie", "Age": 30},
             {"Name": "Daniel", "Age": 35},
         ]
         self.assertEqual(result, expected, msg=msg)
 
     def test_replace_empty(self):
-        msg = "replace missing values with 0 with repalce_empty"
+        msg = "replace missing values with 0 with replace_empty"
         table = Table(self.default_data) + [{"Name": "Elisa"}]
         result = table.replace_empty(0)
         expected = [
             {"Name": "Albert", "Age": 20},
             {"Name": "Bernard", "Age": 25},
             {"Name": "Charlie", "Age": 30},
             {"Name": "Daniel", "Age": 35},
             {"Name": "Elisa", "Age": 0},
         ]
         self.assertEqual(result, expected, msg=msg)
 
+    def test_replace_empty_dict(self):
+        msg = "replace missing values on selected columns with replace_empty"
+        table = Table(self.default_data) + [{}]
+        result = table.replace_empty({"Name": "Elisa"})
+        expected = [
+            {"Name": "Albert", "Age": 20},
+            {"Name": "Bernard", "Age": 25},
+            {"Name": "Charlie", "Age": 30},
+            {"Name": "Daniel", "Age": 35},
+            {"Name": "Elisa"},
+        ]
+        self.assertEqual(result, expected, msg=msg)
+
+    def test_replace_empty_dict2(self):
+        msg = "replace missing values on selected columns with replace_empty"
+        table = Table(self.default_data) + [{}]
+        result = table.replace_empty({"Name": "Elisa", "Age": 5})
+        expected = [
+            {"Name": "Albert", "Age": 20},
+            {"Name": "Bernard", "Age": 25},
+            {"Name": "Charlie", "Age": 30},
+            {"Name": "Daniel", "Age": 35},
+            {"Name": "Elisa", "Age": 5},
+        ]
+        self.assertEqual(result, expected, msg=msg)
+
+    def test_replace_empty_dict3(self):
+        msg = "replace missing values on selected columns with replace_empty"
+        table = Table(self.default_data) + [{"Name": None, "Age": None}]
+        result = table.replace_empty({"Name": "Elisa"})
+        expected = [
+            {"Name": "Albert", "Age": 20},
+            {"Name": "Bernard", "Age": 25},
+            {"Name": "Charlie", "Age": 30},
+            {"Name": "Daniel", "Age": 35},
+            {"Name": "Elisa", "Age": None},
+        ]
+        self.assertEqual(result, expected, msg=msg)
+
     def test_replace_nan(self):
         msg = "replace nan with 0 with repalce_nan"
         table = Table(self.default_data) + [{"Name": "Elisa", "Age": np.nan}]
         result = table.replace_nan(0)
         expected = [
             {"Name": "Albert", "Age": 20},
             {"Name": "Bernard", "Age": 25},
@@ -926,14 +995,28 @@
             {"Name": "Bernard", "Age": 25},
             {"Name": "Charlie", "Age": 30},
             {"Name": "Daniel", "Age": 35},
             {"Name": "new", "Age": None},
         ]
         self.assertEqual(table2, expected, msg=msg)
 
+    def test_add_row_empty(self):
+        msg = "add an empty row with add_row"
+        table = Table(self.default_data)
+        table2 = table.add_row()
+
+        expected = [
+            {"Name": "Albert", "Age": 20},
+            {"Name": "Bernard", "Age": 25},
+            {"Name": "Charlie", "Age": 30},
+            {"Name": "Daniel", "Age": 35},
+            {"Name": None, "Age": None},
+        ]
+        self.assertEqual(table2, expected, msg=msg)
+
     def test_sorted_exception(self):
         msg = "sorted raise error"
         table = Table(self.default_data)
 
         def sort_table():
             return table.sorted()
 
@@ -959,31 +1042,31 @@
     def test_peek_high_n(self):
         msg = "if n is higher than len/3, print the entire table"
         table = Table(self.default_data)
 
         def try_peek():
             return table.peek(3)
 
-        expected =(
-        "Table (4 rows, 2 columns):\n"
-        "0 {'Name': 'Albert', 'Age': 20}\n"
-        "1 {'Name': 'Bernard', 'Age': 25}\n"
-        "2 {'Name': 'Charlie', 'Age': 30}\n"
-        "3 {'Name': 'Daniel', 'Age': 35}\n\n"
+        expected = (
+            "Table (4 rows, 2 columns):\n"
+            "0 {'Name': 'Albert', 'Age': 20}\n"
+            "1 {'Name': 'Bernard', 'Age': 25}\n"
+            "2 {'Name': 'Charlie', 'Age': 30}\n"
+            "3 {'Name': 'Daniel', 'Age': 35}\n\n"
         )
         self.assertStdout(try_peek, expected, msg=msg)
 
     def test_peek_empty(self):
         msg = "peek on empty table"
         table = Table()
 
         def try_peek():
             return table.peek(3)
 
-        expected ="Empty table\n"
+        expected = "Empty table\n"
         self.assertStdout(try_peek, expected, msg=msg)
 
     def test_print(self):
         msg = "print a table"
         table = Table(self.default_data)
 
         def try_print():
@@ -996,36 +1079,36 @@
             "2 {'Name': 'Charlie', 'Age': 30}\n"
             "3 {'Name': 'Daniel', 'Age': 35}\n\n"
         )
         self.assertStdout(try_print, expected, msg=msg)
 
     def test_print_list(self):
         msg = "print a table"
-        table = Table([1,2,3])
+        table = Table([1, 2, 3])
 
         def try_print():
             print(table)
 
         expected = "[1, 2, 3]\n"
         self.assertStdout(try_print, expected, msg=msg)
 
     def test_show_row(self):
-        msg="show row show one row if n2=None"
+        msg = "show row show one row if n2=None"
         table = Table(self.default_data)
-        result=table.show_rows(1)
-        expected="1 {'Name': 'Bernard', 'Age': 25}\n"
+        result = table.show_rows(1)
+        expected = "1 {'Name': 'Bernard', 'Age': 25}\n"
         self.assertEqual(result, expected, msg)
 
     def test_head(self):
         msg = "head(2) return the two first rows"
         table = Table(self.default_data)
         result = table.head(2)
         expected = [{"Name": "Albert", "Age": 20}, {"Name": "Bernard", "Age": 25}]
         self.assertEqual(result, expected, msg=msg)
-        msg2="head return the entire table if n > len(table)"
+        msg2 = "head return the entire table if n > len(table)"
         self.assertEqual(table.head(100), table, msg=msg2)
 
     def test_group_by(self):
         msg = "group_by create a dict of lists"
         result = Table(self.default_data2).group_by("Under_25")
         expected = {
             True: [
@@ -1108,14 +1191,18 @@
                 ["Male", "Under_25"], "Name", is_list=False
             )
 
         self.assertEqual(result1, expected1, msg=msg1)
         self.assertEqual(result2, expected2, msg=msg2)
         self.assertRaises(ValueError, to_param_error)
 
+    def test_to_param_empty(self):
+        msg = "to_param on empty table return empty dict"
+        self.assertEqual(Table().to_param("Name", "Points"), SuperDict(), msg=msg)
+
     def test_is_unique_true(self):
         msg = "is_unique returns True if all values of the column are unique"
         result = Table(self.default_data2).is_unique("Name")
         self.assertTrue(result, msg=msg)
 
     def test_is_unique_false(self):
         msg = "is_unique returns False if some values of the column are repeated"
@@ -1167,7 +1254,13 @@
 
     def test_dataset_from_json(self):
         msg = "dataset_from_json creates a dict of Tables from a json file"
         path = normalize_path("./data/json_dataset.json")
         result = Table.dataset_from_json(path)
         expected = dict(t1=Table(self.default_data), t2=Table(self.default_data2))
         self.assertEqual(result, expected, msg=msg)
+
+    def test_apply(self):
+        msg = "apply a function to a table"
+        result = Table(self.default_data2).apply(len)
+        expected = len(Table(self.default_data2))
+        self.assertEqual(result, expected, msg=msg)
```

### Comparing `mango-0.0.5/mango/tests/test_tools.py` & `mango-0.0.6/mango/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango/tests/test_validation.py` & `mango-0.0.6/mango/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/mango.egg-info/PKG-INFO` & `mango-0.0.6/mango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
```

### Comparing `mango-0.0.5/mango.egg-info/SOURCES.txt` & `mango-0.0.6/mango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mango-0.0.5/setup.py` & `mango-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "xlsxwriter",
     ],
 }
 
 
 setuptools.setup(
     name="mango",
-    version="0.0.5",
+    version="0.0.6",
     author="baobab soluciones",
     author_email="sistemas@baobabsoluciones.es",
     description="Library with a collection of useful classes and methods to DRY",
     long_description=long_description,
     url="https://github.com/baobabsoluciones/mango",
     packages=setuptools.find_packages(),
     classifiers=[
```

