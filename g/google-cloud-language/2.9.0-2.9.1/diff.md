# Comparing `tmp/google-cloud-language-2.9.0.tar.gz` & `tmp/google-cloud-language-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-language-2.9.0.tar", last modified: Thu Feb 16 20:25:19 2023, max compression
+gzip compressed data, was "google-cloud-language-2.9.1.tar", last modified: Mon Mar 27 15:32:56 2023, max compression
```

## Comparing `google-cloud-language-2.9.0.tar` & `google-cloud-language-2.9.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4800 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3881 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.397037 google-cloud-language-2.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.397037 google-cloud-language-2.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.397037 google-cloud-language-2.9.0/google/cloud/language/
--rw-rw-r--   0 root         (0)     1003     2229 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.397037 google-cloud-language-2.9.0/google/cloud/language_v1/
--rw-rw-r--   0 root         (0)     1003     2084 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2933 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.401037 google-cloud-language-2.9.0/google/cloud/language_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.401037 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38402 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    45715 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.401037 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11130 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18357 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18700 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    39816 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.401037 google-cloud-language-2.9.0/google/cloud/language_v1/types/
--rw-rw-r--   0 root         (0)     1003     1811 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    51123 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1/types/language_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.401037 google-cloud-language-2.9.0/google/cloud/language_v1beta2/
--rw-rw-r--   0 root         (0)     1003     2089 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     2943 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.401037 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.401037 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38676 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    45989 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11140 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18373 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18716 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    39851 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/google/cloud/language_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     1811 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    52929 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/google/cloud/language_v1beta2/types/language_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/google_cloud_language.egg-info/
--rw-r--r--   0 root         (0)     1003     4800 2023-02-16 20:25:19.000000 google-cloud-language-2.9.0/google_cloud_language.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2522 2023-02-16 20:25:19.000000 google-cloud-language-2.9.0/google_cloud_language.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-16 20:25:19.000000 google-cloud-language-2.9.0/google_cloud_language.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-02-16 20:25:19.000000 google-cloud-language-2.9.0/google_cloud_language.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-16 20:25:19.000000 google-cloud-language-2.9.0/google_cloud_language.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-02-16 20:25:19.000000 google-cloud-language-2.9.0/google_cloud_language.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-02-16 20:25:19.000000 google-cloud-language-2.9.0/google_cloud_language.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-02-16 20:25:19.409037 google-cloud-language-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2925 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/tests/unit/gapic/language_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/tests/unit/gapic/language_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   157173 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/tests/unit/gapic/language_v1/test_language_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-16 20:25:19.405037 google-cloud-language-2.9.0/tests/unit/gapic/language_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/tests/unit/gapic/language_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003   157246 2023-02-16 20:22:53.000000 google-cloud-language-2.9.0/tests/unit/gapic/language_v1beta2/test_language_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.343803 google-cloud-language-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4800 2023-03-27 15:32:56.343803 google-cloud-language-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3881 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.331802 google-cloud-language-2.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.331802 google-cloud-language-2.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.335802 google-cloud-language-2.9.1/google/cloud/language/
+-rw-rw-r--   0 root         (0)     1003     2229 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.335802 google-cloud-language-2.9.1/google/cloud/language_v1/
+-rw-rw-r--   0 root         (0)     1003     2084 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2933 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.335802 google-cloud-language-2.9.1/google/cloud/language_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.335802 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38418 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    45731 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.335802 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11130 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18357 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18700 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    39817 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.335802 google-cloud-language-2.9.1/google/cloud/language_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1811 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    51159 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1/types/language_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.335802 google-cloud-language-2.9.1/google/cloud/language_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     2089 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2943 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.335802 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.339803 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38692 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    46005 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.339803 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11140 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18373 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18716 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    39852 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.339803 google-cloud-language-2.9.1/google/cloud/language_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     1811 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    52965 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/google/cloud/language_v1beta2/types/language_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.339803 google-cloud-language-2.9.1/google_cloud_language.egg-info/
+-rw-r--r--   0 root         (0)     1003     4800 2023-03-27 15:32:56.000000 google-cloud-language-2.9.1/google_cloud_language.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2522 2023-03-27 15:32:56.000000 google-cloud-language-2.9.1/google_cloud_language.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:32:56.000000 google-cloud-language-2.9.1/google_cloud_language.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:32:56.000000 google-cloud-language-2.9.1/google_cloud_language.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:32:56.000000 google-cloud-language-2.9.1/google_cloud_language.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:32:56.000000 google-cloud-language-2.9.1/google_cloud_language.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:32:56.000000 google-cloud-language-2.9.1/google_cloud_language.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:32:56.343803 google-cloud-language-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2925 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.339803 google-cloud-language-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.339803 google-cloud-language-2.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.339803 google-cloud-language-2.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.339803 google-cloud-language-2.9.1/tests/unit/gapic/language_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/tests/unit/gapic/language_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   157173 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/tests/unit/gapic/language_v1/test_language_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:56.343803 google-cloud-language-2.9.1/tests/unit/gapic/language_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/tests/unit/gapic/language_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   157246 2023-03-27 15:30:19.000000 google-cloud-language-2.9.1/tests/unit/gapic/language_v1beta2/test_language_service.py
```

### Comparing `google-cloud-language-2.9.0/LICENSE` & `google-cloud-language-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/MANIFEST.in` & `google-cloud-language-2.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/PKG-INFO` & `google-cloud-language-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-language
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Language API client library
 Home-page: https://github.com/googleapis/python-language
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-language-2.9.0/README.rst` & `google-cloud-language-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language/gapic_version.py` & `google-cloud-language-2.9.1/google/cloud/language/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/gapic_metadata.json` & `google-cloud-language-2.9.1/google/cloud/language_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/gapic_version.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/services/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/async_client.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -835,16 +835,17 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.language_v1.types.AnnotateTextRequest, dict]]):
                 The request object. The request message for the text
-                annotation API, which can perform multiple analysis
-                types (sentiment, entities, and syntax) in one call.
+                annotation API, which can perform
+                multiple analysis types (sentiment,
+                entities, and syntax) in one call.
             document (:class:`google.cloud.language_v1.types.Document`):
                 Required. Input document.
                 This corresponds to the ``document`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             features (:class:`google.cloud.language_v1.types.AnnotateTextRequest.Features`):
                 Required. The enabled features.
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/client.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -994,16 +994,17 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.language_v1.types.AnnotateTextRequest, dict]):
                 The request object. The request message for the text
-                annotation API, which can perform multiple analysis
-                types (sentiment, entities, and syntax) in one call.
+                annotation API, which can perform
+                multiple analysis types (sentiment,
+                entities, and syntax) in one call.
             document (google.cloud.language_v1.types.Document):
                 Required. Input document.
                 This corresponds to the ``document`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             features (google.cloud.language_v1.types.AnnotateTextRequest.Features):
                 Required. The enabled features.
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/base.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/grpc.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/grpc_asyncio.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/services/language_service/transports/rest.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/services/language_service/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import dataclasses
 import json  # type: ignore
 import re
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, path_template, rest_helpers, rest_streaming
 from google.api_core import exceptions as core_exceptions
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
@@ -355,15 +355,15 @@
         self._interceptor = interceptor or LanguageServiceRestInterceptor()
         self._prep_wrapped_messages(client_info)
 
     class _AnalyzeEntities(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnalyzeEntities")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -452,15 +452,15 @@
             resp = self._interceptor.post_analyze_entities(resp)
             return resp
 
     class _AnalyzeEntitySentiment(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnalyzeEntitySentiment")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -476,15 +476,14 @@
         ) -> language_service.AnalyzeEntitySentimentResponse:
             r"""Call the analyze entity sentiment method over HTTP.
 
             Args:
                 request (~.language_service.AnalyzeEntitySentimentRequest):
                     The request object. The entity-level sentiment analysis
                 request message.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -553,15 +552,15 @@
             resp = self._interceptor.post_analyze_entity_sentiment(resp)
             return resp
 
     class _AnalyzeSentiment(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnalyzeSentiment")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -577,15 +576,14 @@
         ) -> language_service.AnalyzeSentimentResponse:
             r"""Call the analyze sentiment method over HTTP.
 
             Args:
                 request (~.language_service.AnalyzeSentimentRequest):
                     The request object. The sentiment analysis request
                 message.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -654,15 +652,15 @@
             resp = self._interceptor.post_analyze_sentiment(resp)
             return resp
 
     class _AnalyzeSyntax(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnalyzeSyntax")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -749,15 +747,15 @@
             resp = self._interceptor.post_analyze_syntax(resp)
             return resp
 
     class _AnnotateText(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnnotateText")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -775,15 +773,14 @@
 
             Args:
                 request (~.language_service.AnnotateTextRequest):
                     The request object. The request message for the text
                 annotation API, which can perform
                 multiple analysis types (sentiment,
                 entities, and syntax) in one call.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -850,15 +847,15 @@
             resp = self._interceptor.post_annotate_text(resp)
             return resp
 
     class _ClassifyText(LanguageServiceRestStub):
         def __hash__(self):
             return hash("ClassifyText")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -874,15 +871,14 @@
         ) -> language_service.ClassifyTextResponse:
             r"""Call the classify text method over HTTP.
 
             Args:
                 request (~.language_service.ClassifyTextRequest):
                     The request object. The document classification request
                 message.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/types/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1/types/language_service.py` & `google-cloud-language-2.9.1/google/cloud/language_v1/types/language_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.language.v1",
     manifest={
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/gapic_metadata.json` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/gapic_version.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/async_client.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -836,16 +836,17 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.language_v1beta2.types.AnnotateTextRequest, dict]]):
                 The request object. The request message for the text
-                annotation API, which can perform multiple analysis
-                types (sentiment, entities, and syntax) in one call.
+                annotation API, which can perform
+                multiple analysis types (sentiment,
+                entities, and syntax) in one call.
             document (:class:`google.cloud.language_v1beta2.types.Document`):
                 Required. Input document.
                 This corresponds to the ``document`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             features (:class:`google.cloud.language_v1beta2.types.AnnotateTextRequest.Features`):
                 Required. The enabled features.
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/client.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -995,16 +995,17 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.language_v1beta2.types.AnnotateTextRequest, dict]):
                 The request object. The request message for the text
-                annotation API, which can perform multiple analysis
-                types (sentiment, entities, and syntax) in one call.
+                annotation API, which can perform
+                multiple analysis types (sentiment,
+                entities, and syntax) in one call.
             document (google.cloud.language_v1beta2.types.Document):
                 Required. Input document.
                 This corresponds to the ``document`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             features (google.cloud.language_v1beta2.types.AnnotateTextRequest.Features):
                 Required. The enabled features.
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/base.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/grpc.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/grpc_asyncio.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/services/language_service/transports/rest.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/services/language_service/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import dataclasses
 import json  # type: ignore
 import re
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, path_template, rest_helpers, rest_streaming
 from google.api_core import exceptions as core_exceptions
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
@@ -355,15 +355,15 @@
         self._interceptor = interceptor or LanguageServiceRestInterceptor()
         self._prep_wrapped_messages(client_info)
 
     class _AnalyzeEntities(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnalyzeEntities")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -452,15 +452,15 @@
             resp = self._interceptor.post_analyze_entities(resp)
             return resp
 
     class _AnalyzeEntitySentiment(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnalyzeEntitySentiment")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -476,15 +476,14 @@
         ) -> language_service.AnalyzeEntitySentimentResponse:
             r"""Call the analyze entity sentiment method over HTTP.
 
             Args:
                 request (~.language_service.AnalyzeEntitySentimentRequest):
                     The request object. The entity-level sentiment analysis
                 request message.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -553,15 +552,15 @@
             resp = self._interceptor.post_analyze_entity_sentiment(resp)
             return resp
 
     class _AnalyzeSentiment(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnalyzeSentiment")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -577,15 +576,14 @@
         ) -> language_service.AnalyzeSentimentResponse:
             r"""Call the analyze sentiment method over HTTP.
 
             Args:
                 request (~.language_service.AnalyzeSentimentRequest):
                     The request object. The sentiment analysis request
                 message.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -654,15 +652,15 @@
             resp = self._interceptor.post_analyze_sentiment(resp)
             return resp
 
     class _AnalyzeSyntax(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnalyzeSyntax")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -749,15 +747,15 @@
             resp = self._interceptor.post_analyze_syntax(resp)
             return resp
 
     class _AnnotateText(LanguageServiceRestStub):
         def __hash__(self):
             return hash("AnnotateText")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -775,15 +773,14 @@
 
             Args:
                 request (~.language_service.AnnotateTextRequest):
                     The request object. The request message for the text
                 annotation API, which can perform
                 multiple analysis types (sentiment,
                 entities, and syntax) in one call.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -850,15 +847,15 @@
             resp = self._interceptor.post_annotate_text(resp)
             return resp
 
     class _ClassifyText(LanguageServiceRestStub):
         def __hash__(self):
             return hash("ClassifyText")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -874,15 +871,14 @@
         ) -> language_service.ClassifyTextResponse:
             r"""Call the classify text method over HTTP.
 
             Args:
                 request (~.language_service.ClassifyTextRequest):
                     The request object. The document classification request
                 message.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/types/__init__.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/google/cloud/language_v1beta2/types/language_service.py` & `google-cloud-language-2.9.1/google/cloud/language_v1beta2/types/language_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.language.v1beta2",
     manifest={
```

### Comparing `google-cloud-language-2.9.0/google_cloud_language.egg-info/PKG-INFO` & `google-cloud-language-2.9.1/google_cloud_language.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-language
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Language API client library
 Home-page: https://github.com/googleapis/python-language
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-language-2.9.0/google_cloud_language.egg-info/SOURCES.txt` & `google-cloud-language-2.9.1/google_cloud_language.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/setup.py` & `google-cloud-language-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/tests/__init__.py` & `google-cloud-language-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/tests/unit/__init__.py` & `google-cloud-language-2.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/tests/unit/gapic/__init__.py` & `google-cloud-language-2.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/tests/unit/gapic/language_v1/__init__.py` & `google-cloud-language-2.9.1/tests/unit/gapic/language_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/tests/unit/gapic/language_v1/test_language_service.py` & `google-cloud-language-2.9.1/tests/unit/gapic/language_v1/test_language_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/tests/unit/gapic/language_v1beta2/__init__.py` & `google-cloud-language-2.9.1/tests/unit/gapic/language_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-language-2.9.0/tests/unit/gapic/language_v1beta2/test_language_service.py` & `google-cloud-language-2.9.1/tests/unit/gapic/language_v1beta2/test_language_service.py`

 * *Files identical despite different names*

