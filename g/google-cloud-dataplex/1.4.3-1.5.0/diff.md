# Comparing `tmp/google-cloud-dataplex-1.4.3.tar.gz` & `tmp/google-cloud-dataplex-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dataplex-1.4.3.tar", last modified: Mon Mar 27 15:37:04 2023, max compression
+gzip compressed data, was "google-cloud-dataplex-1.5.0.tar", last modified: Wed May 31 20:48:21 2023, max compression
```

## Comparing `google-cloud-dataplex-1.4.3.tar` & `google-cloud-dataplex-1.5.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.442076 google-cloud-dataplex-1.4.3/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4728 2023-03-27 15:37:04.442076 google-cloud-dataplex-1.4.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3809 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.426075 google-cloud-dataplex-1.4.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.426075 google-cloud-dataplex-1.4.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.430075 google-cloud-dataplex-1.4.3/google/cloud/dataplex/
--rw-rw-r--   0 root         (0)     1003     7117 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.430075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/
--rw-rw-r--   0 root         (0)     1003     6310 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    15094 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.430075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.430075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62823 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    71605 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/client.py
--rw-rw-r--   0 root         (0)     1003     5658 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.430075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12118 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25618 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25992 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.434075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62235 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    73403 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/client.py
--rw-rw-r--   0 root         (0)     1003    10807 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.434075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10921 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25499 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25983 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.434075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   182453 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   195369 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/client.py
--rw-rw-r--   0 root         (0)     1003    49482 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.434075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    25823 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    51185 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    52260 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.434075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    61597 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    72083 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/client.py
--rw-rw-r--   0 root         (0)     1003    10685 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.438075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12419 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25614 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26039 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.438075 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/
--rw-rw-r--   0 root         (0)     1003     5512 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16117 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/analyze.py
--rw-rw-r--   0 root         (0)     1003     6555 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/content.py
--rw-rw-r--   0 root         (0)     1003    16506 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/data_profile.py
--rw-rw-r--   0 root         (0)     1003    16078 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/data_quality.py
--rw-rw-r--   0 root         (0)     1003    24250 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/datascans.py
--rw-rw-r--   0 root         (0)     1003    22735 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/logs.py
--rw-rw-r--   0 root         (0)     1003    36598 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/metadata_.py
--rw-rw-r--   0 root         (0)     1003     4952 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/processing.py
--rw-rw-r--   0 root         (0)     1003    49299 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    38490 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003    26001 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/tasks.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.438075 google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/
--rw-r--r--   0 root         (0)     1003     4728 2023-03-27 15:37:04.000000 google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3701 2023-03-27 15:37:04.000000 google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:37:04.000000 google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:37:04.000000 google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:37:04.000000 google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:37:04.000000 google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:37:04.000000 google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:37:04.442076 google-cloud-dataplex-1.4.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2972 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.438075 google-cloud-dataplex-1.4.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.438075 google-cloud-dataplex-1.4.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.438075 google-cloud-dataplex-1.4.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:37:04.442076 google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   154569 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/test_content_service.py
--rw-rw-r--   0 root         (0)     1003   169734 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/test_data_scan_service.py
--rw-rw-r--   0 root         (0)     1003   422173 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/test_dataplex_service.py
--rw-rw-r--   0 root         (0)     1003   174991 2023-03-27 15:35:04.000000 google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/test_metadata_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.081312 google-cloud-dataplex-1.5.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4728 2023-05-31 20:48:21.081312 google-cloud-dataplex-1.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3809 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.065312 google-cloud-dataplex-1.5.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.065312 google-cloud-dataplex-1.5.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.065312 google-cloud-dataplex-1.5.0/google/cloud/dataplex/
+-rw-rw-r--   0 root         (0)     1003     7243 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/
+-rw-rw-r--   0 root         (0)     1003     6436 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15314 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62823 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    71605 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5658 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12118 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25618 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25992 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62227 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    73395 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10807 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.069312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10921 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25499 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25983 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.073312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   186240 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   199302 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/client.py
+-rw-rw-r--   0 root         (0)     1003    49482 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.073312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26223 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    52208 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    53320 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.073312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61597 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    72083 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10685 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.073312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12419 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25614 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26039 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5638 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16335 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/analyze.py
+-rw-rw-r--   0 root         (0)     1003     6555 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/content.py
+-rw-rw-r--   0 root         (0)     1003    15619 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/data_profile.py
+-rw-rw-r--   0 root         (0)     1003    16628 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/data_quality.py
+-rw-rw-r--   0 root         (0)     1003    24703 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/datascans.py
+-rw-rw-r--   0 root         (0)     1003    22735 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/logs.py
+-rw-rw-r--   0 root         (0)     1003    38144 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/metadata_.py
+-rw-rw-r--   0 root         (0)     1003     5857 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/processing.py
+-rw-rw-r--   0 root         (0)     1003    50791 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    39146 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003    26001 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/
+-rw-r--r--   0 root         (0)     1003     4728 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3701 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:48:21.000000 google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:48:21.081312 google-cloud-dataplex-1.5.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2972 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.077312 google-cloud-dataplex-1.5.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:48:21.081312 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   154569 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_content_service.py
+-rw-rw-r--   0 root         (0)     1003   169734 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_data_scan_service.py
+-rw-rw-r--   0 root         (0)     1003   429857 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_dataplex_service.py
+-rw-rw-r--   0 root         (0)     1003   175411 2023-05-31 20:46:20.000000 google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_metadata_service.py
```

### Comparing `google-cloud-dataplex-1.4.3/LICENSE` & `google-cloud-dataplex-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/MANIFEST.in` & `google-cloud-dataplex-1.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/PKG-INFO` & `google-cloud-dataplex-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataplex
-Version: 1.4.3
+Version: 1.5.0
 Summary: Google Cloud Dataplex API client library
 Home-page: https://github.com/googleapis/python-dataplex
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dataplex-1.4.3/README.rst` & `google-cloud-dataplex-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     GetPartitionRequest,
     ListEntitiesRequest,
     ListEntitiesResponse,
     ListPartitionsRequest,
     ListPartitionsResponse,
     Partition,
     Schema,
+    StorageAccess,
     StorageFormat,
     StorageSystem,
     UpdateEntityRequest,
 )
 from google.cloud.dataplex_v1.types.processing import DataSource, ScannedData, Trigger
 from google.cloud.dataplex_v1.types.resources import (
     Action,
@@ -144,14 +145,16 @@
     ListSessionsResponse,
     ListTasksRequest,
     ListTasksResponse,
     ListZoneActionsRequest,
     ListZonesRequest,
     ListZonesResponse,
     OperationMetadata,
+    RunTaskRequest,
+    RunTaskResponse,
     UpdateAssetRequest,
     UpdateEnvironmentRequest,
     UpdateLakeRequest,
     UpdateTaskRequest,
     UpdateZoneRequest,
 )
 from google.cloud.dataplex_v1.types.tasks import Job, Task
@@ -208,14 +211,15 @@
     "GetPartitionRequest",
     "ListEntitiesRequest",
     "ListEntitiesResponse",
     "ListPartitionsRequest",
     "ListPartitionsResponse",
     "Partition",
     "Schema",
+    "StorageAccess",
     "StorageFormat",
     "UpdateEntityRequest",
     "StorageSystem",
     "DataSource",
     "ScannedData",
     "Trigger",
     "Action",
@@ -256,14 +260,16 @@
     "ListSessionsResponse",
     "ListTasksRequest",
     "ListTasksResponse",
     "ListZoneActionsRequest",
     "ListZonesRequest",
     "ListZonesResponse",
     "OperationMetadata",
+    "RunTaskRequest",
+    "RunTaskResponse",
     "UpdateAssetRequest",
     "UpdateEnvironmentRequest",
     "UpdateLakeRequest",
     "UpdateTaskRequest",
     "UpdateZoneRequest",
     "Job",
     "Task",
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex/gapic_version.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,8 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.3"  # {x-release-please-version}
+from .async_client import MetadataServiceAsyncClient
+from .client import MetadataServiceClient
+
+__all__ = (
+    "MetadataServiceClient",
+    "MetadataServiceAsyncClient",
+)
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     GetPartitionRequest,
     ListEntitiesRequest,
     ListEntitiesResponse,
     ListPartitionsRequest,
     ListPartitionsResponse,
     Partition,
     Schema,
+    StorageAccess,
     StorageFormat,
     StorageSystem,
     UpdateEntityRequest,
 )
 from .types.processing import DataSource, ScannedData, Trigger
 from .types.resources import Action, Asset, AssetStatus, Lake, State, Zone
 from .types.service import (
@@ -112,14 +113,16 @@
     ListSessionsResponse,
     ListTasksRequest,
     ListTasksResponse,
     ListZoneActionsRequest,
     ListZonesRequest,
     ListZonesResponse,
     OperationMetadata,
+    RunTaskRequest,
+    RunTaskResponse,
     UpdateAssetRequest,
     UpdateEnvironmentRequest,
     UpdateLakeRequest,
     UpdateTaskRequest,
     UpdateZoneRequest,
 )
 from .types.tasks import Job, Task
@@ -213,19 +216,22 @@
     "ListZonesRequest",
     "ListZonesResponse",
     "MetadataServiceClient",
     "OperationMetadata",
     "Partition",
     "RunDataScanRequest",
     "RunDataScanResponse",
+    "RunTaskRequest",
+    "RunTaskResponse",
     "ScannedData",
     "Schema",
     "Session",
     "SessionEvent",
     "State",
+    "StorageAccess",
     "StorageFormat",
     "StorageSystem",
     "Task",
     "Trigger",
     "UpdateAssetRequest",
     "UpdateContentRequest",
     "UpdateDataScanRequest",
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/gapic_metadata.json` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/gapic_metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999802714646465%*

 * *Differences: {"'services'": "{'DataplexService': {'clients': {'grpc': {'rpcs': {'RunTask': "*

 * *               "OrderedDict([('methods', ['run_task'])])}}, 'grpc-async': {'rpcs': {'RunTask': "*

 * *               "OrderedDict([('methods', ['run_task'])])}}}}}"}*

```diff
@@ -329,14 +329,19 @@
                             ]
                         },
                         "ListZones": {
                             "methods": [
                                 "list_zones"
                             ]
                         },
+                        "RunTask": {
+                            "methods": [
+                                "run_task"
+                            ]
+                        },
                         "UpdateAsset": {
                             "methods": [
                                 "update_asset"
                             ]
                         },
                         "UpdateEnvironment": {
                             "methods": [
@@ -494,14 +499,19 @@
                             ]
                         },
                         "ListZones": {
                             "methods": [
                                 "list_zones"
                             ]
                         },
+                        "RunTask": {
+                            "methods": [
+                                "run_task"
+                            ]
+                        },
                         "UpdateAsset": {
                             "methods": [
                                 "update_asset"
                             ]
                         },
                         "UpdateEnvironment": {
                             "methods": [
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/async_client.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/client.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/pagers.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/transports/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/transports/base.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/transports/grpc.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/async_client.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1034,15 +1034,15 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.dataplex_v1.types.GetDataScanJobRequest, dict]]):
                 The request object. Get DataScanJob request.
             name (:class:`str`):
                 Required. The resource name of the DataScanJob:
-                ``projects/{project}/locations/{location_id}/dataScans/{data_scan_id}/dataScanJobs/{data_scan_job_id}``
+                ``projects/{project}/locations/{location_id}/dataScans/{data_scan_id}/jobs/{data_scan_job_id}``
                 where ``project`` refers to a *project_id* or
                 *project_number* and ``location_id`` refers to a GCP
                 region.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/client.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1305,15 +1305,15 @@
                 print(response)
 
         Args:
             request (Union[google.cloud.dataplex_v1.types.GetDataScanJobRequest, dict]):
                 The request object. Get DataScanJob request.
             name (str):
                 Required. The resource name of the DataScanJob:
-                ``projects/{project}/locations/{location_id}/dataScans/{data_scan_id}/dataScanJobs/{data_scan_job_id}``
+                ``projects/{project}/locations/{location_id}/dataScans/{data_scan_id}/jobs/{data_scan_job_id}``
                 where ``project`` refers to a *project_id* or
                 *project_number* and ``location_id`` refers to a GCP
                 region.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/pagers.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/async_client.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3292,14 +3292,113 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
+    async def run_task(
+        self,
+        request: Optional[Union[service.RunTaskRequest, dict]] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> service.RunTaskResponse:
+        r"""Run an on demand execution of a Task.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import dataplex_v1
+
+            async def sample_run_task():
+                # Create a client
+                client = dataplex_v1.DataplexServiceAsyncClient()
+
+                # Initialize request argument(s)
+                request = dataplex_v1.RunTaskRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = await client.run_task(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.dataplex_v1.types.RunTaskRequest, dict]]):
+                The request object.
+            name (:class:`str`):
+                Required. The resource name of the task:
+                ``projects/{project_number}/locations/{location_id}/lakes/{lake_id}/tasks/{task_id}``.
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.dataplex_v1.types.RunTaskResponse:
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = service.RunTaskRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.run_task,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def get_job(
         self,
         request: Optional[Union[service.GetJobRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/client.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3575,14 +3575,113 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
+    def run_task(
+        self,
+        request: Optional[Union[service.RunTaskRequest, dict]] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> service.RunTaskResponse:
+        r"""Run an on demand execution of a Task.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import dataplex_v1
+
+            def sample_run_task():
+                # Create a client
+                client = dataplex_v1.DataplexServiceClient()
+
+                # Initialize request argument(s)
+                request = dataplex_v1.RunTaskRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.run_task(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.dataplex_v1.types.RunTaskRequest, dict]):
+                The request object.
+            name (str):
+                Required. The resource name of the task:
+                ``projects/{project_number}/locations/{location_id}/lakes/{lake_id}/tasks/{task_id}``.
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.dataplex_v1.types.RunTaskResponse:
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a service.RunTaskRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, service.RunTaskRequest):
+            request = service.RunTaskRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.run_task]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def get_job(
         self,
         request: Optional[Union[service.GetJobRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/pagers.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,19 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=60.0,
                 ),
                 default_timeout=60.0,
                 client_info=client_info,
             ),
+            self.run_task: gapic_v1.method.wrap_method(
+                self.run_task,
+                default_timeout=None,
+                client_info=client_info,
+            ),
             self.get_job: gapic_v1.method.wrap_method(
                 self.get_job,
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
@@ -645,14 +650,23 @@
     ) -> Callable[
         [service.ListJobsRequest],
         Union[service.ListJobsResponse, Awaitable[service.ListJobsResponse]],
     ]:
         raise NotImplementedError()
 
     @property
+    def run_task(
+        self,
+    ) -> Callable[
+        [service.RunTaskRequest],
+        Union[service.RunTaskResponse, Awaitable[service.RunTaskResponse]],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def get_job(
         self,
     ) -> Callable[[service.GetJobRequest], Union[tasks.Job, Awaitable[tasks.Job]]]:
         raise NotImplementedError()
 
     @property
     def cancel_job(
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -870,14 +870,38 @@
                 "/google.cloud.dataplex.v1.DataplexService/ListJobs",
                 request_serializer=service.ListJobsRequest.serialize,
                 response_deserializer=service.ListJobsResponse.deserialize,
             )
         return self._stubs["list_jobs"]
 
     @property
+    def run_task(self) -> Callable[[service.RunTaskRequest], service.RunTaskResponse]:
+        r"""Return a callable for the run task method over gRPC.
+
+        Run an on demand execution of a Task.
+
+        Returns:
+            Callable[[~.RunTaskRequest],
+                    ~.RunTaskResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "run_task" not in self._stubs:
+            self._stubs["run_task"] = self.grpc_channel.unary_unary(
+                "/google.cloud.dataplex.v1.DataplexService/RunTask",
+                request_serializer=service.RunTaskRequest.serialize,
+                response_deserializer=service.RunTaskResponse.deserialize,
+            )
+        return self._stubs["run_task"]
+
+    @property
     def get_job(self) -> Callable[[service.GetJobRequest], tasks.Job]:
         r"""Return a callable for the get job method over gRPC.
 
         Get job resource.
 
         Returns:
             Callable[[~.GetJobRequest],
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -883,14 +883,40 @@
                 "/google.cloud.dataplex.v1.DataplexService/ListJobs",
                 request_serializer=service.ListJobsRequest.serialize,
                 response_deserializer=service.ListJobsResponse.deserialize,
             )
         return self._stubs["list_jobs"]
 
     @property
+    def run_task(
+        self,
+    ) -> Callable[[service.RunTaskRequest], Awaitable[service.RunTaskResponse]]:
+        r"""Return a callable for the run task method over gRPC.
+
+        Run an on demand execution of a Task.
+
+        Returns:
+            Callable[[~.RunTaskRequest],
+                    Awaitable[~.RunTaskResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "run_task" not in self._stubs:
+            self._stubs["run_task"] = self.grpc_channel.unary_unary(
+                "/google.cloud.dataplex.v1.DataplexService/RunTask",
+                request_serializer=service.RunTaskRequest.serialize,
+                response_deserializer=service.RunTaskResponse.deserialize,
+            )
+        return self._stubs["run_task"]
+
+    @property
     def get_job(self) -> Callable[[service.GetJobRequest], Awaitable[tasks.Job]]:
         r"""Return a callable for the get job method over gRPC.
 
         Get job resource.
 
         Returns:
             Callable[[~.GetJobRequest],
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/async_client.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/client.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/pagers.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/transports/base.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/__init__.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     GetPartitionRequest,
     ListEntitiesRequest,
     ListEntitiesResponse,
     ListPartitionsRequest,
     ListPartitionsResponse,
     Partition,
     Schema,
+    StorageAccess,
     StorageFormat,
     StorageSystem,
     UpdateEntityRequest,
 )
 from .processing import DataSource, ScannedData, Trigger
 from .resources import Action, Asset, AssetStatus, Lake, State, Zone
 from .service import (
@@ -100,14 +101,16 @@
     ListSessionsResponse,
     ListTasksRequest,
     ListTasksResponse,
     ListZoneActionsRequest,
     ListZonesRequest,
     ListZonesResponse,
     OperationMetadata,
+    RunTaskRequest,
+    RunTaskResponse,
     UpdateAssetRequest,
     UpdateEnvironmentRequest,
     UpdateLakeRequest,
     UpdateTaskRequest,
     UpdateZoneRequest,
 )
 from .tasks import Job, Task
@@ -156,14 +159,15 @@
     "GetPartitionRequest",
     "ListEntitiesRequest",
     "ListEntitiesResponse",
     "ListPartitionsRequest",
     "ListPartitionsResponse",
     "Partition",
     "Schema",
+    "StorageAccess",
     "StorageFormat",
     "UpdateEntityRequest",
     "StorageSystem",
     "DataSource",
     "ScannedData",
     "Trigger",
     "Action",
@@ -204,14 +208,16 @@
     "ListSessionsResponse",
     "ListTasksRequest",
     "ListTasksResponse",
     "ListZoneActionsRequest",
     "ListZonesRequest",
     "ListZonesResponse",
     "OperationMetadata",
+    "RunTaskRequest",
+    "RunTaskResponse",
     "UpdateAssetRequest",
     "UpdateEnvironmentRequest",
     "UpdateLakeRequest",
     "UpdateTaskRequest",
     "UpdateZoneRequest",
     "Job",
     "Task",
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/analyze.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             proto.MESSAGE,
             number=100,
             oneof="runtime",
             message="Environment.InfrastructureSpec.OsImageRuntime",
         )
 
     class SessionSpec(proto.Message):
-        r"""
+        r"""Configuration for sessions created for this environment.
 
         Attributes:
             max_idle_duration (google.protobuf.duration_pb2.Duration):
                 Optional. The idle time configuration of the
                 session. The session will be auto-terminated at
                 the end of this period.
             enable_fast_startup (bool):
@@ -204,30 +204,31 @@
         )
         enable_fast_startup: bool = proto.Field(
             proto.BOOL,
             number=2,
         )
 
     class SessionStatus(proto.Message):
-        r"""
+        r"""Status of sessions created for this environment.
 
         Attributes:
             active (bool):
                 Output only. Queries over sessions to mark
                 whether the environment is currently active or
                 not
         """
 
         active: bool = proto.Field(
             proto.BOOL,
             number=1,
         )
 
     class Endpoints(proto.Message):
-        r"""
+        r"""URI Endpoints to access sessions associated with the
+        Environment.
 
         Attributes:
             notebooks (str):
                 Output only. URI to serve notebook APIs
             sql (str):
                 Output only. URI to serve SQL APIs
         """
@@ -461,15 +462,15 @@
             projects/{project_id}/locations/{location_id}/lakes/{lake_id}/environment/{environment_id}/sessions/{session_id}
         user_id (str):
             Output only. Email of user running the
             session.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Session start time.
         state (google.cloud.dataplex_v1.types.State):
-
+            Output only. State of Session
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     user_id: str = proto.Field(
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/content.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/content.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/data_profile.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/data_profile.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,126 +31,113 @@
 
 
 class DataProfileSpec(proto.Message):
     r"""DataProfileScan related setting."""
 
 
 class DataProfileResult(proto.Message):
-    r"""DataProfileResult defines the output of DataProfileScan.
-    Each field of the table will have field type specific profile
-    result.
+    r"""DataProfileResult defines the output of DataProfileScan. Each
+    field of the table will have field type specific profile result.
 
     Attributes:
         row_count (int):
-            The count of all rows in the sampled data.
-            Return 0, if zero rows.
+            The count of rows scanned.
         profile (google.cloud.dataplex_v1.types.DataProfileResult.Profile):
-            This represents the profile information per
-            field.
+            The profile information per field.
         scanned_data (google.cloud.dataplex_v1.types.ScannedData):
-            The data scanned for this profile.
+            The data scanned for this result.
     """
 
     class Profile(proto.Message):
-        r"""Profile information describing the structure and layout of
-        the data and contains the profile info.
+        r"""Contains name, type, mode and field type specific profile
+        information.
 
         Attributes:
             fields (MutableSequence[google.cloud.dataplex_v1.types.DataProfileResult.Profile.Field]):
-                The sequence of fields describing data in
-                table entities.
+                List of fields with structural and profile
+                information for each field.
         """
 
         class Field(proto.Message):
-            r"""Represents a column field within a table schema.
+            r"""A field within a table.
 
             Attributes:
                 name (str):
                     The name of the field.
                 type_ (str):
-                    The field data type. Possible values include:
-
-                    -  STRING
-                    -  BYTE
-                    -  INT64
-                    -  INT32
-                    -  INT16
-                    -  DOUBLE
-                    -  FLOAT
-                    -  DECIMAL
-                    -  BOOLEAN
-                    -  BINARY
-                    -  TIMESTAMP
-                    -  DATE
-                    -  TIME
-                    -  NULL
-                    -  RECORD
+                    The data type retrieved from the schema of the data source.
+                    For instance, for a BigQuery native table, it is the
+                    `BigQuery Table
+                    Schema <https://cloud.google.com/bigquery/docs/reference/rest/v2/tables#tablefieldschema>`__.
+                    For a Dataplex Entity, it is the `Entity
+                    Schema <https://cloud.google.com/dataplex/docs/reference/rpc/google.cloud.dataplex.v1#type_3>`__.
                 mode (str):
-                    The mode of the field. Its value will be:
-                    REQUIRED, if it is a required field.
-                    NULLABLE, if it is an optional field.
-                    REPEATED, if it is a repeated field.
+                    The mode of the field. Possible values include:
+
+                    -  REQUIRED, if it is a required field.
+                    -  NULLABLE, if it is an optional field.
+                    -  REPEATED, if it is a repeated field.
                 profile (google.cloud.dataplex_v1.types.DataProfileResult.Profile.Field.ProfileInfo):
-                    The profile information for the corresponding
+                    Profile information for the corresponding
                     field.
             """
 
             class ProfileInfo(proto.Message):
-                r"""ProfileInfo defines the profile information for each schema
-                field type.
+                r"""The profile information for each field type.
 
                 This message has `oneof`_ fields (mutually exclusive fields).
                 For each oneof, at most one member field can be set at the same time.
                 Setting any member of the oneof automatically clears all other
                 members.
 
                 .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
                 Attributes:
                     null_ratio (float):
-                        The ratio of null rows against the rows in
-                        the sampled data.
+                        Ratio of rows with null value against total
+                        scanned rows.
                     distinct_ratio (float):
-                        The ratio of rows that are distinct against
-                        the rows in the sampled data.
+                        Ratio of rows with distinct values against
+                        total scanned rows. Not available for complex
+                        non-groupable field type RECORD and fields with
+                        REPEATABLE mode.
                     top_n_values (MutableSequence[google.cloud.dataplex_v1.types.DataProfileResult.Profile.Field.ProfileInfo.TopNValue]):
-                        The array of top N values of the field in the
-                        sampled data. Currently N is set as 10 or equal
-                        to distinct values in the field, whichever is
-                        smaller. This will be optional for complex
-                        non-groupable data-types such as JSON, ARRAY,
-                        JSON, STRUCT.
+                        The list of top N non-null values and number
+                        of times they occur in the scanned data. N is 10
+                        or equal to the number of distinct values in the
+                        field, whichever is smaller. Not available for
+                        complex non-groupable field type RECORD and
+                        fields with REPEATABLE mode.
                     string_profile (google.cloud.dataplex_v1.types.DataProfileResult.Profile.Field.ProfileInfo.StringFieldInfo):
-                        The corresponding string field profile.
+                        String type field information.
 
                         This field is a member of `oneof`_ ``field_info``.
                     integer_profile (google.cloud.dataplex_v1.types.DataProfileResult.Profile.Field.ProfileInfo.IntegerFieldInfo):
-                        The corresponding integer field profile.
+                        Integer type field information.
 
                         This field is a member of `oneof`_ ``field_info``.
                     double_profile (google.cloud.dataplex_v1.types.DataProfileResult.Profile.Field.ProfileInfo.DoubleFieldInfo):
-                        The corresponding double field profile.
+                        Double type field information.
 
                         This field is a member of `oneof`_ ``field_info``.
                 """
 
                 class StringFieldInfo(proto.Message):
-                    r"""StringFieldInfo defines output info for any string type
-                    field.
+                    r"""The profile information for a string type field.
 
                     Attributes:
                         min_length (int):
-                            The minimum length of the string field in the
-                            sampled data. Optional if zero non-null rows.
+                            Minimum length of non-null values in the
+                            scanned data.
                         max_length (int):
-                            The maximum length of a string field in the
-                            sampled data. Optional if zero non-null rows.
+                            Maximum length of non-null values in the
+                            scanned data.
                         average_length (float):
-                            The average length of a string field in the
-                            sampled data. Optional if zero non-null rows.
+                            Average length of non-null values in the
+                            scanned data.
                     """
 
                     min_length: int = proto.Field(
                         proto.INT64,
                         number=1,
                     )
                     max_length: int = proto.Field(
@@ -159,49 +146,46 @@
                     )
                     average_length: float = proto.Field(
                         proto.DOUBLE,
                         number=3,
                     )
 
                 class IntegerFieldInfo(proto.Message):
-                    r"""IntegerFieldInfo defines output for any integer type field.
+                    r"""The profile information for an integer type field.
 
                     Attributes:
                         average (float):
-                            The average of non-null values of integer
-                            field in the sampled data. Return NaN, if the
-                            field has a NaN. Optional if zero non-null rows.
+                            Average of non-null values in the scanned
+                            data. NaN, if the field has a NaN.
                         standard_deviation (float):
-                            The standard deviation of non-null of integer
-                            field in the sampled data. Return NaN, if the
-                            field has a NaN. Optional if zero non-null rows.
+                            Standard deviation of non-null values in the
+                            scanned data. NaN, if the field has a NaN.
                         min_ (int):
-                            The minimum value of an integer field in the
-                            sampled data. Return NaN, if the field has a
-                            NaN. Optional if zero non-null rows.
+                            Minimum of non-null values in the scanned
+                            data. NaN, if the field has a NaN.
                         quartiles (MutableSequence[int]):
-                            A quartile divide the number of data points
+                            A quartile divides the number of data points
                             into four parts, or quarters, of more-or-less
                             equal size. Three main quartiles used are: The
                             first quartile (Q1) splits off the lowest 25% of
                             data from the highest 75%. It is also known as
                             the lower or 25th empirical quartile, as 25% of
                             the data is below this point. The second
                             quartile (Q2) is the median of a data set. So,
                             50% of the data lies below this point. The third
                             quartile (Q3) splits off the highest 25% of data
                             from the lowest 75%. It is known as the upper or
                             75th empirical quartile, as 75% of the data lies
-                            below this point. So, here the quartiles is
-                            provided as an ordered list of quartile values,
-                            occurring in order Q1, median, Q3.
+                            below this point. Here, the quartiles is
+                            provided as an ordered list of quartile values
+                            for the scanned data, occurring in order Q1,
+                            median, Q3.
                         max_ (int):
-                            The maximum value of an integer field in the
-                            sampled data. Return NaN, if the field has a
-                            NaN. Optional if zero non-null rows.
+                            Maximum of non-null values in the scanned
+                            data. NaN, if the field has a NaN.
                     """
 
                     average: float = proto.Field(
                         proto.DOUBLE,
                         number=1,
                     )
                     standard_deviation: float = proto.Field(
@@ -218,49 +202,46 @@
                     )
                     max_: int = proto.Field(
                         proto.INT64,
                         number=5,
                     )
 
                 class DoubleFieldInfo(proto.Message):
-                    r"""DoubleFieldInfo defines output for any double type field.
+                    r"""The profile information for a double type field.
 
                     Attributes:
                         average (float):
-                            The average of non-null values of double
-                            field in the sampled data. Return NaN, if the
-                            field has a NaN. Optional if zero non-null rows.
+                            Average of non-null values in the scanned
+                            data. NaN, if the field has a NaN.
                         standard_deviation (float):
-                            The standard deviation of non-null of double
-                            field in the sampled data. Return NaN, if the
-                            field has a NaN. Optional if zero non-null rows.
+                            Standard deviation of non-null values in the
+                            scanned data. NaN, if the field has a NaN.
                         min_ (float):
-                            The minimum value of a double field in the
-                            sampled data. Return NaN, if the field has a
-                            NaN. Optional if zero non-null rows.
+                            Minimum of non-null values in the scanned
+                            data. NaN, if the field has a NaN.
                         quartiles (MutableSequence[float]):
-                            A quartile divide the numebr of data points
+                            A quartile divides the number of data points
                             into four parts, or quarters, of more-or-less
                             equal size. Three main quartiles used are: The
                             first quartile (Q1) splits off the lowest 25% of
                             data from the highest 75%. It is also known as
                             the lower or 25th empirical quartile, as 25% of
                             the data is below this point. The second
                             quartile (Q2) is the median of a data set. So,
                             50% of the data lies below this point. The third
                             quartile (Q3) splits off the highest 25% of data
                             from the lowest 75%. It is known as the upper or
                             75th empirical quartile, as 75% of the data lies
-                            below this point. So, here the quartiles is
-                            provided as an ordered list of quartile values,
-                            occurring in order Q1, median, Q3.
+                            below this point. Here, the quartiles is
+                            provided as an ordered list of quartile values
+                            for the scanned data, occurring in order Q1,
+                            median, Q3.
                         max_ (float):
-                            The maximum value of a double field in the
-                            sampled data. Return NaN, if the field has a
-                            NaN. Optional if zero non-null rows.
+                            Maximum of non-null values in the scanned
+                            data. NaN, if the field has a NaN.
                     """
 
                     average: float = proto.Field(
                         proto.DOUBLE,
                         number=1,
                     )
                     standard_deviation: float = proto.Field(
@@ -277,24 +258,22 @@
                     )
                     max_: float = proto.Field(
                         proto.DOUBLE,
                         number=5,
                     )
 
                 class TopNValue(proto.Message):
-                    r"""The TopNValue defines the structure of output of top N values
-                    of a field.
+                    r"""Top N non-null values in the scanned data.
 
                     Attributes:
                         value (str):
-                            The value is the string value of the actual
-                            value from the field.
+                            String value of a top N non-null value.
                         count (int):
-                            The frequency count of the corresponding
-                            value in the field.
+                            Count of the corresponding value in the
+                            scanned data.
                     """
 
                     value: str = proto.Field(
                         proto.STRING,
                         number=1,
                     )
                     count: int = proto.Field(
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/data_quality.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/data_quality.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 class DataQualityResult(proto.Message):
     r"""The output of a DataQualityScan.
 
     Attributes:
         passed (bool):
             Overall data quality result -- ``true`` if all rules passed.
         dimensions (MutableSequence[google.cloud.dataplex_v1.types.DataQualityDimensionResult]):
-            A list of results at the dimension-level.
+            A list of results at the dimension level.
         rules (MutableSequence[google.cloud.dataplex_v1.types.DataQualityRuleResult]):
             A list of all the rules in a job, and their
             results.
         row_count (int):
             The count of rows processed.
         scanned_data (google.cloud.dataplex_v1.types.ScannedData):
             The data scanned for this result.
@@ -88,40 +88,43 @@
         proto.MESSAGE,
         number=7,
         message=processing.ScannedData,
     )
 
 
 class DataQualityRuleResult(proto.Message):
-    r"""DataQualityRuleResult provides a more detailed, per-rule
-    level view of the results.
+    r"""DataQualityRuleResult provides a more detailed, per-rule view
+    of the results.
 
     Attributes:
         rule (google.cloud.dataplex_v1.types.DataQualityRule):
             The rule specified in the DataQualitySpec, as
             is.
         passed (bool):
             Whether the rule passed or failed.
         evaluated_count (int):
             The number of rows a rule was evaluated against. This field
-            is only valid for ColumnMap type rules. Evaluated count can
-            be configured to either (1) include all rows (default) -
-            with null rows automatically failing rule evaluation OR (2)
-            exclude null rows from the evaluated_count, by setting
-            ignore_nulls = true
+            is only valid for ColumnMap type rules.
+
+            Evaluated count can be configured to either
+
+            -  include all rows (default) - with ``null`` rows
+               automatically failing rule evaluation, or
+            -  exclude ``null`` rows from the ``evaluated_count``, by
+               setting ``ignore_nulls = true``.
         passed_count (int):
             The number of rows which passed a rule
             evaluation. This field is only valid for
             ColumnMap type rules.
         null_count (int):
             The number of rows with null values in the
             specified column.
         pass_ratio (float):
-            The ratio of passed_count / evaluated_count. This field is
-            only valid for ColumnMap type rules.
+            The ratio of **passed_count / evaluated_count**. This field
+            is only valid for ColumnMap type rules.
         failing_rows_query (str):
             The query to find rows that did not pass this
             rule. Only applies to ColumnMap and RowCondition
             rules.
     """
 
     rule: "DataQualityRule" = proto.Field(
@@ -153,15 +156,15 @@
         proto.STRING,
         number=10,
     )
 
 
 class DataQualityDimensionResult(proto.Message):
     r"""DataQualityDimensionResult provides a more detailed,
-    per-dimension level view of the results.
+    per-dimension view of the results.
 
     Attributes:
         passed (bool):
             Whether the dimension passed or failed.
     """
 
     passed: bool = proto.Field(
@@ -222,51 +225,56 @@
             provided expression is true.
 
             This field is a member of `oneof`_ ``rule_type``.
         column (str):
             Optional. The unnested column which this rule
             is evaluated against.
         ignore_null (bool):
-            Optional. Rows with null values will automatically fail a
-            rule, unless ignore_null is true. In that case, such null
-            rows are trivially considered passing. Only applicable to
-            ColumnMap rules.
+            Optional. Rows with ``null`` values will automatically fail
+            a rule, unless ``ignore_null`` is ``true``. In that case,
+            such ``null`` rows are trivially considered passing.
+
+            Only applicable to ColumnMap rules.
         dimension (str):
             Required. The dimension a rule belongs to. Results are also
-            aggregated at the dimension-level. Supported dimensions are
-            ["COMPLETENESS", "ACCURACY", "CONSISTENCY", "VALIDITY",
-            "UNIQUENESS", "INTEGRITY"]
+            aggregated at the dimension level. Supported dimensions are
+            **["COMPLETENESS", "ACCURACY", "CONSISTENCY", "VALIDITY",
+            "UNIQUENESS", "INTEGRITY"]**
         threshold (float):
-            Optional. The minimum ratio of passing_rows / total_rows
-            required to pass this rule, with a range of [0.0, 1.0]
+            Optional. The minimum ratio of **passing_rows / total_rows**
+            required to pass this rule, with a range of [0.0, 1.0].
 
-            0 indicates default value (i.e. 1.0)
+            0 indicates default value (i.e. 1.0).
     """
 
     class RangeExpectation(proto.Message):
         r"""Evaluates whether each column value lies between a specified
         range.
 
         Attributes:
             min_value (str):
                 Optional. The minimum column value allowed for a row to pass
-                this validation. At least one of min_value and max_value
-                need to be provided.
+                this validation. At least one of ``min_value`` and
+                ``max_value`` need to be provided.
             max_value (str):
                 Optional. The maximum column value allowed for a row to pass
-                this validation. At least one of min_value and max_value
-                need to be provided.
+                this validation. At least one of ``min_value`` and
+                ``max_value`` need to be provided.
             strict_min_enabled (bool):
                 Optional. Whether each value needs to be strictly greater
-                than ('>') the minimum, or if equality is allowed. Only
-                relevant if a min_value has been defined. Default = false.
+                than ('>') the minimum, or if equality is allowed.
+
+                Only relevant if a ``min_value`` has been defined. Default =
+                false.
             strict_max_enabled (bool):
                 Optional. Whether each value needs to be strictly lesser
-                than ('<') the maximum, or if equality is allowed. Only
-                relevant if a max_value has been defined. Default = false.
+                than ('<') the maximum, or if equality is allowed.
+
+                Only relevant if a ``max_value`` has been defined. Default =
+                false.
         """
 
         min_value: str = proto.Field(
             proto.STRING,
             number=1,
         )
         max_value: str = proto.Field(
@@ -287,29 +295,30 @@
 
     class SetExpectation(proto.Message):
         r"""Evaluates whether each column value is contained by a
         specified set.
 
         Attributes:
             values (MutableSequence[str]):
-
+                Expected values for the column value.
         """
 
         values: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=1,
         )
 
     class RegexExpectation(proto.Message):
         r"""Evaluates whether each column value matches a specified
         regex.
 
         Attributes:
             regex (str):
-
+                A regular expression the column value is
+                expected to match.
         """
 
         regex: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
@@ -318,35 +327,44 @@
 
     class StatisticRangeExpectation(proto.Message):
         r"""Evaluates whether the column aggregate statistic lies between
         a specified range.
 
         Attributes:
             statistic (google.cloud.dataplex_v1.types.DataQualityRule.StatisticRangeExpectation.ColumnStatistic):
-
+                The aggregate metric to evaluate.
             min_value (str):
                 The minimum column statistic value allowed for a row to pass
-                this validation. At least one of min_value and max_value
-                need to be provided.
+                this validation.
+
+                At least one of ``min_value`` and ``max_value`` need to be
+                provided.
             max_value (str):
                 The maximum column statistic value allowed for a row to pass
-                this validation. At least one of min_value and max_value
-                need to be provided.
+                this validation.
+
+                At least one of ``min_value`` and ``max_value`` need to be
+                provided.
             strict_min_enabled (bool):
                 Whether column statistic needs to be strictly greater than
-                ('>') the minimum, or if equality is allowed. Only relevant
-                if a min_value has been defined. Default = false.
+                ('>') the minimum, or if equality is allowed.
+
+                Only relevant if a ``min_value`` has been defined. Default =
+                false.
             strict_max_enabled (bool):
                 Whether column statistic needs to be strictly lesser than
-                ('<') the maximum, or if equality is allowed. Only relevant
-                if a max_value has been defined. Default = false.
+                ('<') the maximum, or if equality is allowed.
+
+                Only relevant if a ``max_value`` has been defined. Default =
+                false.
         """
 
         class ColumnStatistic(proto.Enum):
-            r"""
+            r"""The list of aggregate metrics a rule can be evaluated
+            against.
 
             Values:
                 STATISTIC_UNDEFINED (0):
                     Unspecified statistic type
                 MEAN (1):
                     Evaluate the column mean
                 MIN (2):
@@ -382,36 +400,38 @@
             proto.BOOL,
             number=5,
         )
 
     class RowConditionExpectation(proto.Message):
         r"""Evaluates whether each row passes the specified condition.
         The SQL expression needs to use BigQuery standard SQL syntax and
-        should produce a boolean per row as the result.
+        should produce a boolean value per row as the result.
+
         Example: col1 >= 0 AND col2 < 10
 
         Attributes:
             sql_expression (str):
-
+                The SQL expression.
         """
 
         sql_expression: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
     class TableConditionExpectation(proto.Message):
         r"""Evaluates whether the provided expression is true.
         The SQL expression needs to use BigQuery standard SQL syntax and
         should produce a scalar boolean result.
+
         Example: MIN(col1) >= 0
 
         Attributes:
             sql_expression (str):
-
+                The SQL expression.
         """
 
         sql_expression: str = proto.Field(
             proto.STRING,
             number=1,
         )
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/datascans.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/datascans.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,17 @@
             Required. DataScan identifier.
 
             -  Must contain only lowercase letters, numbers and hyphens.
             -  Must start with a letter.
             -  Must end with a number or a letter.
             -  Must be between 1-63 characters.
             -  Must be unique within the customer project / location.
+        validate_only (bool):
+            Optional. Only validate the request, but do not perform
+            mutations. The default is ``false``.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     data_scan: "DataScan" = proto.Field(
@@ -95,38 +98,49 @@
         number=2,
         message="DataScan",
     )
     data_scan_id: str = proto.Field(
         proto.STRING,
         number=3,
     )
+    validate_only: bool = proto.Field(
+        proto.BOOL,
+        number=4,
+    )
 
 
 class UpdateDataScanRequest(proto.Message):
     r"""Update dataScan request.
 
     Attributes:
         data_scan (google.cloud.dataplex_v1.types.DataScan):
             Required. DataScan resource to be updated.
 
             Only fields specified in ``update_mask`` are updated.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask of fields to update.
+        validate_only (bool):
+            Optional. Only validate the request, but do not perform
+            mutations. The default is ``false``.
     """
 
     data_scan: "DataScan" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="DataScan",
     )
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
+    validate_only: bool = proto.Field(
+        proto.BOOL,
+        number=3,
+    )
 
 
 class DeleteDataScanRequest(proto.Message):
     r"""Delete dataScan request.
 
     Attributes:
         name (str):
@@ -190,15 +204,15 @@
             Required. The resource name of the parent location:
             ``projects/{project}/locations/{location_id}`` where
             ``project`` refers to a *project_id* or *project_number* and
             ``location_id`` refers to a GCP region.
         page_size (int):
             Optional. Maximum number of dataScans to
             return. The service may return fewer than this
-            value. If unspecified, at most 10 scans will be
+            value. If unspecified, at most 500 scans will be
             returned. The maximum value is 1000; values
             above 1000 will be coerced to 1000.
         page_token (str):
             Optional. Page token received from a previous
             ``ListDataScans`` call. Provide this to retrieve the
             subsequent page. When paginating, all other parameters
             provided to ``ListDataScans`` must match the call that
@@ -302,15 +316,15 @@
 
 class GetDataScanJobRequest(proto.Message):
     r"""Get DataScanJob request.
 
     Attributes:
         name (str):
             Required. The resource name of the DataScanJob:
-            ``projects/{project}/locations/{location_id}/dataScans/{data_scan_id}/dataScanJobs/{data_scan_job_id}``
+            ``projects/{project}/locations/{location_id}/dataScans/{data_scan_id}/jobs/{data_scan_job_id}``
             where ``project`` refers to a *project_id* or
             *project_number* and ``location_id`` refers to a GCP region.
         view (google.cloud.dataplex_v1.types.GetDataScanJobRequest.DataScanJobView):
             Optional. Select the DataScanJob view to return. Defaults to
             ``BASIC``.
     """
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/logs.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/logs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/metadata_.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/metadata_.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         "DeletePartitionRequest",
         "ListPartitionsResponse",
         "GetPartitionRequest",
         "Entity",
         "Partition",
         "Schema",
         "StorageFormat",
+        "StorageAccess",
     },
 )
 
 
 class StorageSystem(proto.Enum):
     r"""Identifies the cloud system that manages the data storage.
 
@@ -468,16 +469,16 @@
             last updated.
         id (str):
             Required. A user-provided entity ID. It is
             mutable, and will be used as the published table
             name. Specifying a new ID in an update entity
             request will override the existing value.
             The ID must contain only letters (a-z, A-Z),
-            numbers (0-9), and underscores. Must begin with
-            a letter and consist of 256 or fewer characters.
+            numbers (0-9), and underscores, and consist of
+            256 or fewer characters.
         etag (str):
             Optional. The etag associated with the entity, which can be
             retrieved with a [GetEntity][] request. Required for update
             and delete requests.
         type_ (google.cloud.dataplex_v1.types.Entity.Type):
             Required. Immutable. The type of entity.
         asset (str):
@@ -505,14 +506,22 @@
         format_ (google.cloud.dataplex_v1.types.StorageFormat):
             Required. Identifies the storage format of
             the entity data. It does not apply to entities
             with data stored in BigQuery.
         compatibility (google.cloud.dataplex_v1.types.Entity.CompatibilityStatus):
             Output only. Metadata stores that the entity
             is compatible with.
+        access (google.cloud.dataplex_v1.types.StorageAccess):
+            Output only. Identifies the access mechanism
+            to the entity. Not user settable.
+        uid (str):
+            Output only. System generated unique ID for
+            the Entity. This ID will be different if the
+            Entity is deleted and re-created with the same
+            name.
         schema (google.cloud.dataplex_v1.types.Schema):
             Required. The description of the data structure and layout.
             The schema is not included in list responses. It is only
             included in ``SCHEMA`` and ``FULL`` entity views of a
             ``GetEntity`` response.
     """
 
@@ -640,14 +649,23 @@
         message="StorageFormat",
     )
     compatibility: CompatibilityStatus = proto.Field(
         proto.MESSAGE,
         number=19,
         message=CompatibilityStatus,
     )
+    access: "StorageAccess" = proto.Field(
+        proto.MESSAGE,
+        number=21,
+        message="StorageAccess",
+    )
+    uid: str = proto.Field(
+        proto.STRING,
+        number=22,
+    )
     schema: "Schema" = proto.Field(
         proto.MESSAGE,
         number=50,
         message="Schema",
     )
 
 
@@ -1125,8 +1143,43 @@
         proto.MESSAGE,
         number=12,
         oneof="options",
         message=IcebergOptions,
     )
 
 
+class StorageAccess(proto.Message):
+    r"""Describes the access mechanism of the data within its storage
+    location.
+
+    Attributes:
+        read (google.cloud.dataplex_v1.types.StorageAccess.AccessMode):
+            Output only. Describes the read access
+            mechanism of the data. Not user settable.
+    """
+
+    class AccessMode(proto.Enum):
+        r"""Access Mode determines how data stored within the Entity is
+        read.
+
+        Values:
+            ACCESS_MODE_UNSPECIFIED (0):
+                Access mode unspecified.
+            DIRECT (1):
+                Default. Data is accessed directly using
+                storage APIs.
+            MANAGED (2):
+                Data is accessed through a managed interface
+                using BigQuery APIs.
+        """
+        ACCESS_MODE_UNSPECIFIED = 0
+        DIRECT = 1
+        MANAGED = 2
+
+    read: AccessMode = proto.Field(
+        proto.ENUM,
+        number=21,
+        enum=AccessMode,
+    )
+
+
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/processing.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/processing.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,40 +37,43 @@
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         on_demand (google.cloud.dataplex_v1.types.Trigger.OnDemand):
-            The scan runs one-time shortly after DataScan
-            Creation.
+            The scan runs once via ``RunDataScan`` API.
 
             This field is a member of `oneof`_ ``mode``.
         schedule (google.cloud.dataplex_v1.types.Trigger.Schedule):
             The scan is scheduled to run periodically.
 
             This field is a member of `oneof`_ ``mode``.
     """
 
     class OnDemand(proto.Message):
-        r"""The scan runs one-time via RunDataScan API."""
+        r"""The scan runs once via ``RunDataScan`` API."""
 
     class Schedule(proto.Message):
         r"""The scan is scheduled to run periodically.
 
         Attributes:
             cron (str):
-                Required. Cron schedule (https://en.wikipedia.org/wiki/Cron)
-                for running scans periodically. To explicitly set a timezone
-                to the cron tab, apply a prefix in the cron tab:
-                "CRON_TZ=${IANA_TIME_ZONE}" or "TZ=${IANA_TIME_ZONE}". The
-                ${IANA_TIME_ZONE} may only be a valid string from IANA time
-                zone database. For example, "CRON_TZ=America/New_York 1 \*
-                \* \* \*", or "TZ=America/New_York 1 \* \* \* \*". This
-                field is required for Schedule scans.
+                Required. `Cron <https://en.wikipedia.org/wiki/Cron>`__
+                schedule for running scans periodically.
+
+                To explicitly set a timezone in the cron tab, apply a prefix
+                in the cron tab: **"CRON_TZ=${IANA_TIME_ZONE}"** or
+                **"TZ=${IANA_TIME_ZONE}"**. The **${IANA_TIME_ZONE}** may
+                only be a valid string from IANA time zone database
+                (`wikipedia <https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List>`__).
+                For example, ``CRON_TZ=America/New_York 1 * * * *``, or
+                ``TZ=America/New_York 1 * * * *``.
+
+                This field is required for Schedule scans.
         """
 
         cron: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
@@ -87,30 +90,48 @@
         message=Schedule,
     )
 
 
 class DataSource(proto.Message):
     r"""The data source for DataScan.
 
+    This message has `oneof`_ fields (mutually exclusive fields).
+    For each oneof, at most one member field can be set at the same time.
+    Setting any member of the oneof automatically clears all other
+    members.
+
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         entity (str):
-            Immutable. The dataplex entity that contains the data for
-            DataScan, of the form:
+            Immutable. The Dataplex entity that represents the data
+            source (e.g. BigQuery table) for DataScan, of the form:
             ``projects/{project_number}/locations/{location_id}/lakes/{lake_id}/zones/{zone_id}/entities/{entity_id}``.
 
             This field is a member of `oneof`_ ``source``.
+        resource (str):
+            Immutable. The service-qualified full resource name of the
+            cloud resource for a DataScan job to scan against. The field
+            could be: BigQuery table of type "TABLE" for
+            DataProfileScan/DataQualityScan Format:
+            //bigquery.googleapis.com/projects/PROJECT_ID/datasets/DATASET_ID/tables/TABLE_ID
+
+            This field is a member of `oneof`_ ``source``.
     """
 
     entity: str = proto.Field(
         proto.STRING,
         number=100,
         oneof="source",
     )
+    resource: str = proto.Field(
+        proto.STRING,
+        number=101,
+        oneof="source",
+    )
 
 
 class ScannedData(proto.Message):
     r"""The data scanned during processing (e.g. in incremental
     DataScan)
 
 
@@ -127,20 +148,20 @@
     class IncrementalField(proto.Message):
         r"""A data range denoted by a pair of start/end values of a
         field.
 
         Attributes:
             field (str):
                 The field that contains values which
-                monotonically increases over time (e.g.
-                timestamp).
+                monotonically increases over time (e.g. a
+                timestamp column).
             start (str):
-                Value that marks the start of the range
+                Value that marks the start of the range.
             end (str):
-                Value that marks the end of the range
+                Value that marks the end of the range.
         """
 
         field: str = proto.Field(
             proto.STRING,
             number=1,
         )
         start: str = proto.Field(
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/resources.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,16 +407,21 @@
                 for running discovery periodically. Successive discovery
                 runs must be scheduled at least 60 minutes apart. The
                 default value is to run discovery every 60 minutes. To
                 explicitly set a timezone to the cron tab, apply a prefix in
                 the cron tab: "CRON_TZ=${IANA_TIME_ZONE}" or
                 TZ=${IANA_TIME_ZONE}". The ${IANA_TIME_ZONE} may only be a
                 valid string from IANA time zone database. For example,
-                ``CRON_TZ=America/New_York 1 * * * *``, or
-                ``TZ=America/New_York 1 * * * *``.
+                \`CRON_TZ=America/New_York 1
+
+                -
+
+                   -
+
+                      -  \*\ ``, or``\ TZ=America/New_York 1 \* \* \* \*`.
 
                 This field is a member of `oneof`_ ``trigger``.
         """
 
         class CsvOptions(proto.Message):
             r"""Describe CSV and similar semi-structured data formats.
 
@@ -1052,16 +1057,21 @@
                 for running discovery periodically. Successive discovery
                 runs must be scheduled at least 60 minutes apart. The
                 default value is to run discovery every 60 minutes. To
                 explicitly set a timezone to the cron tab, apply a prefix in
                 the cron tab: "CRON_TZ=${IANA_TIME_ZONE}" or
                 TZ=${IANA_TIME_ZONE}". The ${IANA_TIME_ZONE} may only be a
                 valid string from IANA time zone database. For example,
-                ``CRON_TZ=America/New_York 1 * * * *``, or
-                ``TZ=America/New_York 1 * * * *``.
+                \`CRON_TZ=America/New_York 1
+
+                -
+
+                   -
+
+                      -  \*\ ``, or``\ TZ=America/New_York 1 \* \* \* \*`.
 
                 This field is a member of `oneof`_ ``trigger``.
         """
 
         class CsvOptions(proto.Message):
             r"""Describe CSV and similar semi-structured data formats.
 
@@ -1158,14 +1168,19 @@
             name (str):
                 Immutable. Relative name of the cloud resource that contains
                 the data that is being managed within a lake. For example:
                 ``projects/{project_number}/buckets/{bucket_id}``
                 ``projects/{project_number}/datasets/{dataset_id}``
             type_ (google.cloud.dataplex_v1.types.Asset.ResourceSpec.Type):
                 Required. Immutable. Type of resource.
+            read_access_mode (google.cloud.dataplex_v1.types.Asset.ResourceSpec.AccessMode):
+                Optional. Determines how read permissions are
+                handled for each asset and their associated
+                tables. Only available to storage buckets
+                assets.
         """
 
         class Type(proto.Enum):
             r"""Type of resource.
 
             Values:
                 TYPE_UNSPECIFIED (0):
@@ -1175,35 +1190,61 @@
                 BIGQUERY_DATASET (2):
                     BigQuery dataset.
             """
             TYPE_UNSPECIFIED = 0
             STORAGE_BUCKET = 1
             BIGQUERY_DATASET = 2
 
+        class AccessMode(proto.Enum):
+            r"""Access Mode determines how data stored within the resource is
+            read. This is only applicable to storage bucket assets.
+
+            Values:
+                ACCESS_MODE_UNSPECIFIED (0):
+                    Access mode unspecified.
+                DIRECT (1):
+                    Default. Data is accessed directly using
+                    storage APIs.
+                MANAGED (2):
+                    Data is accessed through a managed interface
+                    using BigQuery APIs.
+            """
+            ACCESS_MODE_UNSPECIFIED = 0
+            DIRECT = 1
+            MANAGED = 2
+
         name: str = proto.Field(
             proto.STRING,
             number=1,
         )
         type_: "Asset.ResourceSpec.Type" = proto.Field(
             proto.ENUM,
             number=2,
             enum="Asset.ResourceSpec.Type",
         )
+        read_access_mode: "Asset.ResourceSpec.AccessMode" = proto.Field(
+            proto.ENUM,
+            number=5,
+            enum="Asset.ResourceSpec.AccessMode",
+        )
 
     class ResourceStatus(proto.Message):
         r"""Status of the resource referenced by an asset.
 
         Attributes:
             state (google.cloud.dataplex_v1.types.Asset.ResourceStatus.State):
                 The current state of the managed resource.
             message (str):
                 Additional information about the current
                 state.
             update_time (google.protobuf.timestamp_pb2.Timestamp):
                 Last update time of the status.
+            managed_access_identity (str):
+                Output only. Service account associated with
+                the BigQuery Connection.
         """
 
         class State(proto.Enum):
             r"""The state of a resource.
 
             Values:
                 STATE_UNSPECIFIED (0):
@@ -1227,14 +1268,18 @@
             number=2,
         )
         update_time: timestamp_pb2.Timestamp = proto.Field(
             proto.MESSAGE,
             number=3,
             message=timestamp_pb2.Timestamp,
         )
+        managed_access_identity: str = proto.Field(
+            proto.STRING,
+            number=4,
+        )
 
     class DiscoveryStatus(proto.Message):
         r"""Status of discovery for an asset.
 
         Attributes:
             state (google.cloud.dataplex_v1.types.Asset.DiscoveryStatus.State):
                 The current status of the discovery feature.
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/service.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         "CreateTaskRequest",
         "UpdateTaskRequest",
         "DeleteTaskRequest",
         "ListTasksRequest",
         "ListTasksResponse",
         "GetTaskRequest",
         "GetJobRequest",
+        "RunTaskRequest",
+        "RunTaskResponse",
         "ListJobsRequest",
         "ListJobsResponse",
         "CancelJobRequest",
         "CreateEnvironmentRequest",
         "UpdateEnvironmentRequest",
         "DeleteEnvironmentRequest",
         "ListEnvironmentsRequest",
@@ -991,14 +993,44 @@
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
+class RunTaskRequest(proto.Message):
+    r"""
+
+    Attributes:
+        name (str):
+            Required. The resource name of the task:
+            ``projects/{project_number}/locations/{location_id}/lakes/{lake_id}/tasks/{task_id}``.
+    """
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class RunTaskResponse(proto.Message):
+    r"""
+
+    Attributes:
+        job (google.cloud.dataplex_v1.types.Job):
+            Jobs created by RunTask API.
+    """
+
+    job: gcd_tasks.Job = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=gcd_tasks.Job,
+    )
+
+
 class ListJobsRequest(proto.Message):
     r"""List jobs request.
 
     Attributes:
         parent (str):
             Required. The resource name of the parent environment:
             ``projects/{project_number}/locations/{location_id}/lakes/{lake_id}/tasks/{task_id}``.
```

### Comparing `google-cloud-dataplex-1.4.3/google/cloud/dataplex_v1/types/tasks.py` & `google-cloud-dataplex-1.5.0/google/cloud/dataplex_v1/types/tasks.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/PKG-INFO` & `google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataplex
-Version: 1.4.3
+Version: 1.5.0
 Summary: Google Cloud Dataplex API client library
 Home-page: https://github.com/googleapis/python-dataplex
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dataplex-1.4.3/google_cloud_dataplex.egg-info/SOURCES.txt` & `google-cloud-dataplex-1.5.0/google_cloud_dataplex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/setup.py` & `google-cloud-dataplex-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/tests/__init__.py` & `google-cloud-dataplex-1.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/tests/unit/__init__.py` & `google-cloud-dataplex-1.5.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/tests/unit/gapic/__init__.py` & `google-cloud-dataplex-1.5.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/__init__.py` & `google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/test_content_service.py` & `google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_content_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/test_data_scan_service.py` & `google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_data_scan_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/test_dataplex_service.py` & `google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_dataplex_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -7964,14 +7964,240 @@
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        service.RunTaskRequest,
+        dict,
+    ],
+)
+def test_run_task(request_type, transport: str = "grpc"):
+    client = DataplexServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.run_task), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = service.RunTaskResponse()
+        response = client.run_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.RunTaskRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, service.RunTaskResponse)
+
+
+def test_run_task_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DataplexServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.run_task), "__call__") as call:
+        client.run_task()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.RunTaskRequest()
+
+
+@pytest.mark.asyncio
+async def test_run_task_async(
+    transport: str = "grpc_asyncio", request_type=service.RunTaskRequest
+):
+    client = DataplexServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.run_task), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            service.RunTaskResponse()
+        )
+        response = await client.run_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.RunTaskRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, service.RunTaskResponse)
+
+
+@pytest.mark.asyncio
+async def test_run_task_async_from_dict():
+    await test_run_task_async(request_type=dict)
+
+
+def test_run_task_field_headers():
+    client = DataplexServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = service.RunTaskRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.run_task), "__call__") as call:
+        call.return_value = service.RunTaskResponse()
+        client.run_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_run_task_field_headers_async():
+    client = DataplexServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = service.RunTaskRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.run_task), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            service.RunTaskResponse()
+        )
+        await client.run_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+def test_run_task_flattened():
+    client = DataplexServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.run_task), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = service.RunTaskResponse()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.run_task(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+def test_run_task_flattened_error():
+    client = DataplexServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.run_task(
+            service.RunTaskRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_run_task_flattened_async():
+    client = DataplexServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.run_task), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = service.RunTaskResponse()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            service.RunTaskResponse()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.run_task(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_run_task_flattened_error_async():
+    client = DataplexServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.run_task(
+            service.RunTaskRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         service.GetJobRequest,
         dict,
     ],
 )
 def test_get_job(request_type, transport: str = "grpc"):
     client = DataplexServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -10450,14 +10676,15 @@
         "list_asset_actions",
         "create_task",
         "update_task",
         "delete_task",
         "list_tasks",
         "get_task",
         "list_jobs",
+        "run_task",
         "get_job",
         "cancel_job",
         "create_environment",
         "update_environment",
         "delete_environment",
         "list_environments",
         "get_environment",
```

### Comparing `google-cloud-dataplex-1.4.3/tests/unit/gapic/dataplex_v1/test_metadata_service.py` & `google-cloud-dataplex-1.5.0/tests/unit/gapic/dataplex_v1/test_metadata_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -728,14 +728,15 @@
             etag="etag_value",
             type_=metadata_.Entity.Type.TABLE,
             asset="asset_value",
             data_path="data_path_value",
             data_path_pattern="data_path_pattern_value",
             catalog_entry="catalog_entry_value",
             system=metadata_.StorageSystem.CLOUD_STORAGE,
+            uid="uid_value",
         )
         response = client.create_entity(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metadata_.CreateEntityRequest()
@@ -749,14 +750,15 @@
     assert response.etag == "etag_value"
     assert response.type_ == metadata_.Entity.Type.TABLE
     assert response.asset == "asset_value"
     assert response.data_path == "data_path_value"
     assert response.data_path_pattern == "data_path_pattern_value"
     assert response.catalog_entry == "catalog_entry_value"
     assert response.system == metadata_.StorageSystem.CLOUD_STORAGE
+    assert response.uid == "uid_value"
 
 
 def test_create_entity_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetadataServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -796,14 +798,15 @@
                 etag="etag_value",
                 type_=metadata_.Entity.Type.TABLE,
                 asset="asset_value",
                 data_path="data_path_value",
                 data_path_pattern="data_path_pattern_value",
                 catalog_entry="catalog_entry_value",
                 system=metadata_.StorageSystem.CLOUD_STORAGE,
+                uid="uid_value",
             )
         )
         response = await client.create_entity(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -818,14 +821,15 @@
     assert response.etag == "etag_value"
     assert response.type_ == metadata_.Entity.Type.TABLE
     assert response.asset == "asset_value"
     assert response.data_path == "data_path_value"
     assert response.data_path_pattern == "data_path_pattern_value"
     assert response.catalog_entry == "catalog_entry_value"
     assert response.system == metadata_.StorageSystem.CLOUD_STORAGE
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_create_entity_async_from_dict():
     await test_create_entity_async(request_type=dict)
 
 
@@ -1006,14 +1010,15 @@
             etag="etag_value",
             type_=metadata_.Entity.Type.TABLE,
             asset="asset_value",
             data_path="data_path_value",
             data_path_pattern="data_path_pattern_value",
             catalog_entry="catalog_entry_value",
             system=metadata_.StorageSystem.CLOUD_STORAGE,
+            uid="uid_value",
         )
         response = client.update_entity(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metadata_.UpdateEntityRequest()
@@ -1027,14 +1032,15 @@
     assert response.etag == "etag_value"
     assert response.type_ == metadata_.Entity.Type.TABLE
     assert response.asset == "asset_value"
     assert response.data_path == "data_path_value"
     assert response.data_path_pattern == "data_path_pattern_value"
     assert response.catalog_entry == "catalog_entry_value"
     assert response.system == metadata_.StorageSystem.CLOUD_STORAGE
+    assert response.uid == "uid_value"
 
 
 def test_update_entity_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetadataServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1074,14 +1080,15 @@
                 etag="etag_value",
                 type_=metadata_.Entity.Type.TABLE,
                 asset="asset_value",
                 data_path="data_path_value",
                 data_path_pattern="data_path_pattern_value",
                 catalog_entry="catalog_entry_value",
                 system=metadata_.StorageSystem.CLOUD_STORAGE,
+                uid="uid_value",
             )
         )
         response = await client.update_entity(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1096,14 +1103,15 @@
     assert response.etag == "etag_value"
     assert response.type_ == metadata_.Entity.Type.TABLE
     assert response.asset == "asset_value"
     assert response.data_path == "data_path_value"
     assert response.data_path_pattern == "data_path_pattern_value"
     assert response.catalog_entry == "catalog_entry_value"
     assert response.system == metadata_.StorageSystem.CLOUD_STORAGE
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_update_entity_async_from_dict():
     await test_update_entity_async(request_type=dict)
 
 
@@ -1414,14 +1422,15 @@
             etag="etag_value",
             type_=metadata_.Entity.Type.TABLE,
             asset="asset_value",
             data_path="data_path_value",
             data_path_pattern="data_path_pattern_value",
             catalog_entry="catalog_entry_value",
             system=metadata_.StorageSystem.CLOUD_STORAGE,
+            uid="uid_value",
         )
         response = client.get_entity(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metadata_.GetEntityRequest()
@@ -1435,14 +1444,15 @@
     assert response.etag == "etag_value"
     assert response.type_ == metadata_.Entity.Type.TABLE
     assert response.asset == "asset_value"
     assert response.data_path == "data_path_value"
     assert response.data_path_pattern == "data_path_pattern_value"
     assert response.catalog_entry == "catalog_entry_value"
     assert response.system == metadata_.StorageSystem.CLOUD_STORAGE
+    assert response.uid == "uid_value"
 
 
 def test_get_entity_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetadataServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1482,14 +1492,15 @@
                 etag="etag_value",
                 type_=metadata_.Entity.Type.TABLE,
                 asset="asset_value",
                 data_path="data_path_value",
                 data_path_pattern="data_path_pattern_value",
                 catalog_entry="catalog_entry_value",
                 system=metadata_.StorageSystem.CLOUD_STORAGE,
+                uid="uid_value",
             )
         )
         response = await client.get_entity(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1504,14 +1515,15 @@
     assert response.etag == "etag_value"
     assert response.type_ == metadata_.Entity.Type.TABLE
     assert response.asset == "asset_value"
     assert response.data_path == "data_path_value"
     assert response.data_path_pattern == "data_path_pattern_value"
     assert response.catalog_entry == "catalog_entry_value"
     assert response.system == metadata_.StorageSystem.CLOUD_STORAGE
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_get_entity_async_from_dict():
     await test_get_entity_async(request_type=dict)
```

