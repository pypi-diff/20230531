# Comparing `tmp/google-cloud-deploy-1.8.0.tar.gz` & `tmp/google-cloud-deploy-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-deploy-1.8.0.tar", last modified: Mon Mar 27 15:07:04 2023, max compression
+gzip compressed data, was "google-cloud-deploy-1.9.0.tar", last modified: Wed May 31 20:47:44 2023, max compression
```

## Comparing `google-cloud-deploy-1.8.0.tar` & `google-cloud-deploy-1.9.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.654127 google-cloud-deploy-1.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4614 2023-03-27 15:07:04.654127 google-cloud-deploy-1.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3701 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.642121 google-cloud-deploy-1.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.642121 google-cloud-deploy-1.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.646123 google-cloud-deploy-1.8.0/google/cloud/deploy/
--rw-rw-r--   0 root         (0)     1003     6018 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.646123 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/
--rw-rw-r--   0 root         (0)     1003     5702 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10242 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.646123 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.646123 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/
--rw-rw-r--   0 root         (0)     1003      757 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/__init__.py
--rw-rw-r--   0 root         (0)     1003   160622 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/async_client.py
--rw-rw-r--   0 root         (0)     1003   176442 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/client.py
--rw-rw-r--   0 root         (0)     1003    25718 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.650125 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    23736 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/base.py
--rw-rw-r--   0 root         (0)     1003    49492 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    50496 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   176296 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.650125 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/
--rw-rw-r--   0 root         (0)     1003     5372 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003   129387 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/cloud_deploy.py
--rw-rw-r--   0 root         (0)     1003     1838 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/deliverypipeline_notification_payload.py
--rw-rw-r--   0 root         (0)     1003     2391 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/jobrun_notification_payload.py
--rw-rw-r--   0 root         (0)     1003     1406 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/log_enums.py
--rw-rw-r--   0 root         (0)     1003     1767 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/release_notification_payload.py
--rw-rw-r--   0 root         (0)     1003     1493 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/release_render_payload.py
--rw-rw-r--   0 root         (0)     1003     2267 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/rollout_notification_payload.py
--rw-rw-r--   0 root         (0)     1003     1760 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/target_notification_payload.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.650125 google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/
--rw-r--r--   0 root         (0)     1003     4614 2023-03-27 15:07:04.000000 google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1861 2023-03-27 15:07:04.000000 google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:07:04.000000 google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:07:04.000000 google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:07:04.000000 google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:07:04.000000 google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:07:04.000000 google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:07:04.654127 google-cloud-deploy-1.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2964 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.650125 google-cloud-deploy-1.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.650125 google-cloud-deploy-1.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.650125 google-cloud-deploy-1.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:07:04.654127 google-cloud-deploy-1.8.0/tests/unit/gapic/deploy_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/tests/unit/gapic/deploy_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   702329 2023-03-27 15:05:04.000000 google-cloud-deploy-1.8.0/tests/unit/gapic/deploy_v1/test_cloud_deploy.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.738395 google-cloud-deploy-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4614 2023-05-31 20:47:44.738395 google-cloud-deploy-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3701 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.726399 google-cloud-deploy-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.726399 google-cloud-deploy-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.730398 google-cloud-deploy-1.9.0/google/cloud/deploy/
+-rw-rw-r--   0 root         (0)     1003     6060 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.730398 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/
+-rw-rw-r--   0 root         (0)     1003     5744 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10242 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.730398 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.730398 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/
+-rw-rw-r--   0 root         (0)     1003      757 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/__init__.py
+-rw-rw-r--   0 root         (0)     1003   160622 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/async_client.py
+-rw-rw-r--   0 root         (0)     1003   176442 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/client.py
+-rw-rw-r--   0 root         (0)     1003    25718 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.730398 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    23736 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    49492 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    50496 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   176296 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.734396 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5414 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003   130658 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/cloud_deploy.py
+-rw-rw-r--   0 root         (0)     1003     1838 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/deliverypipeline_notification_payload.py
+-rw-rw-r--   0 root         (0)     1003     2391 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/jobrun_notification_payload.py
+-rw-rw-r--   0 root         (0)     1003     1406 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/log_enums.py
+-rw-rw-r--   0 root         (0)     1003     1767 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/release_notification_payload.py
+-rw-rw-r--   0 root         (0)     1003     1493 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/release_render_payload.py
+-rw-rw-r--   0 root         (0)     1003     2267 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/rollout_notification_payload.py
+-rw-rw-r--   0 root         (0)     1003     1760 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/target_notification_payload.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.734396 google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/
+-rw-r--r--   0 root         (0)     1003     4614 2023-05-31 20:47:44.000000 google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1861 2023-05-31 20:47:44.000000 google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:47:44.000000 google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-31 20:47:44.000000 google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:47:44.000000 google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-05-31 20:47:44.000000 google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:47:44.000000 google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:47:44.738395 google-cloud-deploy-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2964 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.734396 google-cloud-deploy-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.734396 google-cloud-deploy-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.734396 google-cloud-deploy-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:47:44.734396 google-cloud-deploy-1.9.0/tests/unit/gapic/deploy_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/tests/unit/gapic/deploy_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   702329 2023-05-31 20:45:49.000000 google-cloud-deploy-1.9.0/tests/unit/gapic/deploy_v1/test_cloud_deploy.py
```

### Comparing `google-cloud-deploy-1.8.0/LICENSE` & `google-cloud-deploy-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/MANIFEST.in` & `google-cloud-deploy-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/PKG-INFO` & `google-cloud-deploy-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-deploy
-Version: 1.8.0
+Version: 1.9.0
 Summary: Google Cloud Deploy API client library
 Home-page: https://github.com/googleapis/python-deploy
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-deploy-1.8.0/README.rst` & `google-cloud-deploy-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy/__init__.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     CreateRolloutRequest,
     CreateTargetRequest,
     CustomCanaryDeployment,
     DefaultPool,
     DeleteDeliveryPipelineRequest,
     DeleteTargetRequest,
     DeliveryPipeline,
+    DeployArtifact,
     DeployJob,
     DeployJobRun,
     DeployJobRunMetadata,
     DeploymentJobs,
     ExecutionConfig,
     GetConfigRequest,
     GetDeliveryPipelineRequest,
@@ -159,14 +160,15 @@
     "CreateRolloutRequest",
     "CreateTargetRequest",
     "CustomCanaryDeployment",
     "DefaultPool",
     "DeleteDeliveryPipelineRequest",
     "DeleteTargetRequest",
     "DeliveryPipeline",
+    "DeployArtifact",
     "DeployJob",
     "DeployJobRun",
     "DeployJobRunMetadata",
     "DeploymentJobs",
     "ExecutionConfig",
     "GetConfigRequest",
     "GetDeliveryPipelineRequest",
```

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy/gapic_version.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy/gapic_version.py`

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
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/__init__.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     CreateRolloutRequest,
     CreateTargetRequest,
     CustomCanaryDeployment,
     DefaultPool,
     DeleteDeliveryPipelineRequest,
     DeleteTargetRequest,
     DeliveryPipeline,
+    DeployArtifact,
     DeployJob,
     DeployJobRun,
     DeployJobRunMetadata,
     DeploymentJobs,
     ExecutionConfig,
     GetConfigRequest,
     GetDeliveryPipelineRequest,
@@ -149,14 +150,15 @@
     "CreateTargetRequest",
     "CustomCanaryDeployment",
     "DefaultPool",
     "DeleteDeliveryPipelineRequest",
     "DeleteTargetRequest",
     "DeliveryPipeline",
     "DeliveryPipelineNotificationEvent",
+    "DeployArtifact",
     "DeployJob",
     "DeployJobRun",
     "DeployJobRunMetadata",
     "DeploymentJobs",
     "ExecutionConfig",
     "GetConfigRequest",
     "GetDeliveryPipelineRequest",
```

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/gapic_metadata.json` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/gapic_version.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/gapic_version.py`

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
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/__init__.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/__init__.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/async_client.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/client.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/pagers.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/__init__.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/base.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/grpc.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/grpc_asyncio.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/services/cloud_deploy/transports/rest.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/services/cloud_deploy/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/__init__.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     CreateRolloutRequest,
     CreateTargetRequest,
     CustomCanaryDeployment,
     DefaultPool,
     DeleteDeliveryPipelineRequest,
     DeleteTargetRequest,
     DeliveryPipeline,
+    DeployArtifact,
     DeployJob,
     DeployJobRun,
     DeployJobRunMetadata,
     DeploymentJobs,
     ExecutionConfig,
     GetConfigRequest,
     GetDeliveryPipelineRequest,
@@ -137,14 +138,15 @@
     "CreateRolloutRequest",
     "CreateTargetRequest",
     "CustomCanaryDeployment",
     "DefaultPool",
     "DeleteDeliveryPipelineRequest",
     "DeleteTargetRequest",
     "DeliveryPipeline",
+    "DeployArtifact",
     "DeployJob",
     "DeployJobRun",
     "DeployJobRunMetadata",
     "DeploymentJobs",
     "ExecutionConfig",
     "GetConfigRequest",
     "GetDeliveryPipelineRequest",
```

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/cloud_deploy.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/cloud_deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         "GetTargetRequest",
         "CreateTargetRequest",
         "UpdateTargetRequest",
         "DeleteTargetRequest",
         "Release",
         "BuildArtifact",
         "TargetArtifact",
+        "DeployArtifact",
         "CloudRunRenderMetadata",
         "RenderMetadata",
         "ListReleasesRequest",
         "ListReleasesResponse",
         "GetReleaseRequest",
         "CreateReleaseRequest",
         "Rollout",
@@ -2158,24 +2159,32 @@
         Attributes:
             skaffold_config_path (str):
                 Output only. File path of the resolved
                 Skaffold configuration relative to the URI.
             manifest_path (str):
                 Output only. File path of the rendered
                 manifest relative to the URI.
+            job_manifests_path (str):
+                Output only. File path of the directory of
+                rendered job manifests relative to the URI. This
+                is only set if it is applicable.
         """
 
         skaffold_config_path: str = proto.Field(
             proto.STRING,
             number=1,
         )
         manifest_path: str = proto.Field(
             proto.STRING,
             number=3,
         )
+        job_manifests_path: str = proto.Field(
+            proto.STRING,
+            number=4,
+        )
 
     artifact_uri: str = proto.Field(
         proto.STRING,
         number=4,
         oneof="uri",
     )
     skaffold_config_path: str = proto.Field(
@@ -2190,14 +2199,38 @@
         proto.STRING,
         proto.MESSAGE,
         number=5,
         message=PhaseArtifact,
     )
 
 
+class DeployArtifact(proto.Message):
+    r"""The artifacts produced by a deploy operation.
+
+    Attributes:
+        artifact_uri (str):
+            Output only. URI of a directory containing
+            the artifacts. All paths are relative to this
+            location.
+        manifest_paths (MutableSequence[str]):
+            Output only. File paths of the manifests
+            applied during the deploy operation relative to
+            the URI.
+    """
+
+    artifact_uri: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    manifest_paths: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=2,
+    )
+
+
 class CloudRunRenderMetadata(proto.Message):
     r"""CloudRunRenderMetadata contains Cloud Run information associated
     with a ``Release`` render.
 
     Attributes:
         service (str):
             Output only. The name of the Cloud Run
@@ -2814,15 +2847,15 @@
 
 class DeploymentJobs(proto.Message):
     r"""Deployment job composition.
 
     Attributes:
         deploy_job (google.cloud.deploy_v1.types.Job):
             Output only. The deploy Job. This is the
-            first job run in the phase.
+            deploy job in the phase.
         verify_job (google.cloud.deploy_v1.types.Job):
             Output only. The verify Job. Runs after a
             deploy if the deploy succeeds.
     """
 
     deploy_job: "Job" = proto.Field(
         proto.MESSAGE,
@@ -3542,14 +3575,17 @@
             is in progress or if it succeeded.
         failure_message (str):
             Output only. Additional information about the
             deploy failure, if available.
         metadata (google.cloud.deploy_v1.types.DeployJobRunMetadata):
             Output only. Metadata containing information
             about the deploy job run.
+        artifact (google.cloud.deploy_v1.types.DeployArtifact):
+            Output only. The artifact of a deploy job
+            run, if available.
     """
 
     class FailureCause(proto.Enum):
         r"""Well-known deploy failures.
 
         Values:
             FAILURE_CAUSE_UNSPECIFIED (0):
@@ -3594,14 +3630,19 @@
         number=3,
     )
     metadata: "DeployJobRunMetadata" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="DeployJobRunMetadata",
     )
+    artifact: "DeployArtifact" = proto.Field(
+        proto.MESSAGE,
+        number=5,
+        message="DeployArtifact",
+    )
 
 
 class VerifyJobRun(proto.Message):
     r"""VerifyJobRun contains information specific to a verify ``JobRun``.
 
     Attributes:
         build (str):
```

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/deliverypipeline_notification_payload.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/deliverypipeline_notification_payload.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/jobrun_notification_payload.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/jobrun_notification_payload.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/log_enums.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/log_enums.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/release_notification_payload.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/release_notification_payload.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/release_render_payload.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/release_render_payload.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/rollout_notification_payload.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/rollout_notification_payload.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google/cloud/deploy_v1/types/target_notification_payload.py` & `google-cloud-deploy-1.9.0/google/cloud/deploy_v1/types/target_notification_payload.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/PKG-INFO` & `google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-deploy
-Version: 1.8.0
+Version: 1.9.0
 Summary: Google Cloud Deploy API client library
 Home-page: https://github.com/googleapis/python-deploy
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-deploy-1.8.0/google_cloud_deploy.egg-info/SOURCES.txt` & `google-cloud-deploy-1.9.0/google_cloud_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/setup.py` & `google-cloud-deploy-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/tests/__init__.py` & `google-cloud-deploy-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/tests/unit/__init__.py` & `google-cloud-deploy-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/tests/unit/gapic/__init__.py` & `google-cloud-deploy-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/tests/unit/gapic/deploy_v1/__init__.py` & `google-cloud-deploy-1.9.0/tests/unit/gapic/deploy_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-deploy-1.8.0/tests/unit/gapic/deploy_v1/test_cloud_deploy.py` & `google-cloud-deploy-1.9.0/tests/unit/gapic/deploy_v1/test_cloud_deploy.py`

 * *Files identical despite different names*

