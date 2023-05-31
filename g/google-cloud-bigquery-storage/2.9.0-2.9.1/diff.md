# Comparing `tmp/google-cloud-bigquery-storage-2.9.0.tar.gz` & `tmp/google-cloud-bigquery-storage-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/google-cloud-bigquery-storage-2.9.0.tar", last modified: Mon Sep 27 18:37:23 2021, max compression
+gzip compressed data, was "google-cloud-bigquery-storage-2.9.1.tar", last modified: Thu Oct  7 12:06:10 2021, max compression
```

## Comparing `google-cloud-bigquery-storage-2.9.0.tar` & `google-cloud-bigquery-storage-2.9.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.844699 google-cloud-bigquery-storage-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4874 2021-09-27 18:37:23.844699 google-cloud-bigquery-storage-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3946 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.824709 google-cloud-bigquery-storage-2.9.0/google/
--rw-rw-r--   0 root         (0)     1003      774 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.824709 google-cloud-bigquery-storage-2.9.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      774 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.824709 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage/
--rw-rw-r--   0 root         (0)     1003     4296 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage/__init__.py
--rw-rw-r--   0 root         (0)     1003       90 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.828707 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/
--rw-rw-r--   0 root         (0)     1003     1236 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5564 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/client.py
--rw-rw-r--   0 root         (0)     1003      671 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/exceptions.py
--rw-rw-r--   0 root         (0)     1003     3114 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003     2655 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/gapic_types.py
--rw-rw-r--   0 root         (0)     1003       90 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/py.typed
--rw-rw-r--   0 root         (0)     1003    25194 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/reader.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.828707 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.828707 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/
--rw-rw-r--   0 root         (0)     1003      761 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/__init__.py
--rw-rw-r--   0 root         (0)     1003    20620 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/async_client.py
--rw-rw-r--   0 root         (0)     1003    29056 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.828707 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9041 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15817 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16164 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.828707 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/
--rw-rw-r--   0 root         (0)     1003      765 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/__init__.py
--rw-rw-r--   0 root         (0)     1003    29547 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/async_client.py
--rw-rw-r--   0 root         (0)     1003    36607 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.828707 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11671 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20015 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20424 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.832705 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/
--rw-rw-r--   0 root         (0)     1003     2270 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2331 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/arrow.py
--rw-rw-r--   0 root         (0)     1003     1420 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/avro.py
--rw-rw-r--   0 root         (0)     1003     2251 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/protobuf.py
--rw-rw-r--   0 root         (0)     1003    19342 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/storage.py
--rw-rw-r--   0 root         (0)     1003     8678 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/stream.py
--rw-rw-r--   0 root         (0)     1003     5306 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/table.py
--rw-rw-r--   0 root         (0)     1003    15815 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/writer.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.832705 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/
--rw-rw-r--   0 root         (0)     1003     1283 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     5518 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/client.py
--rw-rw-r--   0 root         (0)     1003      671 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/exceptions.py
--rw-rw-r--   0 root         (0)     1003     3124 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       90 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.832705 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.832705 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/
--rw-rw-r--   0 root         (0)     1003      761 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/__init__.py
--rw-rw-r--   0 root         (0)     1003    20727 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/async_client.py
--rw-rw-r--   0 root         (0)     1003    29163 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.832705 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9051 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15947 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16294 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.832705 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/
--rw-rw-r--   0 root         (0)     1003      765 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/__init__.py
--rw-rw-r--   0 root         (0)     1003    28757 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/async_client.py
--rw-rw-r--   0 root         (0)     1003    35707 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.836703 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11799 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19355 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19764 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.836703 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     2270 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2106 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/arrow.py
--rw-rw-r--   0 root         (0)     1003     1298 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/avro.py
--rw-rw-r--   0 root         (0)     1003     1915 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/protobuf.py
--rw-rw-r--   0 root         (0)     1003    18512 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/storage.py
--rw-rw-r--   0 root         (0)     1003     8289 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/stream.py
--rw-rw-r--   0 root         (0)     1003     2900 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/table.py
--rw-rw-r--   0 root         (0)     1003    15850 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/writer.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.836703 google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/
--rw-r--r--   0 root         (0)     1003     4874 2021-09-27 18:37:23.000000 google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5214 2021-09-27 18:37:23.000000 google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2021-09-27 18:37:23.000000 google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2021-09-27 18:37:23.000000 google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2021-09-27 18:37:23.000000 google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      189 2021-09-27 18:37:23.000000 google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2021-09-27 18:37:23.000000 google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.836703 google-cloud-bigquery-storage-2.9.0/scripts/
--rw-rw-r--   0 root         (0)     1003     6458 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/scripts/fixup_bigquery_storage_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2021-09-27 18:37:23.844699 google-cloud-bigquery-storage-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2765 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.836703 google-cloud-bigquery-storage-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.840701 google-cloud-bigquery-storage-2.9.0/tests/system/
--rw-rw-r--   0 root         (0)     1003      574 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.840701 google-cloud-bigquery-storage-2.9.0/tests/system/assets/
--rw-rw-r--   0 root         (0)     1003       96 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/assets/people_data.csv
--rw-rw-r--   0 root         (0)     1003      694 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/assets/public_samples_copy.sql
--rw-rw-r--   0 root         (0)     1003     7386 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/conftest.py
--rw-rw-r--   0 root         (0)     1003     1339 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.840701 google-cloud-bigquery-storage-2.9.0/tests/system/reader/
--rw-rw-r--   0 root         (0)     1003      574 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/reader/__init__.py
--rw-rw-r--   0 root         (0)     1003     1297 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/reader/conftest.py
--rw-rw-r--   0 root         (0)     1003    18390 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/reader/test_reader.py
--rw-rw-r--   0 root         (0)     1003     3363 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/reader/test_reader_dataframe.py
--rw-rw-r--   0 root         (0)     1003     1217 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/system/test_writer.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.840701 google-cloud-bigquery-storage-2.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.840701 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.840701 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    65432 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1/test_big_query_read.py
--rw-rw-r--   0 root         (0)     1003    86211 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1/test_big_query_write.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 18:37:23.844699 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003    65290 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1beta2/test_big_query_read.py
--rw-rw-r--   0 root         (0)     1003    86276 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1beta2/test_big_query_write.py
--rw-rw-r--   0 root         (0)     1003     2421 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/helpers.py
--rw-rw-r--   0 root         (0)     1003     3611 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/test_client_v1.py
--rw-rw-r--   0 root         (0)     1003    17822 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/test_reader_v1.py
--rw-rw-r--   0 root         (0)     1003    11673 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/test_reader_v1_arrow.py
--rw-rw-r--   0 root         (0)     1003     6149 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/test_writer_v1.py
--rw-rw-r--   0 root         (0)     1003     6169 2021-09-27 18:34:42.000000 google-cloud-bigquery-storage-2.9.0/tests/unit/test_writer_v1beta2.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.117765 google-cloud-bigquery-storage-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4874 2021-10-07 12:06:10.117765 google-cloud-bigquery-storage-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3946 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.101765 google-cloud-bigquery-storage-2.9.1/google/
+-rw-rw-r--   0 root         (0)     1003      774 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.101765 google-cloud-bigquery-storage-2.9.1/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      774 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.101765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage/
+-rw-rw-r--   0 root         (0)     1003     4296 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage/__init__.py
+-rw-rw-r--   0 root         (0)     1003       90 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.101765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/
+-rw-rw-r--   0 root         (0)     1003     1236 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5564 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/client.py
+-rw-rw-r--   0 root         (0)     1003      671 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     3114 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003     2655 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/gapic_types.py
+-rw-rw-r--   0 root         (0)     1003       90 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/py.typed
+-rw-rw-r--   0 root         (0)     1003    25194 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/reader.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.101765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.101765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/
+-rw-rw-r--   0 root         (0)     1003      761 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20620 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/async_client.py
+-rw-rw-r--   0 root         (0)     1003    29056 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.101765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9041 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15817 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16164 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.105765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/
+-rw-rw-r--   0 root         (0)     1003      765 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29547 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/async_client.py
+-rw-rw-r--   0 root         (0)     1003    36607 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.105765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11671 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20015 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20424 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.105765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2270 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2331 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/arrow.py
+-rw-rw-r--   0 root         (0)     1003     1420 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/avro.py
+-rw-rw-r--   0 root         (0)     1003     2251 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/protobuf.py
+-rw-rw-r--   0 root         (0)     1003    19342 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/storage.py
+-rw-rw-r--   0 root         (0)     1003     8678 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/stream.py
+-rw-rw-r--   0 root         (0)     1003     5306 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/table.py
+-rw-rw-r--   0 root         (0)     1003    15815 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/writer.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.105765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     1283 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5518 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/client.py
+-rw-rw-r--   0 root         (0)     1003      671 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     3124 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       90 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.105765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.109765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/
+-rw-rw-r--   0 root         (0)     1003      761 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20727 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/async_client.py
+-rw-rw-r--   0 root         (0)     1003    29163 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.109765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9051 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15947 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16294 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.109765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/
+-rw-rw-r--   0 root         (0)     1003      765 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28757 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/async_client.py
+-rw-rw-r--   0 root         (0)     1003    35707 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.109765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11799 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19355 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19764 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.109765 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     2270 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2106 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/arrow.py
+-rw-rw-r--   0 root         (0)     1003     1298 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/avro.py
+-rw-rw-r--   0 root         (0)     1003     1915 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/protobuf.py
+-rw-rw-r--   0 root         (0)     1003    18512 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/storage.py
+-rw-rw-r--   0 root         (0)     1003     8289 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/stream.py
+-rw-rw-r--   0 root         (0)     1003     2900 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/table.py
+-rw-rw-r--   0 root         (0)     1003    15850 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/writer.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.113765 google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/
+-rw-r--r--   0 root         (0)     1003     4874 2021-10-07 12:06:09.000000 google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5214 2021-10-07 12:06:09.000000 google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-07 12:06:09.000000 google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2021-10-07 12:06:09.000000 google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-07 12:06:09.000000 google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      189 2021-10-07 12:06:09.000000 google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2021-10-07 12:06:09.000000 google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.113765 google-cloud-bigquery-storage-2.9.1/scripts/
+-rw-rw-r--   0 root         (0)     1003     6458 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/scripts/fixup_bigquery_storage_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2021-10-07 12:06:10.117765 google-cloud-bigquery-storage-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2765 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.113765 google-cloud-bigquery-storage-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.113765 google-cloud-bigquery-storage-2.9.1/tests/system/
+-rw-rw-r--   0 root         (0)     1003      574 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.113765 google-cloud-bigquery-storage-2.9.1/tests/system/assets/
+-rw-rw-r--   0 root         (0)     1003       96 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/assets/people_data.csv
+-rw-rw-r--   0 root         (0)     1003      694 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/assets/public_samples_copy.sql
+-rw-rw-r--   0 root         (0)     1003     7386 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/conftest.py
+-rw-rw-r--   0 root         (0)     1003     1339 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.113765 google-cloud-bigquery-storage-2.9.1/tests/system/reader/
+-rw-rw-r--   0 root         (0)     1003      574 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/reader/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1297 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/reader/conftest.py
+-rw-rw-r--   0 root         (0)     1003    18390 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/reader/test_reader.py
+-rw-rw-r--   0 root         (0)     1003     3363 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/reader/test_reader_dataframe.py
+-rw-rw-r--   0 root         (0)     1003     1217 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/system/test_writer.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.117765 google-cloud-bigquery-storage-2.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.117765 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.117765 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    65432 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1/test_big_query_read.py
+-rw-rw-r--   0 root         (0)     1003    86211 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1/test_big_query_write.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-07 12:06:10.117765 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    65290 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1beta2/test_big_query_read.py
+-rw-rw-r--   0 root         (0)     1003    86276 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1beta2/test_big_query_write.py
+-rw-rw-r--   0 root         (0)     1003     2421 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/helpers.py
+-rw-rw-r--   0 root         (0)     1003     3611 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/test_client_v1.py
+-rw-rw-r--   0 root         (0)     1003    17822 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/test_reader_v1.py
+-rw-rw-r--   0 root         (0)     1003    11673 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/test_reader_v1_arrow.py
+-rw-rw-r--   0 root         (0)     1003     6149 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/test_writer_v1.py
+-rw-rw-r--   0 root         (0)     1003     6169 2021-10-07 12:03:27.000000 google-cloud-bigquery-storage-2.9.1/tests/unit/test_writer_v1beta2.py
```

### Comparing `google-cloud-bigquery-storage-2.9.0/LICENSE` & `google-cloud-bigquery-storage-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/MANIFEST.in` & `google-cloud-bigquery-storage-2.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/PKG-INFO` & `google-cloud-bigquery-storage-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-storage
-Version: 2.9.0
+Version: 2.9.1
 Summary: BigQuery Storage API API client library
 Home-page: https://github.com/googleapis/python-bigquery-storage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-storage-2.9.0/README.rst` & `google-cloud-bigquery-storage-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/exceptions.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/gapic_metadata.json` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/gapic_types.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/gapic_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/reader.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/reader.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/async_client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/transports/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/transports/base.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/transports/grpc.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_read/transports/grpc_asyncio.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_read/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/async_client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/transports/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/transports/base.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/transports/grpc.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/services/big_query_write/transports/grpc_asyncio.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/services/big_query_write/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/arrow.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/arrow.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/avro.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/avro.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/protobuf.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/protobuf.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/storage.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/storage.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/stream.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/stream.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/types/table.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/types/table.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1/writer.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1/writer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/exceptions.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/gapic_metadata.json` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/async_client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/base.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/grpc.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/grpc_asyncio.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_read/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/async_client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/client.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/base.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/grpc.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/grpc_asyncio.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/services/big_query_write/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/__init__.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/arrow.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/arrow.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/avro.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/avro.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/protobuf.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/protobuf.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/storage.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/storage.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/stream.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/stream.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/types/table.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/types/table.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google/cloud/bigquery_storage_v1beta2/writer.py` & `google-cloud-bigquery-storage-2.9.1/google/cloud/bigquery_storage_v1beta2/writer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/PKG-INFO` & `google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-storage
-Version: 2.9.0
+Version: 2.9.1
 Summary: BigQuery Storage API API client library
 Home-page: https://github.com/googleapis/python-bigquery-storage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-storage-2.9.0/google_cloud_bigquery_storage.egg-info/SOURCES.txt` & `google-cloud-bigquery-storage-2.9.1/google_cloud_bigquery_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/scripts/fixup_bigquery_storage_v1_keywords.py` & `google-cloud-bigquery-storage-2.9.1/scripts/fixup_bigquery_storage_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/setup.py` & `google-cloud-bigquery-storage-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import io
 import os
 
 import setuptools
 
 name = "google-cloud-bigquery-storage"
 description = "BigQuery Storage API API client library"
-version = "2.9.0"
+version = "2.9.1"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-api-core[grpc] >= 1.26.0, <3.0.0dev",
     "proto-plus >= 1.18.0",
```

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/__init__.py` & `google-cloud-bigquery-storage-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/system/__init__.py` & `google-cloud-bigquery-storage-2.9.1/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/system/assets/public_samples_copy.sql` & `google-cloud-bigquery-storage-2.9.1/tests/system/assets/public_samples_copy.sql`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/system/conftest.py` & `google-cloud-bigquery-storage-2.9.1/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/system/helpers.py` & `google-cloud-bigquery-storage-2.9.1/tests/system/helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/system/reader/__init__.py` & `google-cloud-bigquery-storage-2.9.1/tests/system/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/system/reader/conftest.py` & `google-cloud-bigquery-storage-2.9.1/tests/system/reader/conftest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/system/reader/test_reader.py` & `google-cloud-bigquery-storage-2.9.1/tests/system/reader/test_reader.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/system/reader/test_reader_dataframe.py` & `google-cloud-bigquery-storage-2.9.1/tests/system/reader/test_reader_dataframe.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/system/test_writer.py` & `google-cloud-bigquery-storage-2.9.1/tests/system/test_writer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/__init__.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1/__init__.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1/test_big_query_read.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1/test_big_query_read.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1/test_big_query_write.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1/test_big_query_write.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1beta2/__init__.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1beta2/test_big_query_read.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1beta2/test_big_query_read.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/gapic/bigquery_storage_v1beta2/test_big_query_write.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/gapic/bigquery_storage_v1beta2/test_big_query_write.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/helpers.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/test_client_v1.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/test_client_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/test_reader_v1.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/test_reader_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/test_reader_v1_arrow.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/test_reader_v1_arrow.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/test_writer_v1.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/test_writer_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-storage-2.9.0/tests/unit/test_writer_v1beta2.py` & `google-cloud-bigquery-storage-2.9.1/tests/unit/test_writer_v1beta2.py`

 * *Files identical despite different names*

