# Comparing `tmp/google-cloud-webrisk-1.8.4.tar.gz` & `tmp/google-cloud-webrisk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-webrisk-1.8.4.tar", last modified: Mon Oct 10 16:15:10 2022, max compression
+gzip compressed data, was "google-cloud-webrisk-1.9.0.tar", last modified: Thu Dec 15 17:13:39 2022, max compression
```

## Comparing `google-cloud-webrisk-1.8.4.tar` & `google-cloud-webrisk-1.9.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4976 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4110 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.236479 google-cloud-webrisk-1.8.4/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.240478 google-cloud-webrisk-1.8.4/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.240478 google-cloud-webrisk-1.8.4/google/cloud/webrisk/
--rw-rw-r--   0 root         (0)     1003     1678 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk/__init__.py
--rw-rw-r--   0 root         (0)     1003       81 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.240478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/
--rw-rw-r--   0 root         (0)     1003     1533 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1553 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       81 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.240478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.240478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/
--rw-rw-r--   0 root         (0)     1003      769 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    29980 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37741 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.244478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8694 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16500 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16807 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.244478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/types/
--rw-rw-r--   0 root         (0)     1003     1378 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16799 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/types/webrisk.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.244478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1489 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1328 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       81 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.244478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.244478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/
--rw-rw-r--   0 root         (0)     1003      797 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    24182 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/async_client.py
--rw-rw-r--   0 root         (0)     1003    31663 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.244478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/
--rw-rw-r--   0 root         (0)     1003     1264 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8294 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14371 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14663 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.244478 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1284 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    15155 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/types/webrisk.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/
--rw-r--r--   0 root         (0)     1003     4976 2022-10-10 16:15:10.000000 google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2343 2022-10-10 16:15:10.000000 google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:15:10.000000 google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:15:10.000000 google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:15:10.000000 google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      232 2022-10-10 16:15:10.000000 google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:15:10.000000 google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/scripts/
--rw-rw-r--   0 root         (0)     1003     6155 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/scripts/fixup_webrisk_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6098 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/scripts/fixup_webrisk_v1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2990 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    79639 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1/test_web_risk_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:15:10.248477 google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    72569 2022-10-10 16:11:52.000000 google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1beta1/test_web_risk_service_v1_beta1.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.988054 google-cloud-webrisk-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4975 2022-12-15 17:13:39.988054 google-cloud-webrisk-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4110 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.972053 google-cloud-webrisk-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.972053 google-cloud-webrisk-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.976054 google-cloud-webrisk-1.9.0/google/cloud/webrisk/
+-rw-rw-r--   0 root         (0)     1003     1788 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.976054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/
+-rw-rw-r--   0 root         (0)     1003     1643 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1553 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.976054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.976054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/
+-rw-rw-r--   0 root         (0)     1003      769 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30704 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    38544 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.980054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8574 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16670 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16964 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.980054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1378 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17876 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/types/webrisk.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.980054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1599 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1328 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.980054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.980054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/
+-rw-rw-r--   0 root         (0)     1003      797 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24415 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/async_client.py
+-rw-rw-r--   0 root         (0)     1003    31986 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.980054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/
+-rw-rw-r--   0 root         (0)     1003     1264 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8178 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14471 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14750 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.984054 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1284 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15875 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/types/webrisk.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.984054 google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/
+-rw-r--r--   0 root         (0)     1003     4975 2022-12-15 17:13:39.000000 google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2389 2022-12-15 17:13:39.000000 google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 17:13:39.000000 google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-15 17:13:39.000000 google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 17:13:39.000000 google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      257 2022-12-15 17:13:39.000000 google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-15 17:13:39.000000 google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-15 17:13:39.988054 google-cloud-webrisk-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2861 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.984054 google-cloud-webrisk-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.984054 google-cloud-webrisk-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.984054 google-cloud-webrisk-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.984054 google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    79639 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1/test_web_risk_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 17:13:39.988054 google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    72569 2022-12-15 17:09:53.000000 google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1beta1/test_web_risk_service_v1_beta1.py
```

### Comparing `google-cloud-webrisk-1.8.4/LICENSE` & `google-cloud-webrisk-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/MANIFEST.in` & `google-cloud-webrisk-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/PKG-INFO` & `google-cloud-webrisk-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-webrisk
-Version: 1.8.4
-Summary: Google Cloud Web Risk API client library
+Version: 1.9.0
+Summary: Google Cloud Webrisk API client library
 Home-page: https://github.com/googleapis/python-webrisk
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-webrisk-1.8.4/README.rst` & `google-cloud-webrisk-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.webrisk import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from google.cloud.webrisk_v1.services.web_risk_service.async_client import (
     WebRiskServiceAsyncClient,
 )
 from google.cloud.webrisk_v1.services.web_risk_service.client import (
     WebRiskServiceClient,
 )
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,46 +9,49 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.webrisk import gapic_version as package_version
 
-from .services.web_risk_service import WebRiskServiceAsyncClient, WebRiskServiceClient
+__version__ = package_version.__version__
+
+
+from .services.web_risk_service_v1_beta1 import (
+    WebRiskServiceV1Beta1AsyncClient,
+    WebRiskServiceV1Beta1Client,
+)
 from .types.webrisk import (
     CompressionType,
     ComputeThreatListDiffRequest,
     ComputeThreatListDiffResponse,
-    CreateSubmissionRequest,
     RawHashes,
     RawIndices,
     RiceDeltaEncoding,
     SearchHashesRequest,
     SearchHashesResponse,
     SearchUrisRequest,
     SearchUrisResponse,
-    Submission,
     ThreatEntryAdditions,
     ThreatEntryRemovals,
     ThreatType,
 )
 
 __all__ = (
-    "WebRiskServiceAsyncClient",
+    "WebRiskServiceV1Beta1AsyncClient",
     "CompressionType",
     "ComputeThreatListDiffRequest",
     "ComputeThreatListDiffResponse",
-    "CreateSubmissionRequest",
     "RawHashes",
     "RawIndices",
     "RiceDeltaEncoding",
     "SearchHashesRequest",
     "SearchHashesResponse",
     "SearchUrisRequest",
     "SearchUrisResponse",
-    "Submission",
     "ThreatEntryAdditions",
     "ThreatEntryRemovals",
     "ThreatType",
-    "WebRiskServiceClient",
+    "WebRiskServiceV1Beta1Client",
 )
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/gapic_metadata.json` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/async_client.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.webrisk_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import timestamp_pb2  # type: ignore
@@ -156,17 +167,17 @@
     get_transport_class = functools.partial(
         type(WebRiskServiceClient).get_transport_class, type(WebRiskServiceClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, WebRiskServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the web risk service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -202,21 +213,21 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def compute_threat_list_diff(
         self,
-        request: Union[webrisk.ComputeThreatListDiffRequest, dict] = None,
+        request: Optional[Union[webrisk.ComputeThreatListDiffRequest, dict]] = None,
         *,
-        threat_type: webrisk.ThreatType = None,
-        version_token: bytes = None,
-        constraints: webrisk.ComputeThreatListDiffRequest.Constraints = None,
+        threat_type: Optional[webrisk.ThreatType] = None,
+        version_token: Optional[bytes] = None,
+        constraints: Optional[webrisk.ComputeThreatListDiffRequest.Constraints] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.ComputeThreatListDiffResponse:
         r"""Gets the most recent threat list diffs. These diffs
         should be applied to a local database of hashes to keep
         it up-to-date. If the local database is empty or
         excessively out-of-date, a complete snapshot of the
         database will be returned. This Method only updates a
@@ -237,30 +248,32 @@
 
             async def sample_compute_threat_list_diff():
                 # Create a client
                 client = webrisk_v1.WebRiskServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = webrisk_v1.ComputeThreatListDiffRequest(
-                    threat_type="UNWANTED_SOFTWARE",
+                    threat_type="SOCIAL_ENGINEERING_EXTENDED_COVERAGE",
                 )
 
                 # Make the request
                 response = await client.compute_threat_list_diff(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.webrisk_v1.types.ComputeThreatListDiffRequest, dict]):
+            request (Optional[Union[google.cloud.webrisk_v1.types.ComputeThreatListDiffRequest, dict]]):
                 The request object. Describes an API diff request.
             threat_type (:class:`google.cloud.webrisk_v1.types.ThreatType`):
                 Required. The threat list to update.
                 Only a single ThreatType should be
-                specified.
+                specified per request. If you want to
+                handle multiple ThreatTypes, you must
+                make one request per ThreatType.
 
                 This corresponds to the ``threat_type`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             version_token (:class:`bytes`):
                 The current version token of the
                 client for the requested list (the
@@ -340,20 +353,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def search_uris(
         self,
-        request: Union[webrisk.SearchUrisRequest, dict] = None,
+        request: Optional[Union[webrisk.SearchUrisRequest, dict]] = None,
         *,
-        uri: str = None,
-        threat_types: Sequence[webrisk.ThreatType] = None,
+        uri: Optional[str] = None,
+        threat_types: Optional[MutableSequence[webrisk.ThreatType]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.SearchUrisResponse:
         r"""This method is used to check whether a URI is on a
         given threatList. Multiple threatLists may be searched
         in a single query. The response will list all requested
         threatLists the URI was found to match. If the URI is
         not found on any of the requested ThreatList an empty
@@ -373,35 +386,35 @@
             async def sample_search_uris():
                 # Create a client
                 client = webrisk_v1.WebRiskServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = webrisk_v1.SearchUrisRequest(
                     uri="uri_value",
-                    threat_types="UNWANTED_SOFTWARE",
+                    threat_types=['SOCIAL_ENGINEERING_EXTENDED_COVERAGE'],
                 )
 
                 # Make the request
                 response = await client.search_uris(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.webrisk_v1.types.SearchUrisRequest, dict]):
+            request (Optional[Union[google.cloud.webrisk_v1.types.SearchUrisRequest, dict]]):
                 The request object. Request to check URI entries against
                 threatLists.
             uri (:class:`str`):
                 Required. The URI to be checked for
                 matches.
 
                 This corresponds to the ``uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            threat_types (:class:`Sequence[google.cloud.webrisk_v1.types.ThreatType]`):
+            threat_types (:class:`MutableSequence[google.cloud.webrisk_v1.types.ThreatType]`):
                 Required. The ThreatLists to search
                 in. Multiple ThreatLists may be
                 specified.
 
                 This corresponds to the ``threat_types`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -461,20 +474,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def search_hashes(
         self,
-        request: Union[webrisk.SearchHashesRequest, dict] = None,
+        request: Optional[Union[webrisk.SearchHashesRequest, dict]] = None,
         *,
-        hash_prefix: bytes = None,
-        threat_types: Sequence[webrisk.ThreatType] = None,
+        hash_prefix: Optional[bytes] = None,
+        threat_types: Optional[MutableSequence[webrisk.ThreatType]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.SearchHashesResponse:
         r"""Gets the full hashes that match the requested hash
         prefix. This is used after a hash prefix is looked up in
         a threatList and there is a match. The client side
         threatList only holds partial hashes so the client must
         query this method to determine if there is a full hash
@@ -493,37 +506,40 @@
 
             async def sample_search_hashes():
                 # Create a client
                 client = webrisk_v1.WebRiskServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = webrisk_v1.SearchHashesRequest(
-                    threat_types="UNWANTED_SOFTWARE",
+                    threat_types=['SOCIAL_ENGINEERING_EXTENDED_COVERAGE'],
                 )
 
                 # Make the request
                 response = await client.search_hashes(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.webrisk_v1.types.SearchHashesRequest, dict]):
+            request (Optional[Union[google.cloud.webrisk_v1.types.SearchHashesRequest, dict]]):
                 The request object. Request to return full hashes
                 matched by the provided hash prefixes.
             hash_prefix (:class:`bytes`):
                 A hash prefix, consisting of the most
                 significant 4-32 bytes of a SHA256 hash.
                 For JSON requests, this field is
-                base64-encoded.
+                base64-encoded. Note that if this
+                parameter is provided by a URI, it must
+                be encoded using the web safe base64
+                variant (RFC 4648).
 
                 This corresponds to the ``hash_prefix`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            threat_types (:class:`Sequence[google.cloud.webrisk_v1.types.ThreatType]`):
+            threat_types (:class:`MutableSequence[google.cloud.webrisk_v1.types.ThreatType]`):
                 Required. The ThreatLists to search
                 in. Multiple ThreatLists may be
                 specified.
 
                 This corresponds to the ``threat_types`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -583,30 +599,31 @@
         )
 
         # Done; return the response.
         return response
 
     async def create_submission(
         self,
-        request: Union[webrisk.CreateSubmissionRequest, dict] = None,
+        request: Optional[Union[webrisk.CreateSubmissionRequest, dict]] = None,
         *,
-        parent: str = None,
-        submission: webrisk.Submission = None,
+        parent: Optional[str] = None,
+        submission: Optional[webrisk.Submission] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.Submission:
         r"""Creates a Submission of a URI suspected of containing phishing
         content to be reviewed. If the result verifies the existence of
         malicious phishing content, the site will be added to the
         `Google's Social Engineering
         lists <https://support.google.com/webmasters/answer/6350487/>`__
         in order to protect users that could get exposed to this threat
-        in the future. Only projects with CREATE_SUBMISSION_USERS
-        visibility can use this method.
+        in the future. Only allowlisted projects can use this method
+        during Early Access. Please reach out to Sales or your customer
+        engineer to obtain access.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -631,15 +648,15 @@
                 # Make the request
                 response = await client.create_submission(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.webrisk_v1.types.CreateSubmissionRequest, dict]):
+            request (Optional[Union[google.cloud.webrisk_v1.types.CreateSubmissionRequest, dict]]):
                 The request object. Request to send a potentially phishy
                 URI to WebRisk.
             parent (:class:`str`):
                 Required. The name of the project that is making the
                 submission. This string is in the format
                 "projects/{project_number}".
 
@@ -659,15 +676,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.webrisk_v1.types.Submission:
                 Wraps a URI that might be displaying
-                phishing content.
+                malicious content.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, submission])
         if request is not None and has_flattened_params:
@@ -685,15 +702,15 @@
         if submission is not None:
             request.submission = submission
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.create_submission,
-            default_timeout=60.0,
+            default_timeout=600.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
@@ -713,18 +730,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-webrisk",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("WebRiskServiceAsyncClient",)
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/client.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.webrisk_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import timestamp_pb2  # type: ignore
@@ -55,15 +67,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[WebRiskServiceTransport]]
     _transport_registry["grpc"] = WebRiskServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = WebRiskServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[WebRiskServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -310,30 +322,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, WebRiskServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, WebRiskServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the web risk service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, WebRiskServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -355,14 +367,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -407,21 +420,21 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def compute_threat_list_diff(
         self,
-        request: Union[webrisk.ComputeThreatListDiffRequest, dict] = None,
+        request: Optional[Union[webrisk.ComputeThreatListDiffRequest, dict]] = None,
         *,
-        threat_type: webrisk.ThreatType = None,
-        version_token: bytes = None,
-        constraints: webrisk.ComputeThreatListDiffRequest.Constraints = None,
+        threat_type: Optional[webrisk.ThreatType] = None,
+        version_token: Optional[bytes] = None,
+        constraints: Optional[webrisk.ComputeThreatListDiffRequest.Constraints] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.ComputeThreatListDiffResponse:
         r"""Gets the most recent threat list diffs. These diffs
         should be applied to a local database of hashes to keep
         it up-to-date. If the local database is empty or
         excessively out-of-date, a complete snapshot of the
         database will be returned. This Method only updates a
@@ -442,30 +455,32 @@
 
             def sample_compute_threat_list_diff():
                 # Create a client
                 client = webrisk_v1.WebRiskServiceClient()
 
                 # Initialize request argument(s)
                 request = webrisk_v1.ComputeThreatListDiffRequest(
-                    threat_type="UNWANTED_SOFTWARE",
+                    threat_type="SOCIAL_ENGINEERING_EXTENDED_COVERAGE",
                 )
 
                 # Make the request
                 response = client.compute_threat_list_diff(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.webrisk_v1.types.ComputeThreatListDiffRequest, dict]):
                 The request object. Describes an API diff request.
             threat_type (google.cloud.webrisk_v1.types.ThreatType):
                 Required. The threat list to update.
                 Only a single ThreatType should be
-                specified.
+                specified per request. If you want to
+                handle multiple ThreatTypes, you must
+                make one request per ThreatType.
 
                 This corresponds to the ``threat_type`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             version_token (bytes):
                 The current version token of the
                 client for the requested list (the
@@ -535,20 +550,20 @@
         )
 
         # Done; return the response.
         return response
 
     def search_uris(
         self,
-        request: Union[webrisk.SearchUrisRequest, dict] = None,
+        request: Optional[Union[webrisk.SearchUrisRequest, dict]] = None,
         *,
-        uri: str = None,
-        threat_types: Sequence[webrisk.ThreatType] = None,
+        uri: Optional[str] = None,
+        threat_types: Optional[MutableSequence[webrisk.ThreatType]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.SearchUrisResponse:
         r"""This method is used to check whether a URI is on a
         given threatList. Multiple threatLists may be searched
         in a single query. The response will list all requested
         threatLists the URI was found to match. If the URI is
         not found on any of the requested ThreatList an empty
@@ -568,15 +583,15 @@
             def sample_search_uris():
                 # Create a client
                 client = webrisk_v1.WebRiskServiceClient()
 
                 # Initialize request argument(s)
                 request = webrisk_v1.SearchUrisRequest(
                     uri="uri_value",
-                    threat_types="UNWANTED_SOFTWARE",
+                    threat_types=['SOCIAL_ENGINEERING_EXTENDED_COVERAGE'],
                 )
 
                 # Make the request
                 response = client.search_uris(request=request)
 
                 # Handle the response
                 print(response)
@@ -588,15 +603,15 @@
             uri (str):
                 Required. The URI to be checked for
                 matches.
 
                 This corresponds to the ``uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            threat_types (Sequence[google.cloud.webrisk_v1.types.ThreatType]):
+            threat_types (MutableSequence[google.cloud.webrisk_v1.types.ThreatType]):
                 Required. The ThreatLists to search
                 in. Multiple ThreatLists may be
                 specified.
 
                 This corresponds to the ``threat_types`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -646,20 +661,20 @@
         )
 
         # Done; return the response.
         return response
 
     def search_hashes(
         self,
-        request: Union[webrisk.SearchHashesRequest, dict] = None,
+        request: Optional[Union[webrisk.SearchHashesRequest, dict]] = None,
         *,
-        hash_prefix: bytes = None,
-        threat_types: Sequence[webrisk.ThreatType] = None,
+        hash_prefix: Optional[bytes] = None,
+        threat_types: Optional[MutableSequence[webrisk.ThreatType]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.SearchHashesResponse:
         r"""Gets the full hashes that match the requested hash
         prefix. This is used after a hash prefix is looked up in
         a threatList and there is a match. The client side
         threatList only holds partial hashes so the client must
         query this method to determine if there is a full hash
@@ -678,15 +693,15 @@
 
             def sample_search_hashes():
                 # Create a client
                 client = webrisk_v1.WebRiskServiceClient()
 
                 # Initialize request argument(s)
                 request = webrisk_v1.SearchHashesRequest(
-                    threat_types="UNWANTED_SOFTWARE",
+                    threat_types=['SOCIAL_ENGINEERING_EXTENDED_COVERAGE'],
                 )
 
                 # Make the request
                 response = client.search_hashes(request=request)
 
                 # Handle the response
                 print(response)
@@ -695,20 +710,23 @@
             request (Union[google.cloud.webrisk_v1.types.SearchHashesRequest, dict]):
                 The request object. Request to return full hashes
                 matched by the provided hash prefixes.
             hash_prefix (bytes):
                 A hash prefix, consisting of the most
                 significant 4-32 bytes of a SHA256 hash.
                 For JSON requests, this field is
-                base64-encoded.
+                base64-encoded. Note that if this
+                parameter is provided by a URI, it must
+                be encoded using the web safe base64
+                variant (RFC 4648).
 
                 This corresponds to the ``hash_prefix`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            threat_types (Sequence[google.cloud.webrisk_v1.types.ThreatType]):
+            threat_types (MutableSequence[google.cloud.webrisk_v1.types.ThreatType]):
                 Required. The ThreatLists to search
                 in. Multiple ThreatLists may be
                 specified.
 
                 This corresponds to the ``threat_types`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -758,30 +776,31 @@
         )
 
         # Done; return the response.
         return response
 
     def create_submission(
         self,
-        request: Union[webrisk.CreateSubmissionRequest, dict] = None,
+        request: Optional[Union[webrisk.CreateSubmissionRequest, dict]] = None,
         *,
-        parent: str = None,
-        submission: webrisk.Submission = None,
+        parent: Optional[str] = None,
+        submission: Optional[webrisk.Submission] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.Submission:
         r"""Creates a Submission of a URI suspected of containing phishing
         content to be reviewed. If the result verifies the existence of
         malicious phishing content, the site will be added to the
         `Google's Social Engineering
         lists <https://support.google.com/webmasters/answer/6350487/>`__
         in order to protect users that could get exposed to this threat
-        in the future. Only projects with CREATE_SUBMISSION_USERS
-        visibility can use this method.
+        in the future. Only allowlisted projects can use this method
+        during Early Access. Please reach out to Sales or your customer
+        engineer to obtain access.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -834,15 +853,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.webrisk_v1.types.Submission:
                 Wraps a URI that might be displaying
-                phishing content.
+                malicious content.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, submission])
         if request is not None and has_flattened_params:
@@ -895,18 +914,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-webrisk",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("WebRiskServiceClient",)
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/transports/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/transports/base.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,40 +19,35 @@
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
+from google.cloud.webrisk_v1 import gapic_version as package_version
 from google.cloud.webrisk_v1.types import webrisk
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-webrisk",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class WebRiskServiceTransport(abc.ABC):
     """Abstract transport class for WebRiskService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "webrisk.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
@@ -170,15 +165,15 @@
                     deadline=600.0,
                 ),
                 default_timeout=600.0,
                 client_info=client_info,
             ),
             self.create_submission: gapic_v1.method.wrap_method(
                 self.create_submission,
-                default_timeout=60.0,
+                default_timeout=600.0,
                 client_info=client_info,
             ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/transports/grpc.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "webrisk.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -177,16 +177,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "webrisk.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
@@ -334,16 +334,17 @@
 
         Creates a Submission of a URI suspected of containing phishing
         content to be reviewed. If the result verifies the existence of
         malicious phishing content, the site will be added to the
         `Google's Social Engineering
         lists <https://support.google.com/webmasters/answer/6350487/>`__
         in order to protect users that could get exposed to this threat
-        in the future. Only projects with CREATE_SUBMISSION_USERS
-        visibility can use this method.
+        in the future. Only allowlisted projects can use this method
+        during Early Access. Please reach out to Sales or your customer
+        engineer to obtain access.
 
         Returns:
             Callable[[~.CreateSubmissionRequest],
                     ~.Submission]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/services/web_risk_service/transports/grpc_asyncio.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/services/web_risk_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "webrisk.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -88,23 +88,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "webrisk.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
@@ -340,16 +340,17 @@
 
         Creates a Submission of a URI suspected of containing phishing
         content to be reviewed. If the result verifies the existence of
         malicious phishing content, the site will be added to the
         `Google's Social Engineering
         lists <https://support.google.com/webmasters/answer/6350487/>`__
         in order to protect users that could get exposed to this threat
-        in the future. Only projects with CREATE_SUBMISSION_USERS
-        visibility can use this method.
+        in the future. Only allowlisted projects can use this method
+        during Early Access. Please reach out to Sales or your customer
+        engineer to obtain access.
 
         Returns:
             Callable[[~.CreateSubmissionRequest],
                     Awaitable[~.Submission]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/types/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1/types/webrisk.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/types/webrisk.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.webrisk.v1",
     manifest={
         "ThreatType",
@@ -35,21 +37,22 @@
         "Submission",
         "CreateSubmissionRequest",
     },
 )
 
 
 class ThreatType(proto.Enum):
-    r"""The type of threat. This maps dirrectly to the threat list a
+    r"""The type of threat. This maps directly to the threat list a
     threat may belong to.
     """
     THREAT_TYPE_UNSPECIFIED = 0
     MALWARE = 1
     SOCIAL_ENGINEERING = 2
     UNWANTED_SOFTWARE = 3
+    SOCIAL_ENGINEERING_EXTENDED_COVERAGE = 4
 
 
 class CompressionType(proto.Enum):
     r"""The ways in which threat entry sets can be compressed."""
     COMPRESSION_TYPE_UNSPECIFIED = 0
     RAW = 1
     RICE = 2
@@ -57,15 +60,18 @@
 
 class ComputeThreatListDiffRequest(proto.Message):
     r"""Describes an API diff request.
 
     Attributes:
         threat_type (google.cloud.webrisk_v1.types.ThreatType):
             Required. The threat list to update. Only a
-            single ThreatType should be specified.
+            single ThreatType should be specified per
+            request. If you want to handle multiple
+            ThreatTypes, you must make one request per
+            ThreatType.
         version_token (bytes):
             The current version token of the client for
             the requested list (the client version that was
             received from the last successful diff). If the
             client does not have a version token (this is
             the first time calling ComputeThreatListDiff),
             this may be left empty and a full database
@@ -85,43 +91,45 @@
                 of 2 between 2\ **10 and 2**\ 20. If zero, no diff size
                 limit is set.
             max_database_entries (int):
                 Sets the maximum number of entries that the client is
                 willing to have in the local database. This should be a
                 power of 2 between 2\ **10 and 2**\ 20. If zero, no database
                 size limit is set.
-            supported_compressions (Sequence[google.cloud.webrisk_v1.types.CompressionType]):
+            supported_compressions (MutableSequence[google.cloud.webrisk_v1.types.CompressionType]):
                 The compression types supported by the
                 client.
         """
 
-        max_diff_entries = proto.Field(
+        max_diff_entries: int = proto.Field(
             proto.INT32,
             number=1,
         )
-        max_database_entries = proto.Field(
+        max_database_entries: int = proto.Field(
             proto.INT32,
             number=2,
         )
-        supported_compressions = proto.RepeatedField(
+        supported_compressions: MutableSequence[
+            "CompressionType"
+        ] = proto.RepeatedField(
             proto.ENUM,
             number=3,
             enum="CompressionType",
         )
 
-    threat_type = proto.Field(
+    threat_type: "ThreatType" = proto.Field(
         proto.ENUM,
         number=1,
         enum="ThreatType",
     )
-    version_token = proto.Field(
+    version_token: bytes = proto.Field(
         proto.BYTES,
         number=2,
     )
-    constraints = proto.Field(
+    constraints: Constraints = proto.Field(
         proto.MESSAGE,
         number=3,
         message=Constraints,
     )
 
 
 class ComputeThreatListDiffResponse(proto.Message):
@@ -171,105 +179,105 @@
         Attributes:
             sha256 (bytes):
                 The SHA256 hash of the client state; that is,
                 of the sorted list of all hashes present in the
                 database.
         """
 
-        sha256 = proto.Field(
+        sha256: bytes = proto.Field(
             proto.BYTES,
             number=1,
         )
 
-    response_type = proto.Field(
+    response_type: ResponseType = proto.Field(
         proto.ENUM,
         number=4,
         enum=ResponseType,
     )
-    additions = proto.Field(
+    additions: "ThreatEntryAdditions" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="ThreatEntryAdditions",
     )
-    removals = proto.Field(
+    removals: "ThreatEntryRemovals" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="ThreatEntryRemovals",
     )
-    new_version_token = proto.Field(
+    new_version_token: bytes = proto.Field(
         proto.BYTES,
         number=7,
     )
-    checksum = proto.Field(
+    checksum: Checksum = proto.Field(
         proto.MESSAGE,
         number=8,
         message=Checksum,
     )
-    recommended_next_diff = proto.Field(
+    recommended_next_diff: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class SearchUrisRequest(proto.Message):
     r"""Request to check URI entries against threatLists.
 
     Attributes:
         uri (str):
             Required. The URI to be checked for matches.
-        threat_types (Sequence[google.cloud.webrisk_v1.types.ThreatType]):
+        threat_types (MutableSequence[google.cloud.webrisk_v1.types.ThreatType]):
             Required. The ThreatLists to search in.
             Multiple ThreatLists may be specified.
     """
 
-    uri = proto.Field(
+    uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    threat_types = proto.RepeatedField(
+    threat_types: MutableSequence["ThreatType"] = proto.RepeatedField(
         proto.ENUM,
         number=2,
         enum="ThreatType",
     )
 
 
 class SearchUrisResponse(proto.Message):
     r"""
 
     Attributes:
         threat (google.cloud.webrisk_v1.types.SearchUrisResponse.ThreatUri):
-            The threat list matches. This may be empty if
-            the URI is on no list.
+            The threat list matches. This might be empty
+            if the URI is on no list.
     """
 
     class ThreatUri(proto.Message):
         r"""Contains threat information on a matching uri.
 
         Attributes:
-            threat_types (Sequence[google.cloud.webrisk_v1.types.ThreatType]):
+            threat_types (MutableSequence[google.cloud.webrisk_v1.types.ThreatType]):
                 The ThreatList this threat belongs to.
             expire_time (google.protobuf.timestamp_pb2.Timestamp):
                 The cache lifetime for the returned match.
                 Clients must not cache this response past this
                 timestamp to avoid false positives.
         """
 
-        threat_types = proto.RepeatedField(
+        threat_types: MutableSequence["ThreatType"] = proto.RepeatedField(
             proto.ENUM,
             number=1,
             enum="ThreatType",
         )
-        expire_time = proto.Field(
+        expire_time: timestamp_pb2.Timestamp = proto.Field(
             proto.MESSAGE,
             number=2,
             message=timestamp_pb2.Timestamp,
         )
 
-    threat = proto.Field(
+    threat: ThreatUri = proto.Field(
         proto.MESSAGE,
         number=1,
         message=ThreatUri,
     )
 
 
 class SearchHashesRequest(proto.Message):
@@ -277,110 +285,113 @@
     prefixes.
 
     Attributes:
         hash_prefix (bytes):
             A hash prefix, consisting of the most
             significant 4-32 bytes of a SHA256 hash. For
             JSON requests, this field is base64-encoded.
-        threat_types (Sequence[google.cloud.webrisk_v1.types.ThreatType]):
+            Note that if this parameter is provided by a
+            URI, it must be encoded using the web safe
+            base64 variant (RFC 4648).
+        threat_types (MutableSequence[google.cloud.webrisk_v1.types.ThreatType]):
             Required. The ThreatLists to search in.
             Multiple ThreatLists may be specified.
     """
 
-    hash_prefix = proto.Field(
+    hash_prefix: bytes = proto.Field(
         proto.BYTES,
         number=1,
     )
-    threat_types = proto.RepeatedField(
+    threat_types: MutableSequence["ThreatType"] = proto.RepeatedField(
         proto.ENUM,
         number=2,
         enum="ThreatType",
     )
 
 
 class SearchHashesResponse(proto.Message):
     r"""
 
     Attributes:
-        threats (Sequence[google.cloud.webrisk_v1.types.SearchHashesResponse.ThreatHash]):
+        threats (MutableSequence[google.cloud.webrisk_v1.types.SearchHashesResponse.ThreatHash]):
             The full hashes that matched the requested
             prefixes. The hash will be populated in the key.
         negative_expire_time (google.protobuf.timestamp_pb2.Timestamp):
             For requested entities that did not match the
             threat list, how long to cache the response
             until.
     """
 
     class ThreatHash(proto.Message):
         r"""Contains threat information on a matching hash.
 
         Attributes:
-            threat_types (Sequence[google.cloud.webrisk_v1.types.ThreatType]):
+            threat_types (MutableSequence[google.cloud.webrisk_v1.types.ThreatType]):
                 The ThreatList this threat belongs to.
                 This must contain at least one entry.
             hash_ (bytes):
                 A 32 byte SHA256 hash. This field is in
                 binary format. For JSON requests, hashes are
                 base64-encoded.
             expire_time (google.protobuf.timestamp_pb2.Timestamp):
                 The cache lifetime for the returned match.
                 Clients must not cache this response past this
                 timestamp to avoid false positives.
         """
 
-        threat_types = proto.RepeatedField(
+        threat_types: MutableSequence["ThreatType"] = proto.RepeatedField(
             proto.ENUM,
             number=1,
             enum="ThreatType",
         )
-        hash_ = proto.Field(
+        hash_: bytes = proto.Field(
             proto.BYTES,
             number=2,
         )
-        expire_time = proto.Field(
+        expire_time: timestamp_pb2.Timestamp = proto.Field(
             proto.MESSAGE,
             number=3,
             message=timestamp_pb2.Timestamp,
         )
 
-    threats = proto.RepeatedField(
+    threats: MutableSequence[ThreatHash] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=ThreatHash,
     )
-    negative_expire_time = proto.Field(
+    negative_expire_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class ThreatEntryAdditions(proto.Message):
     r"""Contains the set of entries to add to a local database.
     May contain a combination of compressed and raw data in a single
     response.
 
     Attributes:
-        raw_hashes (Sequence[google.cloud.webrisk_v1.types.RawHashes]):
+        raw_hashes (MutableSequence[google.cloud.webrisk_v1.types.RawHashes]):
             The raw SHA256-formatted entries.
             Repeated to allow returning sets of hashes with
             different prefix sizes.
         rice_hashes (google.cloud.webrisk_v1.types.RiceDeltaEncoding):
             The encoded 4-byte prefixes of SHA256-formatted entries,
             using a Golomb-Rice encoding. The hashes are converted to
             uint32, sorted in ascending order, then delta encoded and
             stored as encoded_data.
     """
 
-    raw_hashes = proto.RepeatedField(
+    raw_hashes: MutableSequence["RawHashes"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="RawHashes",
     )
-    rice_hashes = proto.Field(
+    rice_hashes: "RiceDeltaEncoding" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="RiceDeltaEncoding",
     )
 
 
 class ThreatEntryRemovals(proto.Message):
@@ -393,36 +404,36 @@
             The encoded local, lexicographically-sorted list indices,
             using a Golomb-Rice encoding. Used for sending compressed
             removal indices. The removal indices (uint32) are sorted in
             ascending order, then delta encoded and stored as
             encoded_data.
     """
 
-    raw_indices = proto.Field(
+    raw_indices: "RawIndices" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="RawIndices",
     )
-    rice_indices = proto.Field(
+    rice_indices: "RiceDeltaEncoding" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="RiceDeltaEncoding",
     )
 
 
 class RawIndices(proto.Message):
     r"""A set of raw indices to remove from a local list.
 
     Attributes:
-        indices (Sequence[int]):
+        indices (MutableSequence[int]):
             The indices to remove from a
             lexicographically-sorted local list.
     """
 
-    indices = proto.RepeatedField(
+    indices: MutableSequence[int] = proto.RepeatedField(
         proto.INT32,
         number=1,
     )
 
 
 class RawHashes(proto.Message):
     r"""The uncompressed threat entries in hash format.
@@ -444,19 +455,19 @@
         raw_hashes (bytes):
             The hashes, in binary format, concatenated
             into one long string. Hashes are sorted in
             lexicographic order. For JSON API users, hashes
             are base64-encoded.
     """
 
-    prefix_size = proto.Field(
+    prefix_size: int = proto.Field(
         proto.INT32,
         number=1,
     )
-    raw_hashes = proto.Field(
+    raw_hashes: bytes = proto.Field(
         proto.BYTES,
         number=2,
     )
 
 
 class RiceDeltaEncoding(proto.Message):
     r"""The Rice-Golomb encoded data. Used for sending compressed
@@ -477,42 +488,42 @@
             data. If only a single integer was encoded, this will be
             zero and the single value will be stored in ``first_value``.
         encoded_data (bytes):
             The encoded deltas that are encoded using the
             Golomb-Rice coder.
     """
 
-    first_value = proto.Field(
+    first_value: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    rice_parameter = proto.Field(
+    rice_parameter: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    entry_count = proto.Field(
+    entry_count: int = proto.Field(
         proto.INT32,
         number=3,
     )
-    encoded_data = proto.Field(
+    encoded_data: bytes = proto.Field(
         proto.BYTES,
         number=4,
     )
 
 
 class Submission(proto.Message):
-    r"""Wraps a URI that might be displaying phishing content.
+    r"""Wraps a URI that might be displaying malicious content.
 
     Attributes:
         uri (str):
             Required. The URI that is being reported for
-            phishing content to be analyzed.
+            malicious content to be analyzed.
     """
 
-    uri = proto.Field(
+    uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class CreateSubmissionRequest(proto.Message):
     r"""Request to send a potentially phishy URI to WebRisk.
@@ -523,19 +534,19 @@
             submission. This string is in the format
             "projects/{project_number}".
         submission (google.cloud.webrisk_v1.types.Submission):
             Required. The submission that contains the
             content of the phishing report.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    submission = proto.Field(
+    submission: "Submission" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="Submission",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-from .services.web_risk_service_v1_beta1 import (
-    WebRiskServiceV1Beta1AsyncClient,
-    WebRiskServiceV1Beta1Client,
-)
-from .types.webrisk import (
+from .webrisk import (
     CompressionType,
     ComputeThreatListDiffRequest,
     ComputeThreatListDiffResponse,
     RawHashes,
     RawIndices,
     RiceDeltaEncoding,
     SearchHashesRequest,
@@ -31,23 +26,21 @@
     SearchUrisResponse,
     ThreatEntryAdditions,
     ThreatEntryRemovals,
     ThreatType,
 )
 
 __all__ = (
-    "WebRiskServiceV1Beta1AsyncClient",
-    "CompressionType",
     "ComputeThreatListDiffRequest",
     "ComputeThreatListDiffResponse",
     "RawHashes",
     "RawIndices",
     "RiceDeltaEncoding",
     "SearchHashesRequest",
     "SearchHashesResponse",
     "SearchUrisRequest",
     "SearchUrisResponse",
     "ThreatEntryAdditions",
     "ThreatEntryRemovals",
+    "CompressionType",
     "ThreatType",
-    "WebRiskServiceV1Beta1Client",
 )
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/gapic_metadata.json` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/async_client.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.webrisk_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import timestamp_pb2  # type: ignore
@@ -159,17 +170,17 @@
         type(WebRiskServiceV1Beta1Client).get_transport_class,
         type(WebRiskServiceV1Beta1Client),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, WebRiskServiceV1Beta1Transport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the web risk service v1 beta1 client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -205,21 +216,21 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def compute_threat_list_diff(
         self,
-        request: Union[webrisk.ComputeThreatListDiffRequest, dict] = None,
+        request: Optional[Union[webrisk.ComputeThreatListDiffRequest, dict]] = None,
         *,
-        threat_type: webrisk.ThreatType = None,
-        version_token: bytes = None,
-        constraints: webrisk.ComputeThreatListDiffRequest.Constraints = None,
+        threat_type: Optional[webrisk.ThreatType] = None,
+        version_token: Optional[bytes] = None,
+        constraints: Optional[webrisk.ComputeThreatListDiffRequest.Constraints] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.ComputeThreatListDiffResponse:
         r"""Gets the most recent threat list diffs.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -243,15 +254,15 @@
                 # Make the request
                 response = await client.compute_threat_list_diff(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.webrisk_v1beta1.types.ComputeThreatListDiffRequest, dict]):
+            request (Optional[Union[google.cloud.webrisk_v1beta1.types.ComputeThreatListDiffRequest, dict]]):
                 The request object. Describes an API diff request.
             threat_type (:class:`google.cloud.webrisk_v1beta1.types.ThreatType`):
                 The ThreatList to update.
                 This corresponds to the ``threat_type`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             version_token (:class:`bytes`):
@@ -328,20 +339,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def search_uris(
         self,
-        request: Union[webrisk.SearchUrisRequest, dict] = None,
+        request: Optional[Union[webrisk.SearchUrisRequest, dict]] = None,
         *,
-        uri: str = None,
-        threat_types: Sequence[webrisk.ThreatType] = None,
+        uri: Optional[str] = None,
+        threat_types: Optional[MutableSequence[webrisk.ThreatType]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.SearchUrisResponse:
         r"""This method is used to check whether a URI is on a
         given threatList.
 
         .. code-block:: python
 
@@ -357,35 +368,35 @@
             async def sample_search_uris():
                 # Create a client
                 client = webrisk_v1beta1.WebRiskServiceV1Beta1AsyncClient()
 
                 # Initialize request argument(s)
                 request = webrisk_v1beta1.SearchUrisRequest(
                     uri="uri_value",
-                    threat_types="UNWANTED_SOFTWARE",
+                    threat_types=['UNWANTED_SOFTWARE'],
                 )
 
                 # Make the request
                 response = await client.search_uris(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.webrisk_v1beta1.types.SearchUrisRequest, dict]):
+            request (Optional[Union[google.cloud.webrisk_v1beta1.types.SearchUrisRequest, dict]]):
                 The request object. Request to check URI entries against
                 threatLists.
             uri (:class:`str`):
                 Required. The URI to be checked for
                 matches.
 
                 This corresponds to the ``uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            threat_types (:class:`Sequence[google.cloud.webrisk_v1beta1.types.ThreatType]`):
+            threat_types (:class:`MutableSequence[google.cloud.webrisk_v1beta1.types.ThreatType]`):
                 Required. The ThreatLists to search
                 in.
 
                 This corresponds to the ``threat_types`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -444,20 +455,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def search_hashes(
         self,
-        request: Union[webrisk.SearchHashesRequest, dict] = None,
+        request: Optional[Union[webrisk.SearchHashesRequest, dict]] = None,
         *,
-        hash_prefix: bytes = None,
-        threat_types: Sequence[webrisk.ThreatType] = None,
+        hash_prefix: Optional[bytes] = None,
+        threat_types: Optional[MutableSequence[webrisk.ThreatType]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.SearchHashesResponse:
         r"""Gets the full hashes that match the requested hash
         prefix. This is used after a hash prefix is looked up in
         a threatList and there is a match. The client side
         threatList only holds partial hashes so the client must
         query this method to determine if there is a full hash
@@ -476,37 +487,37 @@
 
             async def sample_search_hashes():
                 # Create a client
                 client = webrisk_v1beta1.WebRiskServiceV1Beta1AsyncClient()
 
                 # Initialize request argument(s)
                 request = webrisk_v1beta1.SearchHashesRequest(
-                    threat_types="UNWANTED_SOFTWARE",
+                    threat_types=['UNWANTED_SOFTWARE'],
                 )
 
                 # Make the request
                 response = await client.search_hashes(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.webrisk_v1beta1.types.SearchHashesRequest, dict]):
+            request (Optional[Union[google.cloud.webrisk_v1beta1.types.SearchHashesRequest, dict]]):
                 The request object. Request to return full hashes
                 matched by the provided hash prefixes.
             hash_prefix (:class:`bytes`):
                 A hash prefix, consisting of the most
                 significant 4-32 bytes of a SHA256 hash.
                 For JSON requests, this field is
                 base64-encoded.
 
                 This corresponds to the ``hash_prefix`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            threat_types (:class:`Sequence[google.cloud.webrisk_v1beta1.types.ThreatType]`):
+            threat_types (:class:`MutableSequence[google.cloud.webrisk_v1beta1.types.ThreatType]`):
                 Required. The ThreatLists to search
                 in.
 
                 This corresponds to the ``threat_types`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -570,18 +581,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-webrisk",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("WebRiskServiceV1Beta1AsyncClient",)
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/client.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.webrisk_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import timestamp_pb2  # type: ignore
@@ -55,15 +67,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[WebRiskServiceV1Beta1Transport]]
     _transport_registry["grpc"] = WebRiskServiceV1Beta1GrpcTransport
     _transport_registry["grpc_asyncio"] = WebRiskServiceV1Beta1GrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[WebRiskServiceV1Beta1Transport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -310,30 +322,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, WebRiskServiceV1Beta1Transport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, WebRiskServiceV1Beta1Transport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the web risk service v1 beta1 client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, WebRiskServiceV1Beta1Transport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -355,14 +367,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -407,21 +420,21 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def compute_threat_list_diff(
         self,
-        request: Union[webrisk.ComputeThreatListDiffRequest, dict] = None,
+        request: Optional[Union[webrisk.ComputeThreatListDiffRequest, dict]] = None,
         *,
-        threat_type: webrisk.ThreatType = None,
-        version_token: bytes = None,
-        constraints: webrisk.ComputeThreatListDiffRequest.Constraints = None,
+        threat_type: Optional[webrisk.ThreatType] = None,
+        version_token: Optional[bytes] = None,
+        constraints: Optional[webrisk.ComputeThreatListDiffRequest.Constraints] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.ComputeThreatListDiffResponse:
         r"""Gets the most recent threat list diffs.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -520,20 +533,20 @@
         )
 
         # Done; return the response.
         return response
 
     def search_uris(
         self,
-        request: Union[webrisk.SearchUrisRequest, dict] = None,
+        request: Optional[Union[webrisk.SearchUrisRequest, dict]] = None,
         *,
-        uri: str = None,
-        threat_types: Sequence[webrisk.ThreatType] = None,
+        uri: Optional[str] = None,
+        threat_types: Optional[MutableSequence[webrisk.ThreatType]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.SearchUrisResponse:
         r"""This method is used to check whether a URI is on a
         given threatList.
 
         .. code-block:: python
 
@@ -549,15 +562,15 @@
             def sample_search_uris():
                 # Create a client
                 client = webrisk_v1beta1.WebRiskServiceV1Beta1Client()
 
                 # Initialize request argument(s)
                 request = webrisk_v1beta1.SearchUrisRequest(
                     uri="uri_value",
-                    threat_types="UNWANTED_SOFTWARE",
+                    threat_types=['UNWANTED_SOFTWARE'],
                 )
 
                 # Make the request
                 response = client.search_uris(request=request)
 
                 # Handle the response
                 print(response)
@@ -569,15 +582,15 @@
             uri (str):
                 Required. The URI to be checked for
                 matches.
 
                 This corresponds to the ``uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            threat_types (Sequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
+            threat_types (MutableSequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
                 Required. The ThreatLists to search
                 in.
 
                 This corresponds to the ``threat_types`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -626,20 +639,20 @@
         )
 
         # Done; return the response.
         return response
 
     def search_hashes(
         self,
-        request: Union[webrisk.SearchHashesRequest, dict] = None,
+        request: Optional[Union[webrisk.SearchHashesRequest, dict]] = None,
         *,
-        hash_prefix: bytes = None,
-        threat_types: Sequence[webrisk.ThreatType] = None,
+        hash_prefix: Optional[bytes] = None,
+        threat_types: Optional[MutableSequence[webrisk.ThreatType]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> webrisk.SearchHashesResponse:
         r"""Gets the full hashes that match the requested hash
         prefix. This is used after a hash prefix is looked up in
         a threatList and there is a match. The client side
         threatList only holds partial hashes so the client must
         query this method to determine if there is a full hash
@@ -658,15 +671,15 @@
 
             def sample_search_hashes():
                 # Create a client
                 client = webrisk_v1beta1.WebRiskServiceV1Beta1Client()
 
                 # Initialize request argument(s)
                 request = webrisk_v1beta1.SearchHashesRequest(
-                    threat_types="UNWANTED_SOFTWARE",
+                    threat_types=['UNWANTED_SOFTWARE'],
                 )
 
                 # Make the request
                 response = client.search_hashes(request=request)
 
                 # Handle the response
                 print(response)
@@ -680,15 +693,15 @@
                 significant 4-32 bytes of a SHA256 hash.
                 For JSON requests, this field is
                 base64-encoded.
 
                 This corresponds to the ``hash_prefix`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            threat_types (Sequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
+            threat_types (MutableSequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
                 Required. The ThreatLists to search
                 in.
 
                 This corresponds to the ``threat_types`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -749,18 +762,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-webrisk",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("WebRiskServiceV1Beta1Client",)
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/base.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,40 +19,35 @@
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
+from google.cloud.webrisk_v1beta1 import gapic_version as package_version
 from google.cloud.webrisk_v1beta1.types import webrisk
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-webrisk",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class WebRiskServiceV1Beta1Transport(abc.ABC):
     """Abstract transport class for WebRiskServiceV1Beta1."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "webrisk.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/grpc.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "webrisk.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -177,16 +177,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "webrisk.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/grpc_asyncio.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/grpc_asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "webrisk.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -88,23 +88,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "webrisk.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/types/__init__.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,38 +9,50 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .webrisk import (
+from google.cloud.webrisk import gapic_version as package_version
+
+__version__ = package_version.__version__
+
+
+from .services.web_risk_service import WebRiskServiceAsyncClient, WebRiskServiceClient
+from .types.webrisk import (
     CompressionType,
     ComputeThreatListDiffRequest,
     ComputeThreatListDiffResponse,
+    CreateSubmissionRequest,
     RawHashes,
     RawIndices,
     RiceDeltaEncoding,
     SearchHashesRequest,
     SearchHashesResponse,
     SearchUrisRequest,
     SearchUrisResponse,
+    Submission,
     ThreatEntryAdditions,
     ThreatEntryRemovals,
     ThreatType,
 )
 
 __all__ = (
+    "WebRiskServiceAsyncClient",
+    "CompressionType",
     "ComputeThreatListDiffRequest",
     "ComputeThreatListDiffResponse",
+    "CreateSubmissionRequest",
     "RawHashes",
     "RawIndices",
     "RiceDeltaEncoding",
     "SearchHashesRequest",
     "SearchHashesResponse",
     "SearchUrisRequest",
     "SearchUrisResponse",
+    "Submission",
     "ThreatEntryAdditions",
     "ThreatEntryRemovals",
-    "CompressionType",
     "ThreatType",
+    "WebRiskServiceClient",
 )
```

### Comparing `google-cloud-webrisk-1.8.4/google/cloud/webrisk_v1beta1/types/webrisk.py` & `google-cloud-webrisk-1.9.0/google/cloud/webrisk_v1beta1/types/webrisk.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.webrisk.v1beta1",
     manifest={
         "ThreatType",
@@ -78,43 +80,45 @@
                 of 2 between 2\ **10 and 2**\ 20. If zero, no diff size
                 limit is set.
             max_database_entries (int):
                 Sets the maximum number of entries that the client is
                 willing to have in the local database. This should be a
                 power of 2 between 2\ **10 and 2**\ 20. If zero, no database
                 size limit is set.
-            supported_compressions (Sequence[google.cloud.webrisk_v1beta1.types.CompressionType]):
+            supported_compressions (MutableSequence[google.cloud.webrisk_v1beta1.types.CompressionType]):
                 The compression types supported by the
                 client.
         """
 
-        max_diff_entries = proto.Field(
+        max_diff_entries: int = proto.Field(
             proto.INT32,
             number=1,
         )
-        max_database_entries = proto.Field(
+        max_database_entries: int = proto.Field(
             proto.INT32,
             number=2,
         )
-        supported_compressions = proto.RepeatedField(
+        supported_compressions: MutableSequence[
+            "CompressionType"
+        ] = proto.RepeatedField(
             proto.ENUM,
             number=3,
             enum="CompressionType",
         )
 
-    threat_type = proto.Field(
+    threat_type: "ThreatType" = proto.Field(
         proto.ENUM,
         number=1,
         enum="ThreatType",
     )
-    version_token = proto.Field(
+    version_token: bytes = proto.Field(
         proto.BYTES,
         number=2,
     )
-    constraints = proto.Field(
+    constraints: Constraints = proto.Field(
         proto.MESSAGE,
         number=3,
         message=Constraints,
     )
 
 
 class ComputeThreatListDiffResponse(proto.Message):
@@ -161,65 +165,65 @@
         Attributes:
             sha256 (bytes):
                 The SHA256 hash of the client state; that is,
                 of the sorted list of all hashes present in the
                 database.
         """
 
-        sha256 = proto.Field(
+        sha256: bytes = proto.Field(
             proto.BYTES,
             number=1,
         )
 
-    response_type = proto.Field(
+    response_type: ResponseType = proto.Field(
         proto.ENUM,
         number=4,
         enum=ResponseType,
     )
-    additions = proto.Field(
+    additions: "ThreatEntryAdditions" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="ThreatEntryAdditions",
     )
-    removals = proto.Field(
+    removals: "ThreatEntryRemovals" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="ThreatEntryRemovals",
     )
-    new_version_token = proto.Field(
+    new_version_token: bytes = proto.Field(
         proto.BYTES,
         number=7,
     )
-    checksum = proto.Field(
+    checksum: Checksum = proto.Field(
         proto.MESSAGE,
         number=8,
         message=Checksum,
     )
-    recommended_next_diff = proto.Field(
+    recommended_next_diff: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class SearchUrisRequest(proto.Message):
     r"""Request to check URI entries against threatLists.
 
     Attributes:
         uri (str):
             Required. The URI to be checked for matches.
-        threat_types (Sequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
+        threat_types (MutableSequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
             Required. The ThreatLists to search in.
     """
 
-    uri = proto.Field(
+    uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    threat_types = proto.RepeatedField(
+    threat_types: MutableSequence["ThreatType"] = proto.RepeatedField(
         proto.ENUM,
         number=2,
         enum="ThreatType",
     )
 
 
 class SearchUrisResponse(proto.Message):
@@ -231,34 +235,34 @@
             the URI is on no list.
     """
 
     class ThreatUri(proto.Message):
         r"""Contains threat information on a matching uri.
 
         Attributes:
-            threat_types (Sequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
+            threat_types (MutableSequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
                 The ThreatList this threat belongs to.
             expire_time (google.protobuf.timestamp_pb2.Timestamp):
                 The cache lifetime for the returned match.
                 Clients must not cache this response past this
                 timestamp to avoid false positives.
         """
 
-        threat_types = proto.RepeatedField(
+        threat_types: MutableSequence["ThreatType"] = proto.RepeatedField(
             proto.ENUM,
             number=1,
             enum="ThreatType",
         )
-        expire_time = proto.Field(
+        expire_time: timestamp_pb2.Timestamp = proto.Field(
             proto.MESSAGE,
             number=2,
             message=timestamp_pb2.Timestamp,
         )
 
-    threat = proto.Field(
+    threat: ThreatUri = proto.Field(
         proto.MESSAGE,
         number=1,
         message=ThreatUri,
     )
 
 
 class SearchHashesRequest(proto.Message):
@@ -266,109 +270,109 @@
     prefixes.
 
     Attributes:
         hash_prefix (bytes):
             A hash prefix, consisting of the most
             significant 4-32 bytes of a SHA256 hash. For
             JSON requests, this field is base64-encoded.
-        threat_types (Sequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
+        threat_types (MutableSequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
             Required. The ThreatLists to search in.
     """
 
-    hash_prefix = proto.Field(
+    hash_prefix: bytes = proto.Field(
         proto.BYTES,
         number=1,
     )
-    threat_types = proto.RepeatedField(
+    threat_types: MutableSequence["ThreatType"] = proto.RepeatedField(
         proto.ENUM,
         number=2,
         enum="ThreatType",
     )
 
 
 class SearchHashesResponse(proto.Message):
     r"""
 
     Attributes:
-        threats (Sequence[google.cloud.webrisk_v1beta1.types.SearchHashesResponse.ThreatHash]):
+        threats (MutableSequence[google.cloud.webrisk_v1beta1.types.SearchHashesResponse.ThreatHash]):
             The full hashes that matched the requested
             prefixes. The hash will be populated in the key.
         negative_expire_time (google.protobuf.timestamp_pb2.Timestamp):
             For requested entities that did not match the
             threat list, how long to cache the response
             until.
     """
 
     class ThreatHash(proto.Message):
         r"""Contains threat information on a matching hash.
 
         Attributes:
-            threat_types (Sequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
+            threat_types (MutableSequence[google.cloud.webrisk_v1beta1.types.ThreatType]):
                 The ThreatList this threat belongs to.
                 This must contain at least one entry.
             hash_ (bytes):
                 A 32 byte SHA256 hash. This field is in
                 binary format. For JSON requests, hashes are
                 base64-encoded.
             expire_time (google.protobuf.timestamp_pb2.Timestamp):
                 The cache lifetime for the returned match.
                 Clients must not cache this response past this
                 timestamp to avoid false positives.
         """
 
-        threat_types = proto.RepeatedField(
+        threat_types: MutableSequence["ThreatType"] = proto.RepeatedField(
             proto.ENUM,
             number=1,
             enum="ThreatType",
         )
-        hash_ = proto.Field(
+        hash_: bytes = proto.Field(
             proto.BYTES,
             number=2,
         )
-        expire_time = proto.Field(
+        expire_time: timestamp_pb2.Timestamp = proto.Field(
             proto.MESSAGE,
             number=3,
             message=timestamp_pb2.Timestamp,
         )
 
-    threats = proto.RepeatedField(
+    threats: MutableSequence[ThreatHash] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=ThreatHash,
     )
-    negative_expire_time = proto.Field(
+    negative_expire_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class ThreatEntryAdditions(proto.Message):
     r"""Contains the set of entries to add to a local database.
     May contain a combination of compressed and raw data in a single
     response.
 
     Attributes:
-        raw_hashes (Sequence[google.cloud.webrisk_v1beta1.types.RawHashes]):
+        raw_hashes (MutableSequence[google.cloud.webrisk_v1beta1.types.RawHashes]):
             The raw SHA256-formatted entries.
             Repeated to allow returning sets of hashes with
             different prefix sizes.
         rice_hashes (google.cloud.webrisk_v1beta1.types.RiceDeltaEncoding):
             The encoded 4-byte prefixes of SHA256-formatted entries,
             using a Golomb-Rice encoding. The hashes are converted to
             uint32, sorted in ascending order, then delta encoded and
             stored as encoded_data.
     """
 
-    raw_hashes = proto.RepeatedField(
+    raw_hashes: MutableSequence["RawHashes"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="RawHashes",
     )
-    rice_hashes = proto.Field(
+    rice_hashes: "RiceDeltaEncoding" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="RiceDeltaEncoding",
     )
 
 
 class ThreatEntryRemovals(proto.Message):
@@ -381,36 +385,36 @@
             The encoded local, lexicographically-sorted list indices,
             using a Golomb-Rice encoding. Used for sending compressed
             removal indices. The removal indices (uint32) are sorted in
             ascending order, then delta encoded and stored as
             encoded_data.
     """
 
-    raw_indices = proto.Field(
+    raw_indices: "RawIndices" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="RawIndices",
     )
-    rice_indices = proto.Field(
+    rice_indices: "RiceDeltaEncoding" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="RiceDeltaEncoding",
     )
 
 
 class RawIndices(proto.Message):
     r"""A set of raw indices to remove from a local list.
 
     Attributes:
-        indices (Sequence[int]):
+        indices (MutableSequence[int]):
             The indices to remove from a
             lexicographically-sorted local list.
     """
 
-    indices = proto.RepeatedField(
+    indices: MutableSequence[int] = proto.RepeatedField(
         proto.INT32,
         number=1,
     )
 
 
 class RawHashes(proto.Message):
     r"""The uncompressed threat entries in hash format.
@@ -430,19 +434,19 @@
         raw_hashes (bytes):
             The hashes, in binary format, concatenated
             into one long string. Hashes are sorted in
             lexicographic order. For JSON API users, hashes
             are base64-encoded.
     """
 
-    prefix_size = proto.Field(
+    prefix_size: int = proto.Field(
         proto.INT32,
         number=1,
     )
-    raw_hashes = proto.Field(
+    raw_hashes: bytes = proto.Field(
         proto.BYTES,
         number=2,
     )
 
 
 class RiceDeltaEncoding(proto.Message):
     r"""The Rice-Golomb encoded data. Used for sending compressed
@@ -463,26 +467,26 @@
             data. If only a single integer was encoded, this will be
             zero and the single value will be stored in ``first_value``.
         encoded_data (bytes):
             The encoded deltas that are encoded using the
             Golomb-Rice coder.
     """
 
-    first_value = proto.Field(
+    first_value: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    rice_parameter = proto.Field(
+    rice_parameter: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    entry_count = proto.Field(
+    entry_count: int = proto.Field(
         proto.INT32,
         number=3,
     )
-    encoded_data = proto.Field(
+    encoded_data: bytes = proto.Field(
         proto.BYTES,
         number=4,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/PKG-INFO` & `google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-webrisk
-Version: 1.8.4
-Summary: Google Cloud Web Risk API client library
+Version: 1.9.0
+Summary: Google Cloud Webrisk API client library
 Home-page: https://github.com/googleapis/python-webrisk
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-webrisk-1.8.4/google_cloud_webrisk.egg-info/SOURCES.txt` & `google-cloud-webrisk-1.9.0/google_cloud_webrisk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/cloud/webrisk/__init__.py
+google/cloud/webrisk/gapic_version.py
 google/cloud/webrisk/py.typed
 google/cloud/webrisk_v1/__init__.py
 google/cloud/webrisk_v1/gapic_metadata.json
+google/cloud/webrisk_v1/gapic_version.py
 google/cloud/webrisk_v1/py.typed
 google/cloud/webrisk_v1/services/__init__.py
 google/cloud/webrisk_v1/services/web_risk_service/__init__.py
 google/cloud/webrisk_v1/services/web_risk_service/async_client.py
 google/cloud/webrisk_v1/services/web_risk_service/client.py
 google/cloud/webrisk_v1/services/web_risk_service/transports/__init__.py
 google/cloud/webrisk_v1/services/web_risk_service/transports/base.py
 google/cloud/webrisk_v1/services/web_risk_service/transports/grpc.py
 google/cloud/webrisk_v1/services/web_risk_service/transports/grpc_asyncio.py
 google/cloud/webrisk_v1/types/__init__.py
 google/cloud/webrisk_v1/types/webrisk.py
 google/cloud/webrisk_v1beta1/__init__.py
 google/cloud/webrisk_v1beta1/gapic_metadata.json
+google/cloud/webrisk_v1beta1/gapic_version.py
 google/cloud/webrisk_v1beta1/py.typed
 google/cloud/webrisk_v1beta1/services/__init__.py
 google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/__init__.py
 google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/async_client.py
 google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/client.py
 google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/__init__.py
 google/cloud/webrisk_v1beta1/services/web_risk_service_v1_beta1/transports/base.py
@@ -34,16 +37,14 @@
 google_cloud_webrisk.egg-info/PKG-INFO
 google_cloud_webrisk.egg-info/SOURCES.txt
 google_cloud_webrisk.egg-info/dependency_links.txt
 google_cloud_webrisk.egg-info/namespace_packages.txt
 google_cloud_webrisk.egg-info/not-zip-safe
 google_cloud_webrisk.egg-info/requires.txt
 google_cloud_webrisk.egg-info/top_level.txt
-scripts/fixup_webrisk_v1_keywords.py
-scripts/fixup_webrisk_v1beta1_keywords.py
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/webrisk_v1/__init__.py
 tests/unit/gapic/webrisk_v1/test_web_risk_service.py
 tests/unit/gapic/webrisk_v1beta1/__init__.py
 tests/unit/gapic/webrisk_v1beta1/test_web_risk_service_v1_beta1.py
```

### Comparing `google-cloud-webrisk-1.8.4/setup.py` & `google-cloud-webrisk-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,76 @@
-# Copyright 2018 Google LLC
+# -*- coding: utf-8 -*-
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+#
 import io
 import os
 
-import setuptools
+import setuptools  # type: ignore
 
-# Package metadata.
+package_root = os.path.abspath(os.path.dirname(__file__))
 
 name = "google-cloud-webrisk"
-description = "Google Cloud Web Risk API client library"
-version = "1.8.4"
-# Should be one of:
-# 'Development Status :: 3 - Alpha'
-# 'Development Status :: 4 - Beta'
-# 'Development Status :: 5 - Production/Stable'
-release_status = "Development Status :: 5 - Production/Stable"
+
+
+description = "Google Cloud Webrisk API client library"
+
+version = {}
+with open(os.path.join(package_root, "google/cloud/webrisk/gapic_version.py")) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
+if version[0] == "0":
+    release_status = "Development Status :: 4 - Beta"
+else:
+    release_status = "Development Status :: 5 - Production/Stable"
+
 dependencies = [
-    "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
+    "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-extras = {}
-
-
-# Setup boilerplate below this line.
+url = "https://github.com/googleapis/python-webrisk"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
-# Only include packages under the 'google' namespace. Do not include tests,
-# benchmarks, etc.
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("google")
 ]
 
-# Determine which namespaces are needed.
 namespaces = ["google"]
 if "google.cloud" in packages:
     namespaces.append("google.cloud")
 
-
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     license="Apache 2.0",
-    url="https://github.com/googleapis/python-webrisk",
+    url=url,
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
@@ -77,18 +78,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "Topic :: Internet",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
+    python_requires=">=3.7",
     namespace_packages=namespaces,
     install_requires=dependencies,
-    extras_require=extras,
-    python_requires=">=3.7",
-    scripts=[
-        "scripts/fixup_webrisk_v1_keywords.py",
-        "scripts/fixup_webrisk_v1beta1_keywords.py",
-    ],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-cloud-webrisk-1.8.4/tests/__init__.py` & `google-cloud-webrisk-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/tests/unit/__init__.py` & `google-cloud-webrisk-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/tests/unit/gapic/__init__.py` & `google-cloud-webrisk-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1/__init__.py` & `google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1/test_web_risk_service.py` & `google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1/test_web_risk_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1beta1/__init__.py` & `google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-webrisk-1.8.4/tests/unit/gapic/webrisk_v1beta1/test_web_risk_service_v1_beta1.py` & `google-cloud-webrisk-1.9.0/tests/unit/gapic/webrisk_v1beta1/test_web_risk_service_v1_beta1.py`

 * *Files identical despite different names*

