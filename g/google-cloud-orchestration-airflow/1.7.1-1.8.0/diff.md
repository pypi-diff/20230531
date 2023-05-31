# Comparing `tmp/google-cloud-orchestration-airflow-1.7.1.tar.gz` & `tmp/google-cloud-orchestration-airflow-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-orchestration-airflow-1.7.1.tar", last modified: Mon Mar 27 16:03:47 2023, max compression
+gzip compressed data, was "google-cloud-orchestration-airflow-1.8.0.tar", last modified: Wed May 31 18:48:37 2023, max compression
```

## Comparing `google-cloud-orchestration-airflow-1.7.1.tar` & `google-cloud-orchestration-airflow-1.8.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:47.003403 google-cloud-orchestration-airflow-1.7.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4926 2023-03-27 16:03:47.003403 google-cloud-orchestration-airflow-1.7.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3968 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.983395 google-cloud-orchestration-airflow-1.7.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.983395 google-cloud-orchestration-airflow-1.7.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.983395 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.987397 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.987397 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service/
--rw-rw-r--   0 root         (0)     1003     3283 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.987397 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/
--rw-rw-r--   0 root         (0)     1003     2825 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4128 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.987397 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.991398 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/
--rw-rw-r--   0 root         (0)     1003      761 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/__init__.py
--rw-rw-r--   0 root         (0)     1003    55879 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/async_client.py
--rw-rw-r--   0 root         (0)     1003    65870 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/client.py
--rw-rw-r--   0 root         (0)     1003     6061 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.991398 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9692 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22079 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22552 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    52792 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.991398 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/__init__.py
--rw-rw-r--   0 root         (0)     1003    20236 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/async_client.py
--rw-rw-r--   0 root         (0)     1003    28753 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/client.py
--rw-rw-r--   0 root         (0)     1003     6127 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.991398 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6890 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14428 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14632 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22147 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.995400 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/types/
--rw-rw-r--   0 root         (0)     1003     2384 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    66125 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/types/environments.py
--rw-rw-r--   0 root         (0)     1003     4199 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/types/image_versions.py
--rw-rw-r--   0 root         (0)     1003     4321 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/types/operations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.995400 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/
--rw-rw-r--   0 root         (0)     1003     3148 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4885 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003      103 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.995400 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.995400 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/
--rw-rw-r--   0 root         (0)     1003      761 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/__init__.py
--rw-rw-r--   0 root         (0)     1003    65214 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/async_client.py
--rw-rw-r--   0 root         (0)     1003    75457 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/client.py
--rw-rw-r--   0 root         (0)     1003     6106 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.995400 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10575 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24495 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25040 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    63125 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.999401 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/__init__.py
--rw-rw-r--   0 root         (0)     1003    20285 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/async_client.py
--rw-rw-r--   0 root         (0)     1003    28802 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/client.py
--rw-rw-r--   0 root         (0)     1003     6172 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.999401 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6900 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14438 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14642 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22172 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.999401 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2702 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    75784 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/types/environments.py
--rw-rw-r--   0 root         (0)     1003     4210 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/types/image_versions.py
--rw-rw-r--   0 root         (0)     1003     4201 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/types/operations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.999401 google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/
--rw-r--r--   0 root         (0)     1003     4926 2023-03-27 16:03:46.000000 google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5387 2023-03-27 16:03:46.000000 google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:03:46.000000 google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       82 2023-03-27 16:03:46.000000 google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:03:46.000000 google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 16:03:46.000000 google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:03:46.000000 google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:03:47.003403 google-cloud-orchestration-airflow-1.7.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3092 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:46.999401 google-cloud-orchestration-airflow-1.7.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:47.003403 google-cloud-orchestration-airflow-1.7.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:47.003403 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:47.003403 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   200368 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1/test_environments.py
--rw-rw-r--   0 root         (0)     1003    98881 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1/test_image_versions.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:47.003403 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   223864 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1beta1/test_environments.py
--rw-rw-r--   0 root         (0)     1003    98916 2023-03-27 16:01:00.000000 google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1beta1/test_image_versions.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4926 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3968 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.139948 google-cloud-orchestration-airflow-1.8.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.139948 google-cloud-orchestration-airflow-1.8.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.139948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.139948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/
+-rw-rw-r--   0 root         (0)     1003     3283 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/
+-rw-rw-r--   0 root         (0)     1003     2825 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4128 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/
+-rw-rw-r--   0 root         (0)     1003      761 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/__init__.py
+-rw-rw-r--   0 root         (0)     1003    55879 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/async_client.py
+-rw-rw-r--   0 root         (0)     1003    65870 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/client.py
+-rw-rw-r--   0 root         (0)     1003     6061 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9692 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22079 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22552 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    52792 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/
+-rw-rw-r--   0 root         (0)     1003      765 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20236 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28753 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/client.py
+-rw-rw-r--   0 root         (0)     1003     6127 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6890 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14428 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14632 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22147 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2384 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    66667 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/environments.py
+-rw-rw-r--   0 root         (0)     1003     4199 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/image_versions.py
+-rw-rw-r--   0 root         (0)     1003     4321 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/operations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     3148 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4885 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003      103 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/
+-rw-rw-r--   0 root         (0)     1003      761 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/__init__.py
+-rw-rw-r--   0 root         (0)     1003    65214 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/async_client.py
+-rw-rw-r--   0 root         (0)     1003    75457 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/client.py
+-rw-rw-r--   0 root         (0)     1003     6106 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.151949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10575 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24495 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25040 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    63125 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.151949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/
+-rw-rw-r--   0 root         (0)     1003      765 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20285 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28802 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/client.py
+-rw-rw-r--   0 root         (0)     1003     6172 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.151949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6900 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14438 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14642 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22172 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.151949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2702 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    76326 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/environments.py
+-rw-rw-r--   0 root         (0)     1003     4210 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/image_versions.py
+-rw-rw-r--   0 root         (0)     1003     4201 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/operations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/
+-rw-r--r--   0 root         (0)     1003     4926 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5387 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       82 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3092 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   200608 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/test_environments.py
+-rw-rw-r--   0 root         (0)     1003    98881 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/test_image_versions.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   224104 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/test_environments.py
+-rw-rw-r--   0 root         (0)     1003    98916 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/test_image_versions.py
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/LICENSE` & `google-cloud-orchestration-airflow-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/MANIFEST.in` & `google-cloud-orchestration-airflow-1.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/PKG-INFO` & `google-cloud-orchestration-airflow-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-orchestration-airflow
-Version: 1.7.1
+Version: 1.8.0
 Summary: Google Cloud Orchestration Airflow API client library
 Home-page: https://github.com/googleapis/python-orchestration-airflow
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/README.rst` & `google-cloud-orchestration-airflow-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service/gapic_version.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/gapic_version.py`

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
-__version__ = "1.7.1"  # {x-release-please-version}
+__version__ = "1.8.0"  # {x-release-please-version}
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/gapic_metadata.json` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/gapic_version.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/gapic_version.py`

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
-__version__ = "1.7.1"  # {x-release-please-version}
+__version__ = "1.8.0"  # {x-release-please-version}
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/async_client.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/client.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/pagers.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/base.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc_asyncio.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/environments/transports/rest.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/async_client.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/client.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/pagers.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/base.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc_asyncio.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/rest.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/types/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/types/environments.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/environments.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,14 +539,21 @@
 
             This field is supported for Cloud Composer environments in
             versions composer-2.\ *.*-airflow-*.*.\* and newer.
         airflow_uri (str):
             Output only. The URI of the Apache Airflow Web UI hosted
             within this environment (see `Airflow web
             interface </composer/docs/how-to/accessing/airflow-web-interface>`__).
+        airflow_byoid_uri (str):
+            Output only. The 'bring your own identity' variant of the
+            URI of the Apache Airflow Web UI hosted within this
+            environment, to be accessed with external identities using
+            workforce identity federation (see `Access environments with
+            workforce identity
+            federation </composer/docs/composer-2/access-environments-with-workforce-identity-federation>`__).
         master_authorized_networks_config (google.cloud.orchestration.airflow.service_v1.types.MasterAuthorizedNetworksConfig):
             Optional. The configuration options for GKE
             cluster master authorized networks. By default
             master authorized networks feature is: - in case
             of private environment: enabled with no external
             networks allowlisted.
             - in case of public environment: disabled.
@@ -638,14 +645,18 @@
         number=16,
         enum=EnvironmentSize,
     )
     airflow_uri: str = proto.Field(
         proto.STRING,
         number=6,
     )
+    airflow_byoid_uri: str = proto.Field(
+        proto.STRING,
+        number=20,
+    )
     master_authorized_networks_config: "MasterAuthorizedNetworksConfig" = proto.Field(
         proto.MESSAGE,
         number=17,
         message="MasterAuthorizedNetworksConfig",
     )
     recovery_config: "RecoveryConfig" = proto.Field(
         proto.MESSAGE,
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/types/image_versions.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/image_versions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1/types/operations.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/operations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/gapic_metadata.json` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/gapic_version.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_version.py`

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
-__version__ = "1.7.1"  # {x-release-please-version}
+__version__ = "1.8.0"  # {x-release-please-version}
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/async_client.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/client.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/pagers.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/base.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc_asyncio.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/rest.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/async_client.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/client.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/pagers.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/base.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc_asyncio.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/rest.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/types/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/types/environments.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/environments.py`

 * *Files 1% similar despite different names*

```diff
@@ -665,14 +665,21 @@
 
             This field is supported for Cloud Composer environments in
             versions composer-1.\ *.*-airflow-*.*.*.
         airflow_uri (str):
             Output only. The URI of the Apache Airflow Web UI hosted
             within this environment (see `Airflow web
             interface </composer/docs/how-to/accessing/airflow-web-interface>`__).
+        airflow_byoid_uri (str):
+            Output only. The 'bring your own identity' variant of the
+            URI of the Apache Airflow Web UI hosted within this
+            environment, to be accessed with external identities using
+            workforce identity federation (see `Access environments with
+            workforce identity
+            federation </composer/docs/composer-2/access-environments-with-workforce-identity-federation>`__).
         encryption_config (google.cloud.orchestration.airflow.service_v1beta1.types.EncryptionConfig):
             Optional. The encryption options for the
             Cloud Composer environment and its dependencies.
             Cannot be updated.
         maintenance_window (google.cloud.orchestration.airflow.service_v1beta1.types.MaintenanceWindow):
             Optional. The maintenance window is the
             period when Cloud Composer components may
@@ -780,14 +787,18 @@
         number=11,
         message="WebServerConfig",
     )
     airflow_uri: str = proto.Field(
         proto.STRING,
         number=6,
     )
+    airflow_byoid_uri: str = proto.Field(
+        proto.STRING,
+        number=21,
+    )
     encryption_config: "EncryptionConfig" = proto.Field(
         proto.MESSAGE,
         number=12,
         message="EncryptionConfig",
     )
     maintenance_window: "MaintenanceWindow" = proto.Field(
         proto.MESSAGE,
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/types/image_versions.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/image_versions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google/cloud/orchestration/airflow/service_v1beta1/types/operations.py` & `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/operations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/PKG-INFO` & `google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-orchestration-airflow
-Version: 1.7.1
+Version: 1.8.0
 Summary: Google Cloud Orchestration Airflow API client library
 Home-page: https://github.com/googleapis/python-orchestration-airflow
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/google_cloud_orchestration_airflow.egg-info/SOURCES.txt` & `google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/setup.py` & `google-cloud-orchestration-airflow-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/tests/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/tests/unit/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1/test_environments.py` & `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/test_environments.py`

 * *Files 0% similar despite different names*

```diff
@@ -2512,14 +2512,15 @@
                     "storage_gb": 0.1053,
                     "min_count": 972,
                     "max_count": 974,
                 },
             },
             "environment_size": 1,
             "airflow_uri": "airflow_uri_value",
+            "airflow_byoid_uri": "airflow_byoid_uri_value",
             "master_authorized_networks_config": {
                 "enabled": True,
                 "cidr_blocks": [
                     {
                         "display_name": "display_name_value",
                         "cidr_block": "cidr_block_value",
                     }
@@ -2704,14 +2705,15 @@
                     "storage_gb": 0.1053,
                     "min_count": 972,
                     "max_count": 974,
                 },
             },
             "environment_size": 1,
             "airflow_uri": "airflow_uri_value",
+            "airflow_byoid_uri": "airflow_byoid_uri_value",
             "master_authorized_networks_config": {
                 "enabled": True,
                 "cidr_blocks": [
                     {
                         "display_name": "display_name_value",
                         "cidr_block": "cidr_block_value",
                     }
@@ -3326,14 +3328,15 @@
                     "storage_gb": 0.1053,
                     "min_count": 972,
                     "max_count": 974,
                 },
             },
             "environment_size": 1,
             "airflow_uri": "airflow_uri_value",
+            "airflow_byoid_uri": "airflow_byoid_uri_value",
             "master_authorized_networks_config": {
                 "enabled": True,
                 "cidr_blocks": [
                     {
                         "display_name": "display_name_value",
                         "cidr_block": "cidr_block_value",
                     }
@@ -3518,14 +3521,15 @@
                     "storage_gb": 0.1053,
                     "min_count": 972,
                     "max_count": 974,
                 },
             },
             "environment_size": 1,
             "airflow_uri": "airflow_uri_value",
+            "airflow_byoid_uri": "airflow_byoid_uri_value",
             "master_authorized_networks_config": {
                 "enabled": True,
                 "cidr_blocks": [
                     {
                         "display_name": "display_name_value",
                         "cidr_block": "cidr_block_value",
                     }
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1/test_image_versions.py` & `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/test_image_versions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1beta1/__init__.py` & `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1beta1/test_environments.py` & `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/test_environments.py`

 * *Files 0% similar despite different names*

```diff
@@ -2792,14 +2792,15 @@
                 "allowed_ip_ranges": [
                     {"value": "value_value", "description": "description_value"}
                 ]
             },
             "database_config": {"machine_type": "machine_type_value"},
             "web_server_config": {"machine_type": "machine_type_value"},
             "airflow_uri": "airflow_uri_value",
+            "airflow_byoid_uri": "airflow_byoid_uri_value",
             "encryption_config": {"kms_key_name": "kms_key_name_value"},
             "maintenance_window": {
                 "start_time": {"seconds": 751, "nanos": 543},
                 "end_time": {},
                 "recurrence": "recurrence_value",
             },
             "workloads_config": {
@@ -2987,14 +2988,15 @@
                 "allowed_ip_ranges": [
                     {"value": "value_value", "description": "description_value"}
                 ]
             },
             "database_config": {"machine_type": "machine_type_value"},
             "web_server_config": {"machine_type": "machine_type_value"},
             "airflow_uri": "airflow_uri_value",
+            "airflow_byoid_uri": "airflow_byoid_uri_value",
             "encryption_config": {"kms_key_name": "kms_key_name_value"},
             "maintenance_window": {
                 "start_time": {"seconds": 751, "nanos": 543},
                 "end_time": {},
                 "recurrence": "recurrence_value",
             },
             "workloads_config": {
@@ -3612,14 +3614,15 @@
                 "allowed_ip_ranges": [
                     {"value": "value_value", "description": "description_value"}
                 ]
             },
             "database_config": {"machine_type": "machine_type_value"},
             "web_server_config": {"machine_type": "machine_type_value"},
             "airflow_uri": "airflow_uri_value",
+            "airflow_byoid_uri": "airflow_byoid_uri_value",
             "encryption_config": {"kms_key_name": "kms_key_name_value"},
             "maintenance_window": {
                 "start_time": {"seconds": 751, "nanos": 543},
                 "end_time": {},
                 "recurrence": "recurrence_value",
             },
             "workloads_config": {
@@ -3889,14 +3892,15 @@
                 "allowed_ip_ranges": [
                     {"value": "value_value", "description": "description_value"}
                 ]
             },
             "database_config": {"machine_type": "machine_type_value"},
             "web_server_config": {"machine_type": "machine_type_value"},
             "airflow_uri": "airflow_uri_value",
+            "airflow_byoid_uri": "airflow_byoid_uri_value",
             "encryption_config": {"kms_key_name": "kms_key_name_value"},
             "maintenance_window": {
                 "start_time": {"seconds": 751, "nanos": 543},
                 "end_time": {},
                 "recurrence": "recurrence_value",
             },
             "workloads_config": {
```

### Comparing `google-cloud-orchestration-airflow-1.7.1/tests/unit/gapic/service_v1beta1/test_image_versions.py` & `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/test_image_versions.py`

 * *Files identical despite different names*

