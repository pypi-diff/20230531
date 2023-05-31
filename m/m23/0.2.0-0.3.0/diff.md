# Comparing `tmp/m23-0.2.0.tar.gz` & `tmp/m23-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m23-0.2.0.tar", last modified: Mon May 22 12:56:49 2023, max compression
+gzip compressed data, was "m23-0.3.0.tar", last modified: Wed May 31 20:59:39 2023, max compression
```

## Comparing `m23-0.2.0.tar` & `m23-0.3.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.752283 m23-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-22 12:56:49.752283 m23-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 12:56:30.000000 m23-0.2.0/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.744283 m23-0.2.0/m23/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 12:56:30.000000 m23-0.2.0/m23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-22 12:56:30.000000 m23-0.2.0/m23/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/align/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-22 12:56:30.000000 m23-0.2.0/m23/align/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 12:56:30.000000 m23-0.2.0/m23/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-22 12:56:30.000000 m23-0.2.0/m23/calibrate/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-22 12:56:30.000000 m23-0.2.0/m23/calibrate/master_calibrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-22 12:56:30.000000 m23-0.2.0/m23/charts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/combine/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-22 12:56:30.000000 m23-0.2.0/m23/combine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-22 12:56:30.000000 m23-0.2.0/m23/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/extract/
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-22 12:56:30.000000 m23-0.2.0/m23/extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/aligned_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/color_normalized_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/flux_log_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/log_file_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/masterflat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/normfactor_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/raw_image_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/reference_log_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/ri_color_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/internight_normalize/
--rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-05-22 12:56:30.000000 m23-0.2.0/m23/internight_normalize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/region.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/norm/
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-22 12:56:30.000000 m23-0.2.0/m23/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-22 12:56:30.000000 m23-0.2.0/m23/norm/get_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.752283 m23-0.2.0/m23/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/generate_masterflat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/nights_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/process_nights.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/renormalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/renormalize_config_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.752283 m23-0.2.0/m23/trans/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-22 12:56:30.000000 m23-0.2.0/m23/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 12:56:30.000000 m23-0.2.0/m23/trans/fits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.752283 m23-0.2.0/m23/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-22 12:56:30.000000 m23-0.2.0/m23/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-22 12:56:30.000000 m23-0.2.0/m23/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-22 12:56:30.000000 m23-0.2.0/m23/utils/flux_to_magnitude.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-22 12:56:30.000000 m23-0.2.0/m23/utils/rename.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 12:56:30.000000 m23-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:56:49.752283 m23-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.912339 m23-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-31 20:59:39.912339 m23-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 20:59:20.000000 m23-0.3.0/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.904339 m23-0.3.0/m23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:20.000000 m23-0.3.0/m23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-31 20:59:20.000000 m23-0.3.0/m23/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/align/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-31 20:59:20.000000 m23-0.3.0/m23/align/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-31 20:59:20.000000 m23-0.3.0/m23/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-31 20:59:20.000000 m23-0.3.0/m23/calibrate/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-31 20:59:20.000000 m23-0.3.0/m23/calibrate/master_calibrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-31 20:59:20.000000 m23-0.3.0/m23/charts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/combine/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-31 20:59:20.000000 m23-0.3.0/m23/combine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-31 20:59:20.000000 m23-0.3.0/m23/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-31 20:59:20.000000 m23-0.3.0/m23/extract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/aligned_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/color_normalized_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/flux_log_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/log_file_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/masterflat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/normfactor_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/raw_image_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/reference_log_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/ri_color_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/internight_normalize/
+-rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-05-31 20:59:20.000000 m23-0.3.0/m23/internight_normalize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-31 20:59:20.000000 m23-0.3.0/m23/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-31 20:59:20.000000 m23-0.3.0/m23/norm/get_line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.912339 m23-0.3.0/m23/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/generate_masterflat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/nights_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/process_nights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/renormalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/renormalize_config_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.912339 m23-0.3.0/m23/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-31 20:59:20.000000 m23-0.3.0/m23/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-31 20:59:20.000000 m23-0.3.0/m23/trans/fits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.912339 m23-0.3.0/m23/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-31 20:59:20.000000 m23-0.3.0/m23/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-31 20:59:20.000000 m23-0.3.0/m23/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-31 20:59:20.000000 m23-0.3.0/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-31 20:59:20.000000 m23-0.3.0/m23/utils/rename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-31 20:59:20.000000 m23-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:59:39.912339 m23-0.3.0/setup.cfg
```

### Comparing `m23-0.2.0/m23/__main__.py` & `m23-0.3.0/m23/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import sys
 from pathlib import Path
 
-from m23 import start_data_processing
+from m23.processor import start_data_processing
 from m23.processor import create_nights_csv, generate_masterflat, renormalize
 
 
 def process(args):
     """
     This is a subcommand that handles data processing for one or more nights
     based on the configuration file path provided
```

### Comparing `m23-0.2.0/m23/align/__init__.py` & `m23-0.3.0/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/calibrate/calibration.py` & `m23-0.3.0/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/calibrate/master_calibrate.py` & `m23-0.3.0/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/charts/__init__.py` & `m23-0.3.0/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/combine/__init__.py` & `m23-0.3.0/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/constants.py` & `m23-0.3.0/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/__init__.py` & `m23-0.3.0/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/aligned_combined_file.py` & `m23-0.3.0/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/color_normalized_file.py` & `m23-0.3.0/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/flux_log_combined_file.py` & `m23-0.3.0/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/log_file_combined_file.py` & `m23-0.3.0/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/masterflat_file.py` & `m23-0.3.0/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/normfactor_file.py` & `m23-0.3.0/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/raw_image_file.py` & `m23-0.3.0/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/reference_log_file.py` & `m23-0.3.0/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/file/ri_color_file.py` & `m23-0.3.0/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/internight_normalize/__init__.py` & `m23-0.3.0/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/matrix/fill.py` & `m23-0.3.0/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/norm/__init__.py` & `m23-0.3.0/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/norm/get_line.py` & `m23-0.3.0/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/processor/config_loader.py` & `m23-0.3.0/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/processor/generate_masterflat.py` & `m23-0.3.0/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/processor/generate_masterflat_config_loader.py` & `m23-0.3.0/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/processor/nights_csv.py` & `m23-0.3.0/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/processor/nights_csv_config_loader.py` & `m23-0.3.0/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/processor/process_nights.py` & `m23-0.3.0/m23/processor/process_nights.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/processor/renormalize.py` & `m23-0.3.0/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/processor/renormalize_config_loader.py` & `m23-0.3.0/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/utils/__init__.py` & `m23-0.3.0/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/utils/date.py` & `m23-0.3.0/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23/utils/rename.py` & `m23-0.3.0/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-0.2.0/m23.egg-info/SOURCES.txt` & `m23-0.3.0/m23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

