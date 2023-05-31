# Comparing `tmp/google-cloud-service-control-1.8.1.tar.gz` & `tmp/google-cloud-service-control-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-service-control-1.8.1.tar", last modified: Mon Mar 27 16:04:08 2023, max compression
+gzip compressed data, was "google-cloud-service-control-1.9.0.tar", last modified: Wed May 31 20:49:11 2023, max compression
```

## Comparing `google-cloud-service-control-1.8.1.tar` & `google-cloud-service-control-1.9.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.425022 google-cloud-service-control-1.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4856 2023-03-27 16:04:08.425022 google-cloud-service-control-1.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3916 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.409014 google-cloud-service-control-1.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.409014 google-cloud-service-control-1.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.413016 google-cloud-service-control-1.8.1/google/cloud/servicecontrol/
--rw-rw-r--   0 root         (0)     1003     2516 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.413016 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/
--rw-rw-r--   0 root         (0)     1003     1988 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2087 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.413016 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.413016 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    13162 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    21749 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.417018 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6171 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12601 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12816 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12263 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.417018 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    17616 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    26029 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.417018 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6933 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14785 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15029 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    16877 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.417018 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/
--rw-rw-r--   0 root         (0)     1003     1492 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6098 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/check_error.py
--rw-rw-r--   0 root         (0)     1003     8908 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/distribution.py
--rw-rw-r--   0 root         (0)     1003     4981 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/http_request.py
--rw-rw-r--   0 root         (0)     1003     8087 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/log_entry.py
--rw-rw-r--   0 root         (0)     1003     5091 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/metric_value.py
--rw-rw-r--   0 root         (0)     1003     7164 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/operation.py
--rw-rw-r--   0 root         (0)     1003    12336 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/quota_controller.py
--rw-rw-r--   0 root         (0)     1003    11573 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/service_controller.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.421020 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/
--rw-rw-r--   0 root         (0)     1003     1151 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     1316 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.421020 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.421020 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    18278 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    26691 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.421020 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6933 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15302 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15546 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17091 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.421020 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/types/
--rw-rw-r--   0 root         (0)     1003      849 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6889 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/types/service_controller.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.425022 google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/
--rw-r--r--   0 root         (0)     1003     4856 2023-03-27 16:04:08.000000 google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3777 2023-03-27 16:04:08.000000 google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:04:08.000000 google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:04:08.000000 google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:04:08.000000 google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 16:04:08.000000 google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:04:08.000000 google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:04:08.425022 google-cloud-service-control-1.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2958 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.425022 google-cloud-service-control-1.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.425022 google-cloud-service-control-1.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.425022 google-cloud-service-control-1.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.425022 google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    63977 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v1/test_quota_controller.py
--rw-rw-r--   0 root         (0)     1003    74966 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v1/test_service_controller.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:04:08.425022 google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    72840 2023-03-27 16:01:11.000000 google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v2/test_service_controller.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4856 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3916 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.300694 google-cloud-service-control-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.300694 google-cloud-service-control-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol/
+-rw-rw-r--   0 root         (0)     1003     2516 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/
+-rw-rw-r--   0 root         (0)     1003     1988 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2087 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/
+-rw-rw-r--   0 root         (0)     1003      773 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13162 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    21749 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6171 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12601 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12816 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12263 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/
+-rw-rw-r--   0 root         (0)     1003      781 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17616 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26029 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6933 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14785 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15029 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    16877 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1492 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6098 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/check_error.py
+-rw-rw-r--   0 root         (0)     1003     8908 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/distribution.py
+-rw-rw-r--   0 root         (0)     1003     4981 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/http_request.py
+-rw-rw-r--   0 root         (0)     1003     8087 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/log_entry.py
+-rw-rw-r--   0 root         (0)     1003     5091 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/metric_value.py
+-rw-rw-r--   0 root         (0)     1003     7164 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/operation.py
+-rw-rw-r--   0 root         (0)     1003    12336 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/quota_controller.py
+-rw-rw-r--   0 root         (0)     1003    11573 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/service_controller.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/
+-rw-rw-r--   0 root         (0)     1003     1197 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1316 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/
+-rw-rw-r--   0 root         (0)     1003      781 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18278 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26691 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6933 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15302 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15546 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17091 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/
+-rw-rw-r--   0 root         (0)     1003      895 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7316 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/service_controller.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/
+-rw-r--r--   0 root         (0)     1003     4856 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3777 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:49:11.316697 google-cloud-service-control-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2958 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    63977 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/test_quota_controller.py
+-rw-rw-r--   0 root         (0)     1003    74966 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/test_service_controller.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    72840 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/test_service_controller.py
```

### Comparing `google-cloud-service-control-1.8.1/LICENSE` & `google-cloud-service-control-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/MANIFEST.in` & `google-cloud-service-control-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/PKG-INFO` & `google-cloud-service-control-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-control
-Version: 1.8.1
+Version: 1.9.0
 Summary: Google Cloud Service Control API client library
 Home-page: https://github.com/googleapis/python-service-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-service-control-1.8.1/README.rst` & `google-cloud-service-control-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol/gapic_version.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/gapic_metadata.json` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/gapic_version.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/async_client.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/client.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/base.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc_asyncio.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/rest.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/async_client.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/client.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/base.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc_asyncio.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/services/service_controller/transports/rest.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/check_error.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/check_error.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/distribution.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/distribution.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/http_request.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/http_request.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/log_entry.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/log_entry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/metric_value.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/metric_value.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/operation.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/operation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/quota_controller.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/quota_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v1/types/service_controller.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/service_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 )
 from .types.service_controller import (
     CheckRequest,
     CheckResponse,
     ReportRequest,
     ReportResponse,
     ResourceInfo,
+    ResourceInfoList,
 )
 
 __all__ = (
     "ServiceControllerAsyncClient",
     "CheckRequest",
     "CheckResponse",
     "ReportRequest",
     "ReportResponse",
     "ResourceInfo",
+    "ResourceInfoList",
     "ServiceControllerClient",
 )
```

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/gapic_metadata.json` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/gapic_version.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/async_client.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/client.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/base.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc_asyncio.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/services/service_controller/transports/rest.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/types/__init__.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 #
 from .service_controller import (
     CheckRequest,
     CheckResponse,
     ReportRequest,
     ReportResponse,
     ResourceInfo,
+    ResourceInfoList,
 )
 
 __all__ = (
     "CheckRequest",
     "CheckResponse",
     "ReportRequest",
     "ReportResponse",
     "ResourceInfo",
+    "ResourceInfoList",
 )
```

### Comparing `google-cloud-service-control-1.8.1/google/cloud/servicecontrol_v2/types/service_controller.py` & `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/service_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     package="google.api.servicecontrol.v2",
     manifest={
         "CheckRequest",
         "ResourceInfo",
         "CheckResponse",
         "ReportRequest",
         "ReportResponse",
+        "ResourceInfoList",
     },
 )
 
 
 class CheckRequest(proto.Message):
     r"""Request message for the Check method.
 
@@ -209,8 +210,23 @@
     r"""Response message for the Report method.
     If the request contains any invalid data, the server returns an
     RPC error.
 
     """
 
 
+class ResourceInfoList(proto.Message):
+    r"""Message containing resource details in a batch mode.
+
+    Attributes:
+        resources (MutableSequence[google.cloud.servicecontrol_v2.types.ResourceInfo]):
+            The resource details.
+    """
+
+    resources: MutableSequence["ResourceInfo"] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message="ResourceInfo",
+    )
+
+
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/PKG-INFO` & `google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-control
-Version: 1.8.1
+Version: 1.9.0
 Summary: Google Cloud Service Control API client library
 Home-page: https://github.com/googleapis/python-service-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-service-control-1.8.1/google_cloud_service_control.egg-info/SOURCES.txt` & `google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/setup.py` & `google-cloud-service-control-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/tests/__init__.py` & `google-cloud-service-control-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/tests/unit/__init__.py` & `google-cloud-service-control-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/tests/unit/gapic/__init__.py` & `google-cloud-service-control-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v1/__init__.py` & `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v1/test_quota_controller.py` & `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/test_quota_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v1/test_service_controller.py` & `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/test_service_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v2/__init__.py` & `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.8.1/tests/unit/gapic/servicecontrol_v2/test_service_controller.py` & `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/test_service_controller.py`

 * *Files identical despite different names*

