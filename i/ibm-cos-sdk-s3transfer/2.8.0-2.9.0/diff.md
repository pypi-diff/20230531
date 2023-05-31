# Comparing `tmp/ibm-cos-sdk-s3transfer-2.8.0.tar.gz` & `tmp/ibm-cos-sdk-s3transfer-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-cos-sdk-s3transfer-2.8.0.tar", last modified: Tue Oct 27 20:35:29 2020, max compression
+gzip compressed data, was "dist/ibm-cos-sdk-s3transfer-2.9.0.tar", last modified: Mon Dec 14 21:54:46 2020, max compression
```

## Comparing `ibm-cos-sdk-s3transfer-2.8.0.tar` & `ibm-cos-sdk-s3transfer-2.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/
--rw-r--r--   0 root         (0) root         (0)       80 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/MANIFEST.in
--rwxr-xr-x   0 root         (0) root         (0)      241 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/requirements-test.txt
--rw-r--r--   0 root         (0) root         (0)      939 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      120 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/
--rwxr-xr-x   0 root         (0) root         (0)    17345 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     5571 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_processpool.py
--rwxr-xr-x   0 root         (0) root         (0)     4546 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/integration/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10737 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_download.py
--rwxr-xr-x   0 root         (0) root         (0)     2990 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_copy.py
--rwxr-xr-x   0 root         (0) root         (0)    12223 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_s3transfer.py
--rwxr-xr-x   0 root         (0) root         (0)     7801 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_upload.py
--rwxr-xr-x   0 root         (0) root         (0)     1269 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_delete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)    26378 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_processpool.py
--rwxr-xr-x   0 root         (0) root         (0)      561 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    36226 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_download.py
--rwxr-xr-x   0 root         (0) root         (0)     3183 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_subscribers.py
--rwxr-xr-x   0 root         (0) root         (0)     3608 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_compat.py
--rwxr-xr-x   0 root         (0) root         (0)    35784 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     6123 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_copies.py
--rwxr-xr-x   0 root         (0) root         (0)     5777 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_manager.py
--rwxr-xr-x   0 root         (0) root         (0)    30436 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_tasks.py
--rwxr-xr-x   0 root         (0) root         (0)    29632 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_s3transfer.py
--rwxr-xr-x   0 root         (0) root         (0)    26256 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_upload.py
--rwxr-xr-x   0 root         (0) root         (0)     2132 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_delete.py
--rwxr-xr-x   0 root         (0) root         (0)    26328 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_futures.py
--rwxr-xr-x   0 root         (0) root         (0)    17878 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_bandwidth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)    10312 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_processpool.py
--rwxr-xr-x   0 root         (0) root         (0)      561 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    18224 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_download.py
--rwxr-xr-x   0 root         (0) root         (0)     7083 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_aspera_manager.py
--rwxr-xr-x   0 root         (0) root         (0)     1438 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     6952 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_manager.py
--rwxr-xr-x   0 root         (0) root         (0)    19757 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_copy.py
--rwxr-xr-x   0 root         (0) root         (0)    21343 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_upload.py
--rwxr-xr-x   0 root         (0) root         (0)     2219 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_delete.py
--rw-r--r--   0 root         (0) root         (0)    11359 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/LICENSE.txt
--rwxr-xr-x   0 root         (0) root         (0)      121 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/
--rwxr-xr-x   0 root         (0) root         (0)    28250 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3204 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/compat.py
--rwxr-xr-x   0 root         (0) root         (0)    30226 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/upload.py
--rw-r--r--   0 root         (0) root         (0)    36369 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/processpool.py
--rwxr-xr-x   0 root         (0) root         (0)     3652 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/subscribers.py
--rwxr-xr-x   0 root         (0) root         (0)    28144 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/download.py
--rwxr-xr-x   0 root         (0) root         (0)     2607 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/delete.py
--rwxr-xr-x   0 root         (0) root         (0)     1090 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)    27479 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/manager.py
--rwxr-xr-x   0 root         (0) root         (0)    21222 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/futures.py
--rwxr-xr-x   0 root         (0) root         (0)    26532 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/utils.py
--rwxr-xr-x   0 root         (0) root         (0)    15651 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/bandwidth.py
--rwxr-xr-x   0 root         (0) root         (0)      863 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      770 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/subscribers.py
--rwxr-xr-x   0 root         (0) root         (0)      986 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)    28588 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/manager.py
--rwxr-xr-x   0 root         (0) root         (0)    25349 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/futures.py
--rwxr-xr-x   0 root         (0) root         (0)     1301 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/utils.py
--rwxr-xr-x   0 root         (0) root         (0)    13524 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/copies.py
--rwxr-xr-x   0 root         (0) root         (0)    16018 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/tasks.py
--rwxr-xr-x   0 root         (0) root         (0)     1362 2020-10-27 20:35:28.000000 ibm-cos-sdk-s3transfer-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_cos_sdk_s3transfer.egg-info/
--rw-r--r--   0 root         (0) root         (0)       24 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_cos_sdk_s3transfer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      939 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_cos_sdk_s3transfer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1839 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_cos_sdk_s3transfer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_cos_sdk_s3transfer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2020-10-27 20:35:29.000000 ibm-cos-sdk-s3transfer-2.8.0/ibm_cos_sdk_s3transfer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)       80 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/MANIFEST.in
+-rwxr-xr-x   0 root         (0) root         (0)      241 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/requirements-test.txt
+-rw-r--r--   0 root         (0) root         (0)      939 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      120 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/
+-rwxr-xr-x   0 root         (0) root         (0)    17345 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     5571 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_processpool.py
+-rwxr-xr-x   0 root         (0) root         (0)     4546 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/integration/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10737 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_download.py
+-rwxr-xr-x   0 root         (0) root         (0)     2990 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_copy.py
+-rwxr-xr-x   0 root         (0) root         (0)    12223 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_s3transfer.py
+-rwxr-xr-x   0 root         (0) root         (0)     7801 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_upload.py
+-rwxr-xr-x   0 root         (0) root         (0)     1269 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_delete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)    26378 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_processpool.py
+-rwxr-xr-x   0 root         (0) root         (0)      561 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    36226 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_download.py
+-rwxr-xr-x   0 root         (0) root         (0)     3183 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_subscribers.py
+-rwxr-xr-x   0 root         (0) root         (0)     3608 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_compat.py
+-rwxr-xr-x   0 root         (0) root         (0)    35784 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     6123 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_copies.py
+-rwxr-xr-x   0 root         (0) root         (0)     5777 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_manager.py
+-rwxr-xr-x   0 root         (0) root         (0)    30436 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_tasks.py
+-rwxr-xr-x   0 root         (0) root         (0)    29632 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_s3transfer.py
+-rwxr-xr-x   0 root         (0) root         (0)    26256 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_upload.py
+-rwxr-xr-x   0 root         (0) root         (0)     2132 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_delete.py
+-rwxr-xr-x   0 root         (0) root         (0)    26328 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_futures.py
+-rwxr-xr-x   0 root         (0) root         (0)    17878 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_bandwidth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)    10312 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_processpool.py
+-rwxr-xr-x   0 root         (0) root         (0)      561 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    18224 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_download.py
+-rwxr-xr-x   0 root         (0) root         (0)     7083 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_aspera_manager.py
+-rwxr-xr-x   0 root         (0) root         (0)     1438 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     6952 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_manager.py
+-rwxr-xr-x   0 root         (0) root         (0)    19757 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_copy.py
+-rwxr-xr-x   0 root         (0) root         (0)    21343 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_upload.py
+-rwxr-xr-x   0 root         (0) root         (0)     2219 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)    11359 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/LICENSE.txt
+-rwxr-xr-x   0 root         (0) root         (0)      121 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/
+-rwxr-xr-x   0 root         (0) root         (0)    28250 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3204 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/compat.py
+-rwxr-xr-x   0 root         (0) root         (0)    30226 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/upload.py
+-rw-r--r--   0 root         (0) root         (0)    36369 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/processpool.py
+-rwxr-xr-x   0 root         (0) root         (0)     3652 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/subscribers.py
+-rwxr-xr-x   0 root         (0) root         (0)    28144 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/download.py
+-rwxr-xr-x   0 root         (0) root         (0)     2607 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/delete.py
+-rwxr-xr-x   0 root         (0) root         (0)     1090 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)    27479 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/manager.py
+-rwxr-xr-x   0 root         (0) root         (0)    21222 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/futures.py
+-rwxr-xr-x   0 root         (0) root         (0)    26532 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    15651 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/bandwidth.py
+-rwxr-xr-x   0 root         (0) root         (0)      863 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      770 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/subscribers.py
+-rwxr-xr-x   0 root         (0) root         (0)      986 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)    28588 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/manager.py
+-rwxr-xr-x   0 root         (0) root         (0)    25349 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/futures.py
+-rwxr-xr-x   0 root         (0) root         (0)     1301 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    13524 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/copies.py
+-rwxr-xr-x   0 root         (0) root         (0)    16018 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/tasks.py
+-rwxr-xr-x   0 root         (0) root         (0)     1362 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_cos_sdk_s3transfer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       24 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_cos_sdk_s3transfer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      939 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_cos_sdk_s3transfer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1839 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_cos_sdk_s3transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_cos_sdk_s3transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2020-12-14 21:54:46.000000 ibm-cos-sdk-s3transfer-2.9.0/ibm_cos_sdk_s3transfer.egg-info/top_level.txt
```

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/PKG-INFO` & `ibm-cos-sdk-s3transfer-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-cos-sdk-s3transfer
-Version: 2.8.0
+Version: 2.9.0
 Summary: IBM S3 Transfer Manager
 Home-page: https://github.com/ibm/ibm-cos-sdk-python-s3transfer
 Author: IBM
 Author-email: 
 License: Apache License 2.0
 Description: # s3transfer - An IBM COS Transfer Manager for Python
```

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/__init__.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_processpool.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_processpool.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/integration/__init__.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_download.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_download.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_copy.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_copy.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_s3transfer.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_s3transfer.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_upload.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_upload.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/integration/test_delete.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/integration/test_delete.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_processpool.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_processpool.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/__init__.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_download.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_download.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_subscribers.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_compat.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_utils.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_copies.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_copies.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_manager.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_tasks.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_tasks.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_s3transfer.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_s3transfer.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_upload.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_upload.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_delete.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_delete.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_futures.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_futures.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/unit/test_bandwidth.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/unit/test_bandwidth.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_processpool.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_processpool.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/functional/__init__.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_download.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_download.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_aspera_manager.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_aspera_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_utils.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_manager.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_copy.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_copy.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_upload.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_upload.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/tests/functional/test_delete.py` & `ibm-cos-sdk-s3transfer-2.9.0/tests/functional/test_delete.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/LICENSE.txt` & `ibm-cos-sdk-s3transfer-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/__init__.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 from ibm_botocore.exceptions import IncompleteReadError
 
 import ibm_s3transfer.compat
 from ibm_s3transfer.exceptions import RetriesExceededError, S3UploadFailedError
 
 
 __author__ = 'IBM'
-__version__ = '2.8.0'
+__version__ = '2.9.0'
 
 
 class NullHandler(logging.Handler):
     def emit(self, record):
         pass
```

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/compat.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/compat.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/upload.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/upload.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/processpool.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/processpool.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/subscribers.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/subscribers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/download.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/download.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/delete.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/delete.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/exceptions.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/manager.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/futures.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/futures.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/utils.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/bandwidth.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/bandwidth.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/constants.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/constants.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/subscribers.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/subscribers.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/exceptions.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/manager.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/futures.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/futures.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/aspera/utils.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/aspera/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/copies.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/copies.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_s3transfer/tasks.py` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_s3transfer/tasks.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/setup.py` & `ibm-cos-sdk-s3transfer-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from setuptools import setup, find_packages
 
 ROOT = os.path.dirname(__file__)
 VERSION_RE = re.compile(r'''__version__ = ['"]([a-z0-9.]+)['"]''')
 
 requires = [
-    'ibm-cos-sdk-core==2.8.0',
+    'ibm-cos-sdk-core==2.9.0',
 ]
 
 
 def get_version():
     init = open(os.path.join(ROOT, 'ibm_s3transfer', '__init__.py')).read()
     return VERSION_RE.search(init).group(1)
```

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_cos_sdk_s3transfer.egg-info/PKG-INFO` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_cos_sdk_s3transfer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-cos-sdk-s3transfer
-Version: 2.8.0
+Version: 2.9.0
 Summary: IBM S3 Transfer Manager
 Home-page: https://github.com/ibm/ibm-cos-sdk-python-s3transfer
 Author: IBM
 Author-email: 
 License: Apache License 2.0
 Description: # s3transfer - An IBM COS Transfer Manager for Python
```

### Comparing `ibm-cos-sdk-s3transfer-2.8.0/ibm_cos_sdk_s3transfer.egg-info/SOURCES.txt` & `ibm-cos-sdk-s3transfer-2.9.0/ibm_cos_sdk_s3transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

