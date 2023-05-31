# Comparing `tmp/pysat-3.0.6.tar.gz` & `tmp/pysat-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysat-3.0.6.tar", last modified: Thu Dec 22 05:57:20 2022, max compression
+gzip compressed data, was "pysat-3.1.0.tar", last modified: Wed May 31 21:18:03 2023, max compression
```

## Comparing `pysat-3.0.6.tar` & `pysat-3.1.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.795657 pysat-3.0.6/
--rw-r--r--   0 russellstoneback   (501) staff       (20)    44106 2022-12-21 19:02:35.000000 pysat-3.0.6/CHANGELOG.md
--rw-r--r--   0 russellstoneback   (501) staff       (20)     3223 2020-06-26 22:48:53.000000 pysat-3.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 russellstoneback   (501) staff       (20)     5812 2022-12-21 00:14:32.000000 pysat-3.0.6/CONTRIBUTING.md
--rw-r--r--   0 russellstoneback   (501) staff       (20)     1481 2020-06-26 22:48:53.000000 pysat-3.0.6/LICENSE
--rw-r--r--   0 russellstoneback   (501) staff       (20)      169 2021-09-24 16:04:15.000000 pysat-3.0.6/MANIFEST.in
--rw-r--r--   0 russellstoneback   (501) staff       (20)     5507 2022-12-22 05:57:20.795797 pysat-3.0.6/PKG-INFO
--rw-r--r--   0 russellstoneback   (501) staff       (20)     4337 2022-08-26 16:25:34.000000 pysat-3.0.6/README.md
--rw-r--r--   0 russellstoneback   (501) staff       (20)      120 2022-12-21 00:14:32.000000 pysat-3.0.6/ecosystem.txt
--rw-r--r--   0 russellstoneback   (501) staff       (20)     7570 2020-04-30 21:46:38.000000 pysat-3.0.6/nrl_sami.py
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.778888 pysat-3.0.6/pysat/
--rw-r--r--   0 russellstoneback   (501) staff       (20)     4433 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/__init__.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    29097 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/_constellation.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    40190 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/_files.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)   156591 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/_instrument.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    79796 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/_meta.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    46337 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/_orbits.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    11794 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/_params.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)      113 2021-09-24 16:04:15.000000 pysat-3.0.6/pysat/citation.txt
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.781134 pysat-3.0.6/pysat/constellations/
--rw-r--r--   0 russellstoneback   (501) staff       (20)      313 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/constellations/__init__.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)      279 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/constellations/single_test.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)      796 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/constellations/testing.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)      148 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/constellations/testing_empty.py
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.783526 pysat-3.0.6/pysat/instruments/
--rw-r--r--   0 russellstoneback   (501) staff       (20)      421 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/instruments/__init__.py
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.784278 pysat-3.0.6/pysat/instruments/methods/
--rw-r--r--   0 russellstoneback   (501) staff       (20)      263 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/instruments/methods/__init__.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    10589 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/instruments/methods/general.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    23922 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/instruments/methods/testing.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     7776 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/instruments/pysat_ndtesting.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    10045 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/instruments/pysat_netcdf.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     7231 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/instruments/pysat_testing.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     8826 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/instruments/pysat_testing2d.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     1789 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/instruments/pysat_testing2d_xarray.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     7841 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/instruments/pysat_testing_xarray.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     9226 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/instruments/pysat_testmodel.py
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.784805 pysat-3.0.6/pysat/instruments/templates/
--rw-r--r--   0 russellstoneback   (501) staff       (20)      266 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/instruments/templates/__init__.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    15192 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/instruments/templates/template_instrument.py
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.791585 pysat-3.0.6/pysat/tests/
--rw-r--r--   0 russellstoneback   (501) staff       (20)      352 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/tests/__init__.py
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.793385 pysat-3.0.6/pysat/tests/classes/
--rw-r--r--   0 russellstoneback   (501) staff       (20)     1944 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/classes/cls_ci.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    41418 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/tests/classes/cls_instrument_access.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     2396 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/tests/classes/cls_instrument_integration.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    38324 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/tests/classes/cls_instrument_iteration.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    15199 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/classes/cls_instrument_library.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    28945 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/tests/classes/cls_instrument_property.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     5381 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/classes/cls_registration.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     2775 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/tests/instrument_test_class.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    15509 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_constellation.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    53819 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_files.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    22047 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_instrument.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    17556 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_instrument_custom.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     2482 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_instrument_index.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     1940 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_instrument_listgen.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    24232 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_instrument_padding.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     8673 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_instruments.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    90597 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_meta.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     4102 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_meta_header.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     7812 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_meta_labels.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    11603 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_methods_general.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     2976 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_methods_testing.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    40334 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_orbits.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     8533 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_params.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    12081 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_registry.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    24997 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_utils.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    12088 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_utils_coords.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    17479 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_utils_files.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    71468 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_utils_io.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     9937 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_utils_testing.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    12058 2022-12-21 00:14:32.000000 pysat-3.0.6/pysat/tests/test_utils_time.py
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.795454 pysat-3.0.6/pysat/utils/
--rw-r--r--   0 russellstoneback   (501) staff       (20)      960 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/utils/__init__.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    27036 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/utils/_core.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     6619 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/utils/coords.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    35281 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/utils/files.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    87668 2022-12-21 19:02:35.000000 pysat-3.0.6/pysat/utils/io.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    10561 2022-09-29 19:57:21.000000 pysat-3.0.6/pysat/utils/registry.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)     6781 2022-07-15 15:36:54.000000 pysat-3.0.6/pysat/utils/testing.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)    11071 2022-07-13 21:04:58.000000 pysat-3.0.6/pysat/utils/time.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)        6 2022-12-21 19:09:54.000000 pysat-3.0.6/pysat/version.txt
-drwxr-xr-x   0 russellstoneback   (501) staff       (20)        0 2022-12-22 05:57:20.780204 pysat-3.0.6/pysat.egg-info/
--rw-r--r--   0 russellstoneback   (501) staff       (20)     5507 2022-12-22 05:57:20.000000 pysat-3.0.6/pysat.egg-info/PKG-INFO
--rw-r--r--   0 russellstoneback   (501) staff       (20)     2381 2022-12-22 05:57:20.000000 pysat-3.0.6/pysat.egg-info/SOURCES.txt
--rw-r--r--   0 russellstoneback   (501) staff       (20)        1 2022-12-22 05:57:20.000000 pysat-3.0.6/pysat.egg-info/dependency_links.txt
--rw-r--r--   0 russellstoneback   (501) staff       (20)        1 2021-04-06 19:46:06.000000 pysat-3.0.6/pysat.egg-info/not-zip-safe
--rw-r--r--   0 russellstoneback   (501) staff       (20)       64 2022-12-22 05:57:20.000000 pysat-3.0.6/pysat.egg-info/requires.txt
--rw-r--r--   0 russellstoneback   (501) staff       (20)        6 2022-12-22 05:57:20.000000 pysat-3.0.6/pysat.egg-info/top_level.txt
--rw-r--r--   0 russellstoneback   (501) staff       (20)       70 2022-08-31 20:25:20.000000 pysat-3.0.6/requirements.txt
--rw-r--r--   0 russellstoneback   (501) staff       (20)     1854 2022-12-22 05:57:20.796443 pysat-3.0.6/setup.cfg
--rw-r--r--   0 russellstoneback   (501) staff       (20)      318 2022-07-13 21:04:58.000000 pysat-3.0.6/setup.py
--rw-r--r--   0 russellstoneback   (501) staff       (20)      143 2022-07-13 21:04:58.000000 pysat-3.0.6/test_requirements.txt
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.938216 pysat-3.1.0/
+-rw-r--r--   0 jklenzin   (502) staff       (20)    48478 2023-05-31 21:10:16.000000 pysat-3.1.0/CHANGELOG.md
+-rw-r--r--   0 jklenzin   (502) staff       (20)     3223 2021-12-28 00:22:47.000000 pysat-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jklenzin   (502) staff       (20)     6253 2023-05-31 20:13:05.000000 pysat-3.1.0/CONTRIBUTING.md
+-rw-r--r--   0 jklenzin   (502) staff       (20)     1481 2021-12-28 00:22:47.000000 pysat-3.1.0/LICENSE
+-rw-r--r--   0 jklenzin   (502) staff       (20)      169 2021-12-28 00:22:47.000000 pysat-3.1.0/MANIFEST.in
+-rw-r--r--   0 jklenzin   (502) staff       (20)     5544 2023-05-31 21:18:03.938487 pysat-3.1.0/PKG-INFO
+-rw-r--r--   0 jklenzin   (502) staff       (20)     4337 2023-04-13 12:01:47.000000 pysat-3.1.0/README.md
+-rw-r--r--   0 jklenzin   (502) staff       (20)      120 2023-04-13 12:01:47.000000 pysat-3.1.0/ecosystem.txt
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.849130 pysat-3.1.0/pysat/
+-rw-r--r--   0 jklenzin   (502) staff       (20)     4433 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/__init__.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    39272 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/_constellation.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    40190 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/_files.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)   167033 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/_instrument.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    84223 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/_meta.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    46337 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/_orbits.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    11794 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/_params.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)      113 2021-12-28 00:22:47.000000 pysat-3.1.0/pysat/citation.txt
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.857115 pysat-3.1.0/pysat/constellations/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      332 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/constellations/__init__.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)      295 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/constellations/single_test.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)      653 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/constellations/testing.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)      148 2023-04-07 18:02:19.000000 pysat-3.1.0/pysat/constellations/testing_empty.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)      451 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/constellations/testing_partial.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.863744 pysat-3.1.0/pysat/instruments/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      421 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/instruments/__init__.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.865985 pysat-3.1.0/pysat/instruments/methods/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      263 2023-04-07 18:02:19.000000 pysat-3.1.0/pysat/instruments/methods/__init__.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    10695 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/instruments/methods/general.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    26161 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/instruments/methods/testing.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     8237 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/instruments/pysat_ndtesting.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     9695 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/instruments/pysat_netcdf.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     7931 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/instruments/pysat_testing.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     8734 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/instruments/pysat_testing2d.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     1789 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/instruments/pysat_testing2d_xarray.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     8322 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/instruments/pysat_testing_xarray.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     9411 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/instruments/pysat_testmodel.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.867617 pysat-3.1.0/pysat/instruments/templates/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      266 2023-04-07 18:02:19.000000 pysat-3.1.0/pysat/instruments/templates/__init__.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    15191 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/instruments/templates/template_instrument.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.902437 pysat-3.1.0/pysat/tests/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      352 2023-04-07 18:02:19.000000 pysat-3.1.0/pysat/tests/__init__.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.929051 pysat-3.1.0/pysat/tests/classes/
+-rw-r--r--   0 jklenzin   (502) staff       (20)     1944 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/classes/cls_ci.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    42794 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/classes/cls_instrument_access.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     2529 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/classes/cls_instrument_integration.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    34072 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/classes/cls_instrument_iteration.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    15804 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/classes/cls_instrument_library.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    29748 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/classes/cls_instrument_property.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     5381 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/classes/cls_registration.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     2775 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/instrument_test_class.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    22033 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_constellation.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    53859 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_files.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    32518 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_instrument.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    17556 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_instrument_custom.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     4743 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_instrument_index.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     1940 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_instrument_listgen.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    30830 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_instrument_padding.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     8673 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_instruments.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    90946 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_meta.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     4102 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_meta_header.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     7812 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_meta_labels.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    11603 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_methods_general.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     2976 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_methods_testing.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    40334 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_orbits.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     8533 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_params.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    12081 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_registry.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    30687 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_utils.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    22546 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_utils_coords.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    17817 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_utils_files.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    76024 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/tests/test_utils_io.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     9937 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_utils_testing.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    12058 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/tests/test_utils_time.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.937414 pysat-3.1.0/pysat/utils/
+-rw-r--r--   0 jklenzin   (502) staff       (20)     1009 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/utils/__init__.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    29058 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/utils/_core.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    12707 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/utils/coords.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    36169 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/utils/files.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    89782 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/utils/io.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    10561 2023-04-13 12:01:47.000000 pysat-3.1.0/pysat/utils/registry.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     6847 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/utils/testing.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    11071 2023-04-07 18:02:19.000000 pysat-3.1.0/pysat/utils/time.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)        6 2023-05-31 20:13:05.000000 pysat-3.1.0/pysat/version.txt
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-05-31 21:18:03.852399 pysat-3.1.0/pysat.egg-info/
+-rw-r--r--   0 jklenzin   (502) staff       (20)     5544 2023-05-31 21:18:03.000000 pysat-3.1.0/pysat.egg-info/PKG-INFO
+-rw-r--r--   0 jklenzin   (502) staff       (20)     2409 2023-05-31 21:18:03.000000 pysat-3.1.0/pysat.egg-info/SOURCES.txt
+-rw-r--r--   0 jklenzin   (502) staff       (20)        1 2023-05-31 21:18:03.000000 pysat-3.1.0/pysat.egg-info/dependency_links.txt
+-rw-r--r--   0 jklenzin   (502) staff       (20)        1 2021-12-28 00:22:59.000000 pysat-3.1.0/pysat.egg-info/not-zip-safe
+-rw-r--r--   0 jklenzin   (502) staff       (20)       64 2023-05-31 21:18:03.000000 pysat-3.1.0/pysat.egg-info/requires.txt
+-rw-r--r--   0 jklenzin   (502) staff       (20)        6 2023-05-31 21:18:03.000000 pysat-3.1.0/pysat.egg-info/top_level.txt
+-rw-r--r--   0 jklenzin   (502) staff       (20)       70 2023-04-13 12:01:47.000000 pysat-3.1.0/requirements.txt
+-rw-r--r--   0 jklenzin   (502) staff       (20)     1854 2023-05-31 21:18:03.940436 pysat-3.1.0/setup.cfg
+-rw-r--r--   0 jklenzin   (502) staff       (20)      318 2023-04-07 18:02:19.000000 pysat-3.1.0/setup.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)      152 2023-05-31 20:13:05.000000 pysat-3.1.0/test_requirements.txt
```

### Comparing `pysat-3.0.6/CHANGELOG.md` & `pysat-3.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,86 @@
 Change Log
 ==========
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](https://semver.org/).
 
+[3.1.0] - 2023-06-02
+--------------------
+* New Features
+  * Added a utility to ensure two xarray Datasets can be concatonated, and
+    incorporated this utility into the Instrument file loading
+  * Added unit tests for different file cadences in the Instrument class
+  * Added `to_inst` method to the Constellation class
+  * Added `export_pysat_info` kwarg to `to_netcdf` routines to select whether
+    pysat instrument info is written to files
+  * Added Constellation class examples to the docs tutorial
+  * Added links to the project standards repository to the docs
+  * Improved formatting of custom kwargs when running `print` on an instrument
+  * Added a core utility to update fill values consistently in the data and
+    metadata
+  * Adapted `check_and_make_path` to treat an empty path as the current dir
+  * Added `meta_kwargs` attribute and kwarg to Instrument, allowing full custom
+    specification of the Meta class on instantiation
+  * Expanded MetaLabels type defaults for 'max_val', 'min_val', and 'fill_val'
+    to include more common data types
+  * Added `data_types` input to Meta and certain MetaLabels methods, allowing
+    the default values to be set to the specified data type when multiple types
+    are allowed, ensure these are updated when adding new data to an Instrument
+  * Added `_update_label_types` to MetaLabels, expanding the Python float/int
+    types to include all numpy float/int types
+  * Added `strict_dim_check` for loading xarray Datasets through netCDF
+  * Added `combine_by_coords` kwarg to `io.load_netcdf` for use on multi-file
+    xarray Datasets
+* Deprecations
+  * Deprecated the Instrument kwarg `labels` in favor of `meta_kwargs` and
+    replaced the `meta_labels` attribute with the `meta_kwargs` attribute
+  * Deprecated the `labels` keyword arg in favor of `meta_kwargs` in the
+    netCDF I/O functions and Instrument sub-module
+  * Deprecated the `malformed_index` kwarg in the test instruments.  This is
+    replaced by `non_monotonic_index` and `non_unique_index`
+* Bug Fix
+  * Allow `pysat.instruments.methods.general.list_files` to handle file
+    cadences other than daily or monthly
+  * Allow equality assessments if optional kwargs are used in Instrument
+  * Fixed an issue with setting single variables in xarray coords (#988)
+  * Fixed `pysat.Instrument.bounds` to handle all input types for `step`
+    and `width` regardless of `start` and `stop` time. Also fixed
+    seasonal bounds specified using file names.
+  * Fixed `pysat.utils.io.apply_table_translation_to_file` check for duplicates
+    in the meta translation table
+  * Fixed an issue when passing dates through load_remote_files (#1022)
+  * Fixed a bug where data may not have any times, but still not be empty
+  * Fixed a bug where metadata with values of None are assigned as useful
+    attributes when attaching metadata to xarray objects
+  * Fixed a bug where a multi_file_day non-monotonic xarray index failed to
+    merge datasets (#1005)
+  * Fixed a bug in testing for setting multiple optional load kwargs (#1097)
+  * Fixed a bug when setting xarray data as a tuple
+  * Fixed a bug when loading constellations for partially empty instrument lists
+  * Fixed a bug when cleaning up temporary directories on windows during testing
+  * Fixed a bug in Instrument loading with a pad, where RangeIndex slicing no
+    longer works on an empty series
+* Maintenance
+  * Added roadmap to readthedocs
+  * Improved the documentation in `pysat.utils.files`
+  * Clarified documentation and tests for name slicing support in pandas
+  * Clarified documentation for adding new instruments
+  * Fixed broken links in docs
+  * Updated docstring header underline lengths and addressed documentation
+    build errors and warnings
+  * Additional unit tests for data padding when a data index is non-monotonic.
+  * Deprecated the `malformed_index` kwarg in the test instruments.  This is
+    replaced by `non_monotonic_index` and `non_unique_index`
+  * Set the `instruments.pysat_testing` tag='no_download' to return an empty
+    pandas DataFrame for `load`
+  * Added `constellations.testing_partial`, which loads a partially empty
+    constellation dataset
+  * Reduced default num_samples for constellation test objects
+  * Improved consistency in metadata for test instruments
+
 [3.0.6] - 2022-12-21
 --------------------
 * Bug Fix
   * Ensure pysat tests do not store temporary directory to file
   * Updated links for supported instruments in documentation
 * Deprecations
   * `pysat_testing2d_xarray` instrument deprecated and replaced by
@@ -222,14 +296,15 @@
    * Added a cap on coveralls to ensure success of continuous integration
    * Updated tests in `test_meta` to search all warnings, not just the first
    * Updated pandas syntax to be compatible with pandas 2.0 (pandas 1.4
      deprecations)
    * Cleaned up excess variables upon import
    * Removed `data_path` check from `pysat.instruments.methods.general.list_files`
    * Compatible with netCDF v1.6.0
+   * Updated default labels in load_netcdf routines to match core pysat metadata
 
 [3.0.1] - 2021-07-28
 --------------------
 * New Features
    * Added a routine for loading CSV files into a pandas DataFrame from a list
      of filenames.
    * Added check for supported `tag` and `inst_id` at pysat.Instrument
```

### Comparing `pysat-3.0.6/CODE_OF_CONDUCT.md` & `pysat-3.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/CONTRIBUTING.md` & `pysat-3.1.0/CONTRIBUTING.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 in the 'About' section of the
 [pysat GitHub Repository.](https://github.com/pysat/pysat) Development meetings
 are generally held fortnightly.
 
 Short version
 -------------
 
-* Submit bug reports and feature requests at [GitHub](https://github.com/pysat/pysat/issues)
+* Submit bug reports and feature requests at
+  [GitHub](https://github.com/pysat/pysat/issues)
 
 * Make pull requests to the ``develop`` branch
 
 Bug reports
 -----------
 
 When [reporting a bug](https://github.com/pysat/pysat/issues) please
@@ -156,7 +157,18 @@
 * Provide testing class methods with informative failure statements and
   descriptive, one-line docstrings
 * Block and inline comments should use proper English grammar and punctuation
   with the exception of single sentences in a block, which may then omit the
   final period
 * When casting is necessary, use `np.int64` and `np.float64` to ensure operating
   system agnosticism
+
+
+Ecosystem Style Guidelines
+--------------------------
+
+If you are creating a new project that you wish to incorporate into the pysat
+ecosystem: welcome!  We have a
+[template repository](https://github.com/pysat/pysatEcosystem_Template) that
+contains many of the common documents needed for a new project that you can use
+to get started. You may find this helpful when getting started, though this
+repository is under active development.
```

### Comparing `pysat-3.0.6/LICENSE` & `pysat-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/PKG-INFO` & `pysat-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pysat
-Version: 3.0.6
+Version: 3.1.0
 Summary: 'Supports science analysis across disparate data platforms'
 Home-page: https://github.com/pysat/pysat
 Author: Russell Stoneback, et al.
 Author-email: pysat.developers@gmail.com
+License: UNKNOWN
 Keywords: pysat,ionosphere,atmosphere,thermosphere,magnetosphere,heliosphere,observations,models,space,satellites,analysis
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -115,7 +117,9 @@
   * xarray
 * The first time the package is run, you will need to specify a directory to
   store data. In python, run:
 ```
 pysat.params['data_dirs'] = 'path/to/directory/that/may/or/may/not/exist'
 ```
   * Nominal organization of data is top_dir/platform/name/tag/inst_id/files
+
+
```

### Comparing `pysat-3.0.6/README.md` & `pysat-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/__init__.py` & `pysat-3.1.0/pysat/__init__.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/_constellation.py` & `pysat-3.1.0/pysat/_constellation.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 Updated by AGB, May 2021, NRL
 
 """
 
 import datetime as dt
 import numpy as np
 import pandas as pds
+import xarray as xr
 
 import pysat
+from pysat.utils.coords import establish_common_coord
 
 
 class Constellation(object):
     """Manage and analyze data from multiple pysat Instruments.
 
     Parameters
     ----------
@@ -420,49 +422,50 @@
             cindex = pds.Index([])
         else:
             stime = None
             etime = None
             out_res = None
 
             for inst in self.instruments:
-                if stime is None:
-                    # Initialize the start and stop time
-                    stime = inst.index[0]
-                    etime = inst.index[-1]
-
-                    # If desired, determine the resolution
-                    if self.index_res is None:
-                        if inst.index.freq is None:
-                            out_res = pysat.utils.time.calc_res(inst.index)
-                        else:
-                            out_res = pysat.utils.time.freq_to_res(
-                                inst.index.freq)
-                else:
-                    # Adjust the start and stop time as appropriate
-                    if self.common_index:
-                        if stime < inst.index[0]:
-                            stime = inst.index[0]
-                        if etime > inst.index[-1]:
-                            etime = inst.index[-1]
+                if len(inst.index) > 0:
+                    if stime is None:
+                        # Initialize the start and stop time
+                        stime = inst.index[0]
+                        etime = inst.index[-1]
+
+                        # If desired, determine the resolution
+                        if self.index_res is None:
+                            if inst.index.freq is None:
+                                out_res = pysat.utils.time.calc_res(inst.index)
+                            else:
+                                out_res = pysat.utils.time.freq_to_res(
+                                    inst.index.freq)
                     else:
-                        if stime > inst.index[0]:
-                            stime = inst.index[0]
-                        if etime < inst.index[-1]:
-                            etime = inst.index[-1]
-
-                    # If desired, determine the resolution
-                    if self.index_res is None:
-                        if inst.index.freq is None:
-                            new_res = pysat.utils.time.calc_res(inst.index)
+                        # Adjust the start and stop time as appropriate
+                        if self.common_index:
+                            if stime < inst.index[0]:
+                                stime = inst.index[0]
+                            if etime > inst.index[-1]:
+                                etime = inst.index[-1]
                         else:
-                            new_res = pysat.utils.time.freq_to_res(
-                                inst.index.freq)
+                            if stime > inst.index[0]:
+                                stime = inst.index[0]
+                            if etime < inst.index[-1]:
+                                etime = inst.index[-1]
+
+                        # If desired, determine the resolution
+                        if self.index_res is None:
+                            if inst.index.freq is None:
+                                new_res = pysat.utils.time.calc_res(inst.index)
+                            else:
+                                new_res = pysat.utils.time.freq_to_res(
+                                    inst.index.freq)
 
-                        if new_res < out_res:
-                            out_res = new_res
+                            if new_res < out_res:
+                                out_res = new_res
 
             # If a resolution in seconds was supplied, calculate the frequency
             if self.index_res is not None:
                 out_res = pds.DateOffset(seconds=self.index_res)
             else:
                 out_res = pds.DateOffset(seconds=out_res)
 
@@ -615,14 +618,214 @@
 
     @property
     def index(self):
         """Obtain time index of loaded data."""
 
         return self._index()
 
+    def to_inst(self, common_coord=True, fill_method=None):
+        """Combine Constellation data into an Instrument.
+
+        Parameters
+        ----------
+        common_coord : bool
+            For Constellations with any xarray.Dataset Instruments, True to
+            include locations where all coordinate arrays cover, False to use
+            the maximum location range from the list of coordinates
+            (default=True)
+        fill_method : str or NoneType
+            Fill method if common data coordinates do not match exactly. If
+            one of 'nearest', 'pad'/'ffill', 'backfill'/'bfill', or None then
+            no interpolation will occur.  If 'linear', 'zero', 'slinear',
+            'quadratic', 'cubic', or 'polynomial' are used, then 1D or ND
+            interpolation will be used. (default=None)
+
+        Returns
+        -------
+        inst : pysat.Instrument
+            A pysat Instrument containing all data from the constellation at a
+            common time index
+
+        Note
+        ----
+        Uses the common index, `self.index`, that was defined using information
+        from the Constellation Instruments in combination with a potential
+        user-supplied resolution defined through `self.index_res`.
+
+        """
+        fill_methods = ['nearest', 'pad', 'ffill', 'backfill', 'bfill']
+        interp_type = [np.float64, np.int64, float, int]
+
+        # Establish the desired time index
+        coords = {'time': self.index}
+        fill_coords = {'time': coords['time']}
+
+        # Initalize the pysat Instrument
+        inst = pysat.Instrument()
+        inst._assign_attrs_from_const(self)
+
+        # Initalize the common data object
+        if inst.pandas_format:
+            data = pds.DataFrame(data={}, index=coords['time'])
+        else:
+            # Get the common coordinates needed for all data
+            for cinst in self.instruments:
+                if not cinst.pandas_format:
+                    for new_coord in cinst.data.coords.keys():
+                        if new_coord not in coords.keys():
+                            coords[new_coord] = cinst.data.coords[new_coord]
+                        elif new_coord != 'time':
+                            # Two instruments have the same coordinate, if they
+                            # are not identical, we need to establish a common
+                            # range and resolution.  Note that this will only
+                            # happen if the coordinates share the same names.
+                            if(len(coords[new_coord])
+                               != len(cinst.data.coords[new_coord])
+                               or coords[new_coord].values
+                               != cinst.data.coords[new_coord].values):
+                                coords[new_coord] = establish_common_coord(
+                                    [coords[new_coord].values,
+                                     cinst.data.coords[new_coord].values],
+                                    common=common_coord)
+
+            data = xr.Dataset(coords=coords)
+
+        # Add the data and metadata from each instrument
+        for cinst in self.instruments:
+            cinst_str = '_'.join([attr for attr in [cinst.platform, cinst.name,
+                                                    cinst.tag, cinst.inst_id]
+                                  if len(attr) > 0])
+            for dvar in cinst.variables:
+                if dvar not in self.variables:
+                    dname = '_'.join([dvar, cinst_str])
+                else:
+                    dname = dvar
+
+                # Determine whether or not this data type is interpolatable
+                fill_meth = fill_method
+                interp_flag = False
+                if cinst[dvar].dtype in interp_type:
+                    if fill_meth not in fill_methods and fill_meth is not None:
+                        interp_flag = True
+                else:
+                    if fill_meth not in fill_methods and fill_meth is not None:
+                        fill_meth = 'nearest'
+
+                # Assign the metadata, if it exists (e.g., not 'time')
+                if dvar in cinst.meta:
+                    inst.meta[dname] = cinst.meta[dvar]
+                    fill_val = cinst.meta[dvar, cinst.meta.labels.fill_val]
+                else:
+                    fill_val = np.nan
+
+                # Populate the data on the common coordinates
+                if cinst.pandas_format or (len(cinst[dvar].dims) == 1
+                                           and 'time' in cinst[dvar].dims):
+                    try:
+                        if cinst.pandas_format:
+                            ivals = cinst[dvar][coords['time']]
+                        else:
+                            ivals = pds.Series(
+                                cinst[dvar].sel({'time':
+                                                 coords['time']}).values,
+                                index=coords['time'])
+                    except KeyError:
+                        # Not all common times are present, need to fill
+                        # or interpolate
+                        if fill_meth is None:
+                            # Pad the data will fill values and then select
+                            if cinst.pandas_format:
+                                cinst_temp = cinst[dvar].copy()
+                            else:
+                                cinst_temp = cinst[dvar].to_pandas()
+                            new_times = [dtime for dtime in coords['time']
+                                         if dtime not in cinst_temp.index]
+                            fill_data = pds.Series(fill_val, index=new_times)
+                            cinst_temp = pds.concat([cinst_temp, fill_data])
+                            cinst_temp = cinst_temp.sort_index()
+                            ivals = cinst_temp[coords['time']]
+                        else:
+                            if cinst.pandas_format:
+                                cinst_temp = cinst[dvar].to_xarray()
+                                if cinst[dvar].index.name != 'time':
+                                    cinst_temp = cinst_temp.rename({
+                                        cinst[dvar].index.name: 'time'})
+                            else:
+                                cinst_temp = cinst[dvar].copy()
+
+                            if interp_flag:
+                                ivals = cinst_temp.interp(coords=fill_coords,
+                                                          method=fill_meth)
+                            else:
+                                ivals = cinst_temp.sel(fill_coords,
+                                                       method=fill_meth)
+
+                            # Get the data from the xarray object
+                            ivals = pds.Series(ivals.values,
+                                               index=coords['time'])
+
+                    # Extend the data
+                    if inst.pandas_format:
+                        val_dict = {dname: ivals}
+                    else:
+                        val_dict = {dname: (('time'), ivals)}
+                    data = data.assign(**val_dict)
+                elif dvar not in coords.keys():
+                    sel_dict = {dim: coords[dim] for dim in cinst[dvar].dims}
+
+                    if fill_meth is None:
+                        cinst_temp = cinst[dvar].copy()
+                        sel_key = ''
+                        while sel_key is not None:
+                            try:
+                                ivals = cinst_temp.sel(sel_dict,
+                                                       method=fill_meth)
+                                sel_key = None
+                            except KeyError as kerr:
+                                # Get the coordinate with values that need to
+                                # to be filled
+                                sel_key = str(kerr).split('index')[-1].split(
+                                    "'")[1]
+
+                                # Set the coordinates for filling
+                                new_coord = {sel_key: [
+                                    cc for cc in sel_dict[sel_key]
+                                    if cc not in cinst_temp.coords[sel_key]]}
+                                for dim in sel_dict.keys():
+                                    if dim not in new_coord.keys():
+                                        new_coord[dim] = sel_dict[dim]
+
+                                # Create a DataArray with fill data
+                                fill_data = xr.DataArray(data=fill_val,
+                                                         coords=new_coord,
+                                                         dims=cinst_temp.dims)
+
+                                if len(fill_data.coords.keys()) < len(
+                                        cinst_temp.coords.keys()):
+                                    fill_data = fill_data.assign_coords(
+                                        {ckey: cinst_temp.coords[ckey]
+                                         for ckey in cinst_temp.coords.keys()
+                                         if ckey not in sel_dict.keys()})
+
+                                # Merge the data objects
+                                cinst_temp = xr.concat([cinst_temp, fill_data],
+                                                       sel_key)
+                    elif interp_flag:
+                        ivals = cinst[dvar].interp(coords=sel_dict,
+                                                   method=fill_meth)
+                    else:
+                        ivals = cinst[dvar].sel(sel_dict, method=fill_meth)
+
+                    # Assign the interpolated data
+                    data = data.assign({dname: (cinst[dvar].dims,
+                                                ivals.values)})
+
+        inst.data = data
+        return inst
+
     def today(self):
         """Obtain UTC date for today, see pysat.Instrument for details."""
 
         return pysat.utils.time.today()
 
     def tomorrow(self):
         """Obtain UTC date for tomorrow, see pysat.Instrument for details."""
@@ -690,15 +893,15 @@
         custom functions whenever the `load` method is called.
 
         Unlike Instrument-level custom functions, Constellation-level custom
         functions should take a Constellation object as their first input
         argument.
 
         See Also
-        ---------
+        --------
         Instrument.custom_attach : base method for attaching custom functions
 
         """
 
         if apply_inst:
             self._call_inst_method('custom_attach', function, at_pos=at_pos,
                                    args=args, kwargs=kwargs)
@@ -708,15 +911,15 @@
 
         return
 
     def custom_clear(self):
         """Clear the custom function list.
 
         See Also
-        ---------
+        --------
         Instrument.custom_clear : base method for clearing custom functions
 
         """
 
         # Clear the Instrument-level custom methods
         self._call_inst_method('custom_clear')
 
@@ -733,15 +936,15 @@
         ----------
         *args : list reference
             References a list of input arguments
         **kwargs : dict reference
             References a dict of input keyword arguments
 
         See Also
-        ---------
+        --------
         Instrument.load : base method for loading Instrument data
 
         """
 
         # Load the data for each instrument
         self._call_inst_method('load', *args, **kwargs)
 
@@ -763,15 +966,15 @@
         ----------
         *args : list reference
             References a list of input arguments
         **kwargs : dict reference
             References a dict of input keyword arguments
 
         See Also
-        ---------
+        --------
         Instrument.download : base method for loading Instrument data
 
         Note
         ----
         If individual instruments require specific kwargs that differ from
         other instruments, define that in the individual instrument rather
         than this method.
```

### Comparing `pysat-3.0.6/pysat/_files.py` & `pysat-3.1.0/pysat/_files.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/_instrument.py` & `pysat-3.1.0/pysat/_instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,20 @@
         If true, pysat will check data to ensure times are unique and
         monotonically increasing (default=True)
     ignore_empty_files : bool
         Flag controling behavior for listing available files. If True, the list
         of files found will be checked to ensure the filesizes are greater than
         zero. Empty files are removed from the stored list of files.
         (default=False)
-    labels : dict
+    labels : dict or NoneType
         Dict where keys are the label attribute names and the values are tuples
-        that have the label values and value types in that order.
-        (default={'units': ('units', str), 'name': ('long_name', str),
-        'notes': ('notes', str), 'desc': ('desc', str),
-        'min_val': ('value_min', float),
-        'max_val': ('value_max', float), 'fill_val': ('fill', float)})
+        that have the label values and value types in that order. If None uses
+        the Meta defaults. Deprecated, use `meta_kwargs` (default=None)
+    meta_kwargs : dict or NoneType
+        Dict to specify custom Meta initialization (default=None)
     custom : list or NoneType
         Input list containing dicts of inputs for `custom_attach` method inputs
         that may be applied or None (default=None)
 
     Attributes
     ----------
     platform
@@ -144,16 +143,16 @@
     kwargs_reserved : dict
         Keyword arguments for reserved method arguments
     load_step : dt.timedelta
         The temporal increment for loading data, defaults to a timestep of one
         day
     meta : pysat.Meta
         Class holding the instrument metadata
-    meta_labels : dict
-        Dict containing defaults for new Meta data labels
+    meta_kwargs : dict
+        Dict containing defaults for Meta data
     orbits : pysat.Orbits
         Interface to extracting data orbit-by-orbit
     pandas_format : bool
         Flag indicating whether `data` is stored as a pandas.DataFrame (True)
         or an xarray.Dataset (False)
     today : dt.datetime
         Date and time for the current day in UT
@@ -249,20 +248,15 @@
     # Define all magic methods
 
     def __init__(self, platform=None, name=None, tag='', inst_id='',
                  clean_level=None, update_files=None, pad=None,
                  orbit_info=None, inst_module=None, data_dir='',
                  directory_format=None, file_format=None,
                  temporary_file_list=False, strict_time_flag=True,
-                 ignore_empty_files=False,
-                 labels={'units': ('units', str), 'name': ('long_name', str),
-                         'notes': ('notes', str), 'desc': ('desc', str),
-                         'min_val': ('value_min', np.float64),
-                         'max_val': ('value_max', np.float64),
-                         'fill_val': ('fill', np.float64)},
+                 ignore_empty_files=False, labels=None, meta_kwargs=None,
                  custom=None, **kwargs):
         """Initialize `pysat.Instrument` object."""
 
         # Check for deprecated usage of None
         if None in [tag, inst_id]:
             warnings.warn(" ".join(["The usage of None in `tag` and `inst_id`",
                                     "has been deprecated and will be removed",
@@ -425,16 +419,23 @@
         # Set up empty data and metadata.
         # Assign null data for user selected data type, `_null_data` assigned
         # when `self.pandas_format` is set in `_assign_attrs`.
         self.data = self._null_data.copy()
 
         # Create Meta instance with appropriate labels.  Meta class methods will
         # use Instrument definition of MetaLabels over the Metadata declaration.
-        self.meta_labels = labels
-        self.meta = pysat.Meta(labels=self.meta_labels)
+        self.meta_kwargs = {} if meta_kwargs is None else meta_kwargs
+
+        if labels is not None:
+            warnings.warn("".join(["`labels` is deprecated, use `meta_kwargs`",
+                                   "with the 'labels' key instead. Support ",
+                                   "for `labels` will be removed in v3.2.0+"]),
+                          DeprecationWarning, stacklevel=2)
+            self.meta_kwargs["labels"] = labels
+        self.meta = pysat.Meta(**self.meta_kwargs)
         self.meta.mutable = False
 
         # Nano-kernel processing variables. Feature processes data on each load.
         self.custom_functions = []
         self.custom_args = []
         self.custom_kwargs = []
 
@@ -585,16 +586,23 @@
                                           == str(other.__dict__[key]))
                         except AttributeError:
                             # If an item missing a required attribute
                             return False
 
                     else:
                         # General check for everything else
-                        checks.append(np.all(self.__dict__[key]
-                                             == other.__dict__[key]))
+                        if isinstance(self.__dict__[key], dict):
+                            try:
+                                checks.append(str(self.__dict__[key])
+                                              == str(other.__dict__[key]))
+                            except AttributeError:
+                                return False
+                        else:
+                            checks.append(np.all(self.__dict__[key]
+                                                 == other.__dict__[key]))
 
                 else:
                     # Both objects don't have the same attached objects
                     return False
             else:
                 # Data comparison area. Established earlier both have data.
                 if self.pandas_format:
@@ -651,15 +659,15 @@
         out_str = "".join(["pysat.Instrument(platform='", self.platform,
                            "', name='", self.name, "', tag='", self.tag,
                            "', inst_id='", self.inst_id,
                            "', clean_level='", self.clean_level,
                            "', pad={:}, orbit_info=".format(self.pad),
                            "{:}, ".format(self.orbit_info),
                            "inst_module=", istr, ", custom=", cstr,
-                           ", **{:}".format(in_kwargs), ")"])
+                           ", **{:}".format(repr(in_kwargs)), ")"])
 
         return out_str
 
     def __str__(self):
         """Descriptively print the basic Instrument properties."""
 
         # Get the basic Instrument properties
@@ -671,17 +679,28 @@
         output_str += "Instrument id: '{:s}'\n".format(self.inst_id)
 
         # Print out the data processing information
         output_str += '\nData Processing\n'
         output_str += '---------------\n'
         output_str += "Cleaning Level: '{:s}'\n".format(self.clean_level)
         output_str += 'Data Padding: {:s}\n'.format(self.pad.__str__())
-        for routine in self.kwargs.keys():
-            output_str += 'Keyword Arguments Passed to {:s}: '.format(routine)
-            output_str += "{:s}\n".format(self.kwargs[routine].__str__())
+
+        # Total kwargs passed to each routine.
+        num_kwargs = sum([len(self.kwargs[routine].keys())
+                          for routine in self.kwargs.keys()])
+        if num_kwargs > 0:
+            output_str += 'Keyword Arguments Passed: \n'
+
+            for routine in self.kwargs.keys():
+                # Only output for routine if kwargs are present.
+                if len(self.kwargs[routine].keys()) > 0:
+                    output_str += "  To {:s}: \n".format(routine)
+                    for key in self.kwargs[routine].keys():
+                        output_str += "    '{:s}': {:s}\n".format(
+                            key, str(self.kwargs[routine][key]))
 
         num_funcs = len(self.custom_functions)
         output_str += "Custom Functions: {:d} applied\n".format(num_funcs)
         if num_funcs > 0:
             for i, func in enumerate(self.custom_functions):
                 output_str += "    {:d}: {:}\n".format(i, func.__repr__())
                 if len(self.custom_args[i]) > 0:
@@ -761,15 +780,15 @@
 
             # By Date
             inst[datetime, 'name']
 
             # Slicing by date, inclusive.
             inst[datetime1:datetime2, 'name']
 
-            # Slicing by name and row/date
+            # Slicing by name and row/date (pandas only)
             inst[datetime1:datetime2, 'name1':'name2']
 
         """
 
         if self.pandas_format:
             if isinstance(key, str):
                 return self.data[key]
@@ -841,18 +860,16 @@
 
             # By Date
             inst[datetime, 'name']
 
             # Slicing by date, inclusive
             inst[datetime1:datetime2, 'name']
 
-            # Slicing by name and row/date
-            inst[datetime1:datetime2, 'name1':'name2']
-
         """
+
         if 'Epoch' in self.data.indexes:
             epoch_name = 'Epoch'
         elif 'time' in self.data.indexes:
             epoch_name = 'time'
         else:
             return xr.Dataset(None)
 
@@ -953,38 +970,51 @@
         Raises
         ------
         ValueError
             If underlying data's datetime index not stored as `Epoch` or `time`.
             If tuple not used when assigning dimensions for new multidimensional
             data.
 
+        Warnings
+        --------
+        If a single new value is set, the value will be broadcast over time.
+
         Note
         ----
         If no metadata provided and if metadata for 'name' not already stored
         then default meta information is also added,
         long_name = 'name', and units = ''.
 
         """
 
         new = copy.deepcopy(new_data)
 
+        # Initialize as empty dict.
+        if self.meta._data_types is None:
+            mutable = self.meta.mutable
+            self.meta.mutable = True
+            self.meta._data_types = {}
+            self.meta.mutable = mutable
+
         # Add data to main pandas.DataFrame, depending upon the input
         # slice, and a name
         if self.pandas_format:
             if isinstance(key, tuple):
                 try:
                     # Pass directly through to loc. This line raises a
                     # FutureWarning if key[0] is a slice. The future behavior
                     # is TypeError, which is already handled correctly below.
                     self.data.loc[key[0], key[1]] = new
                 except (KeyError, TypeError):
                     # TypeError for single integer, slice (pandas 2.0). KeyError
                     # for list, array. Assume key[0] is integer
                     # (including list or slice).
                     self.data.loc[self.data.index[key[0]], key[1]] = new
+
+                self._update_data_types(key[1])
                 self.meta[key[1]] = {}
                 return
             elif not isinstance(new, dict):
                 # Make it a dict to simplify downstream processing
                 new = {'data': new}
 
             # Input dict must have data in 'data',
@@ -1007,20 +1037,22 @@
 
                     if ('meta' not in new) and (key not in self.meta.keys_nD()):
                         # Create an empty Meta instance but with variable names.
                         # This will ensure the correct defaults for all
                         # subvariables.  Meta can filter out empty metadata as
                         # needed, the check above reduces the need to create
                         # Meta instances.
-                        ho_meta = pysat.Meta(labels=self.meta_labels)
+                        ho_meta = pysat.Meta(**self.meta_kwargs)
                         ho_meta[in_data[0].columns] = {}
                         self.meta[key] = ho_meta
 
             # Assign data and any extra metadata
             self.data[key] = in_data
+            self._update_data_types(key)
+
             self.meta[key] = new
 
         else:
             # xarray format chosen for Instrument object
             if not isinstance(new, dict):
                 new = {'data': new}
             in_data = new.pop('data')
@@ -1046,57 +1078,76 @@
                 try:
                     # Try loading as values
                     self.data[key[-1]].loc[indict] = in_data
                 except (TypeError, KeyError):
                     # Try loading indexed as integers
                     self.data[key[-1]][indict] = in_data
 
+                self._update_data_types(key[-1])
                 self.meta[key[-1]] = new
                 return
             elif isinstance(key, str):
                 # Assigning basic variables
-                if isinstance(in_data, xr.DataArray):
-                    # If xarray input, take as is
+                if isinstance(in_data, (xr.DataArray, tuple)):
+                    # If xarray or tuple input, take as is
                     self.data[key] = in_data
-                elif len(np.shape(in_data)) == 1:
+                elif len(np.shape(in_data)) <= 1:
                     # If not an xarray input, but still iterable, then we
                     # go through to process the 1D input
-                    if len(in_data) == len(self.index):
+                    if np.shape(in_data) == np.shape(self.index):
                         # 1D input has the correct length for storage along
-                        # 'Epoch'
+                        # 'Epoch'.
                         self.data[key] = (epoch_name, in_data)
-                    elif len(in_data) == 1:
-                        # Only provided a single number in iterable, make that
-                        # the input for all times
-                        self.data[key] = (epoch_name,
-                                          [in_data[0]] * len(self.index))
+                    elif len(np.shape(in_data)) == 0 or len(in_data) == 1:
+                        # Only a single number, or single in iterable.
+                        if key in self.variables:
+                            # If it already exists, assign as defined.
+                            in_data = np.squeeze(in_data)
+                            if np.shape(self.data[key]) == np.shape(in_data):
+                                self.data[key] = in_data
+                            else:
+                                raise ValueError(' '.join(('Shape of input',
+                                                           'does not match',
+                                                           'existing shape of',
+                                                           key)))
+                        else:
+                            # Otherwise broadcast over time.
+                            warnings.warn(' '.join(('Input for {:}'.format(key),
+                                                    'is a single value.',
+                                                    'Broadcast over epoch.')))
+                            in_data = pysat.utils.listify(in_data)
+                            self.data[key] = (epoch_name,
+                                              in_data * len(self.index))
                     elif len(in_data) == 0:
                         # Provided an empty iterable, make everything NaN
+                        warnings.warn(' '.join(('Input for {:} is'.format(key),
+                                                'empty. Setting to broadcast',
+                                                'as NaN over epoch.')))
                         self.data[key] = (epoch_name,
                                           [np.nan] * len(self.index))
-                elif len(np.shape(in_data)) == 0:
-                    # Not an iterable input, rather a single number.  Make
-                    # that number the input for all times.
-                    self.data[key] = (epoch_name, [in_data] * len(self.index))
+                    else:
+                        raise ValueError(' '.join(('Input for {:}'.format(key),
+                                                   'does not match expected',
+                                                   'dimensions. Value not',
+                                                   'set.')))
                 else:
                     # Multidimensional input that is not an xarray.  The user
                     # needs to provide everything that is required for success.
-                    if isinstance(in_data, tuple):
-                        self.data[key] = in_data
-                    else:
-                        raise ValueError(' '.join(('Must provide dimensions',
-                                                   'for xarray multidim',
-                                                   'data using input tuple.')))
+                    # Passes the data through to get appropriate error from
+                    # xarray.
+                    self.data[key] = in_data
 
             elif hasattr(key, '__iter__'):
                 # Multiple input strings (keys) are provided, but not in tuple
                 # form. Recurse back into this function, setting each input
                 # individually.
                 for keyname in key:
                     self.data[keyname] = in_data[keyname]
+                    self.meta._data_types[keyname] = self.data[
+                        keyname].values.dtype.type
 
             # Attach metadata
             self.meta[key] = new
 
         return
 
     def __iter__(self):
@@ -1137,14 +1188,18 @@
                 nfid = self.files.get_index(fname) + width - 1
                 local_inst.load(fname=fname, stop_fname=self.files[nfid])
                 yield local_inst
 
         elif self._iter_type == 'date':
             # Iterate over dates. A list of dates is generated whenever
             # bounds are set.
+
+            if len(self._iter_list) == 0:
+                raise IndexError('No dates to iterate over, check bounds')
+
             for date in self._iter_list:
                 # Use a copy trick, starting with null data in object
                 self.data = self._null_data
                 local_inst = self.copy()
 
                 # Set the user-specified range of dates
                 end_date = date + self._iter_width
@@ -1443,14 +1498,72 @@
 
         if len(missing) > 0:
             pysat.logger.debug(' '.join(['These Instrument test attributes',
                                          'kept their default  values:',
                                          '{:}'.format(missing)]))
         return
 
+    def _assign_attrs_from_const(self, const):
+        """Update Instrument attributes using Constellation data.
+
+        Parameters
+        ----------
+        const : pysat.Constellation
+            Data contained in a Constellation of Instruments
+
+        Note
+        ----
+        Updates the 'platform', 'name', 'tag', 'inst_id', 'clean_level',
+        'pad', 'clean_level', 'date', 'doy', 'yr', 'acknowledgements',
+        'references', and 'pandas_format' attributes
+
+        """
+        # Define the reference variables
+        up_attrs = ['platform', 'name', 'tag', 'inst_id', 'clean_level', 'pad',
+                    'pandas_format', 'date', 'doy', 'acknowledgements', 'yr',
+                    'references']
+        clean_rank = {'clean': 4, 'dusty': 3, 'dirty': 2, 'none': 1, None: 1}
+        clean_assign = {4: 'clean', 3: 'dusty', 2: 'dirty', 1: 'none'}
+
+        for attr in up_attrs:
+            cattr = [getattr(cinst, attr) for cinst in const.instruments]
+            cattr = list(set(cattr))  # np.unique doesn't work with pad
+
+            if attr == 'pad':
+                # Set the pad value to the longest padding, if padding was set
+                cattr = [ca for ca in cattr if ca is not None]
+                if len(cattr) == 1:
+                    # There was only one set pad, use it
+                    setattr(self, attr, cattr[0])
+                elif len(cattr) > 1:
+                    # There are multiple pads, they can be reliably compared
+                    # using the `freqstr` attribute, which is lowest for the
+                    # longest pad period.
+                    long_pad = cattr[0]
+                    for i in range(1, len(cattr)):
+                        if long_pad.freqstr > cattr[i].freqstr:
+                            long_pad = cattr[i]
+                    setattr(self, attr, long_pad)
+            elif len(cattr) == 1:
+                # There is only one value, set it
+                setattr(self, attr, cattr[0])
+            elif attr == 'clean_level':
+                # Set the clean value to the lowest cleaning rank
+                crank = [clean_rank[cl] for cl in cattr]
+                setattr(self, attr, clean_assign[min(crank)])
+            elif attr == 'pandas_format':
+                # If there is a mix of pandas and xarray data, use xarray
+                setattr(self, attr, False)
+            else:
+                # Combine all unique attributes as a string
+                astr = "\n" if attr in ['acknowledgements',
+                                        'references'] else "_"
+                setattr(self, attr, astr.join(cattr))
+        return
+
     def _load_data(self, date=None, fid=None, inc=None, load_kwargs=None):
         """Load data for an instrument on given date or filename index.
 
         Parameters
         ----------
         date : dt.datetime or NoneType
             File date (default=None)
@@ -1510,20 +1623,20 @@
                 # Ensure units and name are named consistently in new Meta
                 # object as specified by user upon Instrument instantiation
                 mdata.accept_default_labels(self.meta)
                 bad_datetime = False
             except pds.errors.OutOfBoundsDatetime:
                 bad_datetime = True
                 data = self._null_data.copy()
-                mdata = pysat.Meta(labels=self.meta_labels)
+                mdata = pysat.Meta(**self.meta_kwargs)
 
         else:
             bad_datetime = False
             data = self._null_data.copy()
-            mdata = pysat.Meta(labels=self.meta_labels)
+            mdata = pysat.Meta(**self.meta_kwargs)
 
         output_str = '{platform} {name} {tag} {inst_id}'
         output_str = output_str.format(platform=self.platform,
                                        name=self.name, tag=self.tag,
                                        inst_id=self.inst_id)
 
         # Check that data and metadata are the data types we expect
@@ -1800,34 +1913,60 @@
                                                       check_type=check_type,
                                                       export_nan=export_nan)
 
     # -----------------------------------------------------------------------
     # Define all accessible methods
 
     @property
+    def meta_labels(self):
+        """Provide Meta input for labels kwarg, deprecated.
+
+        Returns
+        -------
+        dict
+            Either Meta default provided locally or custom value provided
+            by user and stored in `meta_kwargs['labels']`
+
+        """
+        warnings.warn("".join(["Deprecated attribute, returns `meta_kwargs",
+                               "['labels']` or Meta defaults if not set. Will",
+                               " be removed in pysat 3.2.0+"]),
+                      DeprecationWarning, stacklevel=2)
+        if 'labels' in self.meta_kwargs.keys():
+            return self.meta_kwargs['labels']
+        else:
+            return {'units': ('units', str), 'name': ('long_name', str),
+                    'notes': ('notes', str), 'desc': ('desc', str),
+                    'min_val': ('value_min', (float, int)),
+                    'max_val': ('value_max', (float, int)),
+                    'fill_val': ('fill', (float, int, str))}
+
+    @property
     def bounds(self):
         """Boundaries for iterating over instrument object by date or file.
 
         Parameters
         ----------
         start : dt.datetime, str, or NoneType
-            Start of iteration, if None uses first data date.
-            list-like collection also accepted. (default=None)
+            Start of iteration, disregarding any time of day information.
+            If None uses first data date. List-like collection also
+            accepted, allowing mutliple bound ranges. (default=None)
         stop :  dt.datetime, str, or None
-            Stop of iteration, inclusive. If None uses last data date.
-            list-like collection also accepted. (default=None)
+            Stop of iteration, inclusive of the entire day regardless of
+            time of day in the bounds. If None uses last data date.
+            List-like collection also accepted, allowing mutliple bound
+            ranges, though it must match `start`. (default=None)
         step : str, int, or NoneType
             Step size used when iterating from start to stop. Use a
-            Pandas frequency string ('3D', '1M') when setting bounds by date,
-            an integer when setting bounds by file. Defaults to a single
-            day/file (default='1D', 1).
+            Pandas frequency string ('3D', '1M') or an integer (will assume
+            a base frequency equal to the file frequency). If None, defaults to
+            a single unit of file frequency (typically 1 day) (default=None).
         width : pandas.DateOffset, int, or NoneType
-            Data window used when loading data within iteration. Defaults to a
-            single day/file if not assigned. (default=dt.timedelta(days=1),
-            1)
+            Data window used when loading data within iteration. If None,
+            defaults to a single file frequency (typically 1 day) (default=None)
 
         Raises
         ------
         ValueError
             If `start` and `stop` don't have the same type, or if too many
             input argument supplied, or unequal number of elements in
             `start`/`stop`, or if bounds aren't in increasing order, or if
@@ -1899,31 +2038,49 @@
         elif len(value) == 4:
             # Also includes loading window (data width)
             self._iter_step = value[2]
             self._iter_width = value[3]
         else:
             raise ValueError('Too many input arguments.')
 
+        # Determine the value of the file frequency
+        if hasattr(self.files.files.index, "freqstr"):
+            file_freq = self.files.files.index.freqstr
+            if file_freq is None:
+                if len(self.files.files.index) > 1:
+                    # The frequency needs to be calculated
+                    file_freq = pysat.utils.time.calc_freq(
+                        self.files.files.index)
+                else:
+                    file_freq = '1D'  # This is the pysat default
+        else:
+            file_freq = '1D'  # This is the pysat default
+
         # Pull out start and stop times now that other optional items have
         # been checked out.
         start = value[0]
         stop = value[1]
 
         if (start is None) and (stop is None):
             # Set default using first and last file date
             self._iter_start = [self.files.start_date]
             self._iter_stop = [self.files.stop_date]
             self._iter_type = 'date'
+
+            # Set the hidden iteration parameters if not specified
             if self._iter_step is None:
-                self._iter_step = '1D'
+                self._iter_step = file_freq
+
             if self._iter_width is None:
-                self._iter_width = dt.timedelta(days=1)
+                self._iter_width = pds.tseries.frequencies.to_offset(file_freq)
+
             if self._iter_start[0] is not None:
                 # There are files. Use those dates.
-                ustops = [istop - self._iter_width + dt.timedelta(days=1)
+                ustops = [istop - self._iter_width
+                          + pds.tseries.frequencies.to_offset(self._iter_step)
                           for istop in self._iter_stop]
                 ufreq = self._iter_step
                 self._iter_list = pysat.utils.time.create_date_range(
                     self._iter_start, ustops, freq=ufreq)
             else:
                 # Instrument has no files
                 self._iter_list = []
@@ -1962,21 +2119,29 @@
                 # One of the inputs is a string
                 self._iter_type = 'file'
 
                 # Could be (string, None) or (None, string). Replace None
                 # with first/last, as appropriate.
                 if starts[0] is None:
                     starts = [self.files[0]]
+
                 if stops[0] is None:
                     stops = [self.files[-1]]
 
                 # Default step size
                 if self._iter_step is None:
                     self._iter_step = 1
 
+                if type(self._iter_step) not in [int, np.int32, np.int64]:
+                    # Convert from a frequency string to an index
+                    soff = pds.tseries.frequencies.to_offset(self._iter_step)
+                    foff = pds.tseries.frequencies.to_offset(
+                        self.files.files.index.freq)
+                    self._iter_step = int(soff.n / foff.n)
+
                 # Default window size
                 if self._iter_width is None:
                     self._iter_width = 1
 
                 self._iter_list = []
                 for istart, istop in zip(starts, stops):
                     # Ensure istart begins before istop. Get the index of
@@ -2009,49 +2174,68 @@
                     # to include only year, month, and day
                     starts = [self.files.start_date]
                 if stops[0] is None:
                     stops = [self.files.stop_date]
 
                 # Default step size
                 if self._iter_step is None:
-                    self._iter_step = '1D'
+                    self._iter_step = file_freq
 
                 # Default window size
                 if self._iter_width is None:
-                    self._iter_width = dt.timedelta(days=1)
+                    self._iter_width = pds.tseries.frequencies.to_offset(
+                        file_freq)
 
-                # Create list-like of dates for iteration
-                starts = pysat.utils.time.filter_datetime_input(starts)
-                stops = pysat.utils.time.filter_datetime_input(stops)
-                freq = self._iter_step
-                width = self._iter_width
-
-                # Ensure inputs are in reasonable date order
-                for start, stop in zip(starts, stops):
-                    if start > stop:
-                        estr = ' '.join(('Bounds must be set in increasing',
-                                         'date order.',
-                                         start.strftime('%d %B %Y'),
-                                         'is later than',
-                                         stop.strftime('%d %B %Y')))
-                        raise ValueError(estr)
+                # Identify start/stop pairings that lie outside of the file list
+                good_bounds = list()
+                for i, start in enumerate(starts):
+                    # Ensure there are files
+                    if self.files.stop_date is not None:
+                        # Ensure the start and stop times intersect with
+                        # the file list
+                        if(start <= self.files.stop_date
+                           and stops[i] >= self.files.start_date):
+                            good_bounds.append(i)
+
+                if len(good_bounds) > 0:
+                    # Create list-like of dates for iteration
+                    starts = list(pysat.utils.time.filter_datetime_input(
+                        np.asarray(starts)[good_bounds]))
+                    stops = list(pysat.utils.time.filter_datetime_input(
+                        np.asarray(stops)[good_bounds]))
+                    file_inc = pds.tseries.frequencies.to_offset(file_freq)
+
+                    # Ensure inputs are in reasonable date order
+                    for start, stop in zip(starts, stops):
+                        if start > stop:
+                            estr = ' '.join(('Bounds must be set in increasing',
+                                             'date order.',
+                                             start.strftime('%d %B %Y'),
+                                             'is later than',
+                                             stop.strftime('%d %B %Y')))
+                            raise ValueError(estr)
+
+                    # Account for width of load. Don't extend past bound. To
+                    # avoid pandas shenanigans, only perform adjustments to the
+                    # stop time if the file width and file increment are unequal
+                    ustops = [stop if self._iter_width == file_inc else
+                              stop - self._iter_width + file_inc
+                              for stop in stops]
+
+                    # Date range is inclusive, no need to pad.
+                    self._iter_list = pysat.utils.time.create_date_range(
+                        starts, ustops, freq=self._iter_step)
+                else:
+                    self._iter_list = []
 
-                # Account for width of load. Don't extend past bound.
-                ustops = [stop - width + dt.timedelta(days=1)
-                          for stop in stops]
-
-                # Date range is inclusive, no need to pad.
-                self._iter_list = pysat.utils.time.create_date_range(starts,
-                                                                     ustops,
-                                                                     freq=freq)
-                # go back to time index
+                # Convert the date range back to a time index format
                 self._iter_list = pds.DatetimeIndex(self._iter_list)
 
             else:
-                raise ValueError(' '.join(('Input is not a known type, string',
+                raise ValueError(' '.join(('Input is not a known type: string',
                                            'or datetime')))
             self._iter_start = starts
             self._iter_stop = stops
 
         return
 
     @property
@@ -2201,17 +2385,32 @@
         # Retrieve the appropriate concatenation function
         if self.pandas_format:
             # Specifically do not sort unless otherwise specified
             if 'sort' not in kwargs:
                 kwargs['sort'] = False
             concat_func = pds.concat
         else:
+            # Ensure the dimensions are equal
+            equal_dims = True
+            idat = 0
+            while idat < len(new_data) - 1 and equal_dims:
+                if new_data[idat].dims != new_data[idat + 1].dims:
+                    equal_dims = False
+                idat += 1
+
+            if not equal_dims:
+                # Update the dimensions, padding data where necessary
+                new_data = pysat.utils.coords.expand_xarray_dims(
+                    new_data, self.meta, exclude_dims=['time'])
+
             # Specify the dimension, if not otherwise specified
             if 'dim' not in kwargs:
                 kwargs['dim'] = self.index.name
+
+            # Set the concat function
             concat_func = xr.concat
 
         # Assign the concatenated data to the instrument
         self.data = concat_func(new_data, **kwargs)
         return
 
     def custom_attach(self, function, at_pos='end', args=None, kwargs=None):
@@ -2398,46 +2597,42 @@
                 date = self._iter_list[0]
                 end_date = date + self._iter_width
 
             # Perform load
             self.load(date=date, end_date=end_date, verifyPad=verifyPad)
 
         elif self._iter_type == 'file':
-            first = self.files.get_index(self._iter_list[0])
-            last = self.files.get_index(self._iter_list[-1])
-            step = self._iter_step
-            width = self._iter_width
             if self._fid is not None:
-                # Data already loaded in `.data`
-                if (self._fid < first) | (self._fid + step > last):
+                # Data already loaded in `.data`. Step size is always accounted
+                # for in the list of files. Get location of current file in
+                # iteration list.
+                idx = None
+                fname = self.files[self._fid]
+                for i, name in enumerate(self._iter_list):
+                    if name == fname:
+                        idx = i
+                        break
+
+                if idx is None:
+                    estr = ''.join(('Unable to find loaded filename in the ',
+                                    'supported iteration list. Please check ',
+                                    'the Instrument bounds, `self.bounds` for',
+                                    ' supported iteration ranges.'))
+                    raise StopIteration(estr)
+                elif idx >= len(self._iter_list) - 1:
                     raise StopIteration('Outside the set file boundaries.')
-                else:
-                    # Step size already accounted for in the list of files. Get
-                    # location of current file in iteration list.
-                    idx = None
-                    fname = self.files[self._fid]
-                    for i, name in enumerate(self._iter_list):
-                        if name == fname:
-                            idx = i
-                            break
-                    if idx is None:
-                        estr = ''.join(('Unable to find loaded filename ',
-                                        'in the supported iteration list. ',
-                                        'Please check the Instrument bounds, ',
-                                        '`self.bounds` for supported iteration',
-                                        'ranges.'))
-                        raise StopIteration(estr)
-                    fname = self._iter_list[idx + 1]
+
+                fname = self._iter_list[idx + 1]
             else:
                 # No data loaded yet, start with the first file
                 fname = self._iter_list[0]
 
             # Get location for second file. Note a width of 1 loads single file.
             # Load range of files.
-            nfid = self.files.get_index(fname) + width - 1
+            nfid = self.files.get_index(fname) + self._iter_width - 1
             self.load(fname=fname, stop_fname=self.files[nfid],
                       verifyPad=verifyPad)
 
         return
 
     def prev(self, verifyPad=False):
         """Iterate backwards through the data in Instrument object.
@@ -2485,41 +2680,38 @@
             else:
                 # No data currently loaded, start at the end
                 end_date = self._iter_list[-1] + self._iter_width
                 date = self._iter_list[-1]
                 self.load(date=date, end_date=end_date, verifyPad=verifyPad)
 
         elif self._iter_type == 'file':
-            first = self.files.get_index(self._iter_list[0])
-            last = self.files.get_index(self._iter_list[-1])
-            step = self._iter_step
-            width = self._iter_width
             if self._fid is not None:
-                if (self._fid - step < first) or (self._fid > last):
+                # Find location of the desired file, recall that step size is
+                # already accounted for when createing the iteration file list
+                idx = None
+                fname = self.files[self._fid]
+                for i, name in enumerate(self._iter_list):
+                    if name == fname:
+                        idx = i
+                        break
+
+                if idx is None:
+                    estr = ''.join(('Unable to find loaded filename in the ',
+                                    'supported iteration list. Please check ',
+                                    'the Instrument bounds, `self.bounds` for',
+                                    ' supported iteration ranges.'))
+                    raise StopIteration(estr)
+                elif idx == 0:
                     raise StopIteration('Outside the set file boundaries.')
-                else:
-                    # Find location of the desired file
-                    idx = None
-                    fname = self.files[self._fid]
-                    for i, name in enumerate(self._iter_list):
-                        if name == fname:
-                            idx = i
-                            break
-                    if idx is None:
-                        estr = ''.join(('Unable to find loaded filename ',
-                                        'in the supported iteration list. ',
-                                        'Please check the Instrument bounds, ',
-                                        '`self.bounds` for supported iteration',
-                                        'ranges.'))
-                        raise StopIteration(estr)
-                    fname = self._iter_list[idx - 1]
+
+                fname = self._iter_list[idx - 1]
             else:
                 fname = self._iter_list[-1]
 
-            nfid = self.files.get_index(fname) + width - 1
+            nfid = self.files.get_index(fname) + self._iter_width - 1
             self.load(fname=fname, stop_fname=self.files[nfid],
                       verifyPad=verifyPad)
 
         return
 
     def rename(self, mapper, lowercase_data_labels=False):
         """Rename variables within both data and metadata.
@@ -3025,20 +3217,30 @@
                     self._prev_data, self._prev_meta = self._load_prev()
                     self._curr_data, self._curr_meta = self._load_data(
                         date=self.date, fid=self._fid, inc=self.load_step,
                         load_kwargs=kwargs)
                     self._next_data, self._next_meta = self._load_next()
 
             # Make sure datetime indices for all data is monotonic
+            if self.pandas_format:
+                sort_method = "sort_index"
+                sort_args = []
+            else:
+                sort_method = 'sortby'
+                sort_args = ['time']
+
             if not self._index(self._prev_data).is_monotonic_increasing:
-                self._prev_data.sort_index(inplace=True)
+                self._prev_data = getattr(self._prev_data,
+                                          sort_method)(*sort_args)
             if not self._index(self._curr_data).is_monotonic_increasing:
-                self._curr_data.sort_index(inplace=True)
+                self._curr_data = getattr(self._curr_data,
+                                          sort_method)(*sort_args)
             if not self._index(self._next_data).is_monotonic_increasing:
-                self._next_data.sort_index(inplace=True)
+                self._next_data = getattr(self._next_data,
+                                          sort_method)(*sort_args)
 
             # Make tracking indexes consistent with new loads
             if self._load_by_date:
                 self._next_data_track = curr + self.load_step
                 self._prev_data_track = curr - self.load_step
             else:
                 # File and date loads have to be treated differently
@@ -3106,27 +3308,28 @@
                 stored_data = self.data  # .copy()
                 temp_time = copy.deepcopy(self.index[-1])
 
                 # Pad data using access mechanisms that work for both pandas
                 # and xarray
                 self.data = self._next_data.copy()
                 self.data = self[temp_time:last_pad]
-                if not self.empty:
+                if len(self.index) > 0:
                     if (self.index[0] == temp_time):
                         self.data = self[1:]
                     self.concat_data(stored_data, prepend=True)
                 else:
                     self.data = stored_data
 
-            self.data = self[first_pad:last_pad]
+            if len(self.index) > 0:
+                self.data = self[first_pad:last_pad]
 
-            # Want exclusive end slicing behavior from above
-            if not self.empty:
-                if (self.index[-1] == last_pad) & (not want_last_pad):
-                    self.data = self[:-1]
+                # Want exclusive end slicing behavior from above
+                if not self.empty:
+                    if (self.index[-1] == last_pad) & (not want_last_pad):
+                        self.data = self[:-1]
 
         else:
             # If self.pad is False, load single day
             self.data, meta = self._load_data(date=self.date, fid=self._fid,
                                               inc=self.load_step,
                                               load_kwargs=kwargs)
             if not self.empty:
@@ -3177,14 +3380,42 @@
             if self.strict_time_flag:
                 raise ValueError(' '.join((message, 'To continue to use data,'
                                            'set inst.strict_time_flag=False',
                                            'before loading data')))
             else:
                 warnings.warn(message, stacklevel=2)
 
+        # Transfer any extra attributes in meta to the Instrument object.
+        # Metadata types need to be initialized before preprocess is run.
+        # TODO(#1020): Change the way this kwarg is handled
+        if use_header or ('use_header' in self.kwargs['load']
+                          and self.kwargs['load']['use_header']):
+            self.meta.transfer_attributes_to_header()
+        else:
+            warnings.warn(''.join(['Meta now contains a class for global ',
+                                   'metadata (MetaHeader). Default attachment ',
+                                   'of global attributes to Instrument will ',
+                                   'be Deprecated in pysat 3.2.0+. Set ',
+                                   '`use_header=True` in this load call or ',
+                                   'on Instrument instantiation to remove this',
+                                   ' warning.']), DeprecationWarning,
+                          stacklevel=2)
+            self.meta.transfer_attributes_to_instrument(self)
+
+        # Transfer loaded data types to meta.
+        self.meta.mutable = True
+        if self.meta._data_types is None:
+            self.meta._data_types = {}
+        for key in self.variables:
+            data_type = self.data[key].dtype.type
+            self.meta._data_types[key] = data_type
+
+        self.meta.mutable = False
+        sys.stdout.flush()
+
         # Apply the instrument preprocess routine, if data present
         if not self.empty:
             # Does not require self as input, as it is a partial func
             self._preprocess_rtn(**self.kwargs['preprocess'])
 
         # Clean data, if data is present and cleaning requested
         if (not self.empty) & (self.clean_level != 'none'):
@@ -3197,31 +3428,14 @@
         # Remove the excess data padding, if any applied
         if (self.pad is not None) & (not self.empty) & (not verifyPad):
             self.data = self[first_time: last_time]
             if not self.empty:
                 if (self.index[-1] == last_time) & (not want_last_pad):
                     self.data = self[:-1]
 
-        # Transfer any extra attributes in meta to the Instrument object.
-        # TODO(#1020): Change the way this kwarg is handled
-        if use_header or ('use_header' in self.kwargs['load']
-                          and self.kwargs['load']['use_header']):
-            self.meta.transfer_attributes_to_header()
-        else:
-            warnings.warn(''.join(['Meta now contains a class for global ',
-                                   'metadata (MetaHeader). Default attachment ',
-                                   'of global attributes to Instrument will ',
-                                   'be Deprecated in pysat 3.2.0+. Set ',
-                                   '`use_header=True` in this load call or ',
-                                   'on Instrument instantiation to remove this',
-                                   ' warning.']), DeprecationWarning,
-                          stacklevel=2)
-            self.meta.transfer_attributes_to_instrument(self)
-        self.meta.mutable = False
-        sys.stdout.flush()
         return
 
     def remote_file_list(self, start=None, stop=None, **kwargs):
         """Retrieve a time-series of remote files for chosen instrument.
 
         Parameters
         ----------
@@ -3244,18 +3458,20 @@
         Note
         ----
         Default behaviour is to return all files.  User may additionally
         specify a given year, year/month, or year/month/day combination to
         return a subset of available files.
 
         """
+        # Add the method kwargs if they are not set to defaults
+        if start is not None:
+            kwargs["start"] = start
 
-        # Add the function kwargs
-        kwargs["start"] = start
-        kwargs["stop"] = stop
+        if stop is not None:
+            kwargs["stop"] = stop
 
         # Add the user-supplied kwargs
         rtn_key = 'list_remote_files'
         if rtn_key in self.kwargs.keys():
             for user_key in self.kwargs[rtn_key].keys():
                 # Don't overwrite kwargs supplied directly to this routine
                 if user_key not in kwargs.keys():
@@ -3551,15 +3767,15 @@
             pysat.logger.warning('Requested download over an empty date range.')
 
         return
 
     def to_netcdf4(self, fname=None, base_instrument=None, epoch_name=None,
                    zlib=False, complevel=4, shuffle=True,
                    preserve_meta_case=False, export_nan=None,
-                   unlimited_time=True, modify=False):
+                   export_pysat_info=True, unlimited_time=True, modify=False):
         """Store loaded data into a netCDF4 file.
 
         .. deprecated:: 3.0.2
             Changed `fname` from a kwarg to an arg of type str in the 3.2.0+
             release.
 
         Parameters
@@ -3593,14 +3809,17 @@
              By default, the metadata variables where a value of NaN is allowed
              and written to the netCDF4 file is maintained by the Meta object
              attached to the pysat.Instrument object. A list supplied here
              will override the settings provided by Meta, and all parameters
              included will be written to the file. If not listed
              and a value is NaN then that attribute simply won't be included in
              the netCDF4 file. (default=None)
+        export_pysat_info : bool
+            If True, platform, name, tag, and inst_id will be appended to the
+            metadata.  (default=True)
         unlimited_time : bool
              Flag specifying whether or not the epoch/time dimension should be
              unlimited; it is when the flag is True. (default=True)
         modify : bool
              Flag specifying whether or not the changes made to the Instrument
              object needed to prepare it for writing should also be made to
              this object.  If False, the current Instrument object will remain
@@ -3628,18 +3847,35 @@
         # Write the output file
         pysat.utils.io.inst_to_netcdf(inst, fname=fname,
                                       base_instrument=base_instrument,
                                       epoch_name=epoch_name, zlib=zlib,
                                       complevel=complevel, shuffle=shuffle,
                                       preserve_meta_case=preserve_meta_case,
                                       export_nan=export_nan,
+                                      export_pysat_info=export_pysat_info,
                                       unlimited_time=unlimited_time)
 
         return
 
+    def _update_data_types(self, key):
+        """Update the data types in pysat.Meta object.
+
+        Parameters
+        ----------
+        key : str or list-like
+            Data variable or list of these data variables for which the data
+            type should be updated.
+
+        """
+
+        for lkey in pysat.utils.listify(key):
+            if not isinstance(lkey, slice) and lkey in self.variables:
+                self.meta._data_types[lkey] = self.data[lkey].values.dtype.type
+        return
+
 
 # ----------------------------------------------------------------------------
 #   Utilities and variables supporting the Instrument Object
 
 # Hidden variable to store pysat reserved keywords. Defined here, since these
 # values are used by both the Instrument class and a function defined below.
 # In release 3.2.0+ `freq` will be removed.
```

### Comparing `pysat-3.0.6/pysat/_meta.py` & `pysat-3.1.0/pysat/_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,25 @@
         the desired attribute names and values the metadata for that attribute.
         (default=None)
     labels : dict
         Dict where keys are the label attribute names and the values are tuples
         that have the label values and value types in that order.
         (default={'units': ('units', str), 'name': ('long_name', str),
         'notes': ('notes', str), 'desc': ('desc', str),
-        'min_val': ('value_min', float), 'max_val': ('value_max', float),
-        'fill_val': ('fill', float)})
+        'min_val': ('value_min', (float, int)),
+        'max_val': ('value_max', (float, int)),
+        'fill_val': ('fill', (float, int, str))})
     export_nan : list or NoneType
         List of labels that should be exported even if their value is NaN or
         None for an empty list. When used, metadata with a value of NaN will
         be excluded from export. Will always allow NaN export for labels of
         the float type. (default=None)
+    data_types : dict or NoneType
+        Dict of data types for variables names or None to determine after
+        loading the data. (default=None)
 
     Attributes
     ----------
     data : pandas.DataFrame
         Index is variable standard name, 'units', 'long_name', and other
         defaults are also stored along with additional user provided labels.
     labels : MetaLabels
@@ -159,34 +163,39 @@
 
     # -----------------------------------------------------------------------
     # Define the magic methods
 
     def __init__(self, metadata=None, header_data=None,
                  labels={'units': ('units', str), 'name': ('long_name', str),
                          'notes': ('notes', str), 'desc': ('desc', str),
-                         'min_val': ('value_min', float),
-                         'max_val': ('value_max', float),
-                         'fill_val': ('fill', float)}, export_nan=None):
+                         'min_val': ('value_min', (float, int)),
+                         'max_val': ('value_max', (float, int)),
+                         'fill_val': ('fill', (float, int, str))},
+                 export_nan=None, data_types=None):
         """Initialize `pysat.Meta` object."""
         # Set mutability of Meta attributes.  This flag must be set before
         # anything else, or `__setattr__` breaks.
         self.mutable = True
 
         # Set the global meta data
         self.header = MetaHeader(header_data)
 
         # Set the NaN export list
         self._export_nan = [] if export_nan is None else export_nan
         for lvals in labels.values():
-            if lvals[0] not in self._export_nan and lvals[1] == float:
+            if(lvals[0] not in self._export_nan
+               and float in pysat.utils.listify(lvals[1])):
                 self._export_nan.append(lvals[0])
 
         # Set the labels
         self.labels = MetaLabels(metadata=self, **labels)
 
+        # Set the data types, if provided
+        self._data_types = data_types
+
         # Initialize higher order (nD) data structure container, a dict
         self._ho_data = {}
 
         # Use any user provided data to instantiate object with data.
         # Attributes unit and name labels are called within.
         if metadata is not None:
             if isinstance(metadata, pds.DataFrame):
@@ -362,19 +371,26 @@
             # Make sure the variable names are in good shape.  The Meta object
             # is case insensitive, but case preserving. Convert given data_vars
             # into ones Meta has already seen. If new, then input names
             # become the standard.
             data_vars = self.var_case_name(data_vars)
             meta_vars = list(self.keys())
             def_vars = list()
+            data_var_types = None if self._data_types is None else list()
             for var in data_vars:
                 if var not in meta_vars:
                     def_vars.append(var)
+                    if data_var_types is not None:
+                        if var in self._data_types.keys():
+                            data_var_types.append(self._data_types[var])
+                        else:
+                            data_var_types.append(None)
+
             if len(def_vars) > 0:
-                self._insert_default_values(def_vars)
+                self._insert_default_values(def_vars, data_var_types)
 
             # Check if input dict empty.  If so, no metadata was assigned by
             # the user.  This is an empty call and we can head out,
             # since defaults have been assigned.
             if len(input_data.keys()) == 0:
                 return
 
@@ -408,36 +424,39 @@
                         if ikey in self.labels.label_attrs.keys():
                             iattr = self.labels.label_attrs[ikey]
                             if not isinstance(
                                     to_be_set, self.labels.label_type[iattr]):
                                 # If this is a disagreement between byte data
                                 # and an expected str, resolve it here
                                 if(isinstance(to_be_set, bytes)
-                                   and self.labels.label_type[iattr] == str):
+                                   and str in pysat.utils.listify(
+                                       self.labels.label_type[iattr])):
                                     to_be_set = core_utils.stringify(to_be_set)
                                 else:
                                     # This type is incorrect, try casting it
                                     wmsg = ''.join(['Metadata with type ',
                                                     repr(type(to_be_set)),
                                                     ' does not match expected ',
                                                     'type ',
                                                     repr(self.labels.label_type[
                                                         iattr])])
                                     try:
                                         if hasattr(to_be_set, '__iter__'):
-                                            if self.labels.label_type[
-                                                    iattr] == str:
+                                            if str in pysat.utils.listify(
+                                                    self.labels.label_type[
+                                                    iattr]):
                                                 to_be_set = '\n\n'.join(
                                                     [str(tval) for tval in
                                                      to_be_set])
                                             else:
                                                 raise TypeError("can't recast")
                                         else:
-                                            to_be_set = self.labels.label_type[
-                                                iattr](to_be_set)
+                                            to_be_set = pysat.utils.listify(
+                                                self.labels.label_type[
+                                                    iattr])[0](to_be_set)
 
                                         # Inform user data was recast
                                         pysat.logger.info(''.join((
                                             wmsg, '. Recasting input for ',
                                             repr(var), ' with key ',
                                             repr(ikey))))
                                     except (TypeError, ValueError):
@@ -770,49 +789,78 @@
 
         # If we made it this far, things are good
         return True
 
     # -----------------------------------------------------------------------
     # Define the hidden methods
 
-    def _insert_default_values(self, data_var):
+    def _insert_default_values(self, data_var, data_type=None):
         """Set the default label values for a data variable.
 
         Parameters
         ----------
         data_var : str or list
             Single or multiple data variable name(s).
+        data_type : type, list, or NoneType
+            Type for the data value(s) or None if not specified (default=None)
 
         Note
         ----
         Sets NaN for all float values, -1 for all int values, 'data_var' for
         names labels, '' for all other str values, and None for any other
-        data type.
+        data type. If there are multiple data types, sets the data type (if
+        included).  Otherwise, chooses the first type in the tuple.
 
         """
         # Cycle through each label type to create a list of label names
         # and label default values
         labels = list()
+        lattrs = list()
         default_vals = list()
         name_idx = None
+        need_data_type = dict()
         for i, lattr in enumerate(self.labels.label_type.keys()):
             labels.append(getattr(self.labels, lattr))
+            lattrs.append(lattr)
+            if(isinstance(self.labels.label_type[lattr], tuple)
+               and data_type is not None):
+                need_data_type[lattr] = True
+            else:
+                need_data_type[lattr] = False
 
             if lattr in ['name']:
                 default_vals.append('')
                 name_idx = i
             else:
                 default_vals.append(self.labels.default_values_from_attr(lattr))
 
         # Assign the default values to the DataFrame for this data variable(s).
         data_vars = pysat.utils.listify(data_var)
-        for var in data_vars:
+        if data_type is None:
+            var_types = [None for dvar in data_vars]
+        else:
+            var_types = pysat.utils.listify(data_type)
+
+        for i, var in enumerate(data_vars):
+            # Use the label defaults if this variable doesn't need to consider
+            # the data type
+            if not np.any(list(need_data_type.values())):
+                data_default = list(default_vals)
+            else:
+                data_default = [
+                    self.labels.default_values_from_attr(
+                        lattrs[j], var_types[i]) if need_data_type[lattrs[j]]
+                    else val for j, val in enumerate(default_vals)]
+
+            # The default value for the name must be set after to be consistent
             if name_idx is not None:
-                default_vals[name_idx] = var
-            self._data.loc[var, labels] = default_vals
+                data_default[name_idx] = var
+
+            # Update the meta data to the desired defaults
+            self._data.loc[var, labels] = data_default
 
         return
 
     def _label_setter(self, new_label, current_label, default_type,
                       use_names_default=False):
         """Set default meta attributes for variable.
 
@@ -1614,27 +1662,30 @@
 
 class MetaLabels(object):
     """Store metadata labels for Instrument instance.
 
     Parameters
     ----------
     units : tuple
-        Units label name and value type (default=('units', str))
+        Units label name and value type(s) (default=('units', str))
     name : tuple
-        Name label name and value type (default=('long_name', str))
+        Name label name and value type(s) (default=('long_name', str))
     notes : tuple
-        Notes label name and value type (default=('notes', str))
+        Notes label name and value type(s) (default=('notes', str))
     desc : tuple
-        Description label name and value type (default=('desc', str))
+        Description label name and value type(s) (default=('desc', str))
     min_val : tuple
-        Minimum value label name and value type (default=('value_min', float))
+        Minimum value label name and value type(s)
+        (default=('value_min', (float, int)))
     max_val : tuple
-        Maximum value label name and value type (default=('value_max', float))
+        Maximum value label name and value type(s)
+        (default=('value_max', (float, int)))
     fill_val : tuple
-        Fill value label name and value type (default=('fill', float))
+        Fill value label name and value type(s)
+        (default=('fill', (float, int, str)))
     kwargs : dict
         Dictionary containing optional label attributes, where the keys are the
         attribute names and the values are tuples containing the label name and
         value type
 
     Attributes
     ----------
@@ -1692,17 +1743,17 @@
     updated to use the same values of units, etc. as found in the
     pysat.Instrument object.
 
     """
 
     def __init__(self, metadata=None, units=('units', str),
                  name=('long_name', str), notes=('notes', str),
-                 desc=('desc', str), min_val=('value_min', float),
-                 max_val=('value_max', float), fill_val=('fill', float),
-                 **kwargs):
+                 desc=('desc', str), min_val=('value_min', (float, int)),
+                 max_val=('value_max', (float, int)),
+                 fill_val=('fill', (float, int, str)), **kwargs):
         """Initialize the MetaLabels class."""
 
         # Initialize the coupled metadata
         self.meta = metadata
 
         # Initialize a dictionary of label types, whose keys are the label
         # attributes
@@ -1711,14 +1762,17 @@
                            'min_val': min_val[1], 'max_val': max_val[1],
                            'fill_val': fill_val[1]}
         self.label_attrs = {units[0]: 'units', name[0]: 'name',
                             notes[0]: 'notes', desc[0]: 'desc',
                             min_val[0]: 'min_val', max_val[0]: 'max_val',
                             fill_val[0]: 'fill_val'}
 
+        # Ensure the label types include numpy 64 bit types when appropriate
+        self._update_label_types()
+
         # Ensure all standard label types are valid
         for label in self.label_type.keys():
             if not self._eval_label_type(self.label_type[label]):
                 raise TypeError(''.join([
                     'iterable types like ', repr(self.label_type[label]),
                     ' (set for ', repr(label), ') are not allowed']))
 
@@ -1793,14 +1847,49 @@
         out_str = "MetaLabels:\n"
         out_str += "-----------\n"
         out_str += core_utils.fmt_output_in_cols(lab_attrs, ncols=ncol,
                                                  max_num=nlabels)
 
         return out_str
 
+    def _update_label_types(self):
+        """Update the `label_type` attribute, adjusting types as appropriate."""
+
+        # Update the types as necessary
+        for lkey in self.label_type.keys():
+            if self.label_type[lkey] == float:
+                self.label_type[lkey] = (float, np.float64, np.float32)
+            elif self.label_type[lkey] == int:
+                self.label_type[lkey] = (int, np.int64, np.int32, np.int16,
+                                         np.int8, bool)
+            elif self.label_type[lkey] == str:
+                self.label_type[lkey] = (str, np.str_)
+            elif self.label_type[lkey] == bool:
+                self.label_type[lkey] = (bool, np.bool_)
+            elif isinstance(self.label_type[lkey], tuple):
+                ltypes = list(self.label_type[lkey])
+
+                if float in ltypes:
+                    ltypes.extend([np.float64, np.float32])
+
+                if int in ltypes:
+                    ltypes.extend([np.int64, np.int32, np.int16, np.int8, bool])
+
+                if str in ltypes:
+                    ltypes.append(np.str_)
+
+                if bool in ltypes:
+                    ltypes.append(np.bool_)
+
+                # This may result in duplicate numpy types, but order is more
+                # important than carrying around a duplicate type, as the first
+                # type in the provided tuple is the default type
+                self.label_type[lkey] = tuple(ltypes)
+        return
+
     def _eval_label_type(self, val_type):
         """Evaluate the label type for validity.
 
         Parameters
         ----------
         val_type : type
             Variable type for the value to be assigned to a MetaLabel
@@ -1824,30 +1913,38 @@
                 # If a list can't be cast, the type is not iterable and is
                 # likely valid.  There may be some objects that prove
                 # problematic, but they haven't been encountered yet.
                 pass
 
         return valid
 
-    def default_values_from_type(self, val_type):
+    def default_values_from_type(self, val_type, data_type=None):
         """Retrieve the default values for each label based on their type.
 
         Parameters
         ----------
         val_type : type
             Variable type for the value to be assigned to a MetaLabel
+        data_type : type or NoneType
+            Type for the data values or None if not specified (default=None)
 
         Returns
         -------
         default_val : str, float, int, NoneType
             Sets NaN for all float values, -1 for all int values, and '' for
             all str values, and None for any other data type
 
         """
 
+        if isinstance(val_type, tuple):
+            if data_type in val_type:
+                val_type = data_type
+            else:
+                val_type = val_type[0]
+
         # Perform some pre-checks on type, checks that could error with
         # unexpected input.
         try:
             floating_check = isinstance(val_type(), np.floating)
         except TypeError as err:
             if str(err).find('not a callable function') > 0:
                 floating_check = False
@@ -1882,21 +1979,23 @@
         else:
             mstr = ''.join(('No type match found for ', str(val_type)))
             pysat.logger.info(mstr)
             default_val = None
 
         return default_val
 
-    def default_values_from_attr(self, attr_name):
+    def default_values_from_attr(self, attr_name, data_type=None):
         """Retrieve the default values for each label based on their type.
 
         Parameters
         ----------
         attr_name : str
             Label attribute name (e.g., max_val)
+        data_type : type or NoneType
+            Type for the data values or None if not specified (default=None)
 
         Returns
         -------
         default_val : str, float, int, or NoneType
             Sets NaN for all float values, -1 for all int values, and ''
             for all str values except for 'scale', which defaults to 'linear',
             and None for any other data type
@@ -1913,15 +2012,15 @@
             raise ValueError('unknown label attribute {:}'.format(attr_name))
 
         # Assign the default value
         if attr_name == 'scale':
             default_val = 'linear'
         else:
             default_val = self.default_values_from_type(
-                self.label_type[attr_name])
+                self.label_type[attr_name], data_type=data_type)
             if default_val is None:
                 mstr = ' '.join(('A problem may have been',
                                  'encountered with the user',
                                  'supplied type for Meta',
                                  'attribute: ', attr_name,
                                  'Please check the settings',
                                  'provided to `labels` at',
```

### Comparing `pysat-3.0.6/pysat/_orbits.py` & `pysat-3.1.0/pysat/_orbits.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/_params.py` & `pysat-3.1.0/pysat/_params.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/instruments/methods/general.py` & `pysat-3.1.0/pysat/instruments/methods/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,17 +131,19 @@
         new_out = out.asfreq('D')
 
         for i, out_month in enumerate(out.index):
             if(out_month.month == emonth.month
                and out_month.year == emonth.year):
                 out_month = emonth
 
-            mrange = pds.date_range(start=out_month, periods=2, freq='MS')
-            irange = pds.date_range(*mrange.values, freq="D").values[:-1]
-            new_out[irange] = out.loc[out_month]
+            crange = pds.date_range(start=out_month, periods=2,
+                                    freq=file_cadence)
+            irange = pds.date_range(*crange.values, freq="D").values[:-1]
+            sel_range = new_out.index.intersection(irange)
+            new_out[sel_range] = out.loc[out_month]
 
         # Assign the non-NaN files to out and add days to the filenames
         out = new_out.dropna()
         out = out + '_' + out.index.strftime('%Y-%m-%d')
 
     return out
```

### Comparing `pysat-3.0.6/pysat/instruments/methods/testing.py` & `pysat-3.1.0/pysat/instruments/methods/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,22 @@
     epoch_name : str
         The variable name of the instrument epoch.
     data : pds.DataFrame or xr.Dataset
         The dataset keys from the instrument.
 
     """
     # Create standard metadata for all parameters
-    meta = pysat.Meta()
+    data_types = {'uts': float, 'mlt': float, 'slt': float, 'longitude': float,
+                  'latitude': float, 'altitude': float, 'orbit_num': int,
+                  'dummy1': int, 'dummy2': int, 'dummy3': int, 'dummy4': int,
+                  'unicode_dummy': str, 'string_dummy': str,
+                  'dummy_drifts': float, 'int8_dummy': int, 'int16_dummy': int,
+                  'int32_dummy': int, 'int64_dummy': int, 'profiles': int,
+                  'series_profiles': float}
+    meta = pysat.Meta(data_types=data_types)
     meta['uts'] = {'units': 's', 'long_name': 'Universal Time',
                    'desc': 'Number of seconds since mindight UT',
                    'value_min': 0.0, 'value_max': 86400.0}
     meta['mlt'] = {'units': 'hours', 'long_name': 'Magnetic Local Time',
                    'value_min': 0.0, 'value_max': 24.0,
                    'desc': 'Local time at magnetic field line at equator.'}
     meta['slt'] = {'units': 'hours', 'long_name': 'Solar Local Time',
@@ -167,14 +174,18 @@
                                'value_min': 0., 'value_max': 25., 'units': 'km',
                                'fill': np.nan,
                                'desc': ''.join(['Testing series profiles ',
                                                 'indexed by float.'])}
 
     # Children metadata required for 2D pandas.
     # TODO(#789): Delete after removal of Meta children.
+    data_types = {'density': float, 'fraction': float, 'alt_profiles': float,
+                  'variable_profiles': float, 'profile_height': int,
+                  'variable_profile_height': int, 'images': int, 'x': int,
+                  'y': int, 'z': int, 'image_lat': float, 'image_lon': float}
     alt_profile_meta = pysat.Meta()
     alt_profile_meta['density'] = {'desc': 'Simulated density values.',
                                    'units': 'Log N/cc',
                                    'value_min': 0, 'value_max': np.inf}
     alt_profile_meta['fraction'] = {'value_min': 0., 'value_max': 1.,
                                     'desc': ''.join(['Simulated fractional O+ ',
                                                      'composition.'])}
@@ -646,7 +657,69 @@
                                                            cycle=cycle))
                     with NetworkLock(fname, 'w') as fout:
                         if content is not None:
                             fout.write(content)
                         if timeout is not None:
                             time.sleep(timeout)
     return
+
+
+def non_monotonic_index(index):
+    """Adjust the index to be non-monotonic.
+
+    Parameters
+    ----------
+    index : pds.DatetimeIndex
+        The index generated in an instrument test file.
+
+    Returns
+    -------
+    new_index : pds.DatetimeIndex
+        A non-montonic index
+
+    """
+
+    new_index = index.tolist()
+
+    # Create a non-monotonic index
+    new_index[6:9], new_index[3:6] = new_index[3:6], new_index[6:9]
+
+    # Convert back to DatetimeIndex
+    new_index = pds.to_datetime(new_index)
+
+    return new_index
+
+
+def non_unique_index(index):
+    """Adjust the index to be non-unique.
+
+    Parameters
+    ----------
+    index : pds.DatetimeIndex
+        The index generated in an instrument test file.
+
+    Returns
+    -------
+    new_index : pds.DatetimeIndex
+        A non-unique index
+
+    """
+
+    new_index = index.tolist()
+
+    # Create a non-unique index
+    new_index[1:3] = [new_index[1]] * 2
+
+    # Convert back to DatetimeIndex
+    new_index = pds.to_datetime(new_index)
+
+    return new_index
+
+
+def _warn_malformed_kwarg():
+    """Warn user that kwarg has been deprecated."""
+
+    dstr = ' '.join(['The kwarg malformed_index has been deprecated and',
+                     'will be removed in pysat 3.2.0+. Please use',
+                     'non_monotonic_index or non_unique_index to specify',
+                     'desired behaviour.'])
+    warnings.warn(dstr, DeprecationWarning, stacklevel=2)
```

### Comparing `pysat-3.0.6/pysat/instruments/pysat_ndtesting.py` & `pysat-3.1.0/pysat/instruments/pysat_ndtesting.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,31 +26,36 @@
 # Clean method
 clean = mm_test.clean
 
 # Optional method, preprocess
 preprocess = mm_test.preprocess
 
 
-def load(fnames, tag='', inst_id='', malformed_index=False,
-         start_time=None, num_samples=864, test_load_kwarg=None,
-         max_latitude=90.):
+def load(fnames, tag='', inst_id='', non_monotonic_index=False,
+         non_unique_index=False, malformed_index=False, start_time=None,
+         num_samples=864, test_load_kwarg=None, max_latitude=90.):
     """Load the test files.
 
     Parameters
     ----------
     fnames : list
         List of filenames.
     tag : str
         Tag name used to identify particular data set to be loaded.
         This input is nominally provided by pysat itself. (default='')
     inst_id : str
         Instrument ID used to identify particular data set to be loaded.
         This input is nominally provided by pysat itself. (default='')
+    non_monotonic_index : bool
+        If True, time index will be non-monotonic (default=False)
+    non_unique_index : bool
+        If True, time index will be non-unique (default=False)
     malformed_index : bool
-        If True, the time index will be non-unique and non-monotonic.
+        If True, the time index will be non-unique and non-monotonic. Deprecated
+        and scheduled for removal in pysat 3.2.0.
         (default=False)
     start_time : dt.timedelta or NoneType
         Offset time of start time since midnight UT. If None, instrument data
         will begin at midnight. (default=None)
     num_samples : int
         Maximum number of times to generate.  Data points will not go beyond the
         current day. (default=864)
@@ -77,23 +82,26 @@
     # Create an artificial satellite data set
     iperiod = mm_test.define_period()
     drange = mm_test.define_range()
 
     # Using 100s frequency for compatibility with seasonal analysis unit tests
     uts, index, dates = mm_test.generate_times(fnames, num_samples, freq='100S',
                                                start_time=start_time)
-
+    # TODO(#1094): Remove in pysat 3.2.0
     if malformed_index:
-        index = index.tolist()
-
-        # Create a non-monotonic index
-        index[0:3], index[3:6] = index[3:6], index[0:3]
+        # Warn that kwarg is deprecated and set new kwargs.
+        mm_test._warn_malformed_kwarg()
+        non_monotonic_index = True
+        non_unique_index = True
+
+    if non_monotonic_index:
+        index = mm_test.non_monotonic_index(index)
+    if non_unique_index:
+        index = mm_test.non_unique_index(index)
 
-        # Create a non-unique index
-        index[6:9] = [index[6]] * 3
     data = xr.Dataset({'uts': ((epoch_name), uts)},
                       coords={epoch_name: index})
 
     # Need to create simple orbits here. Have start of first orbit
     # at 2009,1, 0 UT. 14.84 orbits per day. Figure out how far in time from
     # the root start a measurement is and use that info to create a signal
     # that is continuous from that start. Going to presume there are 5820
```

### Comparing `pysat-3.0.6/pysat/instruments/pysat_netcdf.py` & `pysat-3.1.0/pysat/instruments/pysat_netcdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -128,24 +128,17 @@
     warnings.warn("".join(["Downloads are not currently supported for ",
                            "pysat netCDF files"]))
     return
 
 
 def load(fnames, tag='', inst_id='', strict_meta=False, file_format='NETCDF4',
          epoch_name=None, epoch_unit='ms', epoch_origin='unix',
-         pandas_format=True, decode_timedelta=False,
-         load_labels={'units': ('units', str), 'name': ('long_name', str),
-                      'notes': ('notes', str), 'desc': ('desc', str),
-                      'plot': ('plot_label', str), 'axis': ('axis', str),
-                      'scale': ('scale', str),
-                      'min_val': ('value_min', np.float64),
-                      'max_val': ('value_max', np.float64),
-                      'fill_val': ('fill', np.float64)},
-         meta_processor=None,
-         meta_translation=None, drop_meta_labels=None, decode_times=None):
+         pandas_format=True, decode_timedelta=False, meta_kwargs=None,
+         load_labels=None, meta_processor=None, meta_translation=None,
+         drop_meta_labels=None, decode_times=None):
     """Load pysat-created NetCDF data and meta data.
 
     Parameters
     ----------
     fnames : array-like
         iterable of filename strings, full path, to data files to be loaded.
         This input is nominally provided by pysat itself.
@@ -183,21 +176,21 @@
     pandas_format : bool
         Flag specifying if data is stored in a pandas DataFrame (True) or
         xarray Dataset (False). (default=False)
     decode_timedelta : bool
         Used for xarray data (`pandas_format` is False).  If True, variables
         with unit attributes that  are 'timelike' ('hours', 'minutes', etc) are
         converted to `np.timedelta64`. (default=False)
-    load_labels : dict
+    meta_kwargs : dict or NoneType
+        Dict to specify custom Meta initialization or None to use Meta
+        defaults (default=None)
+    load_labels : dict or NoneType
         Dict where keys are the label attribute names and the values are tuples
-        that have the label values and value types in that order.
-        (default={'units': ('units', str), 'name': ('long_name', str),
-        'notes': ('notes', str), 'desc': ('desc', str),
-        'min_val': ('value_min', np.float64),
-        'max_val': ('value_max', np.float64), 'fill_val': ('fill', np.float64)})
+        that have the label values and value types in that order or None to use
+        Meta defaults. Deprecated, use `meta_kwargs` instead. (default=None)
     meta_processor : function or NoneType
         If not None, a dict containing all of the loaded metadata will be
         passed to `meta_processor` which should return a filtered version
         of the input dict. The returned dict is loaded into a pysat.Meta
         instance and returned as `meta`. (default=None)
     meta_translation : dict or NoneType
         Translation table used to map metadata labels in the file to
@@ -230,14 +223,15 @@
     data, mdata = pysat.utils.io.load_netcdf(fnames, strict_meta=strict_meta,
                                              file_format=file_format,
                                              epoch_name=epoch_name,
                                              epoch_unit=epoch_unit,
                                              epoch_origin=epoch_origin,
                                              pandas_format=pandas_format,
                                              decode_timedelta=decode_timedelta,
+                                             meta_kwargs=meta_kwargs,
                                              labels=load_labels,
                                              meta_processor=meta_processor,
                                              meta_translation=meta_translation,
                                              drop_meta_labels=drop_meta_labels,
                                              decode_times=decode_times)
 
     return data, mdata
```

### Comparing `pysat-3.0.6/pysat/instruments/pysat_testing.py` & `pysat-3.1.0/pysat/instruments/pysat_testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,30 +22,30 @@
         'user_password': 'simulates an instrument that requires a password',
         'default_meta': 'simulates an instrument using the default metadata'}
 
 # Dictionary of satellite IDs, list of corresponding tags.
 inst_ids = {'': [tag for tag in tags.keys()]}
 _test_dates = {'': {tag: dt.datetime(2009, 1, 1) for tag in tags.keys()}}
 _test_download = {'': {'no_download': False}}
-_test_load_opt = {'': {'': {'num_samples': 13}}}
+_test_load_opt = {'': {'': [{'num_samples': 13}, {'num_samples': 15}]}}
 
 # Init method
 init = mm_test.init
 
 # Clean method
 clean = mm_test.clean
 
 # Optional method, preprocess
 preprocess = mm_test.preprocess
 
 
 def load(fnames, tag='', inst_id='', sim_multi_file_right=False,
-         sim_multi_file_left=False, root_date=None, malformed_index=False,
-         start_time=None, num_samples=86400, test_load_kwarg=None,
-         max_latitude=90.):
+         sim_multi_file_left=False, root_date=None, non_monotonic_index=False,
+         non_unique_index=False, malformed_index=False, start_time=None,
+         num_samples=86400, test_load_kwarg=None, max_latitude=90.):
     """Load the test files.
 
     Parameters
     ----------
     fnames : list
         List of filenames.
     tag : str
@@ -59,16 +59,21 @@
         `root_date`. (default=False)
     sim_multi_file_left : bool
         Adjusts date range to be 12 hours in the past or twelve hours before
         `root_date`. (default=False)
     root_date : NoneType
         Optional central date, uses _test_dates if not specified.
         (default=None)
+    non_monotonic_index : bool
+        If True, time index will be non-monotonic (default=False)
+    non_unique_index : bool
+        If True, time index will be non-unique (default=False)
     malformed_index : bool
-        If True, time index will be non-unique and non-monotonic (default=False)
+        If True, the time index will be non-unique and non-monotonic. Deprecated
+        and scheduled for removal in pysat 3.2.0. (default=False)
     start_time : dt.timedelta or NoneType
         Offset time of start time since midnight UT. If None, instrument data
         will begin at midnight. (default=None)
     num_samples : int
         Maximum number of times to generate.  Data points will not go beyond the
         current day. (default=86400)
     test_load_kwarg : any
@@ -155,32 +160,40 @@
     data['string_dummy'] = ['test'] * len(data)
     data['unicode_dummy'] = [u'test'] * len(data)
     data['int8_dummy'] = np.ones(len(data), dtype=np.int8)
     data['int16_dummy'] = np.ones(len(data), dtype=np.int16)
     data['int32_dummy'] = np.ones(len(data), dtype=np.int32)
     data['int64_dummy'] = np.ones(len(data), dtype=np.int64)
 
-    # Activate for testing malformed_index, and for instrument_test_class.
-    if malformed_index or tag == 'non_strict':
-        index = index.tolist()
-
-        # Create a non-monotonic index
-        index[0:3], index[3:6] = index[3:6], index[0:3]
-
-        # Create a non-unique index
-        index[6:9] = [index[6]] * 3
+    # TODO(#1094): Remove in pysat 3.2.0
+    if malformed_index:
+        # Warn that kwarg is deprecated and set new kwargs.
+        mm_test._warn_malformed_kwarg()
+        non_monotonic_index = True
+        non_unique_index = True
+
+    # Activate if non-monotonic index is needed.
+    if np.any([non_monotonic_index, (tag == 'non_strict')]):
+        index = mm_test.non_monotonic_index(index)
+
+    # Activate if non-unique index is needed.
+    if np.any([non_unique_index, (tag == 'non_strict')]):
+        index = mm_test.non_unique_index(index)
 
     data.index = index
     data.index.name = 'Epoch'
 
     # Set the meta data
     meta = mm_test.initialize_test_meta('Epoch', data.keys())
 
+    # TODO(#1120): Move logic up so that empty data is returned first.
     if tag == 'default_meta':
         return data, pysat.Meta()
+    elif tag == 'no_download':
+        return pds.DataFrame(), pysat.Meta()
     else:
         return data, meta
 
 
 list_files = functools.partial(mm_test.list_files, test_dates=_test_dates)
 list_remote_files = functools.partial(mm_test.list_remote_files,
                                       test_dates=_test_dates)
```

### Comparing `pysat-3.0.6/pysat/instruments/pysat_testing2d.py` & `pysat-3.1.0/pysat/instruments/pysat_testing2d.py`

 * *Files 14% similar despite different names*

```diff
@@ -148,21 +148,17 @@
     data['unicode_dummy'] = [u'test'] * len(data)
     data['int8_dummy'] = np.ones(len(data), dtype=np.int8)
     data['int16_dummy'] = np.ones(len(data), dtype=np.int16)
     data['int32_dummy'] = np.ones(len(data), dtype=np.int32)
     data['int64_dummy'] = np.ones(len(data), dtype=np.int64)
 
     if malformed_index:
-        index = index.tolist()
-
-        # Create a non-monotonic index
-        index[0:3], index[3:6] = index[3:6], index[0:3]
-
-        # Create a non-unique index
-        index[6:9] = [index[6]] * 3
+        mm_test._warn_malformed_kwarg()
+        index = mm_test.non_monotonic_index(index)
+        index = mm_test.non_unique_index(index)
 
     data.index = index
     data.index.name = 'Epoch'
 
     # Higher rate time signal (for scalar >= 2). This time signal is used
     # for 2D profiles associated with each time in main DataFrame.
     num_profiles = 50 if num_samples >= 50 else num_samples
@@ -176,16 +172,16 @@
     # DataFrame at each time with numeric variables only
     alt_profiles = []
 
     # Series at each time, numeric data only
     series_profiles = []
 
     # Frame indexed by date times
-    frame = pds.DataFrame({'density': data.loc[data.index[0:num_profiles],
-                                               'mlt'].values.copy(),
+    frame = pds.DataFrame({'density':
+                           data.iloc[0:num_profiles]['mlt'].values.copy(),
                            'dummy_str': ['test'] * num_profiles,
                            'dummy_ustr': [u'test'] * num_profiles},
                           index=data.index[0:num_profiles],
                           columns=['density', 'dummy_str', 'dummy_ustr'])
 
     # Frame indexed by float
     dd = np.arange(num_profiles) * 1.2
```

### Comparing `pysat-3.0.6/pysat/instruments/pysat_testing2d_xarray.py` & `pysat-3.1.0/pysat/instruments/pysat_testing2d_xarray.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/instruments/pysat_testing_xarray.py` & `pysat-3.1.0/pysat/instruments/pysat_testing_xarray.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 clean = mm_test.clean
 
 # Optional method, preprocess
 preprocess = mm_test.preprocess
 
 
 def load(fnames, tag='', inst_id='', sim_multi_file_right=False,
-         sim_multi_file_left=False, malformed_index=False,
-         start_time=None, num_samples=86400, test_load_kwarg=None,
-         max_latitude=90.):
+         sim_multi_file_left=False, non_monotonic_index=False,
+         non_unique_index=False, malformed_index=False, start_time=None,
+         num_samples=86400, test_load_kwarg=None, max_latitude=90.):
     """Load the test files.
 
     Parameters
     ----------
     fnames : list
         List of filenames.
     tag : str
@@ -78,16 +78,21 @@
         This input is nominally provided by pysat itself. (default='')
     sim_multi_file_right : bool
         Adjusts date range to be 12 hours in the future or twelve hours beyond
         `root_date`. (default=False)
     sim_multi_file_left : bool
         Adjusts date range to be 12 hours in the past or twelve hours before
         `root_date`. (default=False)
+    non_monotonic_index : bool
+        If True, time index will be non-monotonic (default=False)
+    non_unique_index : bool
+        If True, time index will be non-unique (default=False)
     malformed_index : bool
-        If True, time index will be non-unique and non-monotonic.
+        If True, the time index will be non-unique and non-monotonic. Deprecated
+        and scheduled for removal in pysat 3.2.0. (default=False)
     start_time : dt.timedelta or NoneType
         Offset time of start time since midnight UT. If None, instrument data
         will begin at midnight. (default=None)
     num_samples : int
         Maximum number of times to generate.  Data points will not go beyond the
         current day. (default=86400)
     test_load_kwarg : any
@@ -120,22 +125,25 @@
     if sim_multi_file_right:
         root_date = dt.datetime(2009, 1, 1, 12)
     elif sim_multi_file_left:
         root_date = dt.datetime(2008, 12, 31, 12)
     else:
         root_date = dt.datetime(2009, 1, 1)
 
+    # TODO(#1094): Remove in pysat 3.2.0
     if malformed_index:
-        index = index.tolist()
-
-        # Create a non-monotonic index
-        index[0:3], index[3:6] = index[3:6], index[0:3]
-
-        # Create a non-unique index
-        index[6:9] = [index[6]] * 3
+        # Warn that kwarg is deprecated and set new kwargs.
+        mm_test._warn_malformed_kwarg()
+        non_monotonic_index = True
+        non_unique_index = True
+
+    if non_monotonic_index:
+        index = mm_test.non_monotonic_index(index)
+    if non_unique_index:
+        index = mm_test.non_unique_index(index)
 
     data = xr.Dataset({'uts': ((epoch_name), uts)},
                       coords={epoch_name: index})
 
     # Need to create simple orbits here. Have start of first orbit
     # at 2009,1, 0 UT. 14.84 orbits per day. Figure out how far in time from
     # the root start a measurement is and use that info to create a signal
```

### Comparing `pysat-3.0.6/pysat/instruments/pysat_testmodel.py` & `pysat-3.1.0/pysat/instruments/pysat_testmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,38 +160,41 @@
 
     # Set the meta data
     meta = mm_test.initialize_test_meta(epoch_name, data.keys())
 
     # Adjust metadata from overall defaults
     meta['dummy1'] = {'value_min': -2**32 + 2, 'value_max': 2**32 - 1,
                       'fill': -2**32 + 1}
-    meta['dummy2'] = {'value_min': -2**32 + 2, 'value_max': 2**32 - 1,
-                      'fill': -2**32 + 1}
+    if tag == '':
+        # Assign metadata unique to default tag
+        meta['dummy2'] = {'value_min': -2**32 + 2, 'value_max': 2**32 - 1,
+                          'fill': -2**32 + 1}
 
     if tag == 'pressure_levels':
         # Assigning new metadata for altitude since it differs from default info
         meta['altitude'] = {meta.labels.units: 'cm',
                             meta.labels.name: 'altitude',
                             meta.labels.min_val: 0.,
                             meta.labels.max_val: 1E8,
                             meta.labels.desc: ' '.join(('Altitude (fake) for',
                                                         'each pressure level')),
                             meta.labels.notes: '',
                             meta.labels.fill_val: np.nan}
 
         # Assigning metadata for meridional ion drifts since it differs from
         # default info.
-        meta['iv_mer'] = {meta.labels.units: 'm/s',
-                          meta.labels.name: 'Meridional Ion Drift',
-                          meta.labels.min_val: -250.,
-                          meta.labels.max_val: 250.,
-                          meta.labels.desc: ' '.join(('Non-physical meridional',
-                                                      'ion drifts.')),
-                          meta.labels.notes: '',
-                          meta.labels.fill_val: np.nan}
+        meta['dummy_drifts'] = {meta.labels.units: 'm/s',
+                                meta.labels.name: 'Meridional Ion Drift',
+                                meta.labels.min_val: -250.,
+                                meta.labels.max_val: 250.,
+                                meta.labels.desc: ' '.join(('Non-physical',
+                                                            'meridional',
+                                                            'ion drifts.')),
+                                meta.labels.notes: '',
+                                meta.labels.fill_val: np.nan}
 
         # Assign metadata for the new coordinate axis here, `lev` and `ilev`.
         meta['lev'] = {meta.labels.units: '',
                        meta.labels.name: 'Pressure Level (midpoint)',
                        meta.labels.min_val: -6.875,
                        meta.labels.max_val: 7.125,
                        meta.labels.desc: ' '.join(('Log of atmospheric',
```

### Comparing `pysat-3.0.6/pysat/instruments/templates/template_instrument.py` & `pysat-3.1.0/pysat/instruments/templates/template_instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
 def list_remote_files(tag, inst_id, user=None, password=None):
     """Return a Pandas Series of every file for chosen remote data.
 
     This routine is intended to be used by pysat instrument modules supporting
     a particular NASA CDAWeb dataset.
 
     Parameters
-    -----------
+    ----------
     tag : str
         Denotes type of file to load.  Accepted types are <tag strings>.
     inst_id : str
         Specifies the satellite or instrument ID. Accepted types are
         <inst_id strings>.
     user : str or NoneType
         Username to be passed along to resource with relevant data.
```

### Comparing `pysat-3.0.6/pysat/tests/classes/cls_ci.py` & `pysat-3.1.0/pysat/tests/classes/cls_ci.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/classes/cls_instrument_access.py` & `pysat-3.1.0/pysat/tests/classes/cls_instrument_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 import pandas as pds
 import pytest
 import xarray as xr
 
 import pysat
 from pysat.utils import testing
+from pysat.utils.time import filter_datetime_input
 
 
 class InstAccessTests(object):
     """Basic tests for `pysat.Instrument` data access.
 
     Note
     ----
@@ -89,15 +90,16 @@
         Note
         ----
         Success of test is tied to `self.ref_time`.
 
         """
         # Test that the first loaded time matches the first requested time
         assert self.testInst.index[0] == self.ref_time, \
-            "First loaded time is incorrect"
+            "First loaded time is incorrect {:} != {:}".format(
+                self.testInst.index[0], self.ref_time)
 
         # Test that the Instrument date is set to the requested start date
         self.out = dt.datetime(self.ref_time.year, self.ref_time.month,
                                self.ref_time.day)
         assert self.testInst.date == self.out, \
             "Incorrect Instrument date attribute"
 
@@ -126,27 +128,35 @@
         self.testInst.load(self.ref_time.year, self.ref_doy, **kwargs,
                            use_header=True)
 
         # Test that the loaded date range is correct
         self.eval_successful_load()
         return
 
-    def test_basic_instrument_load_no_data(self, caplog):
-        """Test Instrument load with no data for appropriate log messages."""
+    @pytest.mark.parametrize('pad', [None, dt.timedelta(days=1)])
+    def test_basic_instrument_load_no_data(self, caplog, pad):
+        """Test Instrument load with no data for appropriate log messages.
+
+        Parameters
+        ----------
+        pad : dt.timedelta, pds.DateOffset, NoneType
+            Pad input for load call
+
+        """
 
         # Get a date that is not covered by an Instrument object.
         no_data_d = self.testInst.files.files.index[0] - dt.timedelta(weeks=10)
 
         with caplog.at_level(logging.INFO, logger='pysat'):
 
             # Attempt to load data for a date with no data.
             # Test doesn't check against loading by filename since that produces
             # an error if there is no file. Loading by yr, doy no different
             # than date in this case.
-            self.testInst.load(date=no_data_d, use_header=True)
+            self.testInst.load(date=no_data_d, pad=pad, use_header=True)
 
         # Confirm by checking against caplog that metadata was
         # not assigned.
         captured = caplog.text
 
         assert captured.find("Metadata was not assigned as there") >= 0
 
@@ -342,57 +352,60 @@
         self.testInst.load(self.ref_time.year, self.ref_doy, use_header=True)
         self.eval_successful_load()
         return
 
     def test_basic_instrument_load_leap_year(self):
         """Test if the correct day is being loaded (Leap-Year)."""
 
+        if self.check_nonstandard_cadence():
+            pytest.skip("Test only makes sense for daily cadence")
+
         self.ref_time = dt.datetime(2008, 12, 31)
         self.ref_doy = 366
         self.testInst.load(self.ref_time.year, self.ref_doy, use_header=True)
         self.eval_successful_load()
         return
 
-    @pytest.mark.parametrize("operator,ref_time",
-                             [('next', dt.datetime(2008, 1, 1)),
-                              ('prev', dt.datetime(2010, 12, 31))])
-    def test_file_load_default(self, operator, ref_time):
+    @pytest.mark.parametrize("operator,ref_ind",
+                             [('next', 0), ('prev', -1)])
+    def test_file_load_default(self, operator, ref_ind):
         """Test if correct day loads by default when first invoking iteration.
 
         Parameters
         ----------
         operator : str
             Name of iterator to use.
-        ref_time : dt.datetime
-            Expected date to load when iteration is first invoked.
+        ref_time : int
+            Expected index to load when iteration is first invoked.
 
         """
 
         getattr(self.testInst, operator)()
 
         # Modify ref time since iterator changes load date.
-        self.ref_time = ref_time
+        self.ref_time = filter_datetime_input(
+            self.testInst.files.files.index[ref_ind])
         self.eval_successful_load()
         return
 
     @pytest.mark.parametrize("operator", [('next'), ('prev')])
     def test_file_load_bad_start_file(self, operator):
         """Test Error when starting iteration on a file not in iteration list.
 
         Parameters
         ----------
         operator : str
             Name of iterator to use.
 
         """
 
-        self.testInst.load(fname=self.testInst.files[12], use_header=True)
+        self.testInst.load(fname=self.testInst.files[1], use_header=True)
 
         # Set new bounds that do not include this date.
-        self.testInst.bounds = (self.testInst.files[9], self.testInst.files[20],
+        self.testInst.bounds = (self.testInst.files[0], self.testInst.files[2],
                                 2, 1)
         testing.eval_bad_input(getattr(self.testInst, operator), StopIteration,
                                'Unable to find loaded filename ')
         return
 
     @pytest.mark.parametrize("operator", [('next'), ('prev')])
     def test_file_load_bad_start_date(self, operator):
@@ -422,17 +435,15 @@
         # If mangle_file_date is true, index will not match exactly.
         # Find the closest point instead.
         ind = np.argmin(abs(self.testInst.files.files.index - self.ref_time))
         self.testInst.load(fname=self.testInst.files[ind], use_header=True)
         self.eval_successful_load()
         return
 
-    @pytest.mark.parametrize("operator,direction",
-                             [('next', 1),
-                              ('prev', -1)])
+    @pytest.mark.parametrize("operator,direction", [('next', 1), ('prev', -1)])
     def test_fname_load_default(self, operator, direction):
         """Test correct day loads when moving by day, starting with `fname`.
 
         Parameters
         ----------
         operator : str
             Name of iterator to use.
@@ -444,42 +455,48 @@
         # If mangle_file_date is true, index will not match exactly.
         # Find the closest point.
         ind = np.argmin(abs(self.testInst.files.files.index - self.ref_time))
         self.testInst.load(fname=self.testInst.files[ind], use_header=True)
         getattr(self.testInst, operator)()
 
         # Modify ref time since iterator changes load date.
-        self.ref_time = self.ref_time + direction * dt.timedelta(days=1)
+        foff = pds.tseries.frequencies.to_offset(
+            self.testInst.files.files.index.freqstr)
+        self.ref_time = self.ref_time + direction * foff
         self.eval_successful_load()
         return
 
     def test_filename_load(self):
         """Test if file is loadable by filename with no path."""
 
         self.testInst.load(fname=self.ref_time.strftime('%Y-%m-%d.nofile'),
                            use_header=True)
         self.eval_successful_load()
         return
 
     def test_filenames_load(self):
         """Test if files are loadable by filename range."""
 
-        stop_fname = self.ref_time + dt.timedelta(days=1)
+        foff = pds.tseries.frequencies.to_offset(
+            self.testInst.files.files.index.freqstr)
+        stop_fname = self.ref_time + foff
         stop_fname = stop_fname.strftime('%Y-%m-%d.nofile')
         self.testInst.load(fname=self.ref_time.strftime('%Y-%m-%d.nofile'),
                            stop_fname=stop_fname, use_header=True)
         assert self.testInst.index[0] == self.ref_time
-        assert self.testInst.index[-1] >= self.ref_time + dt.timedelta(days=1)
-        assert self.testInst.index[-1] <= self.ref_time + dt.timedelta(days=2)
+        assert self.testInst.index[-1] >= self.ref_time + foff
+        assert self.testInst.index[-1] <= self.ref_time + (2 * foff)
         return
 
     def test_filenames_load_out_of_order(self):
         """Test error raised if fnames out of temporal order."""
 
-        stop_fname = self.ref_time + dt.timedelta(days=1)
+        foff = pds.tseries.frequencies.to_offset(
+            self.testInst.files.files.index.freqstr)
+        stop_fname = self.ref_time + foff
         stop_fname = stop_fname.strftime('%Y-%m-%d.nofile')
         check_fname = self.ref_time.strftime('%Y-%m-%d.nofile')
         estr = '`stop_fname` must occur at a later date '
 
         testing.eval_bad_input(self.testInst.load, ValueError, estr,
                                input_kwargs={'fname': stop_fname,
                                              'stop_fname': check_fname,
@@ -569,16 +586,18 @@
             If True, sort variable names in pandas before concatenation.  If
             False, do not sort for pandas objects.  For xarray objects, rename
             the epoch if True.
 
         """
 
         # Load a data set to concatonate
-        self.testInst.load(self.ref_time.year, self.ref_doy + 1,
-                           use_header=True)
+        ref_time2 = self.ref_time + pds.tseries.frequencies.to_offset(
+            self.testInst.files.files.index.freqstr)
+        doy2 = int(ref_time2.strftime('%j'))
+        self.testInst.load(ref_time2.year, doy2, use_header=True)
         data2 = self.testInst.data
         len2 = len(self.testInst.index)
 
         # Load a different data set into the instrument
         self.testInst.load(self.ref_time.year, self.ref_doy, use_header=True)
         len1 = len(self.testInst.index)
 
@@ -692,19 +711,32 @@
         """
 
         self.testInst.load(self.ref_time.year, self.ref_doy, use_header=True)
         assert np.all(self.testInst[index, 'mlt']
                       == self.testInst.data['mlt'][index])
         return
 
+    def test_data_access_by_row_slicing(self):
+        """Check that each variable is downsampled."""
+
+        self.testInst.load(self.ref_time.year, self.ref_doy, use_header=True)
+        result = self.testInst[0:10]
+        for variable, array in result.items():
+            assert len(array) == len(self.testInst.data[variable].values[0:10])
+            assert np.all(array == self.testInst.data[variable].values[0:10])
+        return
+
     def test_data_access_by_row_slicing_and_name_slicing(self):
         """Check that each variable is downsampled."""
 
+        if not self.testInst.pandas_format:
+            pytest.skip("name slicing not implemented for xarray")
+
         self.testInst.load(self.ref_time.year, self.ref_doy, use_header=True)
-        result = self.testInst[0:10, :]
+        result = self.testInst[0:10, 'uts':'mlt']
         for variable, array in result.items():
             assert len(array) == len(self.testInst.data[variable].values[0:10])
             assert np.all(array == self.testInst.data[variable].values[0:10])
         return
 
     def test_data_access_by_datetime_and_name(self):
         """Check that datetime can be used to access data."""
@@ -762,14 +794,15 @@
 
     def test_setting_data_by_name_single_element(self):
         """Test setting data by name for a single element."""
 
         self.testInst.load(self.ref_time.year, self.ref_doy, use_header=True)
         self.testInst['doubleMLT'] = 2.
         assert np.all(self.testInst['doubleMLT'] == 2.)
+        assert len(self.testInst['doubleMLT']) == len(self.testInst.index)
 
         self.testInst['nanMLT'] = np.nan
         assert np.all(np.isnan(self.testInst['nanMLT']))
         return
 
     def test_setting_data_by_name_with_meta(self):
         """Test setting data by name with meta."""
```

### Comparing `pysat-3.0.6/pysat/tests/classes/cls_instrument_integration.py` & `pysat-3.1.0/pysat/tests/classes/cls_instrument_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     `pysat.tests.test_instrument`
 
     """
 
     def test_no_stale_data_paths(self, caplog):
         """Ensure stale data paths aren't retained by pysat.Instrument.files."""
 
+        if 'file_date_range' in self.testInst.kwargs['list_files']:
+            pytest.skip("Cannot run eval on pds.DatetimeIndex")
+
         inst_str = repr(self.testInst)
         inst_str = inst_str.replace('update_files=True', 'update_files=False')
         self.testInst = eval(inst_str)
 
         # There should still be a list of files
         assert len(self.testInst.files.files) > 0
```

### Comparing `pysat-3.0.6/pysat/tests/classes/cls_instrument_iteration.py` & `pysat-3.1.0/pysat/tests/test_orbits.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,966 +1,1102 @@
-"""Tests for iteration in the pysat Instrument object and methods.
-
-Note
-----
-Base class stored here, but tests inherited by test_instrument.py
-
-"""
+#!/usr/bin/env python
+# Full license can be found in License.md
+# Full author list can be found in .zenodo.json file
+# DOI:10.5281/zenodo.1199703
+# ----------------------------------------------------------------------------
+"""Test the pysat routines for the orbits class."""
 
 import datetime as dt
+from dateutil.relativedelta import relativedelta
 import numpy as np
 
 import pandas as pds
+# Orbits period is a pandas.Timedelta kwarg, and the pandas repr
+# does not include a module name. Import required to run eval
+# on Orbit representation
+from pandas import Timedelta  # noqa: F401
 import pytest
 
 import pysat
 from pysat.utils import testing
-from pysat.utils.time import filter_datetime_input
 
 
-class InstIterationTests(object):
-    """Basic tests for `pysat.Instrument` iteration methods.
+def filter_data(inst, times):
+    """Remove data from instrument, simulating gaps in the data set.
 
-    Note
-    ----
-    Inherited by classes in test_instrument.py.  Setup and teardown methods are
-    specified there.
+    Parameters
+    ----------
+    inst : pysat.Instrument
+        The instrument to be filtered
+    times : array of dt.datetimes
+        A (2, N) array consisting of the start and stop of each gap in a list of
+        N gaps
 
-    See Also
-    --------
-    `pysat.tests.test_instrument`
+    """
+
+    for time in times:
+        idx, = np.where((inst.index > time[1]) | (inst.index < time[0]))
+        inst.data = inst[idx]
+    return
+
+
+def assert_reversible_orbit(inst, iterations):
+    """Check that an orbit breaks at the same points in both directions.
+
+    Parameters
+    ----------
+    inst : pysat.Instrument
+        The instrument to be checked
+    iterations : int
+        The number of orbits to check in each direction
 
     """
 
-    def generate_fname(self, date):
-        """Generate a filename for support of testing iterations.
+    n_time = []
+    p_time = []
+    control = inst.copy()
+    for j in range(iterations):
+        n_time.append(inst.index[0])
+        inst.orbits.next()
+    for j in range(iterations):
+        inst.orbits.prev()
+        p_time.append(inst.index[0])
+
+    assert all(control.data == inst.data)
+
+    # Don't check breaks for long gap.  See #861
+    if iterations < 30:
+        assert np.all(p_time == n_time[::-1])
+    return
+
+
+def assert_reversible_orbit_symmetric(inst, iterations):
+    """Check that an orbit breaks at the same points around a day cutoff.
+
+    Parameters
+    ----------
+    inst : pysat.Instrument
+        The instrument to be checked
+    iterations : int
+        The number of orbits to check in each direction
 
-        Parameters
-        ----------
-        date : dt.datetime
-            A date to be converted to a filename.
+    """
 
-        Returns
-        -------
-        filename : str
-            Filename formatted to look like test instrument files.
+    control = inst.copy()
+    for j in range(iterations):
+        inst.orbits.next()
 
-        """
+    for j in range(2 * iterations):
+        inst.orbits.prev()
 
-        fname = '{year:04d}-{month:02d}-{day:02d}.nofile'
-        return fname.format(year=date.year, month=date.month, day=date.day)
+    for j in range(iterations):
+        inst.orbits.next()
+    assert all(control.data == inst.data)
+    return
 
-    def eval_iter_list(self, start, stop, dates=False, freq=None):
-        """Evaluate successful generation of iter_list for `self.testInst`.
 
-        Parameters
-        ----------
-        start : dt.datetime or list of dt.datetime
-            Start date for generating iter_list.
-        stop : dt.datetime or list of dt.datetime
-            start date for generating iter_list.
-        dates : bool
-            If True, checks each date.  If False, checks against the _iter_list
-            (default=False)
-        freq : int or NoneType
-            Frequency in days.  If None, use pandas default. (default=None)
+class TestOrbitsUserInterface(object):
+    """Tests the user interface for orbits, including error handling."""
 
-        """
+    def setup_method(self):
+        """Set up User Interface unit tests."""
 
-        kwargs = {'freq': '{:}D'.format(freq)} if freq else {}
+        self.in_args = ['pysat', 'testing']
+        self.in_kwargs = {'clean_level': 'clean', 'update_files': True}
+        self.testInst = None
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        return
 
-        if isinstance(start, dt.datetime):
-            out = pds.date_range(start, stop, **kwargs).tolist()
-        else:
-            out = list()
-            for (istart, istop) in zip(start, stop):
-                out.extend(pds.date_range(istart, istop, **kwargs).tolist())
-        if dates:
-            dates = []
-            for inst in self.testInst:
-                dates.append(inst.date)
-            pysat.utils.testing.assert_lists_equal(dates, out)
-        else:
-            pysat.utils.testing.assert_lists_equal(self.testInst._iter_list,
-                                                   out)
+    def teardown_method(self):
+        """Tear down User Interface tests."""
+
+        del self.in_args, self.in_kwargs, self.testInst, self.stime
+        return
+
+    def test_orbit_w_bad_kind(self):
+        """Test orbit failure with bad 'kind' input."""
+
+        self.in_kwargs['orbit_info'] = {'index': 'mlt', 'kind': 'cats'}
+
+        testing.eval_bad_input(pysat.Instrument, ValueError,
+                               "Unknown kind of orbit requested", self.in_args,
+                               self.in_kwargs)
         return
 
-    def support_iter_evaluations(self, starts, stops, step, width,
-                                 for_loop=False, reverse=False, by_date=True):
-        """Support testing of `.next()`/`.prev()` via dates/files.
+    @pytest.mark.parametrize("info", [({'index': 'magnetic local time',
+                                        'kind': 'longitude'}),
+                                      ({'index': 'magnetic local time',
+                                        'kind': 'lt'}),
+                                      ({'index': 'magnetic local time',
+                                       'kind': 'polar'}),
+                                      ({'index': 'magnetic local time',
+                                        'kind': 'orbit'})])
+    def test_orbit_w_bad_orbit_info(self, info):
+        """Test orbit failure on iteration with orbit initialization.
 
         Parameters
         ----------
-        starts : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        stops : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        step : int
-            The step size for the iteration bounds.
-        width : int
-            The width of the iteration bounds.
-        for_loop : bool
-            If True, iterate via for loop.  If False, iterate via while.
-            (default=False)
-        reverse : bool
-            Direction of iteration.  If True, use `.prev()`. If False, use
-            `.next()`.  (default=False)
-        by_date : bool
-            If True, set bounds by date.  If False, set bounds by filename.
-            (default=False)
-
+        info : dict
+            Passed to Instrument as `orbit_info`
         """
 
-        # Ensure dates are lists for consistency of later code.
-        starts = pysat.utils.listify(starts)
-        stops = pysat.utils.listify(stops)
-
-        if by_date:
-            # Convert step and width to string and timedelta.
-            step = '{:}D'.format(step)
-            width = dt.timedelta(days=width)
-            self.testInst.bounds = (starts, stops, step, width)
-        else:
-            # Convert start and stop to filenames.
-            start_files = [self.generate_fname(date) for date in starts]
-            stop_files = [self.generate_fname(date) for date in stops]
-            self.testInst.bounds = (start_files, stop_files, step, width)
-
-        # Iterate until we run out of bounds
-        dates = []
-        time_range = []
-        if for_loop:
-            # Iterate via for loop option
-            for inst in self.testInst:
-                dates.append(inst.date)
-                time_range.append((inst.index[0],
-                                   inst.index[-1]))
-        else:
-            # Iterate forwards or backwards using `.next()` or `.prev()`
-            if reverse:
-                iterator = self.testInst.prev
-            else:
-                iterator = self.testInst.next
-            try:
-                while True:
-                    iterator()
-                    dates.append(self.testInst.date)
-                    time_range.append((self.testInst.index[0],
-                                       self.testInst.index[-1]))
-            except StopIteration:
-                # Reached the end
-                pass
-
-        # Deal with file or date iteration, make file inputs same as date for
-        # verification purposes.
-        if isinstance(step, int):
-            step = str(step) + 'D'
-        if isinstance(width, int):
-            width = dt.timedelta(days=width)
-
-        out = []
-        for start, stop in zip(starts, stops):
-            tdate = stop - width + dt.timedelta(days=1)
-            out.extend(pds.date_range(start, tdate, freq=step).tolist())
-        if reverse:
-            # Ensure time order is consistent for verify methods.
-            out = out[::-1]
-        pysat.utils.testing.assert_lists_equal(dates, out)
-
-        output = {}
-        output['expected_times'] = out
-        output['observed_times'] = time_range
-        output['starts'] = starts
-        output['stops'] = stops
-        output['width'] = width
-        output['step'] = step
-        return output
+        self.in_kwargs['orbit_info'] = info
+        self.in_kwargs['use_header'] = True
+        self.testInst = pysat.Instrument(*self.in_args, **self.in_kwargs)
+        self.testInst.load(date=self.stime)
 
-    def verify_iteration(self, out, reverse=False, inclusive=True):
-        """Verify loaded dates for iteration, forward or backward.
+        testing.eval_bad_input(self.testInst.orbits.next, ValueError,
+                               "Provided orbit index does not exist")
+        return
+
+    @pytest.mark.parametrize("info", [(None),
+                                      ({'index': 'magnetic local time',
+                                        'kind': 'polar'}),
+                                      ({'index': 'magnetic local time',
+                                        'kind': 'orbit'}),
+                                      ({'index': 'magnetic local time',
+                                        'kind': 'longitude'}),
+                                      ({'index': 'magnetic local time',
+                                        'kind': 'lt'})])
+    def test_orbit_polar_w_missing_orbit_index(self, info):
+        """Test orbit failure on iteration with missing orbit index.
 
         Parameters
         ----------
-        reverse : bool
-            If True, use move backwards through the list. If False, move
-            forwards. (default=False)
-        inclusive : bool
-            If True, check that end of bounds is included in iterated dates.
-            If False, check that end of bounds is excluded from iterated dates.
-            (default=True)
+        info : dict
+            Updated value information for Instrument kwarg 'orbit_info'
 
         """
 
-        # Inclusive checks require shifting some expected dates by 1.
-        delta_inc = dt.timedelta(days=1) if inclusive else dt.timedelta(days=0)
+        self.in_kwargs['orbit_info'] = info
+        self.in_kwargs['use_header'] = True
+        self.testInst = pysat.Instrument(*self.in_args, **self.in_kwargs)
+
+        # Force index to None beforee loading and iterating
+        self.testInst.orbits.orbit_index = None
+        self.testInst.load(date=self.stime)
+        testing.eval_bad_input(self.testInst.orbits.next, ValueError,
+                               "Orbit properties must be defined")
+        return
+
+    def test_orbit_repr(self):
+        """Test the Orbit representation."""
 
-        # Verify range of loaded data for each iteration step.
-        for i, trange in enumerate(out['observed_times']):
-            # Determine the current range.
-            b_range = 0
-            while out['expected_times'][i] > out['stops'][b_range]:
-                b_range += 1
-
-            # Check that loaded range is correct.
-            assert trange[0] == out['expected_times'][i], \
-                "Loaded start time is not correct"
-
-            check = out['expected_times'][i] + out['width']
-            check -= dt.timedelta(days=1)
-            assert trange[1] > check, "End time lower than expected"
-
-            check = out['stops'][b_range] + delta_inc
-            assert trange[1] < check, "End time higher than expected"
-
-            if reverse:
-                end_of_range = out['stops'][b_range] + dt.timedelta(days=1)
-                assert trange[1] < end_of_range, "End time higher than expected"
-                if i == 0:
-                    # Check that first load is before end of bounds.
-                    check = out['stops'][b_range] - out['width']
-                    check += dt.timedelta(days=1)
-
-                    if inclusive:
-                        assert trange[0] == check, \
-                            "Incorrect start time"
-                        assert trange[1] > out['stops'][b_range], \
-                            "Stop time lower than expected"
-                    else:
-                        assert trange[0] < check, \
-                            "Start time higher than expected"
-
-                    check = out['stops'][b_range] + delta_inc
-                    assert trange[1] < check, \
-                        "Stop time higher than expected"
-                elif i == (len(out['observed_times']) - 1):
-                    # Check that last load is at start of bounds.
-                    assert trange[0] == out['starts'][b_range], \
-                        "Loaded start time is not correct"
-                    assert trange[1] > out['starts'][b_range], \
-                        "End time lower than expected"
-                    assert trange[1] < out['starts'][b_range] + out['width'], \
-                        "End time higher than expected"
+        self.in_kwargs['orbit_info'] = {'index': 'mlt'}
+        self.in_kwargs['use_header'] = True
+        self.testInst = pysat.Instrument(*self.in_args, **self.in_kwargs)
+        out_str = self.testInst.orbits.__repr__()
 
+        assert out_str.find("Orbits(") >= 0
         return
 
-    @pytest.mark.parametrize("operator", [('next'), ('prev')])
-    def test_file_load_empty_iteration(self, operator):
-        """Ensure empty iteration list is fine via day iteration.
+    def test_orbit_str(self):
+        """Test the Orbit string representation with data."""
 
-        Parameters
-        ----------
-        operator : str
-            Name of iterator to use.
+        self.in_kwargs['orbit_info'] = {'index': 'mlt'}
+        self.in_kwargs['use_header'] = True
+        self.testInst = pysat.Instrument(*self.in_args, **self.in_kwargs)
+        self.testInst.load(date=self.stime)
+        out_str = self.testInst.orbits.__str__()
 
-        """
+        assert out_str.find("Orbit Settings") >= 0
+        assert out_str.find("Orbit Lind: local time") < 0
+        return
 
-        self.testInst.bounds = (None, None, '10000D',
-                                dt.timedelta(days=10000))
-        testing.eval_bad_input(getattr(self.testInst, operator), StopIteration,
-                               'File list is empty. ')
 
+class TestSpecificUTOrbits(object):
+    """Run the tests for specific behaviour in the MLT orbits."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'mlt'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.inc_min = 97
+        self.etime = None
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime, self.inc_min, self.etime
         return
 
-    @pytest.mark.parametrize("first,second", [('next', 'prev'),
-                                              ('prev', 'next')])
-    def test_passing_bounds_with_iteration(self, first, second):
-        """Test if passing bounds raises StopIteration.
+    @pytest.mark.parametrize('orbit_inc', [(0), (1), (-1), (-2), (14)])
+    def test_single_orbit_call_by_index(self, orbit_inc):
+        """Test successful orbit call by index.
 
         Parameters
         ----------
-        first : str
-            Name of first iterator to use.
-        second : str
-            Name of second iterator to use, should be in the opposite direction.
+        orbit_inc : int
+            Orbit index value
 
         """
 
-        # Load first data
-        getattr(self.testInst, first)()
-        testing.eval_bad_input(getattr(self.testInst, second), StopIteration,
-                               "Outside the set date boundaries")
-        return
-
-    def test_set_bounds_with_frequency(self):
-        """Test setting bounds with non-default step."""
-
-        start = self.ref_time
-        stop = self.ref_time + dt.timedelta(days=14)
-        self.testInst.bounds = (start, stop, 'M')
-        assert np.all(self.testInst._iter_list
-                      == pds.date_range(start, stop, freq='M').tolist())
-        return
-
-    def test_iterate_bounds_with_frequency(self):
-        """Test iterating bounds with non-default step."""
-
-        start = self.ref_time
-        stop = self.ref_time + dt.timedelta(days=15)
-        self.testInst.bounds = (start, stop, '2D')
-        self.eval_iter_list(start, stop, dates=True, freq=2)
-        return
-
-    def test_set_bounds_with_frequency_and_width(self):
-        """Set date bounds with step/width > 1."""
-
-        start = self.ref_time
-        stop = self.ref_time + pds.DateOffset(months=11, days=25)
-        stop = stop.to_pydatetime()
-        self.testInst.bounds = (start, stop, '10D', dt.timedelta(days=10))
-        assert np.all(self.testInst._iter_list
-                      == pds.date_range(start, stop, freq='10D').tolist())
-        return
-
-    # TODO(#863): Remove hardwired dates and streamline here and below
-    # TODO(#902): Combine inclusive and exclusive tests via parametrize
-    @pytest.mark.parametrize(
-        "starts,stops,step,width",
-        [(dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 3), 2, 2),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 4), 2, 3),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 5), 3, 1),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 17), 5, 1)])
-    @pytest.mark.parametrize("by_date", [True, False])
-    def test_iterate_bounds_with_frequency_and_width(self, starts, stops, step,
-                                                     width, by_date):
-        """Test iterate via date with mixed step/width, excludes stop date.
+        # Load the data
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits[orbit_inc]
+
+        # Increment the time
+        if orbit_inc >= 0:
+            self.stime += dt.timedelta(minutes=orbit_inc * self.inc_min)
+        else:
+            self.stime += dt.timedelta(minutes=self.inc_min
+                                       * (np.ceil(1440.0 / self.inc_min)
+                                          + orbit_inc))
+        self.etime = self.stime + dt.timedelta(seconds=(self.inc_min * 60 - 1))
+
+        # Test the time
+        assert (self.testInst.index[0] == self.stime)
+        assert (self.testInst.index[-1] == self.etime)
+        return
+
+    @pytest.mark.parametrize("orbit_ind,raise_err,err_msg", [
+        (17, ValueError, 'Requested an orbit past total'),
+        (None, TypeError, 'not supported between instances of')])
+    def test_single_orbit_call_bad_index(self, orbit_ind, raise_err, err_msg):
+        """Test orbit failure with bad index.
 
         Parameters
         ----------
-        starts : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        stops : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        step : int
-            The step size for the iteration bounds.
-        width : int
-            The width of the iteration bounds.
-        by_date : bool
-            If True, iterate by date.  If False, iterate by filename.
-
+        orbit_ind : int
+            Orbit index value
+        raise_err : Error
+            Error that should be raised
+        err_msg : str
+            Error string that should be raised
         """
 
-        out = self.support_iter_evaluations(starts, stops, step, width,
-                                            for_loop=True,
-                                            by_date=by_date)
-        self.verify_iteration(out, reverse=False, inclusive=False)
+        self.testInst.load(date=self.stime)
+        with pytest.raises(raise_err) as err:
+            self.testInst.orbits[orbit_ind]
 
+        assert str(err).find(err_msg) >= 0, '{:s} not found in {:s}'.format(
+            err_msg, str(err))
         return
 
-    @pytest.mark.parametrize(
-        "starts,stops,step,width",
-        [(dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 4), 2, 2),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 4), 3, 1),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 4), 1, 4),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 5), 4, 1),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 5), 2, 3),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 5), 3, 2)])
-    @pytest.mark.parametrize("by_date", [True, False])
-    def test_iterate_bounds_with_frequency_and_width_incl(self, starts, stops,
-                                                          step, width, by_date):
-        """Test iterate via date with mixed step/width, includes stop date.
+    def test_orbit_number_via_current_multiple_orbit_calls_in_day(self):
+        """Test orbit number with multiple orbits calls in a day."""
 
-        Parameters
-        ----------
-        starts : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        stops : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        step : int
-            The step size for the iteration bounds.
-        width : int
-            The width of the iteration bounds.
-        by_date : bool
-            If True, iterate by date.  If False, iterate by filename.
+        self.testInst.load(date=self.stime)
+        self.testInst.bounds = (self.stime, None)
+        true_vals = np.arange(15)
+        true_vals[-1] = 0
+        test_vals = []
+        for i, inst in enumerate(self.testInst.orbits):
+            if i > 14:
+                break
+            test_vals.append(inst.orbits.current)
+            assert inst.orbits.current == self.testInst.orbits.current
 
-        """
+        assert np.all(test_vals == true_vals)
+        return
+
+    def test_all_single_orbit_calls_in_day(self):
+        """Test all single orbit calls in a day."""
 
-        out = self.support_iter_evaluations(starts, stops, step, width,
-                                            for_loop=True, by_date=by_date)
-        self.verify_iteration(out, reverse=False, inclusive=True)
+        self.testInst.load(date=self.stime)
+        self.testInst.bounds = (self.stime, None)
+        for i, inst in enumerate(self.testInst.orbits):
+            if i > 14:
+                break
 
+            # Test the start index
+            self.etime = self.stime + i * relativedelta(minutes=self.inc_min)
+            assert inst.index[0] == self.etime
+            assert self.testInst.index[0] == self.etime
+
+            # Test the end index
+            self.etime += relativedelta(seconds=((self.inc_min * 60) - 1))
+            assert inst.index[-1] == self.etime
+            assert self.testInst.index[-1] == self.etime
         return
 
-    @pytest.mark.parametrize(
-        "starts,stops,step,width",
-        [(dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10), 2, 2),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 9), 4, 1),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 11), 1, 3),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 11), 1, 11)])
-    @pytest.mark.parametrize("reverse", [True, False])
-    @pytest.mark.parametrize("by_date", [True, False])
-    def test_iterate_with_frequency_and_width_incl(self, starts, stops, step,
-                                                   width, reverse, by_date):
-        """Test iteration via date step/width >1, includes stop date.
+    def test_orbit_next_call_no_loaded_data(self):
+        """Test orbit next call without loading data."""
 
-        Parameters
-        ----------
-        starts : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        stops : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        step : int
-            The step size for the iteration bounds.
-        width : int
-            The width of the iteration bounds.
-        reverse : bool
-            If True, iterate backwards.  If False, iterate forwards.
-        by_date : bool
-            If True, iterate by date.  If False, iterate by filename.
+        self.testInst.orbits.next()
+        assert (self.testInst.index[0] == dt.datetime(2008, 1, 1))
+        assert (self.testInst.index[-1] == dt.datetime(2008, 1, 1, 0, 38, 59))
+        return
 
-        """
+    def test_orbit_prev_call_no_loaded_data(self):
+        """Test orbit previous call without loading data."""
 
-        out = self.support_iter_evaluations(starts, stops, step, width,
-                                            reverse=reverse, by_date=by_date)
-        self.verify_iteration(out, reverse=reverse, inclusive=True)
+        self.testInst.orbits.prev()
 
+        # This isn't a full orbit
+        assert (self.testInst.index[-1]
+                == dt.datetime(2010, 12, 31, 23, 59, 59))
+        assert (self.testInst.index[0] == dt.datetime(2010, 12, 31, 23, 49))
         return
 
-    @pytest.mark.parametrize(
-        "starts,stops,step,width",
-        [(dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 11), 2, 2),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 12), 2, 3),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 13), 3, 2),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 3), 4, 2),
-         (dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 12), 2, 1)])
-    @pytest.mark.parametrize("reverse", [True, False])
-    @pytest.mark.parametrize("by_date", [True, False])
-    def test_iterate_with_frequency_and_width(self, starts, stops, step, width,
-                                              reverse, by_date):
-        """Test iteration with step and width excluding stop date.
+    def test_single_orbit_call_orbit_starts_0_UT_using_next(self):
+        """Test orbit next call with data."""
 
-        Parameters
-        ----------
-        starts : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        stops : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        step : int
-            The step size for the iteration bounds.
-        width : int
-            The width of the iteration bounds.
-        reverse : bool
-            If True, iterate backwards.  If False, iterate forwards.
-        by_date : bool
-            If True, iterate by date.  If False, iterate by filename.
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits.next()
+        self.etime = self.stime + dt.timedelta(seconds=(self.inc_min * 60 - 1))
+        assert (self.testInst.index[0] == self.stime)
+        assert (self.testInst.index[-1] == self.etime)
+        return
 
-        """
+    def test_single_orbit_call_orbit_starts_0_UT_using_prev(self):
+        """Test orbit prev call with data."""
 
-        out = self.support_iter_evaluations(starts, stops, step, width,
-                                            reverse=reverse, by_date=by_date)
-        self.verify_iteration(out, reverse=reverse, inclusive=False)
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits.prev()
+        self.stime += 14 * relativedelta(minutes=self.inc_min)
+        self.etime = self.stime + dt.timedelta(seconds=((self.inc_min * 60)
+                                                        - 1))
+        assert self.testInst.index[0] == self.stime
+        assert self.testInst.index[-1] == self.etime
+        return
+
+    def test_single_orbit_call_orbit_starts_off_0_UT_using_next(self):
+        """Test orbit next call with data for previous day."""
 
+        self.stime -= dt.timedelta(days=1)
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits.next()
+        assert (self.testInst.index[0] == dt.datetime(2008, 12, 30, 23, 45))
+        assert (self.testInst.index[-1]
+                == (dt.datetime(2008, 12, 30, 23, 45)
+                    + relativedelta(seconds=(self.inc_min * 60 - 1))))
         return
 
-    @pytest.mark.parametrize(
-        "starts,stops,step,width",
-        [([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 4), dt.datetime(2009, 1, 13)], 2, 2),
-         ([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 7), dt.datetime(2009, 1, 16)], 3, 1),
-         ([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 6), dt.datetime(2009, 1, 15)], 2, 4)])
-    @pytest.mark.parametrize("reverse", [True, False])
-    @pytest.mark.parametrize("by_date", [True, False])
-    def test_iterate_season_frequency_and_width_incl(self, starts, stops, step,
-                                                     width, reverse, by_date):
-        """Test iteration via date season step/width > 1, include stop date.
+    def test_single_orbit_call_orbit_starts_off_0_UT_using_prev(self):
+        """Test orbit previous call with data for previous day."""
 
-        Parameters
-        ----------
-        starts : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        stops : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        step : int
-            The step size for the iteration bounds.
-        width : int
-            The width of the iteration bounds.
-        reverse : bool
-            If True, iterate backwards.  If False, iterate forwards.
-        by_date : bool
-            If True, iterate by date.  If False, iterate by filename.
+        self.stime -= dt.timedelta(days=1)
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits.prev()
+        assert (self.testInst.index[0]
+                == (dt.datetime(2009, 1, 1)
+                    - relativedelta(minutes=self.inc_min)))
+        assert (self.testInst.index[-1]
+                == (dt.datetime(2009, 1, 1) - relativedelta(seconds=1)))
+        return
 
-        """
 
-        out = self.support_iter_evaluations(starts, stops, step, width,
-                                            reverse=reverse, by_date=by_date)
-        self.verify_iteration(out, reverse=reverse, inclusive=True)
+class TestGeneralOrbitsMLT(object):
+    """Run the general orbit tests by MLT for pandas."""
 
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'mlt'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
         return
 
-    @pytest.mark.parametrize(
-        "starts,stops,step,width",
-        [([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 3), dt.datetime(2009, 1, 12)], 2, 2),
-         ([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 6), dt.datetime(2009, 1, 15)], 3, 1),
-         ([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 7), dt.datetime(2009, 1, 16)], 2, 4)])
-    @pytest.mark.parametrize("reverse", [True, False])
-    @pytest.mark.parametrize("by_date", [True, False])
-    def test_iterate_season_frequency_and_width(self, starts, stops, step,
-                                                width, reverse, by_date):
-        """Test iteration via date season step/width>1, exclude stop date.
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
 
-        Parameters
-        ----------
-        starts : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        stops : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        step : int
-            The step size for the iteration bounds.
-        width : int
-            The width of the iteration bounds.
-        reverse : bool
-            If True, iterate backwards.  If False, iterate forwards.
-        by_date : bool
-            If True, iterate by date.  If False, iterate by filename.
+        del self.testInst, self.stime
+        return
 
-        """
+    def test_equality_with_copy(self):
+        """Test that copy is the same as original."""
+
+        self.out = self.testInst.orbits.copy()
+        assert self.out == self.testInst.orbits
+        return
 
-        out = self.support_iter_evaluations(starts, stops, step, width,
-                                            reverse=reverse, by_date=by_date)
-        self.verify_iteration(out, reverse=reverse, inclusive=False)
+    def test_equality_with_data_with_copy(self):
+        """Test that copy is the same as original if data is loaded."""
 
+        # Load data
+        self.testInst.load(date=self.stime)
+
+        # Load up an orbit
+        self.testInst.orbits[0]
+        self.out = self.testInst.orbits.copy()
+
+        assert self.out == self.testInst.orbits
         return
 
-    @pytest.mark.parametrize("new_bounds,errmsg",
-                             [([dt.datetime(2009, 1, 1)],
-                               "Must supply both a start and stop date/file"),
-                              ([dt.datetime(2009, 1, 1), '2009-01-01.nofile'],
-                               "must all be of the same type"),
-                              ([dt.datetime(2009, 1, 1), 1],
-                               "must all be of the same type"),
-                              ([[dt.datetime(2009, 1, 1)] * 2,
-                                '2009-01-01.nofile'],
-                               "must have the same number of elements"),
-                              ([[dt.datetime(2009, 1, 1)] * 2,
-                               [dt.datetime(2009, 1, 1), '2009-01-01.nofile']],
-                               "must all be of the same type"),
-                              ([dt.datetime(2009, 1, 1),
-                                dt.datetime(2009, 1, 1), '1D',
-                                dt.timedelta(days=1), False],
-                               'Too many input arguments.')])
-    def test_set_bounds_error_message(self, new_bounds, errmsg):
-        """Test ValueError when setting bounds with wrong inputs.
+    def test_inequality_different_data(self):
+        """Test that equality is false if different data."""
 
-        Parameters
-        ----------
-        new_bounds : list
-            Defines new iteration bounds incorrectly.
-        err_msg : str
-            A string pattern that shoul be raised by defining the bounds as
-            in new_bounds.
+        # Load data
+        self.testInst.load(date=self.stime)
 
-        """
+        # Load up an orbit
+        self.testInst.orbits[0]
+
+        # Make copy
+        self.out = self.testInst.orbits.copy()
+
+        # Modify data
+        self.out._full_day_data = self.testInst._null_data
 
-        with pytest.raises(ValueError) as verr:
-            self.testInst.bounds = new_bounds
-        assert str(verr).find(errmsg) >= 0
+        assert self.out != self.testInst.orbits
         return
 
-    def test_set_bounds_string_default_start(self):
-        """Test set bounds with default start."""
+    def test_inequality_modified_object(self):
+        """Test that equality is false if other missing attributes."""
 
-        self.testInst.bounds = [None, '2009-01-01.nofile']
-        assert self.testInst.bounds[0][0] == self.testInst.files[0]
+        self.out = self.testInst.orbits.copy()
+
+        # Remove attribute
+        del self.out.orbit_index
+
+        assert self.testInst.orbits != self.out
         return
 
-    def test_set_bounds_string_default_stop(self):
-        """Test set bounds with default stop."""
+    def test_inequality_reduced_object(self):
+        """Test that equality is false if self missing attributes."""
 
-        self.testInst.bounds = ['2009-01-01.nofile', None]
-        assert self.testInst.bounds[1][0] == self.testInst.files[-1]
+        self.out = self.testInst.orbits.copy()
+        self.out.hi_there = 'hi'
+        assert self.testInst.orbits != self.out
         return
 
-    def test_set_bounds_by_default_dates(self):
-        """Verify bounds behavior with default date related inputs."""
+    def test_inequality_different_type(self):
+        """Test that equality is false if different type."""
 
-        start = self.testInst.files.start_date
-        stop = self.testInst.files.stop_date
-        self.testInst.bounds = (None, None)
-        self.eval_iter_list(start, stop)
-        self.testInst.bounds = None
-        self.eval_iter_list(start, stop)
-        self.testInst.bounds = (start, None)
-        self.eval_iter_list(start, stop)
-        self.testInst.bounds = (None, stop)
-        self.eval_iter_list(start, stop)
+        assert self.testInst.orbits != self.testInst
         return
 
-    @pytest.mark.parametrize("start,stop", [(dt.datetime(2009, 1, 1),
-                                             dt.datetime(2009, 1, 15)),
-                                            ([dt.datetime(2009, 1, 1),
-                                              dt.datetime(2009, 2, 1)],
-                                             [dt.datetime(2009, 1, 15),
-                                              dt.datetime(2009, 2, 15)])])
-    def test_set_bounds_by_date(self, start, stop):
-        """Test setting bounds with datetimes over simple range and season.
+    def test_eval_repr(self):
+        """Test eval of repr recreates object."""
 
-        Parameters
-        ----------
-        start : dt.datetime or list of dt.datetime
-            The start of the new bounds.
-        stop : dt.datetime or list of dt.datetime
-            The stop of the new bounds.
+        # Eval and repr don't play nice for custom functions
+        if len(self.testInst.custom_functions) != 0:
+            self.testInst.custom_clear()
 
-        """
+        self.out = eval(self.testInst.orbits.__repr__())
+        assert self.out == self.testInst.orbits
+        return
+
+    def test_repr_and_copy(self):
+        """Test repr consistent with object copy."""
 
-        self.testInst.bounds = (start, stop)
-        self.eval_iter_list(start, stop)
+        # Not tested with eval due to issues with datetime
+        self.out = self.testInst.orbits.__repr__()
+        second_out = self.testInst.orbits.copy().__repr__()
+        assert self.out == second_out
         return
 
-    @pytest.mark.parametrize("start,stop", [(dt.datetime(2009, 1, 15),
-                                             dt.datetime(2009, 1, 1)),
-                                            ([dt.datetime(2009, 1, 1),
-                                              dt.datetime(2009, 2, 1)],
-                                             [dt.datetime(2009, 1, 12),
-                                              dt.datetime(2009, 1, 15)])])
-    def test_set_bounds_by_date_wrong_order(self, start, stop):
-        """Test error if bounds assignment has stop date before start.
+    def test_load_orbits_w_empty_data(self):
+        """Test orbit loading outside of the instrument data range."""
 
-        Parameters
-        ----------
-        start : dt.datetime or list of dt.datetime
-            The start of the new bounds.
-        stop : dt.datetime or list of dt.datetime
-            The stop of the new bounds.
+        # Set up tine instrument
+        self.stime -= dt.timedelta(days=365 * 100)
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits[0]
 
-        """
+        # Trigger the StopIteration exception
+        testing.eval_bad_input(self.testInst.orbits.next, StopIteration,
+                               'Unable to find loaded date')
+        return
 
-        with pytest.raises(ValueError) as err:
-            self.testInst.bounds = (start, stop)
-        estr = 'Bounds must be set in increasing'
-        assert str(err).find(estr) >= 0
-        return
-
-    @pytest.mark.parametrize(
-        "start,stop", [(dt.datetime(2009, 1, 1, 1, 10),
-                        dt.datetime(2009, 1, 15, 1, 10)),
-                       ([dt.datetime(2009, 1, 1, 1, 10),
-                         dt.datetime(2009, 2, 1, 1, 10)],
-                        [dt.datetime(2009, 1, 15, 1, 10),
-                         dt.datetime(2009, 2, 15, 1, 10)])])
-    def test_set_bounds_by_date_extra_time(self, start, stop):
-        """Test set bounds by date with extra time.
-
-        Note
-        ----
-        Only the date portion is retained, hours and shorter timespans are
-        dropped.
+    def test_less_than_one_orbit_of_data(self):
+        """Test successful load with less than one orbit of data."""
 
-        Parameters
-        ----------
-        start : dt.datetime or list of dt.datetime
-            The start of the new bounds.
-        stop : dt.datetime or list of dt.datetime
-            The stop of the new bounds.
+        def truncate_data(inst):
+            """Local helper function to reduce available data."""
+            inst.data = inst[0:20]
 
-        """
+        self.testInst.custom_attach(truncate_data)
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits.next()
 
-        self.testInst.bounds = (start, stop)
-        start = filter_datetime_input(start)
-        stop = filter_datetime_input(stop)
-        self.eval_iter_list(start, stop)
-        return
-
-    @pytest.mark.parametrize("start,stop", [(dt.datetime(2010, 12, 1),
-                                             dt.datetime(2010, 12, 31)),
-                                            (dt.datetime(2009, 1, 1),
-                                             dt.datetime(2009, 1, 15)),
-                                            ([dt.datetime(2009, 1, 1),
-                                              dt.datetime(2009, 2, 1)],
-                                             [dt.datetime(2009, 1, 15),
-                                              dt.datetime(2009, 2, 15)]),
-                                            ([dt.datetime(2009, 1, 1, 1, 10),
-                                              dt.datetime(2009, 2, 1, 1, 10)],
-                                             [dt.datetime(2009, 1, 15, 1, 10),
-                                              dt.datetime(2009, 2, 15, 1, 10)])
-                                            ])
-    def test_iterate_over_bounds_set_by_date(self, start, stop):
-        """Test iterate over bounds via single date range.
+        # A recursion issue has been observed in this area.
+        # Checking for date to limit reintroduction potential.
+        assert self.testInst.date == self.stime
+        # Store comparison data
+        saved_data = self.testInst.copy()
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits[0]
+        assert all(self.testInst.data == saved_data.data)
+        d1check = self.testInst.date == saved_data.date
+        assert d1check
+        return
 
-        Parameters
-        ----------
-        start : dt.datetime or list of dt.datetime
-            The start of the new bounds.
-        stop : dt.datetime or list of dt.datetime
-            The stop of the new bounds.
+    def test_less_than_one_orbit_of_data_four_ways_two_days(self):
+        """Test successful loading of different partial orbits."""
 
-        """
+        # Create situation where the < 1 orbit split across two days
+        def manual_orbits(inst):
+            """Local function for breaking up orbits."""
+            if inst.date == dt.datetime(2009, 1, 5):
+                inst.data = inst[0:20]
+            elif inst.date == dt.datetime(2009, 1, 4):
+                inst.data = inst[-20:]
+            return
 
-        self.testInst.bounds = (start, stop)
-        # Filter time inputs.
-        start = filter_datetime_input(start)
-        stop = filter_datetime_input(stop)
-        self.eval_iter_list(start, stop, dates=True)
-        return
-
-    def test_iterate_over_default_bounds(self):
-        """Test iterate over default bounds."""
-
-        date_range = pds.date_range(self.ref_time,
-                                    self.ref_time + dt.timedelta(days=10))
-        self.testInst.kwargs['list_files']['file_date_range'] = date_range
-        self.testInst.files.refresh()
-        self.testInst.bounds = (None, None)
-        self.eval_iter_list(date_range[0], date_range[-1], dates=True)
-        return
-
-    @pytest.mark.parametrize(
-        "starts,stops,step,width",
-        [([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 3), dt.datetime(2009, 1, 12)], 2, 2),
-         ([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 6), dt.datetime(2009, 1, 15)], 3, 1),
-         ([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 7), dt.datetime(2009, 1, 16)], 2, 4)])
-    @pytest.mark.parametrize("by_date", [True, False])
-    def test_iterate_over_bounds_season_step_width(self, starts, stops, step,
-                                                   width, by_date):
-        """Test iterate over season, step/width > 1, exclude stop bounds.
+        self.testInst.custom_attach(manual_orbits)
+        self.stime += dt.timedelta(days=3)
+        self.testInst.load(date=self.stime)
 
-        Parameters
-        ----------
-        starts : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        stops : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        step : int
-            The step size for the iteration bounds.
-        width : int
-            The width of the iteration bounds.
-        by_date : bool
-            If True, iterate by date.  If False, iterate by filename.
+        # Starting from no orbit calls next loads first orbit
+        self.testInst.orbits.next()
 
-        """
+        # Store comparison data
+        saved_data = self.testInst.copy()
+        self.testInst.load(date=self.stime + dt.timedelta(days=1))
+        self.testInst.orbits[0]
+        if self.testInst.orbits.num == 1:
+            # Equivalence occurs only when there is one orbit,
+            # some test settings can violate this assumption.
+            assert all(self.testInst.data == saved_data.data)
 
-        out = self.support_iter_evaluations(starts, stops, step, width,
-                                            for_loop=True, by_date=by_date)
-        self.verify_iteration(out, reverse=False, inclusive=False)
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits[0]
+        assert all(self.testInst.data == saved_data.data)
 
+        self.testInst.load(date=self.stime + dt.timedelta(days=1))
+        self.testInst.orbits.prev()
+        if self.testInst.orbits.num == 1:
+            assert all(self.testInst.data == saved_data.data)
+
+        # A recursion issue has been observed in this area.
+        # Checking for date to limit reintroduction potential.
+        d1check = self.testInst.date == saved_data.date
+        assert d1check
         return
 
-    @pytest.mark.parametrize(
-        "starts,stops,step,width",
-        [([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 4), dt.datetime(2009, 1, 13)], 2, 2),
-         ([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 7), dt.datetime(2009, 1, 16)], 3, 1),
-         ([dt.datetime(2009, 1, 1), dt.datetime(2009, 1, 10)],
-          [dt.datetime(2009, 1, 6), dt.datetime(2009, 1, 15)], 2, 4)])
-    @pytest.mark.parametrize("by_date", [True, False])
-    def test_iterate_bounds_season_step_width_incl(self, starts, stops, step,
-                                                   width, by_date):
-        """Test iterate over season, step/width > 1, includes stop bounds.
+    @pytest.mark.parametrize("iterations", [(10), (20)])
+    def test_repeated_orbit_calls(self, iterations):
+        """Test that repeated orbit calls are reversible."""
 
-        Parameters
-        ----------
-        starts : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        stops : dt.datetime or list of dt.datetime
-            The start date for iterations, or dates for iteration over multiple
-            segments.
-        step : int
-            The step size for the iteration bounds.
-        width : int
-            The width of the iteration bounds.
-        by_date : bool
-            If True, iterate by date.  If False, iterate by filename.
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits.next()
+        assert_reversible_orbit(self.testInst, iterations)
+        return
 
-        """
+    @pytest.mark.parametrize("iterations", [(10), (20)])
+    def test_repeated_orbit_calls_alternative(self, iterations):
+        """Test repeated orbit calls are reversible using alternate pattern."""
+
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits.next()
+        assert_reversible_orbit_symmetric(self.testInst, iterations)
+        return
+
+
+class TestGeneralOrbitsMLTxarray(TestGeneralOrbitsMLT):
+    """Run the general orbit tests by MLT for xarray."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing_xarray',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'mlt'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing_xarray._test_dates['']['']
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime
+        return
+
+
+class TestGeneralOrbitsNonStandardIteration(object):
+    """Test for non standard data setups.
 
-        out = self.support_iter_evaluations(starts, stops, step, width,
-                                            for_loop=True, by_date=by_date)
-        self.verify_iteration(out, reverse=False, inclusive=True)
+    Note
+    ----
+    Create an iteration window that is larger than step size.
+    Ensure the overlapping data doesn't end up in the orbit iteration.
+
+    """
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'mlt'},
+                                         update_files=True,
+                                         use_header=True)
+        self.testInst.bounds = (self.testInst.files.files.index[0],
+                                self.testInst.files.files.index[11],
+                                '2D', dt.timedelta(days=3))
+        self.orbit_starts = []
+        self.orbit_stops = []
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
 
+        del self.testInst, self.orbit_starts, self.orbit_stops
         return
 
-    def test_set_bounds_by_fname(self):
-        """Test set bounds by fname."""
-
-        start = '2009-01-01.nofile'
-        stop = '2009-01-03.nofile'
-        self.testInst.bounds = (start, stop)
-        assert np.all(self.testInst._iter_list
-                      == ['2009-01-01.nofile', '2009-01-02.nofile',
-                          '2009-01-03.nofile'])
-        return
-
-    def test_iterate_over_bounds_set_by_fname(self):
-        """Test iterate over bounds set by fname."""
-
-        start = '2009-01-01.nofile'
-        stop = '2009-01-15.nofile'
-        start_d = dt.datetime(2009, 1, 1)
-        stop_d = dt.datetime(2009, 1, 15)
-        self.testInst.bounds = (start, stop)
-        self.eval_iter_list(start_d, stop_d, dates=True)
-        return
-
-    @pytest.mark.parametrize("start,stop", [('2009-01-13.nofile',
-                                             '2009-01-01.nofile'),
-                                            (['2009-01-01.nofile',
-                                              '2009-02-03.nofile'],
-                                             ['2009-01-03.nofile',
-                                              '2009-02-01.nofile'])])
-    def test_set_bounds_by_fname_wrong_order(self, start, stop):
-        """Test for error if stop file before start file.
+    def test_no_orbit_overlap_with_overlapping_iteration(self):
+        """Ensure error when overlap in iteration data."""
+
+        testing.eval_bad_input(self.testInst.orbits.next, ValueError,
+                               'Orbit iteration is not currently supported ')
+
+        return
+
+    @pytest.mark.parametrize("bounds_type", ['by_date', 'by_file'])
+    def test_no_orbit_overlap_with_nonoverlapping_iteration(self, bounds_type):
+        """Ensure orbit data does not overlap when overlap in iteration data.
 
         Parameters
         ----------
-        start : str or list of strs
-            The starting filename(s) for the new bounds.
-        stop : str or list of strs
-            The stop filename(s) for the new bounds.
+        bounds_type : str
+            Enforce bounds `by_date` or `by_file`
 
         """
 
-        with pytest.raises(ValueError) as err:
-            self.testInst.bounds = (start, stop)
-        estr = 'Bounds must be in increasing date'
-        assert str(err).find(estr) >= 0
+        if bounds_type == 'by_date':
+            bounds = (self.testInst.files.files.index[0],
+                      self.testInst.files.files.index[11],
+                      '2D', dt.timedelta(days=2))
+        elif bounds_type == 'by_file':
+            bounds = (self.testInst.files[0], self.testInst.files[11], 2, 2)
+
+        self.testInst.bounds = bounds
+
+        for inst in self.testInst.orbits:
+            self.orbit_starts.append(inst.index[0])
+            self.orbit_stops.append(inst.index[-1])
+        self.orbit_starts = pds.Series(self.orbit_starts)
+        self.orbit_stops = pds.Series(self.orbit_stops)
+        assert self.orbit_starts.is_monotonic_increasing
+        assert self.orbit_stops.is_monotonic_increasing
         return
 
-    @pytest.mark.parametrize("operator", ['next', 'prev'])
-    def test_iterate_over_bounds_set_by_fname_via_attr(self, operator):
-        """Test iterate over bounds set by fname via operators.
+
+class TestGeneralOrbitsLong(TestGeneralOrbitsMLT):
+    """Run the general orbit tests by Longitude for pandas."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'longitude',
+                                                     'kind': 'longitude'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime
+        return
+
+
+class TestGeneralOrbitsLongXarray(TestGeneralOrbitsMLT):
+    """Run the general orbit tests by Longitude for xarray."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing_xarray',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'longitude',
+                                                     'kind': 'longitude'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime
+        return
+
+
+class TestGeneralOrbitsOrbitNumber(TestGeneralOrbitsMLT):
+    """Run the general orbit tests by Orbit Number for pandas."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'orbit_num',
+                                                     'kind': 'orbit'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime
+        return
+
+
+class TestGeneralOrbitsOrbitNumberXarray(TestGeneralOrbitsMLT):
+    """Run the general orbit tests by Orbit Number for xarray."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing_xarray',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'orbit_num',
+                                                     'kind': 'orbit'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing_xarray._test_dates['']['']
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime
+        return
+
+
+class TestGeneralOrbitsLatitude(TestGeneralOrbitsMLT):
+    """Run the general orbit tests for orbits defined by Latitude for pandas."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'latitude',
+                                                     'kind': 'polar'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime
+        return
+
+
+class TestGeneralOrbitsLatitudeXarray(TestGeneralOrbitsMLT):
+    """Run the general orbit tests for orbits defined by Latitude for xarray."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing_xarray',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'latitude',
+                                                     'kind': 'polar'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing_xarray._test_dates['']['']
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime
+        return
+
+
+class TestOrbitsGappyData(object):
+    """Gappy orbit tests defined  for orbits defined by MLT for pandas."""
+
+    def setup_class(self):
+        """Set up variables inherited by all classes."""
+
+        self.deltime = np.array([[dt.timedelta(hours=1, minutes=37),
+                                  dt.timedelta(hours=3, minutes=14)],
+                                 [dt.timedelta(hours=10),
+                                  dt.timedelta(hours=12)],
+                                 [dt.timedelta(hours=22),
+                                  dt.timedelta(days=1, hours=2)],
+                                 [dt.timedelta(days=12),
+                                  dt.timedelta(days=14)],
+                                 [dt.timedelta(days=19, hours=1),
+                                  dt.timedelta(days=24, hours=23)],
+                                 [dt.timedelta(days=24, hours=23, minutes=30),
+                                  dt.timedelta(days=25, hours=3)]])
+
+    def teardown_class(self):
+        """Clean up variables inherited by all classes."""
+
+        del self.deltime
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'mlt'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.gaps = self.stime + self.deltime
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.gaps})
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime, self.gaps
+        return
+
+    @pytest.mark.parametrize("day,iterations", [(1, 20), (19, 45), (25, 20)])
+    def test_repeat_orbit_calls_cutoffs_with_gaps(self, day, iterations):
+        """Test that orbits are selected at same cutoffs when reversed.
 
         Parameters
         ----------
-        operator : str
-            Name of iterator to use.
+        day : int
+            Loads data for `self.stime` + `day` - 1
+        iterations : int
+            Number of iterations to test, passed to `assert_reversible_orbit`
 
         """
 
-        start = '2009-01-01.nofile'
-        stop = '2009-01-15.nofile'
-        start_d = dt.datetime(2009, 1, 1)
-        stop_d = dt.datetime(2009, 1, 15)
-        self.testInst.bounds = (start, stop)
-        dates = []
-        loop_next = True
-        while loop_next:
-            try:
-                getattr(self.testInst, operator)()
-                dates.append(self.testInst.date)
-            except StopIteration:
-                loop_next = False
-        out = pds.date_range(start_d, stop_d).tolist()
-        pysat.utils.testing.assert_lists_equal(dates, out)
-        return
-
-    def test_set_bounds_by_fname_season(self):
-        """Test set bounds by fname season."""
-
-        start = ['2009-01-01.nofile', '2009-02-01.nofile']
-        stop = ['2009-01-03.nofile', '2009-02-03.nofile']
-        self.testInst.bounds = (start, stop)
-        assert np.all(self.testInst._iter_list
-                      == ['2009-01-01.nofile', '2009-01-02.nofile',
-                          '2009-01-03.nofile', '2009-02-01.nofile',
-                          '2009-02-02.nofile', '2009-02-03.nofile'])
-        return
-
-    def test_iterate_over_bounds_set_by_fname_season(self):
-        """Test set bounds using multiple filenames."""
-
-        start = ['2009-01-01.nofile', '2009-02-01.nofile']
-        stop = ['2009-01-15.nofile', '2009-02-15.nofile']
-        start_d = [dt.datetime(2009, 1, 1), dt.datetime(2009, 2, 1)]
-        stop_d = [dt.datetime(2009, 1, 15), dt.datetime(2009, 2, 15)]
-        self.testInst.bounds = (start, stop)
-        self.eval_iter_list(start_d, stop_d, dates=True)
-        return
-
-    def test_set_bounds_fname_with_frequency(self):
-        """Test set bounds using filenames and non-default step."""
-
-        start = '2009-01-01.nofile'
-        start_date = dt.datetime(2009, 1, 1)
-        stop = '2009-01-03.nofile'
-        stop_date = dt.datetime(2009, 1, 3)
-        self.testInst.bounds = (start, stop, 2)
-        out = pds.date_range(start_date, stop_date, freq='2D').tolist()
-
-        # Convert filenames in list to a date
-        for i, item in enumerate(self.testInst._iter_list):
-            snip = item.split('.')[0]
-            ref_snip = out[i].strftime('%Y-%m-%d')
-            assert snip == ref_snip
-        return
-
-    def test_iterate_bounds_fname_with_frequency(self):
-        """Test iterate over bounds using filenames and non-default step."""
-
-        start = '2009-01-01.nofile'
-        start_date = dt.datetime(2009, 1, 1)
-        stop = '2009-01-03.nofile'
-        stop_date = dt.datetime(2009, 1, 3)
-        self.testInst.bounds = (start, stop, 2)
-
-        self.eval_iter_list(start_date, stop_date, dates=True, freq=2)
-        return
-
-    def test_set_bounds_fname_with_frequency_and_width(self):
-        """Test set fname bounds with step/width > 1."""
-
-        start = '2009-01-01.nofile'
-        start_date = dt.datetime(2009, 1, 1)
-        stop = '2009-01-03.nofile'
-        stop_date = dt.datetime(2009, 1, 3)
-        self.testInst.bounds = (start, stop, 2, 2)
-        out = pds.date_range(start_date, stop_date - dt.timedelta(days=1),
-                             freq='2D').tolist()
-        # Convert filenames in list to a date
-        date_list = []
-        for item in self.testInst._iter_list:
-            snip = item.split('.')[0]
-            date_list.append(dt.datetime.strptime(snip, '%Y-%m-%d'))
-        assert np.all(date_list == out)
+        # Start date offsets aligned to times defined in TestOrbitsGappyData
+        self.testInst.load(date=(self.stime + dt.timedelta(days=(day - 1))))
+        self.testInst.orbits.next()
+        assert_reversible_orbit(self.testInst, iterations)
         return
 
-    def test_iteration_in_list_comprehension(self):
-        """Test list comprehensions for length, uniqueness, iteration."""
 
-        self.testInst.bounds = (self.testInst.files.files.index[0],
-                                self.testInst.files.files.index[9])
-        # Ensure no data to begin
-        assert self.testInst.empty
-
-        # Perform comprehension and ensure there are as many as there should be
-        insts = [inst for inst in self.testInst]
-        assert len(insts) == 10
-
-        # Get list of dates
-        dates = pds.Series([inst.date for inst in insts])
-        assert dates.is_monotonic_increasing
-
-        # Dates are unique
-        assert np.all(np.unique(dates) == dates.values)
-
-        # Iteration instruments are not the same as original
-        for inst in insts:
-            assert not (inst is self.testInst)
+class TestOrbitsGappyDataXarray(TestOrbitsGappyData):
+    """Gappy orbit tests defined  for orbits defined by MLT for xarray."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing_xarray',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'mlt'},
+                                         update_files=True,
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.gaps = self.stime + self.deltime
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.gaps})
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime, self.gaps
+        return
+
+
+class TestOrbitsGappyData2(object):
+    """Additional gappy orbit tests for orbits defined by MLT for pandas."""
+
+    def setup_class(self):
+        """Set up variables inherited by all classes."""
+
+        self.times = [[dt.datetime(2008, 12, 31, 4),
+                       dt.datetime(2008, 12, 31, 5, 37)],
+                      [dt.datetime(2009, 1, 1),
+                       dt.datetime(2009, 1, 1, 1, 37)]]
+        for seconds in np.arange(38):
+            day = (dt.datetime(2009, 1, 2)
+                   + dt.timedelta(days=int(seconds)))
+            self.times.append([day, day
+                               + dt.timedelta(hours=1, minutes=37,
+                                              seconds=int(seconds))
+                               - dt.timedelta(seconds=20)])
+
+    def teardown_class(self):
+        """Clean up variables inherited by all classes."""
+
+        del self.times
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'mlt'},
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.times})
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime
+        return
+
+    def test_repeated_orbit_calls_alternative(self):
+        """Test repeated orbit calls are reversible."""
+
+        self.testInst.load(date=self.stime)
+        self.testInst.orbits.next()
+        assert_reversible_orbit_symmetric(self.testInst, 20)
+        return
+
+
+class TestOrbitsGappyData2Xarray(TestOrbitsGappyData2):
+    """Run additional gappy orbit tests for orbits defined by MLT for xarray."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing_xarray',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'mlt'},
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.times})
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime
+        return
+
+
+class TestOrbitsGappyLongData(TestOrbitsGappyData):
+    """Gappy orbit tests defined  for orbits defined by Longitude for pandas."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'longitude',
+                                                     'kind': 'longitude'},
+                                         use_header=True)
+
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.gaps = self.stime + self.deltime
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.gaps})
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime, self.gaps
+        return
+
+
+class TestOrbitsGappyLongDataXarray(TestOrbitsGappyData):
+    """Gappy orbit tests defined  for orbits defined by Longitude for xarray."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing_xarray',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'longitude',
+                                                     'kind': 'longitude'},
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.gaps = self.stime + self.deltime
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.gaps})
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime, self.gaps
+        return
+
+
+class TestOrbitsGappyOrbitNumData(TestOrbitsGappyData):
+    """Gappy orbit tests defined  by Orbit Number for pandas."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'orbit_num',
+                                                     'kind': 'orbit'},
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.gaps = self.stime + self.deltime
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.gaps})
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime, self.gaps
+        return
+
+
+class TestOrbitsGappyOrbitNumDataXarray(TestOrbitsGappyData):
+    """Gappy orbit tests defined  by Orbit Number for xarray."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing_xarray',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'orbit_num',
+                                                     'kind': 'orbit'},
+                                         use_header=True)
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.gaps = self.stime + self.deltime
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.gaps})
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime, self.gaps
+        return
+
+
+class TestOrbitsGappyOrbitLatData(TestOrbitsGappyData):
+    """Gappy orbit tests defined  by Latitude for pandas."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'latitude',
+                                                     'kind': 'polar'},
+                                         use_header=True)
+
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.gaps = self.stime + self.deltime
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.gaps})
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.stime, self.gaps
+        return
+
+
+class TestOrbitsGappyOrbitLatDataXarray(TestOrbitsGappyData):
+    """Gappy orbit tests defined by Latitude for xarray."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        self.testInst = pysat.Instrument('pysat', 'testing_xarray',
+                                         clean_level='clean',
+                                         orbit_info={'index': 'latitude',
+                                                     'kind': 'polar'},
+                                         use_header=True)
+
+        self.stime = pysat.instruments.pysat_testing._test_dates['']['']
+        self.gaps = self.stime + self.deltime
+        self.testInst.custom_attach(filter_data, kwargs={'times': self.gaps})
+        return
 
-        # Check there is data after iteration
-        assert not self.testInst.empty
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
 
+        del self.testInst, self.stime, self.gaps
         return
```

### Comparing `pysat-3.0.6/pysat/tests/classes/cls_instrument_library.py` & `pysat-3.1.0/pysat/tests/classes/cls_instrument_library.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
         '''
 
 """
 
 import datetime as dt
 from importlib import import_module
+import sys
 import tempfile
 import warnings
 
 import pytest
 
 import pysat
 from pysat.utils import generate_instrument_list
@@ -105,24 +106,37 @@
                   'inst_ids': dict, 'tag': str, 'inst_id': str,
                   'acknowledgements': str, 'references': str}
 
     def setup_class(self):
         """Initialize the testing setup once before all tests are run."""
 
         # Use a temporary directory so that the user's setup is not altered.
-        self.tempdir = tempfile.TemporaryDirectory()
+        # TODO(#974): Remove if/else when support for Python 3.9 is dropped.
+        if sys.version_info.minor >= 10:
+            self.tempdir = tempfile.TemporaryDirectory(
+                ignore_cleanup_errors=True)
+        else:
+            self.tempdir = tempfile.TemporaryDirectory()
         self.saved_path = pysat.params['data_dirs']
         pysat.params._set_data_dirs(path=self.tempdir.name, store=False)
         return
 
     def teardown_class(self):
         """Clean up downloaded files and parameters from tests."""
 
         pysat.params._set_data_dirs(self.saved_path, store=False)
-        self.tempdir.cleanup()
+        # Remove the temporary directory. In Windows, this occasionally fails
+        # by raising a wide variety of different error messages. Python 3.10+
+        # can handle this, but lower Python versions cannot.
+        # TODO(#974): Remove try/except when support for Python 3.9 is dropped.
+        try:
+            self.tempdir.cleanup()
+        except Exception:
+            pass
+
         del self.saved_path, self.tempdir
         return
 
     def initialize_test_package(self, inst_loc, user_info=None):
         """Generate custom instrument lists for each category of tests.
 
         Parameters
```

### Comparing `pysat-3.0.6/pysat/tests/classes/cls_instrument_property.py` & `pysat-3.1.0/pysat/tests/classes/cls_instrument_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 Note
 ----
 Base class stored here, but tests inherited by test_instrument.py
 
 """
 
 import datetime as dt
+import functools
 from importlib import reload
 import logging
 import numpy as np
 import warnings
 
 import pandas as pds
 import pytest
 import xarray as xr
 
 import pysat
+from pysat.instruments.methods import testing as ps_meth
 from pysat.utils import testing
 from pysat.utils.time import filter_datetime_input
 
 
 class InstPropertyTests(object):
     """Basic tests for `pysat.Instrument` properties.
 
@@ -142,14 +144,29 @@
         # Get index if a pds.Series is returned.
         if isinstance(self.out, pds.Series):
             self.out = self.out.index
         assert filter_datetime_input(self.out[0]) == self.ref_time
         assert filter_datetime_input(self.out[-1]) == stop
         return
 
+    def test_remote_file_list_with_default_dates(self):
+        """Test setting the start / stop dates as default kwargs."""
+
+        # Set new defaults for kwargs
+        start = dt.datetime(2018, 1, 1)
+        stop = dt.datetime(2018, 2, 1)
+
+        # Update remote_file_list default dates
+        self.testInst._list_remote_files_rtn = functools.partial(
+            ps_meth.list_remote_files, start=start, stop=stop)
+
+        files = self.testInst.remote_file_list()
+        assert filter_datetime_input(files.index[0]) == start
+        assert filter_datetime_input(files.index[-1]) == stop
+
     @pytest.mark.parametrize("no_remote_files", [True, False])
     @pytest.mark.parametrize("download_keys", [
         (["start"]), (["start", "stop"]), (["date_array"]), ([])])
     def test_download_updated_files(self, caplog, no_remote_files,
                                     download_keys):
         """Test `download_updated_files` and default bounds are updated.
 
@@ -615,14 +632,17 @@
             assert captured.find(test_str) >= 0
 
         return
 
     def test_error_undefined_input_keywords(self):
         """Test for error if undefined keywords provided at instantiation."""
 
+        if 'file_date_range' in self.testInst.kwargs['list_files']:
+            pytest.skip("Cannot run eval on pds.DatetimeIndex")
+
         # Add a new keyword
         self.testInst.kwargs['load']['undefined_keyword1'] = True
         self.testInst.kwargs['load']['undefined_keyword2'] = False
 
         estr = "".join(("unknown keywords supplied: ['undefined_keyword1',",
                         " 'undefined_keyword2']"))
         with pytest.raises(ValueError) as verr:
```

### Comparing `pysat-3.0.6/pysat/tests/classes/cls_registration.py` & `pysat-3.1.0/pysat/tests/classes/cls_registration.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/instrument_test_class.py` & `pysat-3.1.0/pysat/tests/instrument_test_class.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_constellation.py` & `pysat-3.1.0/pysat/tests/test_constellation.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Full author list can be found in .zenodo.json file
 # DOI:10.5281/zenodo.1199703
 # ----------------------------------------------------------------------------
 """Unit tests for the Constellation class."""
 
 import datetime as dt
 import logging
+import numpy as np
 import pandas as pds
 import pytest
 
 import pysat
 from pysat import constellations
 from pysat.tests.classes.cls_registration import TestWithRegistration
 from pysat.utils import testing
@@ -256,20 +257,26 @@
         self.inst = list(constellations.testing.instruments)
         self.const = pysat.Constellation(instruments=self.inst, use_header=True)
         self.ref_time = pysat.instruments.pysat_testing._test_dates['']['']
         self.attrs = ["platforms", "names", "tags", "inst_ids", "instruments",
                       "bounds", "empty", "empty_partial", "index_res",
                       "common_index", "date", "yr", "doy", "yesterday", "today",
                       "tomorrow", "variables"]
+        self.inst_attrs = ['platform', 'name', 'tag', 'inst_id', 'clean_level',
+                           'pandas_format', "empty", "yr", 'pad', 'date',
+                           'doy', 'acknowledgements', 'references']
+        self.dims = ['time', 'x', 'y', 'z', 'profile_height', 'latitude',
+                     'longitude', 'altitude']
         return
 
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
-        del self.inst, self.const, self.ref_time, self.attrs
+        del self.inst, self.const, self.ref_time, self.attrs, self.dims
+        del self.inst_attrs
         return
 
     def test_has_required_attrs(self):
         """Ensure the instrument has all required attributes present."""
 
         for req_attr in self.attrs:
             assert hasattr(self.const, req_attr)
@@ -330,25 +337,27 @@
         assert self.const.empty
         assert self.const.empty_partial
         return
 
     def test_empty_flag_data_empty_partial_load(self):
         """Test the status of the empty flag for partially loaded data."""
 
-        # Load only one instrument and test the status flag
-        self.const.instruments[0].load(date=self.ref_time, use_header=True)
+        self.const = pysat.Constellation(
+            const_module=constellations.testing_partial, use_header=True)
+        self.const.load(date=self.ref_time)
         assert self.const.empty_partial
         assert not self.const.empty
         return
 
     def test_empty_flag_data_not_empty_partial_load(self):
         """Test the alt status of the empty flag for partially loaded data."""
 
-        # Load only one instrument and test the status flag for alternate flag
-        self.const.instruments[0].load(date=self.ref_time, use_header=True)
+        self.const = pysat.Constellation(
+            const_module=constellations.testing_partial, use_header=True)
+        self.const.load(date=self.ref_time)
         assert not self.const._empty(all_inst=False)
         return
 
     def test_empty_flag_data_not_empty(self):
         """Test the status of the empty flag for loaded data."""
 
         # Load data and test the status flag
@@ -425,7 +434,146 @@
 
     def test_bad_call_inst_method(self):
         """Test raises AttributeError for missing Instrument method."""
 
         testing.eval_bad_input(self.const._call_inst_method, AttributeError,
                                "unknown method", ['not a method'])
         return
+
+    @pytest.mark.parametrize('common_coord', [True, False])
+    @pytest.mark.parametrize('fill_method', [None, 'nearest', 'linear'])
+    def test_to_inst_xarray(self, common_coord, fill_method):
+        """Test conversion of Constellation of mixed type to xarray Instrument.
+
+        Parameters
+        ----------
+        common_coord : bool
+            For Constellations with any xarray.Dataset Instruments, True to
+            include locations where all coordinate arrays cover, False to use
+            the maximum location range from the list of coordinates
+        fill_method : str or NoneType
+            Fill method if common data coordinates do not match exactly. If
+            one of 'nearest', 'pad'/'ffill', 'backfill'/'bfill', or None then
+            no interpolation will occur.  If 'linear', 'zero', 'slinear',
+            'quadratic', 'cubic', or 'polynomial' are used, then 1D or ND
+            interpolation will be used.
+
+        """
+
+        self.const.load(date=self.ref_time)
+        out_inst = self.const.to_inst(common_coord, fill_method)
+
+        # Test the output instrument attributes
+        assert not out_inst.pandas_format
+        assert out_inst.platform == 'pysat'
+        assert out_inst.tag == ''
+        assert out_inst.inst_id == ''
+        assert out_inst.clean_level == 'clean'
+        assert out_inst.pad is None
+        assert out_inst.date == self.ref_time
+        assert out_inst.doy == int(self.ref_time.strftime('%j'))
+        assert np.all([out_inst.name.find(iname) >= 0
+                       for iname in self.const.names])
+
+        # Test the output instrument data
+        testing.assert_lists_equal(self.dims, list(out_inst.data.dims.keys()))
+        testing.assert_list_contains(self.dims,
+                                     list(out_inst.data.coords.keys()))
+        testing.assert_list_contains(['variable_profile_height', 'image_lon',
+                                      'image_lat'],
+                                     list(out_inst.data.coords.keys()))
+
+        for cinst in self.const.instruments:
+            for var in cinst.variables:
+                var_name = '_'.join([var, cinst.platform, cinst.name])
+                assert (var in out_inst.variables
+                        or var_name in out_inst.variables), \
+                    "missing variable: {:s} or {:s}".format(var, var_name)
+                assert (var == 'time' or var in out_inst.meta
+                        or var_name in out_inst.meta), \
+                    "missing variable in metadata: {:s} or {:s}".format(
+                        var, var_name)
+
+        # Test the output instrument index
+        testing.assert_lists_equal(list(out_inst.index), list(self.const.index))
+
+        return
+
+    def test_to_inst_pandas_w_pad(self):
+        """Test Constellation `to_inst` with single, padded pandas Instrument.
+
+        """
+        # Redefine the Instrument and constellation
+        self.inst = pysat.Instrument(
+            inst_module=pysat.instruments.pysat_testing, use_header=True,
+            pad=pds.DateOffset(hours=1), num_samples=10)
+        self.const = pysat.Constellation(instruments=[self.inst],
+                                         use_header=True)
+
+        # Load the data
+        self.inst.load(date=self.ref_time)
+        self.const.load(date=self.ref_time)
+
+        # Convert the Constellation into an Instrument equivalent to `self.inst`
+        out_inst = self.const.to_inst()
+
+        # Test the output instrument attributes
+        assert out_inst.pandas_format
+
+        for iattr in self.inst_attrs:
+            assert getattr(out_inst, iattr) == getattr(self.inst, iattr), \
+                "Unexpected value for Instrument attribute {:}".format(iattr)
+
+        # Test the output instrument data
+        testing.assert_lists_equal(self.inst.variables, out_inst.variables)
+        assert np.all(out_inst.data == self.inst.data)
+
+        # Test the output instrument metadata
+        assert out_inst.meta == self.inst.meta
+
+        # Test the output instrument index
+        testing.assert_lists_equal(list(out_inst.index), list(self.inst.index))
+
+        return
+
+    def test_to_inst_mult_pad_clean(self):
+        """Test Constellation `to_inst` with multiple clean levels and pads."""
+        # Redefine the Instrument and constellation
+        clean_level = 'dirty'
+        pad = pds.DateOffset(hours=1)
+        self.inst = [
+            pysat.Instrument(inst_module=pysat.instruments.pysat_testing,
+                             use_header=True, pad=pad, num_samples=10),
+            pysat.Instrument(inst_module=pysat.instruments.pysat_testing,
+                             use_header=True, pad=2 * pad,
+                             clean_level=clean_level, num_samples=10)]
+        self.const = pysat.Constellation(instruments=self.inst, use_header=True)
+
+        # Load the Instrument and Constellation data
+        self.inst[-1].load(date=self.ref_time)
+        self.const.load(date=self.ref_time)
+
+        # Convert the Constellation into an Instrument equivalent to `self.inst`
+        out_inst = self.const.to_inst()
+
+        # Test the output instrument attributes
+        assert out_inst.pandas_format
+
+        for iattr in self.inst_attrs:
+            assert getattr(out_inst, iattr) == getattr(self.inst[1], iattr), \
+                "Unexpected value for Instrument attribute {:}".format(iattr)
+
+        # Test the output instrument data and metadata
+        for var in self.inst[1].variables:
+            out_var = "_".join([var, self.inst[1].platform, self.inst[1].name])
+            assert out_var in out_inst.variables, \
+                "missing data variable: {:s}".format(out_var)
+            assert out_var in out_inst.meta, \
+                "missing metadata variable: {:s}".format(out_var)
+            assert np.all(out_inst[out_var] == self.inst[1][var]), \
+                "mismatched data for: {:s}".format(var)
+
+        # Test the output instrument index
+        testing.assert_lists_equal(list(out_inst.index),
+                                   list(self.inst[1].index))
+
+        return
```

### Comparing `pysat-3.0.6/pysat/tests/test_files.py` & `pysat-3.1.0/pysat/tests/test_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,20 +592,22 @@
     def test_instrument_has_files(self):
         """Test that instrument generates file list if there are files."""
         import pysat.instruments.pysat_testing
 
         root_fname = ''.join(('pysat_testing_junk_{year:04d}_gold_{day:03d}_'
                               'stuff_{month:02d}_{hour:02d}_{minute:02d}_'
                               '{second:02d}.pysat_testing_file'))
-        # create a bunch of files by year and doy
+
+        # Create a group of files by year and doy
         start = dt.datetime(2007, 12, 31)
         stop = dt.datetime(2008, 1, 10)
         create_files(self.testInst, start, stop, freq='100min',
                      use_doy=False, root_fname=root_fname)
-        # create the same range of dates
+
+        # Create a DatetimeIndex with the same range of dates as the new files
         dates = pysat.utils.time.create_date_range(start, stop, freq='100min')
 
         pysat.instruments.pysat_testing.list_files = functools.partial(
             list_files, version=self.version)
         inst = pysat.Instrument(platform='pysat', name='testing',
                                 update_files=True)
         reload(pysat.instruments.pysat_testing)
```

### Comparing `pysat-3.0.6/pysat/tests/test_instrument.py` & `pysat-3.1.0/pysat/tests/test_instrument.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 """Tests the pysat Instrument object and methods."""
 
+import datetime as dt
 from importlib import reload
 import numpy as np
+import pandas as pds
 import pytest
 import warnings
 import xarray as xr
 
 import pysat
 import pysat.instruments.pysat_ndtesting
 import pysat.instruments.pysat_testing
@@ -14,14 +16,15 @@
 import pysat.instruments.pysat_testing_xarray
 
 from pysat.tests.classes.cls_instrument_access import InstAccessTests
 from pysat.tests.classes.cls_instrument_integration import InstIntegrationTests
 from pysat.tests.classes.cls_instrument_iteration import InstIterationTests
 from pysat.tests.classes.cls_instrument_property import InstPropertyTests
 from pysat.utils import testing
+from pysat.utils.time import filter_datetime_input
 
 
 class TestBasics(InstAccessTests, InstIntegrationTests, InstIterationTests,
                  InstPropertyTests):
     """Unit tests for pysat.Instrument object."""
 
     def setup_class(self):
@@ -60,14 +63,120 @@
 
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.out, self.ref_time, self.ref_doy
         return
 
+    def check_nonstandard_cadence(self):
+        """Check for nonstandard cadence in tests."""
+
+        if hasattr(self, 'freq'):
+            min_freq = pds.tseries.frequencies.to_offset('D')
+            return pds.tseries.frequencies.to_offset(self.freq) != min_freq
+        else:
+            # Uses standard frequency
+            return False
+
+
+class TestInstCadence(TestBasics):
+    """Unit tests for pysat.Instrument objects with the default file cadance."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        reload(pysat.instruments.pysat_testing)
+        self.ref_time = pysat.instruments.pysat_testing._test_dates['']['']
+        self.freq = 'D'
+
+        date_range = pds.date_range(self.ref_time - pds.DateOffset(years=1),
+                                    self.ref_time + pds.DateOffset(years=2)
+                                    - pds.DateOffset(days=1), freq=self.freq)
+        self.testInst = pysat.Instrument(platform='pysat', name='testing',
+                                         num_samples=10,
+                                         clean_level='clean',
+                                         update_files=True,
+                                         use_header=True,
+                                         file_date_range=date_range,
+                                         **self.testing_kwargs)
+        self.ref_doy = int(self.ref_time.strftime('%j'))
+        self.out = None
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.out, self.ref_time, self.ref_doy, self.freq
+        return
+
+
+class TestInstMonthlyCadence(TestInstCadence):
+    """Unit tests for pysat.Instrument objects with a monthly file cadance."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        reload(pysat.instruments.pysat_testing)
+        self.ref_time = pysat.instruments.pysat_testing._test_dates['']['']
+        self.freq = 'MS'
+
+        date_range = pds.date_range(self.ref_time - pds.DateOffset(years=1),
+                                    self.ref_time
+                                    + pds.DateOffset(years=2, days=-1),
+                                    freq=self.freq)
+        self.testInst = pysat.Instrument(platform='pysat', name='testing',
+                                         num_samples=10,
+                                         clean_level='clean',
+                                         update_files=True,
+                                         use_header=True,
+                                         file_date_range=date_range,
+                                         **self.testing_kwargs)
+        self.ref_doy = int(self.ref_time.strftime('%j'))
+        self.out = None
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.out, self.ref_time, self.ref_doy, self.freq
+        return
+
+
+class TestInstYearlyCadence(TestInstCadence):
+    """Unit tests for pysat.Instrument objects with a monthly file cadance."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        reload(pysat.instruments.pysat_testing)
+        self.ref_time = pysat.instruments.pysat_testing._test_dates['']['']
+        self.freq = 'AS'
+
+        # Since these are yearly files, use a longer date range
+        date_range = pds.date_range(self.ref_time - pds.DateOffset(years=1),
+                                    self.ref_time
+                                    + pds.DateOffset(years=5, days=-1),
+                                    freq=self.freq)
+        self.testInst = pysat.Instrument(platform='pysat', name='testing',
+                                         num_samples=10,
+                                         clean_level='clean',
+                                         update_files=True,
+                                         use_header=True,
+                                         file_date_range=date_range,
+                                         **self.testing_kwargs)
+        self.ref_doy = int(self.ref_time.strftime('%j'))
+        self.out = None
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.out, self.ref_time, self.ref_doy, self.freq
+        return
+
 
 class TestBasicsInstModule(TestBasics):
     """Basic tests for instrument instantiated via inst_module."""
 
     def setup_method(self):
         """Set up the unit test environment for each method."""
 
@@ -76,15 +185,15 @@
         self.testInst = pysat.Instrument(inst_module=imod,
                                          num_samples=10,
                                          clean_level='clean',
                                          update_files=True,
                                          use_header=True,
                                          **self.testing_kwargs)
         self.ref_time = imod._test_dates['']['']
-        self.ref_doy = 1
+        self.ref_doy = int(self.ref_time.strftime('%j'))
         self.out = None
         return
 
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.out, self.ref_time, self.ref_doy
@@ -102,17 +211,17 @@
         self.testInst = pysat.Instrument(platform='pysat',
                                          name='testing_xarray',
                                          num_samples=10,
                                          clean_level='clean',
                                          update_files=True,
                                          use_header=True,
                                          **self.testing_kwargs)
-        self.ref_time = \
-            pysat.instruments.pysat_testing_xarray._test_dates['']['']
-        self.ref_doy = 1
+        self.ref_time = pysat.instruments.pysat_testing_xarray._test_dates[
+            '']['']
+        self.ref_doy = int(self.ref_time.strftime('%j'))
         self.out = None
         return
 
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.out, self.ref_time, self.ref_doy
@@ -130,15 +239,15 @@
         self.testInst = pysat.Instrument(platform='pysat', name='testing2d',
                                          num_samples=50,
                                          clean_level='clean',
                                          update_files=True,
                                          use_header=True,
                                          **self.testing_kwargs)
         self.ref_time = pysat.instruments.pysat_testing2d._test_dates['']['']
-        self.ref_doy = 1
+        self.ref_doy = int(self.ref_time.strftime('%j'))
         self.out = None
         return
 
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.out, self.ref_time, self.ref_doy
@@ -161,26 +270,49 @@
         self.testInst = pysat.Instrument(platform='pysat',
                                          name='ndtesting',
                                          num_samples=10,
                                          clean_level='clean',
                                          update_files=True,
                                          use_header=True,
                                          **self.testing_kwargs)
-        self.ref_time = \
-            pysat.instruments.pysat_ndtesting._test_dates['']['']
-        self.ref_doy = 1
+        self.ref_time = pysat.instruments.pysat_ndtesting._test_dates['']['']
+        self.ref_doy = int(self.ref_time.strftime('%j'))
         self.out = None
         return
 
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.out, self.ref_time, self.ref_doy
         return
 
+    def test_setting_data_as_tuple(self):
+        """Test setting data as a tuple."""
+
+        self.testInst.load(self.ref_time.year, self.ref_doy, use_header=True)
+        self.testInst['doubleMLT'] = ('time', 2. * self.testInst['mlt'].values)
+        assert np.all(self.testInst['doubleMLT'] == 2. * self.testInst['mlt'])
+        return
+
+    def test_xarray_not_empty_notime(self):
+        """Test that xarray empty is False even if there is no time data."""
+        # Load data and confirm it exists
+        self.testInst.load(date=self.ref_time)
+        assert not self.testInst.empty
+
+        # Downselect to no time data
+        self.testInst.data = self.testInst[self.ref_time + dt.timedelta(days=1):
+                                           self.ref_time + dt.timedelta(days=2)]
+        assert not self.testInst.empty
+        assert len(self.testInst.index) == 0
+        for dim in self.testInst.data.dims.keys():
+            if dim != 'time':
+                assert len(self.testInst[dim]) > 0
+        return
+
     @pytest.mark.parametrize("index", [(0),
                                        ([0, 1, 2, 3]),
                                        (slice(0, 10)),
                                        (np.array([0, 1, 2, 3]))])
     def test_data_access_by_2d_indices_and_name(self, index):
         """Check that variables and be accessed by each supported index type.
 
@@ -273,14 +405,84 @@
         target : bool
             Target response for `self.testInst.empty`.
 
         """
 
         self.testInst.data = data
         assert self.testInst.empty == target
+        return
+
+    @pytest.mark.parametrize("val,warn_msg",
+                             [([], "broadcast as NaN"),
+                              (27., "Broadcast over epoch"),
+                              (np.array([27.]), "Broadcast over epoch")])
+    def test_set_xarray_single_value_warnings(self, val, warn_msg):
+        """Check for warning messages when setting xarray values.
+
+        Parameters
+        ----------
+        val : float or iterable
+            Value to be added as a new data variable.
+        warn_msg : str
+            Excerpt from expected warning message.
+
+        """
+
+        warnings.simplefilter("always")
+
+        self.testInst.load(date=self.ref_time, use_header=True)
+
+        with warnings.catch_warnings(record=True) as self.war:
+            self.testInst["new_val"] = val
+        testing.eval_warnings(self.war, warn_msg, warn_type=UserWarning)
+
+    def test_set_xarray_single_value_errors(self):
+        """Check for warning messages when setting xarray values.
+
+        Parameters
+        ----------
+        val : float or iterable
+            Value to be added as a new data variable.
+        warn_msg : str
+            Excerpt from expected warning message.
+
+        """
+
+        self.testInst.load(date=self.ref_time, use_header=True)
+        self.testInst.data = self.testInst.data.assign_coords(
+            {'preset_val': np.array([1.0, 2.0])})
+
+        with pytest.raises(ValueError) as verr:
+            self.testInst['preset_val'] = 1.0
+
+        estr = 'Shape of input does not match'
+        assert str(verr).find(estr) > 0
+        return
+
+    @pytest.mark.parametrize("new_val", [3.0, np.array([3.0])])
+    def test_set_xarray_single_value_broadcast(self, new_val):
+        """Check that single values are correctly broadcast.
+
+        Parameters
+        ----------
+        new_val : float or iterable
+            Should be a single value, potentially an array with one element.
+
+        """
+
+        self.testInst.load(date=self.ref_time, use_header=True)
+        self.testInst.data = self.testInst.data.assign_coords(
+            {'preset_val': 1.0})
+
+        self.testInst['preset_val'] = new_val
+        self.testInst['new_val'] = new_val
+        # Existing coords should be not be broadcast
+        assert self.testInst['preset_val'].size == 1
+        # New variables broadcast over time
+        assert len(self.testInst['new_val']) == len(self.testInst.index)
 
 
 class TestBasicsShiftedFileDates(TestBasics):
     """Basic tests for pandas `pysat.Instrument` with shifted file dates."""
 
     def setup_method(self):
         """Set up the unit test environment for each method."""
@@ -291,15 +493,15 @@
                                          clean_level='clean',
                                          update_files=True,
                                          mangle_file_dates=True,
                                          strict_time_flag=True,
                                          use_header=True,
                                          **self.testing_kwargs)
         self.ref_time = pysat.instruments.pysat_testing._test_dates['']['']
-        self.ref_doy = 1
+        self.ref_doy = int(self.ref_time.strftime('%j'))
         self.out = None
         return
 
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.out, self.ref_time, self.ref_doy
@@ -407,14 +609,74 @@
         # Ensure the minimum number of warnings were raised.
         assert len(self.war) >= len(self.warn_msgs)
 
         # Test the warning messages, ensuring each attribute is present.
         testing.eval_warnings(self.war, self.warn_msgs)
         return
 
+    def test_instrument_labels(self):
+        """Test deprecation of `labels` kwarg in Instrument."""
+        self.in_kwargs['labels'] = {
+            'units': ('units', str), 'name': ('long_name', str),
+            'notes': ('notes', str), 'desc': ('desc', str),
+            'min_val': ('value_min', float), 'max_val': ('value_max', float),
+            'fill_val': ('fill', float)}
+
+        # Catch the warnings
+        with warnings.catch_warnings(record=True) as self.war:
+            tinst = pysat.Instrument(use_header=True, **self.in_kwargs)
+
+        self.warn_msgs = np.array(["`labels` is deprecated, use `meta_kwargs`"])
+
+        # Evaluate the warning output
+        self.eval_warnings()
+
+        # Evaluate the performance
+        assert float in tinst.meta.labels.label_type['fill_val']
+        return
+
+    @pytest.mark.parametrize('use_kwargs', [True, False])
+    def test_instrument_meta_labels(self, use_kwargs):
+        """Test deprecation of `meta_labels` attribute in Instrument.
+
+        Parameters
+        ----------
+        use_kwargs : bool
+            If True, specify labels on input.  If False, use defaults.
+
+        """
+        if use_kwargs:
+            self.in_kwargs['meta_kwargs'] = {'labels': {
+                'units': ('units', str), 'name': ('long_name', str),
+                'notes': ('notes', str), 'desc': ('desc', str),
+                'min_val': ('value_min', float),
+                'max_val': ('value_max', float), 'fill_val': ('fill', float)}}
+
+        # Catch the warnings
+        with warnings.catch_warnings(record=True) as self.war:
+            tinst = pysat.Instrument(use_header=True, **self.in_kwargs)
+            labels = tinst.meta_labels
+
+        self.warn_msgs = np.array(["Deprecated attribute, returns `meta_kwarg"])
+
+        # Evaluate the warning output
+        self.eval_warnings()
+
+        # Evaluate the performance
+        if not use_kwargs:
+            self.in_kwargs['meta_kwargs'] = {'labels': {
+                'units': ('units', str), 'name': ('long_name', str),
+                'notes': ('notes', str), 'desc': ('desc', str),
+                'min_val': ('value_min', (float, int)),
+                'max_val': ('value_max', (float, int)),
+                'fill_val': ('fill', (float, int, str))}}
+
+        assert labels == self.in_kwargs['meta_kwargs']['labels']
+        return
+
     def test_generic_meta_translator(self):
         """Test deprecation of `generic_meta_translator`."""
 
         # Catch the warnings
         with warnings.catch_warnings(record=True) as self.war:
             tinst = pysat.Instrument(use_header=True, **self.in_kwargs)
             tinst.generic_meta_translator(tinst.meta)
```

### Comparing `pysat-3.0.6/pysat/tests/test_instrument_custom.py` & `pysat-3.1.0/pysat/tests/test_instrument_custom.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_instrument_listgen.py` & `pysat-3.1.0/pysat/tests/test_instrument_listgen.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_instrument_padding.py` & `pysat-3.1.0/pysat/tests/test_instrument_padding.py`

 * *Files 10% similar despite different names*

```diff
@@ -465,14 +465,39 @@
         self.ref_doy = 1
         self.testInst.load(self.ref_time.year, self.ref_doy)
         self.delta = dt.timedelta(seconds=0)
         self.eval_index_start_end()
         return
 
 
+class TestDataPaddingNonMonotonic(TestDataPadding):
+    """Unit tests for non-montonic pandas `pysat.Instrument` with data pad."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        reload(pysat.instruments.pysat_testing)
+        self.testInst = pysat.Instrument(platform='pysat', name='testing',
+                                         clean_level='clean',
+                                         pad={'minutes': 5},
+                                         non_monotonic_index=True,
+                                         update_files=True,
+                                         use_header=True)
+        self.ref_time = dt.datetime(2009, 1, 2)
+        self.ref_doy = 2
+        self.delta = dt.timedelta(minutes=5)
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.ref_time, self.ref_doy, self.delta
+        return
+
+
 class TestDataPaddingXArray(TestDataPadding):
     """Unit tests for xarray `pysat.Instrument` with data padding."""
 
     def setup_method(self):
         """Set up the unit test environment for each method."""
 
         reload(pysat.instruments.pysat_testing_xarray)
@@ -490,14 +515,40 @@
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.ref_time, self.ref_doy, self.delta
         return
 
 
+class TestDataPaddingXArrayNonMonotonic(TestDataPadding):
+    """Unit tests for non-montonic xarray `pysat.Instrument` with data pad."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        reload(pysat.instruments.pysat_testing_xarray)
+        self.testInst = pysat.Instrument(platform='pysat',
+                                         name='testing_xarray',
+                                         clean_level='clean',
+                                         pad={'minutes': 5},
+                                         non_monotonic_index=True,
+                                         update_files=True,
+                                         use_header=True)
+        self.ref_time = dt.datetime(2009, 1, 2)
+        self.ref_doy = 2
+        self.delta = dt.timedelta(minutes=5)
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.ref_time, self.ref_doy, self.delta
+        return
+
+
 class TestMultiFileRightDataPaddingBasics(TestDataPadding):
     """Unit tests for pandas `pysat.Instrument` with right offset data pad."""
 
     def setup_method(self):
         """Set up the unit test environment for each method."""
 
         reload(pysat.instruments.pysat_testing)
@@ -516,14 +567,41 @@
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.ref_time, self.ref_doy, self.delta
         return
 
 
+class TestMultiFileRightDataPaddingBasicsNonMonotonic(TestDataPadding):
+    """Tests for non-monotonic pandas `pysat.Instrument` with right data pad."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        reload(pysat.instruments.pysat_testing)
+        self.testInst = pysat.Instrument(platform='pysat', name='testing',
+                                         clean_level='clean',
+                                         update_files=True,
+                                         sim_multi_file_right=True,
+                                         non_monotonic_index=True,
+                                         pad={'minutes': 5},
+                                         use_header=True)
+        self.testInst.multi_file_day = True
+        self.ref_time = dt.datetime(2009, 1, 2)
+        self.ref_doy = 2
+        self.delta = dt.timedelta(minutes=5)
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.ref_time, self.ref_doy, self.delta
+        return
+
+
 class TestMultiFileRightDataPaddingBasicsXarray(TestDataPadding):
     """Unit tests for xarray `pysat.Instrument` with right offset data pad."""
 
     def setup_method(self):
         """Set up the unit test environment for each method."""
 
         reload(pysat.instruments.pysat_testing_xarray)
@@ -543,14 +621,42 @@
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.ref_time, self.ref_doy, self.delta
         return
 
 
+class TestMultiFileRightDataPaddingBasicsXarrayNonMonotonic(TestDataPadding):
+    """Tests for non-monotonic xarray `pysat.Instrument` with right data pad."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        reload(pysat.instruments.pysat_testing_xarray)
+        self.testInst = pysat.Instrument(platform='pysat',
+                                         name='testing_xarray',
+                                         clean_level='clean',
+                                         update_files=True,
+                                         sim_multi_file_right=True,
+                                         non_monotonic_index=True,
+                                         pad={'minutes': 5},
+                                         use_header=True)
+        self.testInst.multi_file_day = True
+        self.ref_time = dt.datetime(2009, 1, 2)
+        self.ref_doy = 2
+        self.delta = dt.timedelta(minutes=5)
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.ref_time, self.ref_doy, self.delta
+        return
+
+
 class TestMultiFileLeftDataPaddingBasics(TestDataPadding):
     """Unit tests for pandas `pysat.Instrument` with left offset data pad."""
 
     def setup_method(self):
         """Set up the unit test environment for each method."""
 
         reload(pysat.instruments.pysat_testing)
@@ -570,14 +676,42 @@
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.ref_time, self.ref_doy, self.delta
         return
 
 
+class TestMultiFileLeftDataPaddingBasicsNonMonotonic(TestDataPadding):
+    """Tests for non-monotonic pandas `pysat.Instrument` with left data pad."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        reload(pysat.instruments.pysat_testing)
+        self.testInst = pysat.Instrument(platform='pysat',
+                                         name='testing',
+                                         clean_level='clean',
+                                         update_files=True,
+                                         sim_multi_file_left=True,
+                                         non_monotonic_index=True,
+                                         pad={'minutes': 5},
+                                         use_header=True)
+        self.testInst.multi_file_day = True
+        self.ref_time = dt.datetime(2009, 1, 2)
+        self.ref_doy = 2
+        self.delta = dt.timedelta(minutes=5)
+        return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.ref_time, self.ref_doy, self.delta
+        return
+
+
 class TestMultiFileLeftDataPaddingBasicsXarray(TestDataPadding):
     """Unit tests for xarray `pysat.Instrument` with left offset data pad."""
 
     def setup_method(self):
         """Set up the unit test environment for each method."""
 
         reload(pysat.instruments.pysat_testing_xarray)
@@ -589,13 +723,41 @@
                                          pad={'minutes': 5},
                                          use_header=True)
         self.testInst.multi_file_day = True
         self.ref_time = dt.datetime(2009, 1, 2)
         self.ref_doy = 2
         self.delta = dt.timedelta(minutes=5)
         return
+
+    def teardown_method(self):
+        """Clean up the unit test environment after each method."""
+
+        del self.testInst, self.ref_time, self.ref_doy, self.delta
+        return
+
+
+class TestMultiFileLeftDataPaddingBasicsXarrayNonMonotonic(TestDataPadding):
+    """Tests for non-monotonic xarray `pysat.Instrument` with left data pad."""
+
+    def setup_method(self):
+        """Set up the unit test environment for each method."""
+
+        reload(pysat.instruments.pysat_testing_xarray)
+        self.testInst = pysat.Instrument(platform='pysat',
+                                         name='testing_xarray',
+                                         clean_level='clean',
+                                         update_files=True,
+                                         sim_multi_file_left=True,
+                                         non_monotonic_index=True,
+                                         pad={'minutes': 5},
+                                         use_header=True)
+        self.testInst.multi_file_day = True
+        self.ref_time = dt.datetime(2009, 1, 2)
+        self.ref_doy = 2
+        self.delta = dt.timedelta(minutes=5)
+        return
 
     def teardown_method(self):
         """Clean up the unit test environment after each method."""
 
         del self.testInst, self.ref_time, self.ref_doy, self.delta
         return
```

### Comparing `pysat-3.0.6/pysat/tests/test_instruments.py` & `pysat-3.1.0/pysat/tests/test_instruments.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_meta.py` & `pysat-3.1.0/pysat/tests/test_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         self.meta = pysat.Meta()
         self.mutable = True
 
         self.meta_labels = {'units': ('Units', str),
                             'name': ('Long_Name', str),
                             'desc': ('Desc', str),
                             'notes': ('Notes', str),
-                            'min_val': ('Minimum', np.float64),
-                            'max_val': ('Maximum', np.float64),
-                            'fill_val': ('Fill_Value', np.float64)}
+                            'min_val': ('Minimum', (float, int)),
+                            'max_val': ('Maximum', (float, int)),
+                            'fill_val': ('Fill_Value', (float, int, str))}
         self.dval = None
         self.default_name = ['long_name']
         self.default_nan = ['fill', 'value_min', 'value_max']
         self.default_val = {'notes': '', 'units': '', 'desc': ''}
         self.frame_list = ['dummy_frame1', 'dummy_frame2']
         return
 
@@ -75,16 +75,23 @@
             self.meta = self.testInst.meta
 
             # Update the mutable flag, if desired
             if not keep_mutable:
                 self.meta.mutable = self.mutable
         return
 
-    def eval_meta_settings(self):
-        """Test the Meta settings for a specified value."""
+    def eval_meta_settings(self, isfloat=True):
+        """Test the Meta settings for a specified value.
+
+        Parameters
+        ----------
+        isfloat : bool
+            True if data type is float, False if it is int, str, or other
+
+        """
         # Test the Meta data for the data value, self.dval
         for lkey in self.default_name:
             assert self.meta[self.dval, lkey] == self.dval, \
                 "{:} differs from the default value ({:} != {:})".format(
                     lkey.__repr__(), self.meta[self.dval, lkey].__repr__(),
                     self.dval.__repr__())
 
@@ -377,15 +384,15 @@
 
         # Test the warning
         assert len(war) >= 1
         assert war[0].category == UserWarning
         assert 'Metadata with type' in str(war[0].message)
         assert 'Dropping input' in str(war[0].message)
 
-        # Check that meta is blank
+        # Check that meta is set to the expected default
         assert np.isnan(self.meta['fake_var']['value_max'])
         return
 
     # -------------------------
     # Test the logging messages
 
     @pytest.mark.parametrize('bad_val', [[1, 2], 1, 2.0, True, None])
@@ -400,16 +407,17 @@
         """
 
         with caplog.at_level(logging.INFO, logger='pysat'):
             self.meta['fake_var'] = {'units': bad_val}
 
         # Test the warning
         captured = caplog.text
-        assert captured.find('Metadata with type') >= 0
-        assert captured.find('Recasting input') >= 0
+        estr = "missing expected message in: {:}".format(captured)
+        assert captured.find('Metadata with type') >= 0, estr
+        assert captured.find('Recasting input') >= 0, estr
 
         # Check that meta is set
         if hasattr(bad_val, "__iter__"):
             exp_val = "\n\n".join([str(bval) for bval in bad_val])
         else:
             exp_val = str(bad_val)
         assert self.meta['fake_var']['units'] == exp_val
@@ -727,16 +735,16 @@
 
         """
 
         # Set the desired values
         self.dval = 'test_meta_dict_assignment'
         self.default_val = {
             getattr(self.meta.labels, mattr): ' '.join(['test', mattr])
-            if self.meta.labels.label_type[mattr] == str else -47
-            for mattr in self.meta.labels.label_type.keys()}
+            if str in pysat.utils.listify(self.meta.labels.label_type[mattr])
+            else -47 for mattr in self.meta.labels.label_type.keys()}
         self.default_name = []
         self.default_nan = []
 
         if custom_attr is not None:
             self.default_val[custom_attr] = 'Custom Attribute Value'
 
         # Assign the meta data using a dictionary
@@ -760,17 +768,17 @@
 
         """
 
         # Set the desired values
         dvals = ['mult1', 'mult2']
         default_vals = {
             getattr(self.meta.labels, mattr): [
-                ' '.join(['test', mattr, self.dval])
-                if self.meta.labels.label_type[mattr] == str else -47
-                for self.dval in dvals]
+                ' '.join(['test', mattr, self.dval]) if str
+                in pysat.utils.listify(self.meta.labels.label_type[mattr])
+                else -47 for self.dval in dvals]
             for mattr in self.meta.labels.label_type.keys()}
         self.default_name = []
         self.default_nan = []
 
         if custom_attr is not None:
             default_vals[custom_attr] = ['Custom Attr {:s}'.format(self.dval)
                                          for self.dval in dvals]
@@ -1011,15 +1019,15 @@
             if slabel in self.default_name:
                 self.default_name.pop(self.default_name.index(slabel))
             elif slabel in self.default_nan:
                 self.default_nan.pop(self.default_nan.index(slabel))
             self.default_val[slabel] = vals[i]
             set_dict[slabel] = vals[i]
 
-        # Initialize the Meta data
+        # Initialize the Meta data using the new data type
         self.testInst[self.dval] = set_dict
         self.meta = self.testInst.meta
 
         # Test the Meta settings
         self.eval_meta_settings()
         return
 
@@ -1970,17 +1978,17 @@
         self.meta = pysat.Meta()
         self.mutable = False
 
         self.meta_labels = {'units': ('Units', str),
                             'name': ('Long_Name', str),
                             'desc': ('Desc', str),
                             'notes': ('Notes', str),
-                            'min_val': ('Minimum', np.float64),
-                            'max_val': ('Maximum', np.float64),
-                            'fill_val': ('Fill_Value', np.float64)}
+                            'min_val': ('Minimum', (float, int)),
+                            'max_val': ('Maximum', (float, int)),
+                            'fill_val': ('Fill_Value', (float, int, str))}
         self.dval = None
         self.default_name = ['long_name']
         self.default_nan = ['fill', 'value_min', 'value_max']
         self.default_val = {'notes': '', 'units': '', 'desc': ''}
         self.frame_list = ['dummy_frame1', 'dummy_frame2']
         return
```

### Comparing `pysat-3.0.6/pysat/tests/test_meta_header.py` & `pysat-3.1.0/pysat/tests/test_meta_header.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_meta_labels.py` & `pysat-3.1.0/pysat/tests/test_meta_labels.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_methods_general.py` & `pysat-3.1.0/pysat/tests/test_methods_general.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_methods_testing.py` & `pysat-3.1.0/pysat/tests/test_methods_testing.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_params.py` & `pysat-3.1.0/pysat/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_registry.py` & `pysat-3.1.0/pysat/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_utils.py` & `pysat-3.1.0/pysat/tests/test_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,124 @@
 import warnings
 
 import pysat
 from pysat.tests.classes.cls_registration import TestWithRegistration
 from pysat import utils
 
 
+class TestUpdateFill(object):
+    """Tests for the core utility `update_fill_values`."""
+
+    def setup_method(self):
+        """Set up the test enviroment."""
+        self.ref_time = pysat.instruments.pysat_testing._test_dates['']['']
+        self.new_fill_val = -47.0
+        return
+
+    def teardown_method(self):
+        """Clean up the test environment."""
+        del self.ref_time, self.new_fill_val
+        return
+
+    @pytest.mark.parametrize("name", ["ndtesting", "testing", "testmodel"])
+    @pytest.mark.parametrize("variables", [('mlt'), (['mlt'])])
+    def test_update_fill_values_numbers(self, name, variables):
+        """Test `update_fill_values` for the desired behaviour.
+
+        Parameters
+        ----------
+        name : str
+            Instrument name
+        variables : str or list-like
+            Variables to update (should be int or float type)
+
+        """
+
+        # Initalize the instrument
+        inst = pysat.Instrument('pysat', name, use_header=True)
+        inst.load(date=self.ref_time)
+
+        # Ensure there are fill values to check
+        test_vars = pysat.utils.listify(variables)
+        for var in test_vars:
+            inst[var].values[0] = inst.meta[var, inst.meta.labels.fill_val]
+
+        # Update the fill values
+        pysat.utils.update_fill_values(inst, variables, self.new_fill_val)
+
+        # Ensure the fill values are updated
+        for var in test_vars:
+            assert inst.meta[var,
+                             inst.meta.labels.fill_val] == self.new_fill_val, \
+                "meta fill value not updated for {:}".format(var)
+            assert np.all(inst[var].values[0] == self.new_fill_val), \
+                "filled data values not updated for {:}".format(var)
+        return
+
+    @pytest.mark.parametrize("name", ["ndtesting", "testing", "testmodel"])
+    def test_update_fill_values_by_type(self, name):
+        """Test `update_fill_values` for the desired behaviour.
+
+        Parameters
+        ----------
+        name : str
+            Instrument name
+
+        """
+
+        # Initalize the instrument
+        inst = pysat.Instrument('pysat', name, use_header=True)
+        inst.load(date=self.ref_time)
+
+        # Ensure there are fill values to check
+        str_vars = [var for var in inst.variables if var in inst.meta.keys()
+                    and isinstance(inst[var].values[0], str)
+                    and inst.meta[var, inst.meta.labels.fill_val] is not None]
+        num_types = [int, float, np.float64, np.int64]
+        if inst.pandas_format:
+            num_vars = [var for var in inst.variables if var in inst.meta.keys()
+                        and inst[var].dtype.type in num_types
+                        and inst.meta[var, inst.meta.labels.fill_val]
+                        is not None]
+        else:
+            num_vars = [var for var in inst.variables if var in inst.meta.keys()
+                        and var not in inst.data.coords.keys()
+                        and inst[var].dtype.type in num_types
+                        and inst.meta[var, inst.meta.labels.fill_val]
+                        is not None]
+
+        for var in num_vars:
+            inst[var].values[0] = inst.meta[var, inst.meta.labels.fill_val]
+
+        for var in str_vars:
+            inst[var].values[0] = str(inst.meta[var, inst.meta.labels.fill_val])
+
+        # Update and check the numeric fill values
+        pysat.utils.update_fill_values(inst, num_vars, self.new_fill_val)
+
+        for var in num_vars:
+            assert inst.meta[var,
+                             inst.meta.labels.fill_val] == self.new_fill_val, \
+                "meta fill value not updated for {:}".format(var)
+            assert np.all(inst[var].values[0] == self.new_fill_val), \
+                "filled data values not updated for {:}".format(var)
+
+        # Update and check the string fill values
+        self.new_fill_val = 'fill'
+        pysat.utils.update_fill_values(inst, str_vars, self.new_fill_val)
+
+        for var in str_vars:
+            assert inst.meta[var,
+                             inst.meta.labels.fill_val] == self.new_fill_val, \
+                "meta fill value not updated for {:}".format(var)
+            assert np.all(inst[var].values[0] == self.new_fill_val), \
+                "filled data values not updated for {:}".format(var)
+        return
+
+
 class TestCIonly(object):
     """Tests where we mess with local settings.
 
     Note
     ----
     These only run in CI environments such as GitHub Actions to avoid breaking
     an end user's setup
@@ -629,14 +739,45 @@
                 # User info should be correct
                 assert inst['user_info'] == self.user_info['pysat_testmodel']
         for inst in self.inst_list['no_download']:
             # `user_info` should not be in any of these
             assert ('user_info' not in inst.keys())
         return
 
+    def test_list_kwargs_passthrough(self):
+        """Test that kwargs are passed through to lists correctly."""
+
+        # Iterate over unique instruments gathered
+        for inst in self.inst_list['download']:
+            # kwargs should not be passed to download
+            assert ('kwargs' not in inst.keys())
+
+            # Construct list of tests with optional load kwargs for this
+            # instrument.
+            list_kwargs = []
+            for opt_inst in self.inst_list['load_options']:
+                if inst['inst_module'] == opt_inst['inst_module']:
+                    if 'kwargs' in opt_inst.keys():
+                        list_kwargs.append(opt_inst['kwargs'].copy())
+
+            # Check if instrument has optional load kwargs
+            if hasattr(inst['inst_module'], '_test_load_opt'):
+                load_opt = getattr(inst['inst_module'], '_test_load_opt')
+                try:
+                    load_opt = load_opt[inst['inst_id']][inst['tag']]
+                    # Check that options specified in module match generated
+                    # test list.
+                    utils.testing.assert_lists_equal(list_kwargs, load_opt)
+                except KeyError:
+                    # Optional load kwargs not defined for this tag / inst_id
+                    # combination.
+                    pass
+
+        return
+
 
 class TestDeprecation(object):
     """Unit test for deprecation warnings."""
 
     @pytest.mark.parametrize("kwargs,msg_inds",
                              [({'fnames': None}, [0, 1]),
                               ({'fnames': 'no_file', 'file_format': None},
```

### Comparing `pysat-3.0.6/pysat/tests/test_utils_files.py` & `pysat-3.1.0/pysat/tests/test_utils_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -370,26 +370,38 @@
         assert np.all(file_info['content_modified_time']
                       <= today + dt.timedelta(days=1))
         assert np.all(file_info['content_modified_time']
                       >= today - dt.timedelta(days=1))
 
         return
 
-    def test_check_and_make_path_exists(self):
-        """Test successful pass at creating existing directory."""
-
-        # Create a temporary directory
-        tempdir = tempfile.TemporaryDirectory()
-        assert os.path.isdir(tempdir.name)
+    @pytest.mark.parametrize("use_cwd", [True, False])
+    def test_check_and_make_path_exists(self, use_cwd):
+        """Test successful pass at creating existing directory.
+
+        Parameters
+        ----------
+        use_cwd : bool
+            Use current working directory or a temporary directory
+
+        """
+        if use_cwd:
+            dir_name = ""
+        else:
+            # Create a temporary directory
+            tempdir = tempfile.TemporaryDirectory()
+            dir_name = tempdir.name
+            assert os.path.isdir(tempdir.name)
 
         # Assert check_and_make_path does not re-create the directory
-        assert not pysat.utils.files.check_and_make_path(tempdir.name)
+        assert not pysat.utils.files.check_and_make_path(dir_name)
 
-        # Clean up temporary directory
-        tempdir.cleanup()
+        if not use_cwd:
+            # Clean up temporary directory
+            tempdir.cleanup()
         return
 
     @pytest.mark.parametrize("trailer", [None, '', 'extra',
                                          os.path.join('extra', 'extra'),
                                          os.path.join('yes', 'way', '..',
                                                       'brah'),
                                          os.path.join('.', 'yeppers')])
```

### Comparing `pysat-3.0.6/pysat/tests/test_utils_io.py` & `pysat-3.1.0/pysat/tests/test_utils_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,50 @@
         self.loaded_inst, meta = io.load_netcdf(
             outfile, pandas_format=self.testInst.pandas_format,
             epoch_name=default_epoch_name, **tkwargs)
         self.eval_loaded_data()
 
         return
 
+    @pytest.mark.parametrize("kwargs,target",
+                             [({}, True),
+                              ({'export_pysat_info': True}, True),
+                              ({'export_pysat_info': False}, False)])
+    def test_basic_write_and_read_netcdf_export_pysat_info(self, kwargs,
+                                                           target):
+        """Test basic netCDF4 read/write with optional pysat info export.
+
+        Parameters
+        ----------
+        kwargs : dict
+            Specify value of `export_pysat_info`. An empty dict sets to
+            default value.
+        target : bool
+            True indicates that pysat info should be written to the file.
+
+        """
+        # Create a bunch of files by year and doy
+        outfile = os.path.join(self.tempdir.name, 'pysat_test_ncdf.nc')
+        self.testInst.load(date=self.stime, use_header=True)
+
+        io.inst_to_netcdf(self.testInst, fname=outfile, preserve_meta_case=True,
+                          epoch_name=default_epoch_name, **kwargs)
+
+        tkwargs = decode_times_val(self.testInst.pandas_format)
+
+        self.loaded_inst, meta = io.load_netcdf(
+            outfile, pandas_format=self.testInst.pandas_format,
+            epoch_name=default_epoch_name, **tkwargs)
+
+        for key in ['platform', 'name', 'tag', 'inst_id', 'acknowledgements',
+                    'references']:
+            assert hasattr(meta.header, key) == target
+
+        return
+
     @pytest.mark.parametrize("add_path", [(''), ('unknown_dir')])
     def test_inst_write_and_read_netcdf(self, add_path):
         """Test Instrument netCDF4 read/write, including non-existent paths.
 
         Parameters
         ----------
         add_path : str
@@ -342,24 +378,27 @@
             input_kwargs={'epoch_name': 'whoosthat',
                           'pandas_format': self.testInst.pandas_format,
                           'decode_times': decode_times})
         return
 
     @pytest.mark.parametrize("write_epoch,war_msg", [('epoch',
                                                       'is not a dimension.')])
+    @pytest.mark.parametrize("strict_dim_check", [True, False])
     def test_read_netcdf4_epoch_not_xarray_dimension(self, caplog, write_epoch,
-                                                     war_msg):
+                                                     war_msg, strict_dim_check):
         """Test netCDF4 load `epoch_name` not a dimension.
 
         Parameters
         ----------
         write_epoch : str
             Label used for datetime data when writing file.
         war_msg : str
             Warning message to test for.
+        strict_dim_check : bool
+            If True, raises warning. If False, does not raise warning.
 
         """
 
         if not self.testInst.pandas_format:
             # Load data
             outfile = os.path.join(self.tempdir.name,
                                    'pysat_test_ncdf.nc')
@@ -370,18 +409,21 @@
 
             # Evaluate the expected warning
             with caplog.at_level(logging.WARNING, logger='pysat'):
                 tkwargs = decode_times_val(self.testInst.pandas_format)
 
                 io.load_netcdf(outfile, epoch_name='slt',
                                pandas_format=self.testInst.pandas_format,
-                               **tkwargs)
+                               strict_dim_check=strict_dim_check, **tkwargs)
 
             self.out = caplog.text
-            assert self.out.find(war_msg)
+            if strict_dim_check:
+                assert self.out.find(war_msg) >= 0
+            else:
+                assert self.out.find(war_msg) < 0
         return
 
     @pytest.mark.parametrize("wkwargs, lkwargs", [
         ({"zlib": True}, {}), ({}, {}), ({"unlimited_time": False}, {}),
         ({"epoch_name": "Santa"}, {"epoch_name": "Santa"})])
     def test_write_and_read_netcdf4_w_kwargs(self, wkwargs, lkwargs):
         """Test success of writing and reading a netCDF4 file.
@@ -893,15 +935,15 @@
 
         # Set the input parameters
         mdict = self.testInst.meta[dvar].to_dict()
 
         if dvar.find('int8') >= 0:
             data_type = bool
         else:
-            data_type = type(self.testInst[dvar][0])
+            data_type = type(self.testInst[dvar].values[0])
 
         # Get the filtered output
         with warnings.catch_warnings(record=True) as war:
             fdict = io.filter_netcdf4_metadata(self.testInst, mdict, data_type,
                                                export_nan=export_nan,
                                                remove=remove,
                                                check_type=check_type)
@@ -945,20 +987,25 @@
                     assert ((mdict[mkey] is None) | is_nan), \
                         "{:} is not a fill value: {:}".format(repr(mkey),
                                                               repr(mdict[mkey]))
 
                     assert mkey not in export_nan, \
                         "{:} should have been exported".format(repr(mkey))
             else:
-                if mkey in export_nan and np.isnan(mdict[mkey]):
+                if(mkey in export_nan and not np.issubdtype(data_type, str)
+                   and np.isnan(mdict[mkey])):
                     assert np.isnan(fdict[mkey])
                 else:
-                    assert fdict[mkey] == mdict[mkey], \
-                        "meta data {:} changed".format(repr(mkey))
-
+                    if mkey in check_type and fdict[mkey] != mdict[mkey]:
+                        assert fdict[mkey] == data_type(mdict[mkey]), \
+                            "unexpected recast meta data {:} value".format(
+                                repr(mkey))
+                    else:
+                        assert fdict[mkey] == mdict[mkey], \
+                            "meta data {:} changed".format(repr(mkey))
         return
 
     @pytest.mark.parametrize('missing', [True, False])
     def test_add_netcdf4_standards_to_meta(self, missing):
         """Test for simplified SPDF ISTP/IACG NetCDF standards after update.
 
         Parameters
@@ -1572,15 +1619,15 @@
             Used by `apply_table_translation_to_file` to translate metadata from
             keys into values.
 
         """
 
         # Apply translation
         testing.eval_bad_input(io.apply_table_translation_to_file,
-                               ValueError, 'There is a duplicated',
+                               ValueError, 'There are duplicated variable',
                                input_args=(self.test_inst, self.meta_dict,
                                            meta_trans))
 
         return
 
     def test_from_file_table_translation_default(self):
         """Test `apply_table_translation_from_file` standard."""
@@ -1604,17 +1651,21 @@
         """Test `apply_table_translation_from_file` inconsistency message."""
 
         # Apply default translation
         self.out = io.apply_table_translation_to_file(self.test_inst,
                                                       self.meta_dict)
 
         # Shift values of _FillValue but not FillVal
+        fkey = '_FillValue'
         for key in self.out.keys():
             if '_FillValue' in self.out[key].keys():
-                self.out[key]['_FillValue'] += 1
+                if isinstance(self.out[key][fkey], str):
+                    self.out[key][fkey] += 'shift'
+                else:
+                    self.out[key]['_FillValue'] += 1
 
         # Get default inverse translation
         from_trans = io.default_from_netcdf_translation_table(
             self.test_inst.meta)
 
         # Apply inverse
         with caplog.at_level(logging.WARNING, logger='pysat'):
@@ -1835,7 +1886,72 @@
 
     def teardown_method(self):
         """Cleanup test environment."""
 
         del self.test_inst, self.test_date, self.out, self.meta_dict
 
         return
+
+
+class TestIODeprecation(object):
+    """Unit tests for deprecation warnings in `utils.io`."""
+
+    def setup_method(self):
+        """Set up the test environment."""
+
+        # Create temporary directory
+        self.tempdir = tempfile.TemporaryDirectory()
+        self.saved_path = pysat.params['data_dirs']
+        pysat.params['data_dirs'] = self.tempdir.name
+
+        self.outfile = os.path.join(self.tempdir.name, 'pysat_test_ncdf.nc')
+        self.in_kwargs = {'labels': {
+            'units': ('units', str), 'name': ('long_name', str),
+            'notes': ('notes', str), 'desc': ('desc', str),
+            'min_val': ('value_min', float), 'max_val': ('value_max', float),
+            'fill_val': ('fill', float)}}
+
+        return
+
+    def teardown_method(self):
+        """Clean up the test environment."""
+
+        pysat.params['data_dirs'] = self.saved_path
+
+        # Remove the temporary directory
+        self.tempdir.cleanup()
+
+        # Clear the attributes
+        del self.tempdir, self.saved_path, self.outfile, self.in_kwargs
+        return
+
+    @pytest.mark.parametrize("inst_name,load_func", [
+        ("testing", io.load_netcdf_pandas),
+        ("ndtesting", io.load_netcdf_xarray)])
+    def test_load_netcdf_labels(self, inst_name, load_func):
+        """Test deprecation of `labels` kwarg in different load functions.
+
+        Parameters
+        ----------
+        inst_name : str
+            Instrument name for test Instrument
+        load_func : function
+            NetCDF load method with deprecation warning
+
+        """
+
+        # Create a test file
+        testInst = pysat.Instrument(platform='pysat', name=inst_name,
+                                    num_samples=100, update_files=True,
+                                    use_header=True)
+        testInst.load(date=testInst.inst_module._test_dates[''][''])
+        io.inst_to_netcdf(testInst, fname=self.outfile)
+
+        # Catch the warnings
+        with warnings.catch_warnings(record=True) as war:
+            load_func(self.outfile, **self.in_kwargs)
+
+        # Test the warnings
+        assert len(war) >= 1
+        testing.eval_warnings(war,
+                              ["`labels` is deprecated, use `meta_kwargs`"])
+        return
```

### Comparing `pysat-3.0.6/pysat/tests/test_utils_testing.py` & `pysat-3.1.0/pysat/tests/test_utils_testing.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/tests/test_utils_time.py` & `pysat-3.1.0/pysat/tests/test_utils_time.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/utils/__init__.py` & `pysat-3.1.0/pysat/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 from pysat.utils._core import generate_instrument_list
 from pysat.utils._core import get_mapped_value
 from pysat.utils._core import listify
 from pysat.utils._core import load_netcdf4
 from pysat.utils._core import NetworkLock
 from pysat.utils._core import scale_units
 from pysat.utils._core import stringify
+from pysat.utils._core import update_fill_values
 from pysat.utils import coords
 from pysat.utils import files
 from pysat.utils import io
 from pysat.utils import registry
 from pysat.utils import testing
 from pysat.utils import time
```

### Comparing `pysat-3.0.6/pysat/utils/_core.py` & `pysat-3.1.0/pysat/utils/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,15 +148,20 @@
     Note
     ----
     Does not accept dict_keys or dict_values as input.
 
     """
 
     # Cast as an array-like object
-    arr_iter = np.asarray(iterable)
+    try:
+        arr_iter = np.asarray(iterable)
+    except ValueError:
+        # This is necessary for Python 3.6 compatibility when using listify
+        # on slices
+        arr_iter = np.asarray([iterable])
 
     # Treat output differently based on the array shape
     if arr_iter.shape == ():
         list_iter = [arr_iter.tolist()]
     elif arr_iter.shape[0] == 0:
         list_iter = arr_iter.tolist()
     else:
@@ -406,18 +411,19 @@
 
     Returns
     -------
     output : dict
         Dictionary with keys 'names', 'download', 'no_download' that contain
         lists with different information for each key:
         'names' - list of platform_name combinations
-        'download' - dict containing 'inst_module', 'tag', and 'inst_id' for
-        instruments with download routines
-        'no_download' - dict containing 'inst_module', 'tag', and 'inst_id' for
-        instruments without download routines
+        'download' - list of dicts containing 'inst_module', 'tag', and
+        'inst_id' for instruments with download routines
+        'load_options' - list of dicts containing load and download options
+        'no_download' - list of dicts containing 'inst_module', 'tag', and
+        'inst_id' for instruments without download routines
 
     Note
     ----
     This routine currently supports classification of instruments for unit
     tests both in the core package and in seperate instrument packages that
     use pysat.
 
@@ -470,23 +476,26 @@
                     ci_skip = ((os.environ.get('CI') == 'true')
                                and not inst._test_download_ci)
                     # Some instruments will be skipped in CI but run
                     # locally. Check for this flag.
                     if not ci_skip:
                         # Check if instrument is configured for download tests.
                         if inst._test_download:
-                            instrument_download.append(in_dict)
+                            instrument_download.append(in_dict.copy())
                             if hasattr(module, '_test_load_opt'):
                                 # Add optional load tests
                                 try:
                                     kw_list = module._test_load_opt[iid][tag]
                                     kw_list = pysat.utils.listify(kw_list)
                                     for kwargs in kw_list:
                                         in_dict['kwargs'] = kwargs
-                                        instrument_optional_load.append(in_dict)
+
+                                        # Append as copy so kwargs are unique.
+                                        instrument_optional_load.append(
+                                            in_dict.copy())
                                 except KeyError:
                                     # Option does not exist for tag/inst_id
                                     # combo
                                     pass
 
                         elif not inst._password_req:
                             # We don't want to test download for this combo, but
@@ -667,14 +676,63 @@
                     print("".join([mod_str, " [", tag.__repr__(), " ",
                                    inst_id.__repr__(), "]  ",
                                    inst_info[platform][name]['inst_ids_tags'][
                                        inst_id][tag]]))
     return
 
 
+def update_fill_values(inst, variables=None, new_fill_val=np.nan):
+    """Update Instrument data so that the fill value is consistent with Meta.
+
+    Parameters
+    ----------
+    inst : pysat.Instrument
+        Instrument object with data loaded
+    variables : str, list, or NoneType
+        List of variables to update or None to update all (default=None)
+    new_fill_val : any
+        New fill value to use (default=np.nan)
+
+    Note
+    ----
+    On Windows OS, this function may not work for data variables that are also
+    xarray coordinates.
+
+    """
+
+    if not inst.empty:
+        # Get the variables (if needed) and ensure they are list-like
+        if variables is None:
+            variables = list(inst.variables)
+        else:
+            variables = listify(variables)
+
+        for var in variables:
+            if var in inst.meta.keys():
+                # Get the old fill value
+                old_fill_val = inst.meta[var, inst.meta.labels.fill_val]
+
+                # Update the Meta data
+                inst.meta[var] = {inst.meta.labels.fill_val: new_fill_val}
+
+                # Update the variable data
+                try:
+                    if np.isnan(old_fill_val):
+                        ifill = np.where(np.isnan(inst[var].values))
+                    else:
+                        ifill = np.where(inst[var].values == old_fill_val)
+                except TypeError:
+                    ifill = np.where(inst[var].values == old_fill_val)
+
+                if len(ifill[0]) > 0:
+                    inst[var].values[ifill] = new_fill_val
+
+    return
+
+
 class NetworkLock(Lock):
     """Unit tests for NetworkLock manager."""
 
     def __init__(self, *args, **kwargs):
         """Initialize lock manager compatible with networked file systems.
 
         Parameters
@@ -704,14 +762,15 @@
             timeout = kwargs['timeout']
             del kwargs['timeout']
         else:
             timeout = pysat.params['file_timeout']
 
         super(NetworkLock, self).__init__(timeout=timeout,
                                           *args, **kwargs)
+        return
 
     def release(self):
         """Release the Lock from the file system.
 
         From portalocker docs:
           On some networked filesystems it might be needed to force
           a `os.fsync()` before closing the file so it's
@@ -724,7 +783,8 @@
             # In case of network file system
             os.fsync(self.fh.fileno())
         except OSError:
             # Not a network file system
             pass
 
         super(NetworkLock, self).release()
+        return
```

### Comparing `pysat-3.0.6/pysat/utils/files.py` & `pysat-3.1.0/pysat/utils/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,35 +22,40 @@
 
 def process_parsed_filenames(stored, two_digit_year_break=None):
     """Create a Files pandas Series of filenames from a formatted dict.
 
     Parameters
     ----------
     stored : collections.orderedDict
-        Dict produced by `parse_fixed_width_filenames` or
-        `parse_delimited_filenames`
+        Ordered dictionary produced by `parse_fixed_width_filenames` or
+        `parse_delimited_filenames`, containing date, time, version, and
+        other information extracted from the filenames.
     two_digit_year_break : int or NoneType
         If filenames only store two digits for the year, then
         '1900' will be added for years >= two_digit_year_break
         and '2000' will be added for years < two_digit_year_break.
-        If None, then four-digit years are assumed.
-        (default=None)
+        If None, then four-digit years are assumed. (default=None)
 
     Returns
     -------
     pds.Series
         Series, indexed by datetime, with file strings
 
     Note
     ----
     If two files have the same date and time information in the filename then
     the file with the higher version/revision/cycle is used. Series returned
     only has one file per datetime. Version is required for this filtering,
     revision and cycle are optional.
 
+    See Also
+    --------
+    pysat.utils.files.parse_fixed_width_filenames,
+    pysat.utils.files.parse_delimited_filenames
+
     """
 
     search_dict = construct_searchstring_from_format(stored['format_str'])
     keys = search_dict['keys']
 
     if len(stored['files']) > 0:
         # Deal with the possibility of two digit years. Years above
@@ -118,21 +123,21 @@
         else:
             return pds.Series(files, index=index).sort_index()
     else:
         return pds.Series(None, dtype='object')
 
 
 def parse_fixed_width_filenames(files, format_str):
-    """Parse list of files, extracting data identified by `format_str`.
+    """Extract specified info from a list of files with a fixed name width.
 
     Parameters
     ----------
     files : list
         List of files, typically provided by
-        `files.search_local_system_formatted_filename`.
+        `pysat.utils.files.search_local_system_formatted_filename`.
     format_str : str
         Provides the naming pattern of the instrument files and the
         locations of date information so an ordered list may be produced.
         Supports all provided string formatting codes though only 'year',
         'month', 'day', 'hour', 'minute', 'second', 'version', 'revision',
         and 'cycle' will be used for time and sorting information. For example,
         `instrument-{year:4d}_{month:02d}-{day:02d}_v{version:02d}.cdf`, or
@@ -149,14 +154,18 @@
     Note
     ----
     The function uses the lengths of the fixed characters within `format_str`,
     as well as the supplied lengths for template variables, to determine
     where to parse out information. Thus, support for the wildcard '*' is
     limited to locations before the first template variable.
 
+    See Also
+    --------
+    pysat.utils.files.search_local_system_formatted_filename
+
     """
 
     # Create storage for data to be parsed from filenames
     ordered_keys = ['year', 'month', 'day', 'hour', 'minute', 'second',
                     'version', 'revision', 'cycle']
     stored = collections.OrderedDict({kk: list() for kk in ordered_keys})
 
@@ -219,29 +228,29 @@
     # Include format string as convenience for later functions
     stored['format_str'] = format_str
 
     return stored
 
 
 def parse_delimited_filenames(files, format_str, delimiter):
-    """Parse list of files, extracting data identified by format_str.
+    """Extract specified info from a list of files using a delimiter.
 
     Will parse file using `delimiter` though the function does not require
     every parsed item to be a variable, and more than one variable
     may be within a parsed section. Thus, the main practical
     difference with `parse_fixed_width_filenames` is more support for
     the use of the wildcard '*' within `format_str`. Overuse
     of the '*' wildcard increases the probability of false positive matches
     if there are multiple instrument files in the directory.
 
     Parameters
     ----------
     files : list
         List of files, typically provided by
-        `files.search_local_system_formatted_filename`.
+        `pysat.utils.files.search_local_system_formatted_filename`.
     format_str : str
         Provides the naming pattern of the instrument files and the
         locations of date information so an ordered list may be produced.
         Supports all provided string formatting codes though only 'year',
         'month', 'day', 'hour', 'minute', 'second', 'version', 'revision',
         and 'cycle' will be used for time and sorting information. For example,
         `*_{year:4d}_{month:02d}_{day:02d}_*_v{version:02d}_*.cdf`
@@ -261,14 +270,18 @@
     The '*' wildcard is supported when leading, trailing, or wholly contained
     between delimiters, such as 'data_name-{year:04d}-*-{day:02d}.txt',
     or '*-{year:04d}*-*-{day:02d}*', where '-' is the delimiter.
     There can not be a mixture of a template variable and '*' without a
     delimiter in between, unless the '*' occurs after the variables. The
     '*' should not be used to replace the delimited character in the filename.
 
+    See Also
+    --------
+    pysat.utils.files.search_local_system_formatted_filename
+
     """
 
     # Create storage for data to be parsed from filenames
     ordered_keys = ['year', 'month', 'day', 'hour', 'minute', 'second',
                     'version', 'revision', 'cycle']
     stored = collections.OrderedDict({kk: None for kk in ordered_keys})
 
@@ -533,15 +546,14 @@
 
     """
 
     # Import required here to avoid circular import
     from pysat import Instrument
 
     # Get a list of supported instruments
-    # Best solved with an upcoming method in pull #633
     insts = available_instruments()
 
     if test_run:
         print('Performing a test run. No files will be moved.\n')
 
     if len(insts.keys()) == 0:
         ostr = ''.join(('No registered instruments detected. Please register ',
@@ -735,43 +747,57 @@
 
 def check_and_make_path(path, expand_path=False):
     """Check if path exists and create it if needed.
 
     Parameters
     ----------
     path : str
-        Directory path without any file names. Creates all
-        necessary directories to complete the path.
+        String specifying a directory path without any file names. All
+        directories needed to create the full path will be created.
     expand_path : bool
         If True, input `path` will be processed through `os.path.expanduser`
-        and `os.path.expandvars`.
+        (accounting for `~` and `~user` constructs, if $HOME and user are known)
+        and `os.path.expandvars` (accounting for environment variables)
 
     Returns
     -------
     made_dir : bool
         True, if new directory made. False, if path already existed.
 
     Raises
     ------
     ValueError
-        If input path and internally constructed path are not equal, or
-        if an invalid path supplied.
+        If an invalid path is supplied.
+    RuntimeError
+        If the input path and internally constructed paths differ.
+
+    See Also
+    --------
+    os.path.expanduser, os.path.expandvars
 
     """
 
     if expand_path:
-        # Account for home references, multi-platform
+        # Account for home, user, and environment variables references
         path = os.path.expanduser(path)
         path = os.path.expandvars(path)
 
-    if not os.path.exists(path):
-        # Make path, checking to see that each level exists before attempting
+    if len(path) == 0:
+        # The user wants to write to the current directory
+        path = os.getcwd()
+
+    # Set the output
+    made_dir = not os.path.exists(path)
+
+    if made_dir:
+        # The directory(ies) need to be made, check to see whether or not each
+        # level exists before attempting to make each directory in the path
         root_path, local_dir = os.path.split(path)
 
-        # Check that we have a remotely valid path
+        # Check that we have a potentially valid path
         if len(root_path) == 0:
             raise ValueError('Invalid path specification.')
 
         # Iterate through given path until we hit a directory that exists.
         make_dir = list()
         while not os.path.exists(root_path):
             if len(local_dir) > 0:
@@ -788,52 +814,52 @@
             # Avoid case where input is path='/stuff/level/'.
             # The trailing '/' leads to a local_dir=''
             make_dir.append(local_dir)
 
         while len(make_dir) > 0:
             local_dir = make_dir.pop()
             root_path = os.path.join(root_path, local_dir)
-            if (local_dir != '..') and (local_dir != '.'):
+            if local_dir != '..' and local_dir != '.':
                 # Deal with case of path='... /path1/../final_path' or
                 # path='... /path1/./final_path'
                 os.mkdir(root_path)
 
         if os.path.normpath(root_path) != os.path.normpath(path):
             estr = ''.join(['Desired and constructed paths unexpectedly differ',
                             '. Please post an issue at https://github.com/pysa',
                             't/pysat/issues'])
-            raise ValueError(estr)
+            raise RuntimeError(estr)
 
-        return True
-    else:
-        return False
+    return made_dir
 
 
 def get_file_information(paths, root_dir=''):
-    """Create a dict with values from `os.stat` attributes for input path(s).
+    """Retrieve system statistics for the input path(s).
 
     Parameters
     ----------
     paths : str or list
         Full pathnames of files to get attribute information.
     root_dir : str
         Common root path shared by all paths, if any. (default='')
 
     Returns
     -------
     file_info : dict
-        Keyed by file attribute. Each attribute maps to a list
+        Keyed by file attribute, which uses names that mirror or are expanded
+        upon those used by `os.stat`. Each attribute maps to a list
         of values for each file in `paths`.
 
     See Also
     --------
-    os.stat : Get variety of file attributes
+    os.stat
 
     """
 
+    # Ensure the input is a list
     paths = listify(paths)
 
     # Mapping of output key to the attribute name returned by `os.stat`
     attrs = {'content_modified_time': 'st_mtime', 'mode': 'st_mode',
              'size': 'st_size', 'inode': 'st_ino', 'device': 'st_dev',
              'nlink': 'st_nlink', 'uid': 'st_uid', 'gid': 'st_gid',
              'last_access_time': 'st_atime',
```

### Comparing `pysat-3.0.6/pysat/utils/io.py` & `pysat-3.1.0/pysat/utils/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,30 +47,32 @@
             if data_key in xarr_lvars:
                 for i in range(len(xarr_lvars)):
                     if data_key == xarr_lvars[i]:
                         break
 
                 # Cycle through all the pysat MetaData labels and transfer
                 for meta_key in pysat_meta[data_key].keys():
-                    # Assign attributes
-                    xr_data[xarr_vars[i]].attrs[meta_key] = pysat_meta[
-                        data_key][meta_key]
+                    # Assign attributes with values that are not None
+                    if pysat_meta[data_key][meta_key] is not None:
+                        xr_data[xarr_vars[i]].attrs[meta_key] = pysat_meta[
+                            data_key][meta_key]
 
             else:
                 wstr = ''.join(['Did not find data for metadata variable ',
                                 data_key, '.'])
                 warnings.warn(wstr)
 
     # Transfer metadata for the main time index. Cycle through all the pysat
     # MetaData labels and transfer.
     if epoch_name in pysat_meta.keys():
         for meta_key in pysat_meta[epoch_name].keys():
-            # Assign attributes
-            xr_data[epoch_name].attrs[meta_key] = pysat_meta[epoch_name][
-                meta_key]
+            # Assign attributes that are not None
+            if pysat_meta[epoch_name][meta_key] is not None:
+                xr_data[epoch_name].attrs[meta_key] = pysat_meta[epoch_name][
+                    meta_key]
 
     return
 
 
 def filter_netcdf4_metadata(inst, mdata_dict, coltype, remove=False,
                             check_type=None, export_nan=None, varname=''):
     """Filter metadata properties to be consistent with netCDF4.
@@ -511,43 +513,48 @@
     """Translate labels in `meta_dict` using `trans_table`.
 
     Parameters
     ----------
     inst : pysat.Instrument
         Instrument object with data to be written to file.
     meta_dict : dict
-        Output starting from `Instrument.meta.to_dict() `supplying attribute
+        Output starting from `Instrument.meta.to_dict()` supplying attribute
         data.
     trans_table : dict or NoneType
         Keyed by current metalabels containing a list of
         metadata labels to use within the returned dict. If None,
         a default translation using `self.labels` will be used except
         `self.labels.fill_val` will be mapped to
         `['_FillValue', 'FillVal', 'fill']`.
 
     Returns
     -------
     export_dict : dict
         A dictionary of the metadata for each variable of an output file.
 
+    Raises
+    ------
+    ValueError
+        If there is a duplicated variable label in the translation table
+
     """
 
     export_dict = {}
 
     if trans_table is None:
         trans_table = default_to_netcdf_translation_table(inst)
 
     # Confirm there are no duplicated translation labels
-    trans_labels = [trans_table[key] for key in trans_table.keys()]
-    for i in np.arange(len(trans_labels)):
-        item = trans_labels.pop(0)
-        if item in trans_labels:
-            estr = ''.join(['There is a duplicated variable label value in ',
-                            '`trans_table`: ', item])
-            raise ValueError(estr)
+    trans_labels = list()
+    for key in trans_table.keys():
+        trans_labels.extend(trans_table[key])
+
+    if np.unique(trans_labels).shape[0] != len(trans_labels):
+        raise ValueError(''.join(['There are duplicated variable label values',
+                                  ' in `trans_table`']))
 
     # Translate each metadata label if a translation is provided
     for key in meta_dict.keys():
         export_dict[key] = {}
         loop_meta_dict = meta_dict[key]
         for orig_key in loop_meta_dict:
             if orig_key in trans_table:
@@ -686,23 +693,18 @@
 
     return meta_dict
 
 
 def load_netcdf(fnames, strict_meta=False, file_format='NETCDF4',
                 epoch_name=None, epoch_unit='ms', epoch_origin='unix',
                 pandas_format=True, decode_timedelta=False,
-                labels={'units': ('units', str), 'name': ('long_name', str),
-                        'notes': ('notes', str), 'desc': ('desc', str),
-                        'plot': ('plot_label', str), 'axis': ('axis', str),
-                        'scale': ('scale', str),
-                        'min_val': ('value_min', np.float64),
-                        'max_val': ('value_max', np.float64),
-                        'fill_val': ('fill', np.float64)},
+                combine_by_coords=True, meta_kwargs=None, labels=None,
                 meta_processor=None, meta_translation=None,
-                drop_meta_labels=None, decode_times=None):
+                drop_meta_labels=None, decode_times=None,
+                strict_dim_check=True):
     """Load netCDF-3/4 file produced by pysat.
 
     Parameters
     ----------
     fnames : str or array_like
         Filename(s) to load, will fail if None. (default=None)
     strict_meta : bool
@@ -735,21 +737,25 @@
     pandas_format : bool
         Flag specifying if data is stored in a pandas DataFrame (True) or
         xarray Dataset (False). (default=False)
     decode_timedelta : bool
         Used for xarray data (`pandas_format` is False).  If True, variables
         with unit attributes that  are 'timelike' ('hours', 'minutes', etc) are
         converted to `np.timedelta64`. (default=False)
-    labels : dict
+    combine_by_coords : bool
+        Used for xarray data (`pandas_format` is False) when loading a
+        multi-file dataset. If True, uses `xarray.combine_by_coords`. If False,
+        uses `xarray.combine_nested`. (default=True)
+    meta_kwargs : dict or NoneType
+        Dict to specify custom Meta initialization or None to use Meta
+        defaults (default=None)
+    labels : dict or NoneType
         Dict where keys are the label attribute names and the values are tuples
-        that have the label values and value types in that order.
-        (default={'units': ('units', str), 'name': ('long_name', str),
-        'notes': ('notes', str), 'desc': ('desc', str),
-        'min_val': ('value_min', np.float64),
-        'max_val': ('value_max', np.float64), 'fill_val': ('fill', np.float64)})
+        that have the label values and value types in that order. None to use
+        meta defaults.  Deprecated, use `meta_kwargs` instead. (default=None)
     meta_processor : function or NoneType
         If not None, a dict containing all of the loaded metadata will be
         passed to `meta_processor` which should return a filtered version
         of the input dict. The returned dict is loaded into a pysat.Meta
         instance and returned as `meta`. (default=None)
     meta_translation : dict or NoneType
         Translation table used to map metadata labels in the file to
@@ -764,14 +770,18 @@
         to metadata as loaded from the file. (default=None)
     decode_times : bool or NoneType
         If True, variables with unit attributes that are 'timelike' ('hours',
         'minutes', etc) are converted to `np.timedelta64` by xarray. If False,
         then `epoch_name` will be converted to datetime using `epoch_unit`
         and `epoch_origin`. If None, will be set to False for backwards
         compatibility. For xarray only. (default=None)
+    strict_dim_check : bool
+        Used for xarray data (`pandas_format` is False). If True, warn the user
+        that the desired epoch is not present in `xarray.dims`.  If False,
+        no warning is raised. (default=True)
 
     Returns
     -------
     data : pandas.DataFrame or xarray.Dataset
         Class holding file data
     meta : pysat.Meta
         Class holding file meta data
@@ -796,46 +806,40 @@
             raise ValueError(estr)
 
         data, meta = load_netcdf_pandas(fnames, strict_meta=strict_meta,
                                         file_format=file_format,
                                         epoch_name=epoch_name,
                                         epoch_unit=epoch_unit,
                                         epoch_origin=epoch_origin,
-                                        labels=labels,
+                                        meta_kwargs=meta_kwargs, labels=labels,
                                         meta_processor=meta_processor,
                                         meta_translation=meta_translation,
                                         drop_meta_labels=drop_meta_labels)
     else:
         data, meta = load_netcdf_xarray(fnames, strict_meta=strict_meta,
                                         file_format=file_format,
                                         epoch_name=epoch_name,
                                         epoch_unit=epoch_unit,
                                         epoch_origin=epoch_origin,
                                         decode_timedelta=decode_timedelta,
-                                        labels=labels,
+                                        combine_by_coords=combine_by_coords,
+                                        meta_kwargs=meta_kwargs, labels=labels,
                                         meta_processor=meta_processor,
                                         meta_translation=meta_translation,
                                         drop_meta_labels=drop_meta_labels,
-                                        decode_times=decode_times)
+                                        decode_times=decode_times,
+                                        strict_dim_check=strict_dim_check)
 
     return data, meta
 
 
 def load_netcdf_pandas(fnames, strict_meta=False, file_format='NETCDF4',
                        epoch_name='Epoch', epoch_unit='ms', epoch_origin='unix',
-                       labels={'units': ('units', str),
-                               'name': ('long_name', str),
-                               'notes': ('notes', str), 'desc': ('desc', str),
-                               'plot': ('plot_label', str),
-                               'axis': ('axis', str), 'scale': ('scale', str),
-                               'min_val': ('value_min', np.float64),
-                               'max_val': ('value_max', np.float64),
-                               'fill_val': ('fill', np.float64)},
-                       meta_processor=None, meta_translation=None,
-                       drop_meta_labels=None):
+                       meta_kwargs=None, labels=None, meta_processor=None,
+                       meta_translation=None, drop_meta_labels=None):
     """Load netCDF-3/4 file produced by pysat in a pandas format.
 
     Parameters
     ----------
     fnames : str or array_like
         Filename(s) to load
     strict_meta : bool
@@ -859,21 +863,21 @@
         `pandas.to_datetime`.  Accepts timestamp-convertable objects, as well as
         two specific strings for commonly used calendars.  These conversions are
         handled by `pandas.to_datetime`.
         If ‘unix’ (or POSIX) time; origin is set to 1970-01-01.
         If ‘julian’, `epoch_unit` must be ‘D’, and origin is set to beginning of
         Julian Calendar. Julian day number 0 is assigned to the day starting at
         noon on January 1, 4713 BC. (default='unix')
-    labels : dict
+    meta_kwargs : dict or NoneType
+        Dict to specify custom Meta initialization or None to use Meta
+        defaults (default=None)
+    labels : dict or NoneType
         Dict where keys are the label attribute names and the values are tuples
-        that have the label values and value types in that order.
-        (default={'units': ('units', str), 'name': ('long_name', str),
-        'notes': ('notes', str), 'desc': ('desc', str),
-        'min_val': ('value_min', np.float64),
-        'max_val': ('value_max', np.float64), 'fill_val': ('fill', np.float64)})
+        that have the label values and value types in that order or None to use
+        Meta defaults. Deprecated, use `meta_kwargs` instead. (default=None)
     meta_processor : function or NoneType
         If not None, a dict containing all of the loaded metadata will be
         passed to `meta_processor` which should return a filtered version
         of the input dict. The returned dict is loaded into a pysat.Meta
         instance and returned as `meta`. (default=None)
     meta_translation : dict or NoneType
         Translation table used to map metadata labels in the file to
@@ -922,15 +926,26 @@
 
     # Initialize local variables
     saved_meta = None
     running_idx = 0
     running_store = []
     two_d_keys = []
     two_d_dims = []
-    meta = pysat.Meta(labels=labels)
+
+    if meta_kwargs is None:
+        meta_kwargs = {}
+
+    if labels is not None:
+        warnings.warn("".join(["`labels` is deprecated, use `meta_kwargs`",
+                               "with the 'labels' key instead. Support ",
+                               "for `labels` will be removed in v3.2.0+"]),
+                      DeprecationWarning, stacklevel=2)
+        meta_kwargs['labels'] = labels
+
+    meta = pysat.Meta(**meta_kwargs)
 
     # Store all metadata in a dict that may be filtered before
     # assignment to `meta`.
     full_mdict = {}
 
     if meta_translation is None:
         # Assign default translation using `meta`
@@ -1169,15 +1184,15 @@
     # labels.
     filt_mdict = meta_array_expander(filt_mdict)
 
     # Assign filtered metadata to pysat.Meta instance
     for key in filt_mdict:
         if 'meta' in filt_mdict[key].keys():
             # Higher order metadata
-            dim_meta = pysat.Meta(labels=labels)
+            dim_meta = pysat.Meta(**meta_kwargs)
             for skey in filt_mdict[key]['meta'].keys():
                 dim_meta[skey] = filt_mdict[key]['meta'][skey]
 
             # Remove HO metdata that was just transfered elsewhere
             filt_mdict[key].pop('meta')
 
             # Assign standard metdata
@@ -1190,26 +1205,18 @@
             meta[key] = filt_mdict[key]
 
     return data, meta
 
 
 def load_netcdf_xarray(fnames, strict_meta=False, file_format='NETCDF4',
                        epoch_name='time', epoch_unit='ms', epoch_origin='unix',
-                       decode_timedelta=False,
-                       labels={'units': ('units', str),
-                               'name': ('long_name', str),
-                               'notes': ('notes', str), 'desc': ('desc', str),
-                               'plot': ('plot_label', str),
-                               'axis': ('axis', str),
-                               'scale': ('scale', str),
-                               'min_val': ('value_min', np.float64),
-                               'max_val': ('value_max', np.float64),
-                               'fill_val': ('fill', np.float64)},
-                       meta_processor=None, meta_translation=None,
-                       drop_meta_labels=None, decode_times=False):
+                       decode_timedelta=False, combine_by_coords=True,
+                       meta_kwargs=None, labels=None, meta_processor=None,
+                       meta_translation=None, drop_meta_labels=None,
+                       decode_times=False, strict_dim_check=True):
     """Load netCDF-3/4 file produced by pysat into an xarray Dataset.
 
     Parameters
     ----------
     fnames : str or array_like
         Filename(s) to load.
     strict_meta : bool
@@ -1236,21 +1243,25 @@
         If ‘unix’ (or POSIX) time; origin is set to 1970-01-01.
         If ‘julian’, `epoch_unit` must be ‘D’, and origin is set to beginning of
         Julian Calendar. Julian day number 0 is assigned to the day starting at
         noon on January 1, 4713 BC. (default='unix')
     decode_timedelta : bool
         If True, variables with unit attributes that are 'timelike' ('hours',
         'minutes', etc) are converted to `np.timedelta64`. (default=False)
-    labels : dict
+    combine_by_coords : bool
+        Used for xarray data (`pandas_format` is False) when loading a
+        multi-file dataset. If True, uses `xarray.combine_by_coords`. If False,
+        uses `xarray.combine_nested`. (default=True)
+    meta_kwargs : dict or NoneType
+        Dict to specify custom Meta initialization or None to use Meta
+        defaults (default=None)
+    labels : dict or NoneType
         Dict where keys are the label attribute names and the values are tuples
-        that have the label values and value types in that order.
-        (default={'units': ('units', str), 'name': ('long_name', str),
-        'notes': ('notes', str), 'desc': ('desc', str),
-        'min_val': ('value_min', np.float64),
-        'max_val': ('value_max', np.float64), 'fill_val': ('fill', np.float64)})
+        that have the label values and value types in that order or None to use
+        Meta defaults. Deprecated, use `meta_kwargs` instead. (default=None)
     meta_processor : function or NoneType
         If not None, a dict containing all of the loaded metadata will be
         passed to `meta_processor` which should return a filtered version
         of the input dict. The returned dict is loaded into a pysat.Meta
         instance and returned as `meta`. (default=None)
     meta_translation : dict or NoneType
         Translation table used to map metadata labels in the file to
@@ -1265,14 +1276,18 @@
         to metadata as loaded from the file. (default=None)
     decode_times : bool or NoneType
         If True, variables with unit attributes that are 'timelike' ('hours',
         'minutes', etc) are converted to `np.timedelta64` by xarray. If False,
         then `epoch_name` will be converted to datetime using `epoch_unit`
         and `epoch_origin`. If None, will be set to False for backwards
         compatibility. (default=None)
+    strict_dim_check : bool
+        Used for xarray data (`pandas_format` is False). If True, warn the user
+        that the desired epoch is not present in `xarray.dims`.  If False,
+        no warning is raised. (default=True)
 
     Returns
     -------
     data : xarray.Dataset
         Class holding file data
     meta : pysat.Meta
         Class holding file meta data
@@ -1294,15 +1309,25 @@
         epoch_name = 'time'
 
     # Ensure inputs are in the correct format
     fnames = pysat.utils.listify(fnames)
     file_format = file_format.upper()
 
     # Initialize local variables
-    meta = pysat.Meta(labels=labels)
+    if meta_kwargs is None:
+        meta_kwargs = {}
+
+    if labels is not None:
+        warnings.warn("".join(["`labels` is deprecated, use `meta_kwargs`",
+                               "with the 'labels' key instead. Support ",
+                               "for `labels` will be removed in v3.2.0+"]),
+                      DeprecationWarning, stacklevel=2)
+        meta_kwargs['labels'] = labels
+
+    meta = pysat.Meta(**meta_kwargs)
 
     # Store all metadata in a dict that may be filtered before
     # assignment to `meta`.
     full_mdict = {}
 
     if meta_translation is None:
         # Assign default translation using `meta`
@@ -1310,35 +1335,41 @@
 
     # Drop metadata labels initialization
     if drop_meta_labels is None:
         drop_meta_labels = []
     else:
         drop_meta_labels = pysat.utils.listify(drop_meta_labels)
 
+    if combine_by_coords:
+        combine_kw = {'combine': 'by_coords'}
+    else:
+        combine_kw = {'combine': 'nested', 'concat_dim': epoch_name}
+
     # Load the data differently for single or multiple files
     if len(fnames) == 1:
         data = xr.open_dataset(fnames[0], decode_timedelta=decode_timedelta,
                                decode_times=decode_times)
     else:
         data = xr.open_mfdataset(fnames, decode_timedelta=decode_timedelta,
-                                 combine='by_coords', decode_times=decode_times)
+                                 decode_times=decode_times, **combine_kw)
 
     # Need to get a list of all variables, dimensions, and coordinates.
     all_vars = xarray_all_vars(data)
 
     # Rename `epoch_name` to 'time'
     if epoch_name != 'time':
         if 'time' not in all_vars:
             if epoch_name in data.dims:
                 data = data.rename({epoch_name: 'time'})
             elif epoch_name in all_vars:
                 data = data.rename({epoch_name: 'time'})
-                wstr = ''.join(['Epoch label: "', epoch_name, '"',
-                                ' is not a dimension.'])
-                pysat.logger.warning(wstr)
+                if strict_dim_check:
+                    wstr = ''.join(['Epoch label: "', epoch_name, '"',
+                                    ' is not a dimension.'])
+                    pysat.logger.warning(wstr)
             else:
                 estr = ''.join(['Epoch label: "', epoch_name, '"',
                                 ' was not found in loaded dimensions [',
                                 ', '.join(all_vars), ']'])
                 raise KeyError(estr)
         else:
             estr = ''.join(["'time' already present in file. Can't rename ",
@@ -1433,15 +1464,15 @@
         new_dict = {}
 
     # Update basic labels, if they are missing.
     epoch_label = 'Milliseconds since 1970-1-1 00:00:00'
     basic_labels = [inst.meta.labels.units]
 
     for label in basic_labels:
-        if label not in new_dict or len(new_dict[label]) == 0:
+        if label not in new_dict or new_dict[label] == '':
             new_dict[label] = epoch_label
 
     # Assign name
     new_dict[inst.meta.labels.name] = epoch_name
 
     # Update the time standards
     time_dict = {'calendar': 'standard', 'Format': 'i8', 'Var_Type': 'data',
@@ -1526,16 +1557,16 @@
 
     return all_vars
 
 
 def inst_to_netcdf(inst, fname, base_instrument=None, epoch_name=None,
                    mode='w', zlib=False, complevel=4, shuffle=True,
                    preserve_meta_case=False, check_type=None, export_nan=None,
-                   unlimited_time=True, meta_translation=None,
-                   meta_processor=None):
+                   export_pysat_info=True, unlimited_time=True,
+                   meta_translation=None, meta_processor=None):
     """Store pysat data in a netCDF4 file.
 
     Parameters
     ----------
     inst : pysat.Instrument
         Instrument object with loaded data to save
     fname : str
@@ -1576,14 +1607,17 @@
         By default, the metadata variables where a value of NaN is allowed
         and written to the netCDF4 file is maintained by the Meta object
         attached to the pysat.Instrument object. A list supplied here
         will override the settings provided by Meta, and all parameters
         included will be written to the file. If not listed
         and a value is NaN then that attribute simply won't be included in
         the netCDF4 file. (default=None)
+    export_pysat_info : bool
+        Appends the platform, name, tag, and inst_id to the metadata
+        if True. Otherwise these attributes are lost. (default=True)
     unlimited_time : bool
         Flag specifying whether or not the epoch/time dimension should be
         unlimited; it is when the flag is True. (default=True)
     meta_translation : dict or NoneType
         The keys in the input dict are used to map
         metadata labels for `inst` to one or more values used when writing
         the file. E.g., `{meta.labels.fill_val: ['FillVal', '_FillValue']}`
@@ -1684,31 +1718,36 @@
     # Add additional metadata to conform to standards
     attrb_dict['pysat_version'] = pysat.__version__
     if 'Conventions' not in attrb_dict:
         attrb_dict['Conventions'] = 'pysat-simplified SPDF ISTP/IACG for NetCDF'
     if 'Text_Supplement' not in attrb_dict:
         attrb_dict['Text_Supplement'] = ''
 
+    # TODO(#1122): Evaluate whether pop is necessary for all these.
     # Remove any attributes with the names below. pysat is responsible
     # for including them in the file.
     pysat_items = ['Date_End', 'Date_Start', 'File', 'File_Date',
-                   'Generation_Date', 'Logical_File_ID']
+                   'Generation_Date', 'Logical_File_ID', 'acknowledgements',
+                   'references']
     for pitem in pysat_items:
         if pitem in attrb_dict:
             pysat.logger.debug('Removing {} attribute and replacing.'.format(
                 pitem))
             attrb_dict.pop(pitem)
 
     # Set the general file information
-    attrb_dict['platform'] = inst.platform
-    attrb_dict['name'] = inst.name
-    attrb_dict['tag'] = inst.tag
-    attrb_dict['inst_id'] = inst.inst_id
-    attrb_dict['acknowledgements'] = inst.acknowledgements
-    attrb_dict['references'] = inst.references
+    if export_pysat_info:
+        # For operational instruments, these should be set separately.
+        attrb_dict['platform'] = inst.platform
+        attrb_dict['name'] = inst.name
+        attrb_dict['tag'] = inst.tag
+        attrb_dict['inst_id'] = inst.inst_id
+        attrb_dict['acknowledgements'] = inst.acknowledgements
+        attrb_dict['references'] = inst.references
+
     attrb_dict['Date_End'] = dt.datetime.strftime(
         inst.index[-1], '%a, %d %b %Y,  %Y-%m-%dT%H:%M:%S.%f')
     attrb_dict['Date_End'] = attrb_dict['Date_End'][:-3] + ' UTC'
 
     attrb_dict['Date_Start'] = dt.datetime.strftime(
         inst.index[0], '%a, %d %b %Y,  %Y-%m-%dT%H:%M:%S.%f')
     attrb_dict['Date_Start'] = attrb_dict['Date_Start'][:-3] + ' UTC'
@@ -1752,20 +1791,17 @@
     # Ensure `meta_translation` has default values for items not assigned.
     # This is needed for the higher order pandas support and may be removed.
     def_meta_trans = default_to_netcdf_translation_table(inst)
     for key in def_meta_trans.keys():
         if key not in meta_translation:
             meta_translation[key] = def_meta_trans[key]
 
-    # Get current metadata in dictionary form
+    # Get current metadata in dictionary form and add epoch metadata
     export_meta = inst.meta.to_dict()
-
-    # Add in epoch metadata, not normally stored in meta.
-    epoch_meta = return_epoch_metadata(inst, epoch_name)
-    export_meta[epoch_name] = epoch_meta
+    export_meta[epoch_name] = return_epoch_metadata(inst, epoch_name)
 
     # Ensure the metadata is set and updated to netCDF4 standards
     export_meta = add_netcdf4_standards_to_metadict(inst, export_meta,
                                                     epoch_name,
                                                     check_type=check_type,
                                                     export_nan=export_nan)
 
@@ -1857,18 +1893,25 @@
                         cdfkey[:] = data.values.astype(coltype)
                 else:
                     # It is a Series of objects.  First, figure out what the
                     # individual object types are.  Then, act as needed.
 
                     # Use info in coltype to get real datatype of object
                     if coltype == str:
+                        if '_FillValue' in export_meta[lower_key].keys():
+                            str_fill = export_meta[lower_key]['_FillValue']
+                            del export_meta[lower_key]['_FillValue']
+                        else:
+                            str_fill = ''
+
                         cdfkey = out_data.createVariable(case_key, coltype,
                                                          dimensions=epoch_name,
                                                          complevel=complevel,
-                                                         shuffle=shuffle)
+                                                         shuffle=shuffle,
+                                                         fill_value=str_fill)
 
                         # Set metadata
                         cdfkey.setncatts(export_meta[lower_key])
 
                         # Time to actually write the data now
                         cdfkey[:] = data.values
 
@@ -1988,17 +2031,16 @@
                                 cdfkey[:, :] = temp_cdf_data
 
                         # We are done storing the actual data for the given
                         # higher order variable. Now we need to store the index
                         # for all of that fancy data.
 
                         # Get index information
-                        idx = good_data_loc
                         data, coltype, datetime_flag = inst._get_data_info(
-                            inst[key].iloc[idx].index)
+                            inst[key].iloc[good_data_loc].index)
 
                         # Create dimension variable to store index in netCDF4
                         cdfkey = out_data.createVariable(case_key, coltype,
                                                          dimensions=var_dim,
                                                          zlib=zlib,
                                                          complevel=complevel,
                                                          shuffle=shuffle)
@@ -2030,15 +2072,16 @@
         xr_data = xr.Dataset(inst.data)
 
         # Convert datetime values into integers as done for pandas
         xr_data['time'] = (inst['time'].values.astype(np.int64)
                            * 1.0E-6).astype(np.int64)
 
         # Update 'time' dimension to `epoch_name`
-        xr_data = xr_data.rename({'time': epoch_name})
+        if epoch_name != 'time':
+            xr_data = xr_data.rename({'time': epoch_name})
 
         # Transfer metadata
         pysat_meta_to_xarray_attr(xr_data, export_meta, epoch_name)
 
         # If the case needs to be preserved, update Dataset variables.
         if preserve_meta_case:
             for var in xarray_vars_no_time(xr_data, time_label=epoch_name):
@@ -2056,14 +2099,20 @@
         # in `encoding` for data found to be string type.
         for var in xr_data.keys():
             vtype = xr_data[var].dtype
 
             # Account for possible type for unicode strings
             if vtype == np.dtype('<U4'):
                 vtype = str
+                # TODO(#1102): xarray does not yet support '_FillValue' for
+                # unicode strings (https://github.com/pydata/xarray/issues/1647)
+                if '_FillValue' in xr_data[var].attrs:
+                    del xr_data[var].attrs['_FillValue']
+            elif vtype == str:
+                encoding[var]['dtype'] = 'S1'
 
             if vtype == str:
                 encoding[var]['zlib'] = False
 
         if unlimited_time:
             xr_data.encoding['unlimited_dims'] = {epoch_name: True}
```

### Comparing `pysat-3.0.6/pysat/utils/registry.py` & `pysat-3.1.0/pysat/utils/registry.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat/utils/testing.py` & `pysat-3.1.0/pysat/utils/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,15 @@
 
     if input_kwargs is None:
         input_kwargs = {}
 
     # Call the function, catching only the expected error type
     try:
         func(*input_args, **input_kwargs)
+        raise AssertionError('no {:} raised'.format(repr(error)))
     except error as err:
         # Evaluate the error message
         assert str(err).find(err_msg) >= 0, \
             "unexpected error message ('{:}' not in '{:}')".format(err_msg,
                                                                    str(err))
 
     return
```

### Comparing `pysat-3.0.6/pysat/utils/time.py` & `pysat-3.1.0/pysat/utils/time.py`

 * *Files identical despite different names*

### Comparing `pysat-3.0.6/pysat.egg-info/PKG-INFO` & `pysat-3.1.0/pysat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pysat
-Version: 3.0.6
+Version: 3.1.0
 Summary: 'Supports science analysis across disparate data platforms'
 Home-page: https://github.com/pysat/pysat
 Author: Russell Stoneback, et al.
 Author-email: pysat.developers@gmail.com
+License: UNKNOWN
 Keywords: pysat,ionosphere,atmosphere,thermosphere,magnetosphere,heliosphere,observations,models,space,satellites,analysis
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -115,7 +117,9 @@
   * xarray
 * The first time the package is run, you will need to specify a directory to
   store data. In python, run:
 ```
 pysat.params['data_dirs'] = 'path/to/directory/that/may/or/may/not/exist'
 ```
   * Nominal organization of data is top_dir/platform/name/tag/inst_id/files
+
+
```

### Comparing `pysat-3.0.6/pysat.egg-info/SOURCES.txt` & `pysat-3.1.0/pysat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 ecosystem.txt
-nrl_sami.py
 requirements.txt
 setup.cfg
 setup.py
 test_requirements.txt
 pysat/__init__.py
 pysat/_constellation.py
 pysat/_files.py
@@ -25,14 +24,15 @@
 pysat.egg-info/not-zip-safe
 pysat.egg-info/requires.txt
 pysat.egg-info/top_level.txt
 pysat/constellations/__init__.py
 pysat/constellations/single_test.py
 pysat/constellations/testing.py
 pysat/constellations/testing_empty.py
+pysat/constellations/testing_partial.py
 pysat/instruments/__init__.py
 pysat/instruments/pysat_ndtesting.py
 pysat/instruments/pysat_netcdf.py
 pysat/instruments/pysat_testing.py
 pysat/instruments/pysat_testing2d.py
 pysat/instruments/pysat_testing2d_xarray.py
 pysat/instruments/pysat_testing_xarray.py
```

### Comparing `pysat-3.0.6/setup.cfg` & `pysat-3.1.0/setup.cfg`

 * *Files identical despite different names*

