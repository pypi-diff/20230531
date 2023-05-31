# Comparing `tmp/google-cloud-redis-2.9.2.tar.gz` & `tmp/google-cloud-redis-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-redis-2.9.2.tar", last modified: Tue Oct  4 00:11:35 2022, max compression
+gzip compressed data, was "google-cloud-redis-2.9.3.tar", last modified: Mon Oct 10 16:19:41 2022, max compression
```

## Comparing `google-cloud-redis-2.9.2.tar` & `google-cloud-redis-2.9.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.439576 google-cloud-redis-2.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4713 2022-10-04 00:11:35.439576 google-cloud-redis-2.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3815 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.427574 google-cloud-redis-2.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.427574 google-cloud-redis-2.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.431575 google-cloud-redis-2.9.2/google/cloud/redis/
--rw-rw-r--   0 root         (0)     1003     2193 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis/__init__.py
--rw-rw-r--   0 root         (0)     1003       79 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.431575 google-cloud-redis-2.9.2/google/cloud/redis_v1/
--rw-rw-r--   0 root         (0)     1003     2068 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3313 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.431575 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.431575 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/
--rw-rw-r--   0 root         (0)     1003      753 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/__init__.py
--rw-rw-r--   0 root         (0)     1003    68553 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/async_client.py
--rw-rw-r--   0 root         (0)     1003    79000 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/client.py
--rw-rw-r--   0 root         (0)     1003     5736 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.431575 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10835 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26553 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    27153 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.431575 google-cloud-redis-2.9.2/google/cloud/redis_v1/types/
--rw-rw-r--   0 root         (0)     1003     1934 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    34629 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1/types/cloud_redis.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.431575 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2068 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3323 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.431575 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.435575 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/
--rw-rw-r--   0 root         (0)     1003      753 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/__init__.py
--rw-rw-r--   0 root         (0)     1003    68864 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/async_client.py
--rw-rw-r--   0 root         (0)     1003    79312 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/client.py
--rw-rw-r--   0 root         (0)     1003     5781 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.435575 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10839 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26622 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    27222 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.435575 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1934 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    36115 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/types/cloud_redis.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.435575 google-cloud-redis-2.9.2/google_cloud_redis.egg-info/
--rw-r--r--   0 root         (0)     1003     4713 2022-10-04 00:11:35.000000 google-cloud-redis-2.9.2/google_cloud_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2228 2022-10-04 00:11:35.000000 google-cloud-redis-2.9.2/google_cloud_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:11:35.000000 google-cloud-redis-2.9.2/google_cloud_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-04 00:11:35.000000 google-cloud-redis-2.9.2/google_cloud_redis.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:11:35.000000 google-cloud-redis-2.9.2/google_cloud_redis.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      184 2022-10-04 00:11:35.000000 google-cloud-redis-2.9.2/google_cloud_redis.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-04 00:11:35.000000 google-cloud-redis-2.9.2/google_cloud_redis.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.435575 google-cloud-redis-2.9.2/scripts/
--rw-rw-r--   0 root         (0)     1003     6526 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/scripts/fixup_redis_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6526 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/scripts/fixup_redis_v1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-04 00:11:35.439576 google-cloud-redis-2.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2953 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.435575 google-cloud-redis-2.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.435575 google-cloud-redis-2.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.439576 google-cloud-redis-2.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.439576 google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   159059 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1/test_cloud_redis.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:11:35.439576 google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   159141 2022-10-04 00:08:17.000000 google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1beta1/test_cloud_redis.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4713 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3815 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.317057 google-cloud-redis-2.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.321056 google-cloud-redis-2.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.321056 google-cloud-redis-2.9.3/google/cloud/redis/
+-rw-rw-r--   0 root         (0)     1003     2193 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis/__init__.py
+-rw-rw-r--   0 root         (0)     1003       79 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.321056 google-cloud-redis-2.9.3/google/cloud/redis_v1/
+-rw-rw-r--   0 root         (0)     1003     2068 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3313 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.321056 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.325055 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/
+-rw-rw-r--   0 root         (0)     1003      753 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/__init__.py
+-rw-rw-r--   0 root         (0)     1003    68553 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/async_client.py
+-rw-rw-r--   0 root         (0)     1003    79000 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/client.py
+-rw-rw-r--   0 root         (0)     1003     5736 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.325055 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10835 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26553 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27153 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.325055 google-cloud-redis-2.9.3/google/cloud/redis_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1934 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34629 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1/types/cloud_redis.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.325055 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2068 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3323 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.325055 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.325055 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/
+-rw-rw-r--   0 root         (0)     1003      753 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/__init__.py
+-rw-rw-r--   0 root         (0)     1003    68864 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/async_client.py
+-rw-rw-r--   0 root         (0)     1003    79312 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/client.py
+-rw-rw-r--   0 root         (0)     1003     5781 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.325055 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10839 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26622 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27222 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.325055 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1934 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    36115 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/types/cloud_redis.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/google_cloud_redis.egg-info/
+-rw-r--r--   0 root         (0)     1003     4713 2022-10-10 16:19:41.000000 google-cloud-redis-2.9.3/google_cloud_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2228 2022-10-10 16:19:41.000000 google-cloud-redis-2.9.3/google_cloud_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:19:41.000000 google-cloud-redis-2.9.3/google_cloud_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:19:41.000000 google-cloud-redis-2.9.3/google_cloud_redis.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:19:41.000000 google-cloud-redis-2.9.3/google_cloud_redis.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      256 2022-10-10 16:19:41.000000 google-cloud-redis-2.9.3/google_cloud_redis.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:19:41.000000 google-cloud-redis-2.9.3/google_cloud_redis.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/scripts/
+-rw-rw-r--   0 root         (0)     1003     6526 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/scripts/fixup_redis_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6526 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/scripts/fixup_redis_v1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3022 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   159059 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1/test_cloud_redis.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:19:41.329054 google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   159141 2022-10-10 16:16:19.000000 google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1beta1/test_cloud_redis.py
```

### Comparing `google-cloud-redis-2.9.2/LICENSE` & `google-cloud-redis-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/MANIFEST.in` & `google-cloud-redis-2.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/PKG-INFO` & `google-cloud-redis-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-redis
-Version: 2.9.2
+Version: 2.9.3
 Summary: Google Cloud Memorystore for Redis API client library
 Home-page: https://github.com/googleapis/python-redis
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-redis-2.9.2/README.rst` & `google-cloud-redis-2.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/gapic_metadata.json` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/services/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/async_client.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/client.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/pagers.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/transports/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/transports/base.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/transports/grpc.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/services/cloud_redis/transports/grpc_asyncio.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/services/cloud_redis/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/types/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1/types/cloud_redis.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1/types/cloud_redis.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/gapic_metadata.json` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/async_client.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/client.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/pagers.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/transports/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/transports/base.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/transports/grpc.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/services/cloud_redis/transports/grpc_asyncio.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/services/cloud_redis/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/types/__init__.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google/cloud/redis_v1beta1/types/cloud_redis.py` & `google-cloud-redis-2.9.3/google/cloud/redis_v1beta1/types/cloud_redis.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/google_cloud_redis.egg-info/PKG-INFO` & `google-cloud-redis-2.9.3/google_cloud_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-redis
-Version: 2.9.2
+Version: 2.9.3
 Summary: Google Cloud Memorystore for Redis API client library
 Home-page: https://github.com/googleapis/python-redis
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-redis-2.9.2/google_cloud_redis.egg-info/SOURCES.txt` & `google-cloud-redis-2.9.3/google_cloud_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/scripts/fixup_redis_v1_keywords.py` & `google-cloud-redis-2.9.3/scripts/fixup_redis_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/scripts/fixup_redis_v1beta1_keywords.py` & `google-cloud-redis-2.9.3/scripts/fixup_redis_v1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/setup.py` & `google-cloud-redis-2.9.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 
 import setuptools
 
 # Package metadata.
 
 name = "google-cloud-redis"
 description = "Google Cloud Memorystore for Redis API client library"
-version = "2.9.2"
+version = "2.9.3"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
-    "protobuf >= 3.20.2, <5.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 extras = {"libcst": "libcst >= 0.2.5"}
 
 # Setup boilerplate below this line.
 
 package_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `google-cloud-redis-2.9.2/tests/__init__.py` & `google-cloud-redis-2.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/tests/unit/__init__.py` & `google-cloud-redis-2.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/tests/unit/gapic/__init__.py` & `google-cloud-redis-2.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1/__init__.py` & `google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1/test_cloud_redis.py` & `google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1/test_cloud_redis.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1beta1/__init__.py` & `google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-redis-2.9.2/tests/unit/gapic/redis_v1beta1/test_cloud_redis.py` & `google-cloud-redis-2.9.3/tests/unit/gapic/redis_v1beta1/test_cloud_redis.py`

 * *Files identical despite different names*

