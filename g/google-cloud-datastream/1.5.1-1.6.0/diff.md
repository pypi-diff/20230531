# Comparing `tmp/google-cloud-datastream-1.5.1.tar.gz` & `tmp/google-cloud-datastream-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-datastream-1.5.1.tar", last modified: Mon Mar 27 15:52:30 2023, max compression
+gzip compressed data, was "google-cloud-datastream-1.6.0.tar", last modified: Wed May 31 18:40:40 2023, max compression
```

## Comparing `google-cloud-datastream-1.5.1.tar` & `google-cloud-datastream-1.6.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.046039 google-cloud-datastream-1.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4683 2023-03-27 15:52:30.046039 google-cloud-datastream-1.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3758 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.030038 google-cloud-datastream-1.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.030038 google-cloud-datastream-1.5.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.034038 google-cloud-datastream-1.5.1/google/cloud/datastream/
--rw-rw-r--   0 root         (0)     1003     5078 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.034038 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/
--rw-rw-r--   0 root         (0)     1003     4916 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10384 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.034038 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.034038 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/
--rw-rw-r--   0 root         (0)     1003      753 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003   141640 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/async_client.py
--rw-rw-r--   0 root         (0)     1003   157494 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/client.py
--rw-rw-r--   0 root         (0)     1003    31348 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.034038 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    19242 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/base.py
--rw-rw-r--   0 root         (0)     1003    46386 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    47307 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   160720 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.038038 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/types/
--rw-rw-r--   0 root         (0)     1003     4661 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    44728 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/types/datastream.py
--rw-rw-r--   0 root         (0)     1003    62594 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1/types/datastream_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.038038 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/
--rw-rw-r--   0 root         (0)     1003     4154 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8809 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.038038 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.038038 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/
--rw-rw-r--   0 root         (0)     1003      753 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003   111029 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/async_client.py
--rw-rw-r--   0 root         (0)     1003   125201 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/client.py
--rw-rw-r--   0 root         (0)     1003    26460 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.038038 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15616 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py
--rw-rw-r--   0 root         (0)     1003    36520 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    37308 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   116775 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.042039 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/types/
--rw-rw-r--   0 root         (0)     1003     3893 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    38294 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/types/datastream.py
--rw-rw-r--   0 root         (0)     1003    40603 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/types/datastream_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.042039 google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/
--rw-r--r--   0 root         (0)     1003     4683 2023-03-27 15:52:29.000000 google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2747 2023-03-27 15:52:29.000000 google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:29.000000 google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:52:29.000000 google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:29.000000 google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:52:29.000000 google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:52:29.000000 google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:52:30.046039 google-cloud-datastream-1.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2980 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.042039 google-cloud-datastream-1.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.042039 google-cloud-datastream-1.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.042039 google-cloud-datastream-1.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.042039 google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   654092 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1/test_datastream.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.042039 google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1alpha1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003   511456 2023-03-27 15:49:32.000000 google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1alpha1/test_datastream.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.058371 google-cloud-datastream-1.6.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4683 2023-05-31 18:40:40.058371 google-cloud-datastream-1.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3758 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.042370 google-cloud-datastream-1.6.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.042370 google-cloud-datastream-1.6.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.046371 google-cloud-datastream-1.6.0/google/cloud/datastream/
+-rw-rw-r--   0 root         (0)     1003     5078 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.046371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/
+-rw-rw-r--   0 root         (0)     1003     4916 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10384 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.046371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/
+-rw-rw-r--   0 root         (0)     1003      753 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003   141640 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/async_client.py
+-rw-rw-r--   0 root         (0)     1003   157494 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/client.py
+-rw-rw-r--   0 root         (0)     1003    31348 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19242 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    46386 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    47307 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   160720 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4661 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44898 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/datastream.py
+-rw-rw-r--   0 root         (0)     1003    64096 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/datastream_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003     4154 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8809 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.050371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/
+-rw-rw-r--   0 root         (0)     1003      753 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003   111029 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/async_client.py
+-rw-rw-r--   0 root         (0)     1003   125201 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/client.py
+-rw-rw-r--   0 root         (0)     1003    26460 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15616 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    36520 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    37308 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   116775 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/
+-rw-rw-r--   0 root         (0)     1003     3893 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38294 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/datastream.py
+-rw-rw-r--   0 root         (0)     1003    40603 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/datastream_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/
+-rw-r--r--   0 root         (0)     1003     4683 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2747 2023-05-31 18:40:40.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-31 18:40:39.000000 google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-31 18:40:40.058371 google-cloud-datastream-1.6.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2980 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.054371 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   654798 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/test_datastream.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:40:40.058371 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   511456 2023-05-31 18:37:27.000000 google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/test_datastream.py
```

### Comparing `google-cloud-datastream-1.5.1/LICENSE` & `google-cloud-datastream-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/MANIFEST.in` & `google-cloud-datastream-1.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/PKG-INFO` & `google-cloud-datastream-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datastream
-Version: 1.5.1
+Version: 1.6.0
 Summary: Google Cloud Datastream API client library
 Home-page: https://github.com/googleapis/python-datastream
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-datastream-1.5.1/README.rst` & `google-cloud-datastream-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream/gapic_version.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/gapic_metadata.json` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/gapic_version.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/async_client.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/client.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/pagers.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/base.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/grpc.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/services/datastream/transports/rest.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/services/datastream/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/types/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/types/datastream.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/datastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1052,14 +1052,17 @@
             with the same request ID was received, and if
             so, will ignore the second request. This
             prevents clients from accidentally creating
             duplicate commitments.
             The request ID must be a valid UUID with the
             exception that zero UUID is not supported
             (00000000-0000-0000-0000-000000000000).
+        force (bool):
+            Optional. If set to true, will skip
+            validations.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     private_connection_id: str = proto.Field(
@@ -1071,14 +1074,18 @@
         number=3,
         message=datastream_resources.PrivateConnection,
     )
     request_id: str = proto.Field(
         proto.STRING,
         number=4,
     )
+    force: bool = proto.Field(
+        proto.BOOL,
+        number=6,
+    )
 
 
 class ListPrivateConnectionsRequest(proto.Message):
     r"""Request for listing private connections.
 
     Attributes:
         parent (str):
```

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1/types/datastream_resources.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1/types/datastream_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,20 @@
 
 
 class BigQueryProfile(proto.Message):
     r"""BigQuery warehouse profile."""
 
 
 class StaticServiceIpConnectivity(proto.Message):
-    r"""Static IP address connectivity."""
+    r"""Static IP address connectivity. Used when the source database
+    is configured to allow incoming connections from the Datastream
+    public IP addresses for the region specified in the connection
+    profile.
+
+    """
 
 
 class ForwardSshTunnelConnectivity(proto.Message):
     r"""Forward SSH Tunnel connectivity.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
@@ -788,23 +793,28 @@
     Attributes:
         include_objects (google.cloud.datastream_v1.types.OracleRdbms):
             Oracle objects to include in the stream.
         exclude_objects (google.cloud.datastream_v1.types.OracleRdbms):
             Oracle objects to exclude from the stream.
         max_concurrent_cdc_tasks (int):
             Maximum number of concurrent CDC tasks. The
-            number should be non negative. If not set (or
-            set to 0), the system's default value will be
+            number should be non-negative. If not set (or
+            set to 0), the system's default value is used.
+        max_concurrent_backfill_tasks (int):
+            Maximum number of concurrent backfill tasks.
+            The number should be non-negative. If not set
+            (or set to 0), the system's default value is
             used.
         drop_large_objects (google.cloud.datastream_v1.types.OracleSourceConfig.DropLargeObjects):
             Drop large object values.
 
             This field is a member of `oneof`_ ``large_objects_handling``.
         stream_large_objects (google.cloud.datastream_v1.types.OracleSourceConfig.StreamLargeObjects):
-            Stream large object values.
+            Stream large object values. NOTE: This
+            feature is currently experimental.
 
             This field is a member of `oneof`_ ``large_objects_handling``.
     """
 
     class DropLargeObjects(proto.Message):
         r"""Configuration to drop large object values."""
 
@@ -821,14 +831,18 @@
         number=2,
         message="OracleRdbms",
     )
     max_concurrent_cdc_tasks: int = proto.Field(
         proto.INT32,
         number=3,
     )
+    max_concurrent_backfill_tasks: int = proto.Field(
+        proto.INT32,
+        number=4,
+    )
     drop_large_objects: DropLargeObjects = proto.Field(
         proto.MESSAGE,
         number=100,
         oneof="large_objects_handling",
         message=DropLargeObjects,
     )
     stream_large_objects: StreamLargeObjects = proto.Field(
@@ -963,20 +977,26 @@
     Attributes:
         include_objects (google.cloud.datastream_v1.types.PostgresqlRdbms):
             PostgreSQL objects to include in the stream.
         exclude_objects (google.cloud.datastream_v1.types.PostgresqlRdbms):
             PostgreSQL objects to exclude from the
             stream.
         replication_slot (str):
-            Required. The name of the logical replication
-            slot that's configured with the pgoutput plugin.
+            Required. Immutable. The name of the logical
+            replication slot that's configured with the
+            pgoutput plugin.
         publication (str):
             Required. The name of the publication that includes the set
             of all tables that are defined in the stream's
             include_objects.
+        max_concurrent_backfill_tasks (int):
+            Maximum number of concurrent backfill tasks.
+            The number should be non negative. If not set
+            (or set to 0), the system's default value will
+            be used.
     """
 
     include_objects: "PostgresqlRdbms" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="PostgresqlRdbms",
     )
@@ -989,14 +1009,18 @@
         proto.STRING,
         number=3,
     )
     publication: str = proto.Field(
         proto.STRING,
         number=4,
     )
+    max_concurrent_backfill_tasks: int = proto.Field(
+        proto.INT32,
+        number=5,
+    )
 
 
 class MysqlColumn(proto.Message):
     r"""MySQL Column.
 
     Attributes:
         column (str):
@@ -1118,14 +1142,19 @@
         exclude_objects (google.cloud.datastream_v1.types.MysqlRdbms):
             MySQL objects to exclude from the stream.
         max_concurrent_cdc_tasks (int):
             Maximum number of concurrent CDC tasks. The
             number should be non negative. If not set (or
             set to 0), the system's default value will be
             used.
+        max_concurrent_backfill_tasks (int):
+            Maximum number of concurrent backfill tasks.
+            The number should be non negative. If not set
+            (or set to 0), the system's default value will
+            be used.
     """
 
     include_objects: "MysqlRdbms" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="MysqlRdbms",
     )
@@ -1134,14 +1163,18 @@
         number=2,
         message="MysqlRdbms",
     )
     max_concurrent_cdc_tasks: int = proto.Field(
         proto.INT32,
         number=3,
     )
+    max_concurrent_backfill_tasks: int = proto.Field(
+        proto.INT32,
+        number=4,
+    )
 
 
 class SourceConfig(proto.Message):
     r"""The configuration of the stream source.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
@@ -1264,15 +1297,16 @@
             data to.
         file_rotation_mb (int):
             The maximum file size to be saved in the
             bucket.
         file_rotation_interval (google.protobuf.duration_pb2.Duration):
             The maximum duration for which new events are
             added before a file is closed and a new file is
-            created.
+            created. Values within the range of 15-60
+            seconds are allowed.
         avro_file_format (google.cloud.datastream_v1.types.AvroFileFormat):
             AVRO file format configuration.
 
             This field is a member of `oneof`_ ``file_format``.
         json_file_format (google.cloud.datastream_v1.types.JsonFileFormat):
             JSON file format configuration.
 
@@ -1303,15 +1337,15 @@
         number=101,
         oneof="file_format",
         message="JsonFileFormat",
     )
 
 
 class BigQueryDestinationConfig(proto.Message):
-    r"""
+    r"""BigQuery destination configuration
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
@@ -1336,29 +1370,30 @@
     """
 
     class SingleTargetDataset(proto.Message):
         r"""A single target dataset to which all data will be streamed.
 
         Attributes:
             dataset_id (str):
-
+                The dataset ID of the target dataset.
         """
 
         dataset_id: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
     class SourceHierarchyDatasets(proto.Message):
         r"""Destination datasets are created so that hierarchy of the
         destination data objects matches the source hierarchy.
 
         Attributes:
             dataset_template (google.cloud.datastream_v1.types.BigQueryDestinationConfig.SourceHierarchyDatasets.DatasetTemplate):
-
+                The dataset template to use for dynamic
+                dataset creation.
         """
 
         class DatasetTemplate(proto.Message):
             r"""Dataset template used for dynamic dataset creation.
 
             Attributes:
                 location (str):
```

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/gapic_metadata.json` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/gapic_version.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/async_client.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/client.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/pagers.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/types/__init__.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/types/datastream.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/datastream.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google/cloud/datastream_v1alpha1/types/datastream_resources.py` & `google-cloud-datastream-1.6.0/google/cloud/datastream_v1alpha1/types/datastream_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/PKG-INFO` & `google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datastream
-Version: 1.5.1
+Version: 1.6.0
 Summary: Google Cloud Datastream API client library
 Home-page: https://github.com/googleapis/python-datastream
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-datastream-1.5.1/google_cloud_datastream.egg-info/SOURCES.txt` & `google-cloud-datastream-1.6.0/google_cloud_datastream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/setup.py` & `google-cloud-datastream-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/tests/__init__.py` & `google-cloud-datastream-1.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/tests/unit/__init__.py` & `google-cloud-datastream-1.6.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/tests/unit/gapic/__init__.py` & `google-cloud-datastream-1.6.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1/__init__.py` & `google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1/test_datastream.py` & `google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1/test_datastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -10417,14 +10417,15 @@
                                 }
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "max_concurrent_cdc_tasks": 2550,
+                "max_concurrent_backfill_tasks": 3076,
                 "drop_large_objects": {},
                 "stream_large_objects": {},
             },
             "mysql_source_config": {
                 "include_objects": {
                     "mysql_databases": [
                         {
@@ -10446,14 +10447,15 @@
                                 }
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "max_concurrent_cdc_tasks": 2550,
+                "max_concurrent_backfill_tasks": 3076,
             },
             "postgresql_source_config": {
                 "include_objects": {
                     "postgresql_schemas": [
                         {
                             "schema": "schema_value",
                             "postgresql_tables": [
@@ -10475,14 +10477,15 @@
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "replication_slot": "replication_slot_value",
                 "publication": "publication_value",
+                "max_concurrent_backfill_tasks": 3076,
             },
         },
         "destination_config": {
             "destination_connection_profile": "destination_connection_profile_value",
             "gcs_destination_config": {
                 "path": "path_value",
                 "file_rotation_mb": 1693,
@@ -10762,14 +10765,15 @@
                                 }
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "max_concurrent_cdc_tasks": 2550,
+                "max_concurrent_backfill_tasks": 3076,
                 "drop_large_objects": {},
                 "stream_large_objects": {},
             },
             "mysql_source_config": {
                 "include_objects": {
                     "mysql_databases": [
                         {
@@ -10791,14 +10795,15 @@
                                 }
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "max_concurrent_cdc_tasks": 2550,
+                "max_concurrent_backfill_tasks": 3076,
             },
             "postgresql_source_config": {
                 "include_objects": {
                     "postgresql_schemas": [
                         {
                             "schema": "schema_value",
                             "postgresql_tables": [
@@ -10820,14 +10825,15 @@
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "replication_slot": "replication_slot_value",
                 "publication": "publication_value",
+                "max_concurrent_backfill_tasks": 3076,
             },
         },
         "destination_config": {
             "destination_connection_profile": "destination_connection_profile_value",
             "gcs_destination_config": {
                 "path": "path_value",
                 "file_rotation_mb": 1693,
@@ -10992,14 +10998,15 @@
                                 }
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "max_concurrent_cdc_tasks": 2550,
+                "max_concurrent_backfill_tasks": 3076,
                 "drop_large_objects": {},
                 "stream_large_objects": {},
             },
             "mysql_source_config": {
                 "include_objects": {
                     "mysql_databases": [
                         {
@@ -11021,14 +11028,15 @@
                                 }
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "max_concurrent_cdc_tasks": 2550,
+                "max_concurrent_backfill_tasks": 3076,
             },
             "postgresql_source_config": {
                 "include_objects": {
                     "postgresql_schemas": [
                         {
                             "schema": "schema_value",
                             "postgresql_tables": [
@@ -11050,14 +11058,15 @@
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "replication_slot": "replication_slot_value",
                 "publication": "publication_value",
+                "max_concurrent_backfill_tasks": 3076,
             },
         },
         "destination_config": {
             "destination_connection_profile": "destination_connection_profile_value",
             "gcs_destination_config": {
                 "path": "path_value",
                 "file_rotation_mb": 1693,
@@ -11315,14 +11324,15 @@
                                 }
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "max_concurrent_cdc_tasks": 2550,
+                "max_concurrent_backfill_tasks": 3076,
                 "drop_large_objects": {},
                 "stream_large_objects": {},
             },
             "mysql_source_config": {
                 "include_objects": {
                     "mysql_databases": [
                         {
@@ -11344,14 +11354,15 @@
                                 }
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "max_concurrent_cdc_tasks": 2550,
+                "max_concurrent_backfill_tasks": 3076,
             },
             "postgresql_source_config": {
                 "include_objects": {
                     "postgresql_schemas": [
                         {
                             "schema": "schema_value",
                             "postgresql_tables": [
@@ -11373,14 +11384,15 @@
                             ],
                         }
                     ]
                 },
                 "exclude_objects": {},
                 "replication_slot": "replication_slot_value",
                 "publication": "publication_value",
+                "max_concurrent_backfill_tasks": 3076,
             },
         },
         "destination_config": {
             "destination_connection_profile": "destination_connection_profile_value",
             "gcs_destination_config": {
                 "path": "path_value",
                 "file_rotation_mb": 1693,
@@ -13575,14 +13587,15 @@
 
     unset_fields = transport_class(
         credentials=ga_credentials.AnonymousCredentials()
     ).create_private_connection._get_unset_required_fields(jsonified_request)
     # Check that path parameters and body parameters are not mixing in.
     assert not set(unset_fields) - set(
         (
+            "force",
             "private_connection_id",
             "request_id",
         )
     )
     jsonified_request.update(unset_fields)
 
     # verify required fields with non-default values are left alone
@@ -13641,14 +13654,15 @@
         credentials=ga_credentials.AnonymousCredentials
     )
 
     unset_fields = transport.create_private_connection._get_unset_required_fields({})
     assert set(unset_fields) == (
         set(
             (
+                "force",
                 "privateConnectionId",
                 "requestId",
             )
         )
         & set(
             (
                 "parent",
```

### Comparing `google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1alpha1/__init__.py` & `google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.5.1/tests/unit/gapic/datastream_v1alpha1/test_datastream.py` & `google-cloud-datastream-1.6.0/tests/unit/gapic/datastream_v1alpha1/test_datastream.py`

 * *Files identical despite different names*

