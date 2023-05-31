# Comparing `tmp/google-cloud-automlops-1.1.1.tar.gz` & `tmp/google-cloud-automlops-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-automlops-1.1.1.tar", last modified: Tue May 16 17:39:33 2023, max compression
+gzip compressed data, was "google-cloud-automlops-1.1.2.tar", last modified: Wed May 31 20:15:39 2023, max compression
```

## Comparing `google-cloud-automlops-1.1.1.tar` & `google-cloud-automlops-1.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.211176 google-cloud-automlops-1.1.1/
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.200431 google-cloud-automlops-1.1.1/AutoMLOps/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    15403 2023-05-16 14:47:23.000000 google-cloud-automlops-1.1.1/AutoMLOps/AutoMLOps.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-05-12 15:42:26.000000 google-cloud-automlops-1.1.1/AutoMLOps/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.200853 google-cloud-automlops-1.1.1/AutoMLOps/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:44:02.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.201602 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:44:07.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2258 2023-05-12 20:14:34.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.202142 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/constructs/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        0 2023-05-10 19:53:15.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/constructs/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9302 2023-05-15 18:22:07.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/constructs/scripts.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.202879 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:43:10.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2271 2023-05-12 18:33:19.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/base.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.203927 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:43:27.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11973 2023-05-12 20:11:24.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.205923 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:43:45.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20675 2023-05-12 18:34:14.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/cloudrun.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3421 2023-05-12 18:34:54.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/component.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8842 2023-05-12 18:37:02.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/pipeline.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    31558 2023-05-15 18:21:03.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/scripts.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8702 2023-05-12 18:55:25.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/scaffold.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.207291 google-cloud-automlops-1.1.1/AutoMLOps/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:34:44.000000 google-cloud-automlops-1.1.1/AutoMLOps/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3231 2023-05-16 15:37:55.000000 google-cloud-automlops-1.1.1/AutoMLOps/utils/constants.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9583 2023-05-10 20:13:43.000000 google-cloud-automlops-1.1.1/AutoMLOps/utils/utils.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.1/LICENSE
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14196 2023-05-16 17:39:33.211001 google-cloud-automlops-1.1.1/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13327 2023-05-11 17:20:14.000000 google-cloud-automlops-1.1.1/README.md
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.208212 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14196 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1265 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/SOURCES.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/dependency_links.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/requires.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       16 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/top_level.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-05-16 17:39:33.211225 google-cloud-automlops-1.1.1/setup.cfg
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1949 2023-05-12 18:42:41.000000 google-cloud-automlops-1.1.1/setup.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.208356 google-cloud-automlops-1.1.1/tests/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:34:44.000000 google-cloud-automlops-1.1.1/tests/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.209048 google-cloud-automlops-1.1.1/tests/unit/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      702 2023-02-07 20:59:28.000000 google-cloud-automlops-1.1.1/tests/unit/AutoMLOps_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:22:39.000000 google-cloud-automlops-1.1.1/tests/unit/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.209424 google-cloud-automlops-1.1.1/tests/unit/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:22:44.000000 google-cloud-automlops-1.1.1/tests/unit/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.209799 google-cloud-automlops-1.1.1/tests/unit/frameworks/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:22:57.000000 google-cloud-automlops-1.1.1/tests/unit/frameworks/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.210113 google-cloud-automlops-1.1.1/tests/unit/frameworks/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:23:03.000000 google-cloud-automlops-1.1.1/tests/unit/frameworks/kfp/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.210660 google-cloud-automlops-1.1.1/tests/unit/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:23:13.000000 google-cloud-automlops-1.1.1/tests/unit/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11516 2023-05-15 19:11:22.000000 google-cloud-automlops-1.1.1/tests/unit/utils/utils_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.844866 google-cloud-automlops-1.1.2/
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.837869 google-cloud-automlops-1.1.2/AutoMLOps/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    15625 2023-05-31 14:59:43.000000 google-cloud-automlops-1.1.2/AutoMLOps/AutoMLOps.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-05-30 16:10:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.838063 google-cloud-automlops-1.1.2/AutoMLOps/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.838674 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2258 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.839003 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        0 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9302 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/constructs/scripts.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.839460 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2271 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/base.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.840225 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11141 2023-05-31 15:01:47.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.841402 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20675 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/cloudrun.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3711 2023-05-31 15:06:44.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/component.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8842 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/pipeline.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    24885 2023-05-30 13:56:22.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/scripts.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8731 2023-05-31 14:09:50.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/scaffold.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.842058 google-cloud-automlops-1.1.2/AutoMLOps/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3167 2023-05-31 14:13:28.000000 google-cloud-automlops-1.1.2/AutoMLOps/utils/constants.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9886 2023-05-31 15:19:43.000000 google-cloud-automlops-1.1.2/AutoMLOps/utils/utils.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.2/LICENSE
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13880 2023-05-31 20:15:39.844672 google-cloud-automlops-1.1.2/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13012 2023-05-31 17:17:30.000000 google-cloud-automlops-1.1.2/README.md
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.842846 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13880 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1265 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/SOURCES.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/dependency_links.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/requires.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       16 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/top_level.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-05-31 20:15:39.844920 google-cloud-automlops-1.1.2/setup.cfg
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1949 2023-05-30 16:09:56.000000 google-cloud-automlops-1.1.2/setup.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.842996 google-cloud-automlops-1.1.2/tests/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.843382 google-cloud-automlops-1.1.2/tests/unit/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      702 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/AutoMLOps_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.843562 google-cloud-automlops-1.1.2/tests/unit/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.843748 google-cloud-automlops-1.1.2/tests/unit/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/frameworks/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.843945 google-cloud-automlops-1.1.2/tests/unit/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/frameworks/kfp/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.844317 google-cloud-automlops-1.1.2/tests/unit/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11523 2023-05-30 14:04:41.000000 google-cloud-automlops-1.1.2/tests/unit/utils/utils_test.py
```

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/AutoMLOps.py` & `google-cloud-automlops-1.1.2/AutoMLOps/AutoMLOps.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,21 @@
 from AutoMLOps.frameworks.kfp import builder as KfpBuilder
 from AutoMLOps.frameworks.kfp import scaffold as KfpScaffold
 from AutoMLOps.deployments.cloudbuild import builder as CloudBuildBuilder
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format='%(message)s')
 logger = logging.getLogger()
 
+make_dirs([OUTPUT_DIR])
+
 def go(project_id: str,
        pipeline_params: Dict,
        af_registry_location: Optional[str] = 'us-central1',
        af_registry_name: Optional[str] = 'vertex-mlops-af',
+       base_image: Optional[str] = 'python:3.9-slim',
        cb_trigger_location: Optional[str] = 'us-central1',
        cb_trigger_name: Optional[str] = 'automlops-trigger',
        cloud_run_location: Optional[str] = 'us-central1',
        cloud_run_name: Optional[str] = 'run-pipeline',
        cloud_tasks_queue_location: Optional[str] = 'us-central1',
        cloud_tasks_queue_name: Optional[str] = 'queueing-svc',
        csr_branch_name: Optional[str] = 'automlops',
@@ -62,24 +65,24 @@
        gs_bucket_location: Optional[str] = 'us-central1',
        gs_bucket_name: Optional[str] = None,
        pipeline_runner_sa: Optional[str] = None,
        run_local: Optional[bool] = True,
        schedule_location: Optional[str] = 'us-central1',
        schedule_name: Optional[str] = 'AutoMLOps-schedule',
        schedule_pattern: Optional[str] = 'No Schedule Specified',
-       use_kfp_spec: Optional[bool] = False,
        vpc_connector: Optional[str] = 'No VPC Specified'):
     """Generates relevant pipeline and component artifacts,
        then builds, compiles, and submits the PipelineJob.
 
     Args:
         project_id: The project ID.
         pipeline_params: Dictionary containing runtime pipeline parameters.
         af_registry_location: Region of the Artifact Registry.
         af_registry_name: Artifact Registry name where components are stored.
+        base_image: The image to use in the component base dockerfile.
         cb_trigger_location: The location of the cloudbuild trigger.
         cb_trigger_name: The name of the cloudbuild trigger.
         cloud_run_location: The location of the cloud runner service.
         cloud_run_name: The name of the cloud runner service.
         cloud_tasks_queue_location: The location of the cloud tasks queue.
         cloud_tasks_queue_name: The name of the cloud tasks queue.
         csr_branch_name: The name of the csr branch to push to to trigger cb job.
@@ -88,31 +91,30 @@
         gs_bucket_location: Region of the GS bucket.
         gs_bucket_name: GS bucket name where pipeline run metadata is stored.
         pipeline_runner_sa: Service Account to runner PipelineJobs.
         run_local: Flag that determines whether to use Cloud Run CI/CD.
         schedule_location: The location of the scheduler resource.
         schedule_name: The name of the scheduler resource.
         schedule_pattern: Cron formatted value used to create a Scheduled retrain job.
-        use_kfp_spec: Flag that determines the format of the component yamls.
         vpc_connector: The name of the vpc connector to use.
     """
     generate(project_id, pipeline_params, af_registry_location,
-             af_registry_name, cb_trigger_location, cb_trigger_name,
+             af_registry_name, base_image, cb_trigger_location, cb_trigger_name,
              cloud_run_location, cloud_run_name, cloud_tasks_queue_location,
              cloud_tasks_queue_name, csr_branch_name, csr_name,
              custom_training_job_specs, gs_bucket_location, gs_bucket_name,
              pipeline_runner_sa, run_local, schedule_location,
-             schedule_name, schedule_pattern, use_kfp_spec,
-             vpc_connector)
+             schedule_name, schedule_pattern, vpc_connector)
     run(run_local)
 
 def generate(project_id: str,
              pipeline_params: Dict,
              af_registry_location: Optional[str] = 'us-central1',
              af_registry_name: Optional[str] = 'vertex-mlops-af',
+             base_image: Optional[str] = 'python:3.9-slim',
              cb_trigger_location: Optional[str] = 'us-central1',
              cb_trigger_name: Optional[str] = 'automlops-trigger',
              cloud_run_location: Optional[str] = 'us-central1',
              cloud_run_name: Optional[str] = 'run-pipeline',
              cloud_tasks_queue_location: Optional[str] = 'us-central1',
              cloud_tasks_queue_name: Optional[str] = 'queueing-svc',
              csr_branch_name: Optional[str] = 'automlops',
@@ -121,15 +123,14 @@
              gs_bucket_location: Optional[str] = 'us-central1',
              gs_bucket_name: Optional[str] = None,
              pipeline_runner_sa: Optional[str] = None,
              run_local: Optional[bool] = True,
              schedule_location: Optional[str] = 'us-central1',
              schedule_name: Optional[str] = 'AutoMLOps-schedule',
              schedule_pattern: Optional[str] = 'No Schedule Specified',
-             use_kfp_spec: Optional[bool] = False,
              vpc_connector: Optional[str] = 'No VPC Specified'):
     """Generates relevant pipeline and component artifacts.
 
     Args: See go() function.
     """
     # Validate that run_local=False if schedule_pattern parameter is set
     validate_schedule(schedule_pattern, run_local)
@@ -141,21 +142,20 @@
     # Make necessary directories
     make_dirs(GENERATED_DIRS)
 
     # Switch statement to go here for different frameworks and deployments:
 
     # Build files required to run a Kubeflow Pipeline
     KfpBuilder.build(project_id, pipeline_params, af_registry_location,
-        af_registry_name, cb_trigger_location, cb_trigger_name,
+        af_registry_name, base_image, cb_trigger_location, cb_trigger_name,
         cloud_run_location, cloud_run_name, cloud_tasks_queue_location,
         cloud_tasks_queue_name, csr_branch_name, csr_name,
         custom_training_job_specs, gs_bucket_location, default_bucket_name,
         default_pipeline_runner_sa, run_local, schedule_location,
-        schedule_name, schedule_pattern, use_kfp_spec,
-        vpc_connector)
+        schedule_name, schedule_pattern, vpc_connector)
 
     CloudBuildBuilder.build(af_registry_location, af_registry_name, cloud_run_location,
         cloud_run_name, default_pipeline_runner_sa, project_id,
         run_local, schedule_pattern, vpc_connector)
 
 def run(run_local: bool):
     """Builds, compiles, and submits the PipelineJob.
@@ -303,7 +303,13 @@
             name=name,
             description=description)
     else:
         return KfpScaffold.create_pipeline_scaffold(
             func=func,
             name=name,
             description=description)
+
+def clear_cache():
+    """Deletes all temporary files stored in the cache directory."""
+    execute_process(f'rm -rf {OUTPUT_DIR}', to_null=False)
+    make_dirs([OUTPUT_DIR])
+    logging.info('Cache cleared.')
```

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/__init__.py` & `google-cloud-automlops-1.1.2/AutoMLOps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 import, with the end goal of becoming a Jupyter plugin to Vertex
 Workbench managed notebooks. The tool will generate yaml-component
 definitions, complete with Dockerfiles and requirements.txts for all
 Kubeflow components defined in a notebook. It will also generate a
 series of directories to support the creation of Vertex Pipelines.
 """
 # pylint: disable=invalid-name
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 __author__ = 'Sean Rastatter'
 __credits__ = 'Google'
```

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/deployments/__init__.py` & `google-cloud-automlops-1.1.2/AutoMLOps/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/__init__.py` & `google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/builder.py` & `google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/builder.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/constructs/scripts.py` & `google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/constructs/scripts.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/__init__.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/base.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/__init__.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/builder.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,43 +20,43 @@
 
 from typing import Dict, List, Optional
 from AutoMLOps.utils.utils import (
     execute_process,
     get_components_list,
     make_dirs,
     read_yaml_file,
+    is_using_kfp_spec,
     write_and_chmod,
     write_file,
     write_yaml_file
 )
 from AutoMLOps.utils.constants import (
     BASE_DIR,
-    DEFAULT_IMAGE,
     GENERATED_BUILD_COMPONENTS_SH_FILE,
-    GENERATED_CLOUDBUILD_FILE,
     GENERATED_DEFAULTS_FILE,
     GENERATED_COMPONENT_BASE,
     GENERATED_PIPELINE_FILE,
     GENERATED_PIPELINE_SPEC_SH_FILE,
     GENERATED_RESOURCES_SH_FILE,
     GENERATED_RUN_PIPELINE_SH_FILE,
     GENERATED_RUN_ALL_SH_FILE,
-    PIPELINE_TMPFILE,
+    PIPELINE_CACHE_FILE,
     GENERATED_LICENSE,
     GENERATED_PARAMETER_VALUES_PATH
 )
 from AutoMLOps.frameworks.kfp.constructs.cloudrun import KfpCloudRun
 from AutoMLOps.frameworks.kfp.constructs.component import KfpComponent
 from AutoMLOps.frameworks.kfp.constructs.pipeline import KfpPipeline
 from AutoMLOps.frameworks.kfp.constructs.scripts import KfpScripts
 
 def build(project_id: str,
           pipeline_params: Dict,
           af_registry_location: Optional[str],
           af_registry_name: Optional[str],
+          base_image: Optional[str],
           cb_trigger_location: Optional[str],
           cb_trigger_name: Optional[str],
           cloud_run_location: Optional[str],
           cloud_run_name: Optional[str],
           cloud_tasks_queue_location: Optional[str],
           cloud_tasks_queue_name: Optional[str],
           csr_branch_name: Optional[str],
@@ -65,117 +65,107 @@
           gs_bucket_location: Optional[str],
           gs_bucket_name: Optional[str],
           pipeline_runner_sa: Optional[str],
           run_local: Optional[bool],
           schedule_location: Optional[str],
           schedule_name: Optional[str],
           schedule_pattern: Optional[str],
-          use_kfp_spec: Optional[bool],
           vpc_connector: Optional[str]):
     """Constructs scripts for resource deployment and running Kubeflow pipelines.
 
     Args:
         af_registry_location: Region of the Artifact Registry.
         af_registry_name: Artifact Registry name where components are stored.
+        base_image: The image to use in the component base dockerfile.
         cb_trigger_location: The location of the cloudbuild trigger.
         cb_trigger_name: The name of the cloudbuild trigger.
         cloud_run_location: The location of the cloud runner service.
         cloud_run_name: The name of the cloud runner service.
         cloud_tasks_queue_location: The location of the cloud tasks queue.
         cloud_tasks_queue_name: The name of the cloud tasks queue.
         csr_branch_name: The name of the csr branch to push to to trigger cb job.
         csr_name: The name of the cloud source repo to use.
-        default_image: The image to use in the dockerfile.
         gs_bucket_location: Region of the GS bucket.
         gs_bucket_name: GS bucket name where pipeline run metadata is stored.
         pipeline_runner_sa: Service Account to runner PipelineJobs.
         project_id: The project ID.
         run_local: Flag that determines whether to use Cloud Run CI/CD.
         schedule_location: The location of the scheduler resource.
         schedule_name: The name of the scheduler resource.
         schedule_pattern: Cron formatted value used to create a Scheduled retrain job.
-        base_dir: Top directory name.
         vpc_connector: The name of the vpc connector to use.
     """
 
     # Get scripts builder object
     kfp_scripts = KfpScripts(
-        af_registry_location, af_registry_name, cb_trigger_location,
+        af_registry_location, af_registry_name, base_image, cb_trigger_location,
         cb_trigger_name, cloud_run_location, cloud_run_name,
         cloud_tasks_queue_location, cloud_tasks_queue_name, csr_branch_name,
-        csr_name, DEFAULT_IMAGE, gs_bucket_location, gs_bucket_name,
+        csr_name, gs_bucket_location, gs_bucket_name,
         pipeline_runner_sa, project_id, run_local, schedule_location,
         schedule_name, schedule_pattern, BASE_DIR, vpc_connector)
 
     # Write defaults.yaml
     write_file(GENERATED_DEFAULTS_FILE, kfp_scripts.defaults, 'w+')
 
     # Write scripts for building pipeline, building components, running pipeline, and running all files
     write_and_chmod(GENERATED_PIPELINE_SPEC_SH_FILE, kfp_scripts.build_pipeline_spec)
     write_and_chmod(GENERATED_BUILD_COMPONENTS_SH_FILE, kfp_scripts.build_components)
     write_and_chmod(GENERATED_RUN_PIPELINE_SH_FILE, kfp_scripts.run_pipeline)
     write_and_chmod(GENERATED_RUN_ALL_SH_FILE, kfp_scripts.run_all)
 
-    # Write scripts to create resources and cloud build config
+    # Write scripts to create resources
     write_and_chmod(GENERATED_RESOURCES_SH_FILE, kfp_scripts.create_resources_script)
-    write_file(GENERATED_CLOUDBUILD_FILE, kfp_scripts.create_cloudbuild_config, 'w+')
 
     # Copy tmp pipeline file over to AutoMLOps directory
-    execute_process(f'cp {PIPELINE_TMPFILE} {GENERATED_PIPELINE_FILE}', to_null=False)
+    execute_process(f'cp {PIPELINE_CACHE_FILE} {GENERATED_PIPELINE_FILE}', to_null=False)
 
     # Create components and pipelines
     components_path_list = get_components_list()
     for path in components_path_list:
-        build_component(path, BASE_DIR, GENERATED_DEFAULTS_FILE, use_kfp_spec)
-    build_pipeline(custom_training_job_specs, GENERATED_DEFAULTS_FILE, pipeline_params, BASE_DIR)
+        build_component(path)
+    build_pipeline(custom_training_job_specs, pipeline_params)
 
     # Write dockerfile to the component base directory
     write_file(f'{GENERATED_COMPONENT_BASE}/Dockerfile', kfp_scripts.dockerfile, 'w')
 
     # Write requirements.txt to the component base directory
     write_file(f'{GENERATED_COMPONENT_BASE}/requirements.txt', kfp_scripts.requirements, 'w')
 
     # Build the cloud run files
     if not run_local:
-        build_cloudrun(BASE_DIR, GENERATED_DEFAULTS_FILE)
+        build_cloudrun()
 
-
-def build_component(component_path: str,
-                    base_dir: str,
-                    defaults_file: str,
-                    use_kfp_spec: bool):
+def build_component(component_path: str):
     """Constructs and writes component.yaml and {component_name}.py files.
         component.yaml: Contains the Kubeflow custom component definition.
         {component_name}.py: Contains the python code from the Jupyter cell.
 
     Args:
         component_path: Path to the temporary component yaml. This file
             is used to create the permanent component.yaml, and deleted
             after calling AutoMLOps.generate().
-        base_dir: Top directory name.
-        defaults_file: Path to the default config variables yaml.
-        use_kfp_spec: Flag that determines the format of the component yamls.
     """
     # Read in component specs
     component_spec = read_yaml_file(component_path)
 
     # If using kfp, remove spaces in name and convert to lowercase
-    if use_kfp_spec:
+    if is_using_kfp_spec(component_spec['implementation']['container']['image']):
         component_spec['name'] = component_spec['name'].replace(' ', '_').lower()
 
     # Set and create directory for component, and set directory for task
-    component_dir = base_dir + 'components/' + component_spec['name']
-    task_filepath = (base_dir
+    component_dir = BASE_DIR + 'components/' + component_spec['name']
+    task_filepath = (BASE_DIR
                      + 'components/component_base/src/'
                      + component_spec['name']
                      + '.py')
     make_dirs([component_dir])
 
     # Initialize component scripts builder
-    kfp_comp = KfpComponent(component_spec, defaults_file)
+    kfp_comp = KfpComponent(component_spec, GENERATED_DEFAULTS_FILE)
 
     # Write task script to component base
     write_file(task_filepath, kfp_comp.task, 'w+')
 
     # Update component_spec to include correct image and startup command
     component_spec['implementation']['container']['image'] = kfp_comp.compspec_image
     component_spec['implementation']['container']['command'] = [
@@ -183,39 +173,34 @@
         f'''/pipelines/component/src/{component_spec['name']+'.py'}''']
 
     # Write license and component spec to the appropriate component.yaml file
     filename = component_dir + '/component.yaml'
     write_file(filename, GENERATED_LICENSE, 'w')
     write_yaml_file(filename, component_spec, 'a')
 
-
 def build_pipeline(custom_training_job_specs: List[Dict],
-                   defaults_file: str,
-                   pipeline_parameter_values: dict,
-                   base_dir: str):
+                   pipeline_parameter_values: dict):
     """Constructs and writes pipeline.py, pipeline_runner.py, and pipeline_parameter_values.json files.
         pipeline.py: Generates a Kubeflow pipeline spec from custom components.
         pipeline_runner.py: Sends a PipelineJob to Vertex AI using pipeline spec.
         pipeline_parameter_values.json: Provides runtime parameters for the PipelineJob.
 
     Args:
         custom_training_job_specs: Specifies the specs to run the training job with.
-        defaults_file: Path to the default config variables yaml.
         pipeline_parameter_values: Dictionary of runtime parameters for the PipelineJob.
-        base_dir: Top directory name.
     Raises:
         Exception: If an error is encountered reading/writing to a file.
     """
     # Set paths
-    pipeline_file = base_dir + 'pipelines/pipeline.py'
-    pipeline_runner_file = base_dir + 'pipelines/pipeline_runner.py'
-    pipeline_params_file = base_dir + GENERATED_PARAMETER_VALUES_PATH
+    pipeline_file = BASE_DIR + 'pipelines/pipeline.py'
+    pipeline_runner_file = BASE_DIR + 'pipelines/pipeline_runner.py'
+    pipeline_params_file = BASE_DIR + GENERATED_PARAMETER_VALUES_PATH
 
     # Initializes pipeline scripts builder
-    kfp_pipeline = KfpPipeline(custom_training_job_specs, defaults_file)
+    kfp_pipeline = KfpPipeline(custom_training_job_specs, GENERATED_DEFAULTS_FILE)
     try:
         with open(pipeline_file, 'r+', encoding='utf-8') as file:
             pipeline_scaffold = file.read()
             file.seek(0, 0)
             file.write(GENERATED_LICENSE)
             file.write(kfp_pipeline.pipeline_imports)
             for line in pipeline_scaffold.splitlines():
@@ -228,44 +213,39 @@
     # Construct pipeline_runner.py
     write_file(pipeline_runner_file, kfp_pipeline.pipeline_runner, 'w+')
 
     # Construct pipeline_parameter_values.json
     serialized_params = json.dumps(pipeline_parameter_values, indent=4)
     write_file(pipeline_params_file, serialized_params, 'w+')
 
-def build_cloudrun(base_dir: str,
-                   defaults_file: str,):
+def build_cloudrun():
     """Constructs and writes a Dockerfile, requirements.txt, and
        main.py to the cloud_run/run_pipeline directory. Also
        constructs and writes a main.py, requirements.txt, and
        pipeline_parameter_values.json to the
        cloud_run/queueing_svc directory.
-
-    Args:
-        base_dir: Top directory name.
-        defaults_file: Path to the default config variables yaml.
     """
     # Make new directories
-    make_dirs([base_dir + 'cloud_run',
-               base_dir + 'cloud_run/run_pipeline',
-               base_dir + 'cloud_run/queueing_svc'])
+    make_dirs([BASE_DIR + 'cloud_run',
+               BASE_DIR + 'cloud_run/run_pipeline',
+               BASE_DIR + 'cloud_run/queueing_svc'])
 
     # Initialize cloud run scripts object
-    cloudrun_scripts = KfpCloudRun(defaults_file)
+    cloudrun_scripts = KfpCloudRun(GENERATED_DEFAULTS_FILE)
 
     # Set new folders as variables
-    cloudrun_base = base_dir + 'cloud_run/run_pipeline'
-    queueing_svc_base = base_dir + 'cloud_run/queueing_svc'
+    cloudrun_base = BASE_DIR + 'cloud_run/run_pipeline'
+    queueing_svc_base = BASE_DIR + 'cloud_run/queueing_svc'
 
     # Write cloud run dockerfile
     write_file(f'{cloudrun_base}/Dockerfile', cloudrun_scripts.dockerfile, 'w')
 
     # Write requirements files for cloud run base and queueing svc
     write_file(f'{cloudrun_base}/requirements.txt', cloudrun_scripts.cloudrun_base_reqs, 'w')
     write_file(f'{queueing_svc_base}/requirements.txt', cloudrun_scripts.queueing_svc_reqs, 'w')
 
     # Write main code files for cloud run base and queueing svc
     write_file(f'{cloudrun_base}/main.py', cloudrun_scripts.cloudrun_base, 'w')
     write_file(f'{queueing_svc_base}/main.py', cloudrun_scripts.queueing_svc, 'w')
 
     # Copy runtime parameters over to queueing_svc dir
-    execute_process(f'''cp -r {base_dir + GENERATED_PARAMETER_VALUES_PATH} {base_dir + 'cloud_run/queueing_svc'}''', to_null=False)
+    execute_process(f'''cp -r {BASE_DIR + GENERATED_PARAMETER_VALUES_PATH} {BASE_DIR + 'cloud_run/queueing_svc'}''', to_null=False)
```

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/__init__.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/cloudrun.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/cloudrun.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/component.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """Code strings for a kfp component."""
 
 # pylint: disable=line-too-long
 
 from AutoMLOps.utils.constants import GENERATED_LICENSE
+from AutoMLOps.utils.utils import is_using_kfp_spec
 from AutoMLOps.frameworks.base import Component
 
 class KfpComponent(Component):
     """Child class that generates files related to kfp components."""
     def __init__(self, component_spec: dict, defaults_file: str):
         """Instantiate Component scripts object with all necessary attributes.
 
@@ -38,24 +39,27 @@
     def _create_task(self):
         """Creates the content of the cell python code to be written to a file with required imports.
 
         Returns:
             str: Contents of component base source code.
         """
         custom_code = self._component_spec['implementation']['container']['command'][-1]
-        default_imports = (
-            GENERATED_LICENSE +
+        default_imports = (GENERATED_LICENSE +
             'import argparse\n'
             'import json\n'
+            'from kfp.v2.components import executor\n')
+        if not is_using_kfp_spec(self._component_spec['implementation']['container']['image']):
+            custom_imports = ('\n'
             'import kfp\n'
             'from kfp.v2 import dsl\n'
-            'from kfp.v2.components import executor\n'
             'from kfp.v2.dsl import *\n'
             'from typing import *\n'
             '\n')
+        else:
+            custom_imports = '' # the above is already included as part of the kfp spec
         main_func = (
             '\n'
             '''def main():\n'''
             '''    """Main executor."""\n'''
             '''    parser = argparse.ArgumentParser()\n'''
             '''    parser.add_argument('--executor_input', type=str)\n'''
             '''    parser.add_argument('--function_to_execute', type=str)\n'''
@@ -66,15 +70,15 @@
             '\n'
             '''    executor.Executor(\n'''
             '''        executor_input=executor_input,\n'''
             '''        function_to_execute=function_to_execute).execute()\n'''
             '\n'
             '''if __name__ == '__main__':\n'''
             '''    main()\n''')
-        return default_imports + custom_code + main_func
+        return default_imports + custom_imports + custom_code + main_func
 
     def _create_compspec_image(self):
         """Write the correct image for the component spec.
 
         Returns:
             str: Component spec image.
         """
```

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/pipeline.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/pipeline.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/scripts.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/scripts.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 )
 
 class KfpScripts():
     """Generates files related to running kubeflow pipelines."""
     def __init__(self,
                  af_registry_location: str,
                  af_registry_name: str,
+                 base_image: str,
                  cb_trigger_location: str,
                  cb_trigger_name: str,
                  cloud_run_location: str,
                  cloud_run_name: str,
                  cloud_tasks_queue_location: str,
                  cloud_tasks_queue_name: str,
                  csr_branch_name: str,
                  csr_name: str,
-                 default_image: str,
                  gs_bucket_location: str,
                  gs_bucket_name: str,
                  pipeline_runner_sa: str,
                  project_id: str,
                  run_local: str,
                  schedule_location: str,
                  schedule_name: str,
@@ -68,15 +68,15 @@
             cb_trigger_name: The name of the cloudbuild trigger.
             cloud_run_location: The location of the cloud runner service.
             cloud_run_name: The name of the cloud runner service.
             cloud_tasks_queue_location: The location of the cloud tasks queue.
             cloud_tasks_queue_name: The name of the cloud tasks queue.
             csr_branch_name: The name of the csr branch to push to to trigger cb job.
             csr_name: The name of the cloud source repo to use.
-            default_image: The image to use in the dockerfile.
+            base_image: The image to use in the dockerfile.
             gs_bucket_location: Region of the GS bucket.
             gs_bucket_name: GS bucket name where pipeline run metadata is stored.
             pipeline_runner_sa: Service Account to runner PipelineJobs.
             project_id: The project ID.
             run_local: Flag that determines whether to use Cloud Run CI/CD.
             schedule_location: The location of the scheduler resource.
             schedule_name: The name of the scheduler resource.
@@ -104,23 +104,22 @@
         self.__cloud_tasks_queue_name = cloud_tasks_queue_name
         self.__vpc_connector = vpc_connector
         self.__cloud_run_name = cloud_run_name
         self.__cloud_run_location = cloud_run_location
         self.__cloud_schedule_location = schedule_location
         self.__cloud_schedule_name = schedule_name
         self.__cloud_schedule_pattern = schedule_pattern
-        self.__default_image = default_image
+        self.__base_image = base_image
 
         # Set generated scripts as public attributes
         self.build_pipeline_spec = self._build_pipeline_spec()
         self.build_components = self._build_components()
         self.run_pipeline = self._run_pipeline()
         self.run_all = self._run_all()
         self.create_resources_script = self._create_resources_script()
-        self.create_cloudbuild_config = self._create_cloudbuild_config()
         self.dockerfile = self._create_dockerfile()
         self.defaults = self._create_default_config()
         self.requirements = self._create_requirements()
 
     def _build_pipeline_spec(self):
         """Builds content of a shell script to build the pipeline specs.
 
@@ -378,151 +377,23 @@
                 f'\n'
                 f'  echo "Cloudbuild Trigger already exists in project $PROJECT_ID for repo ${LEFT_BRACKET}CLOUD_SOURCE_REPO{RIGHT_BRACKET}"\n'
                 f'\n'
                 f'fi\n')
 
         return create_resources_script
 
-    def _create_cloudbuild_config(self):
-        """Builds the content of cloudbuild.yaml.
-
-        Args:
-            str: Text content of cloudbuild.yaml.
-        """
-        vpc_connector_tail = ''
-        if self.__vpc_connector != 'No VPC Specified':
-            vpc_connector_tail = (
-                f'\n'
-                f'           "--ingress", "internal",\n'
-                f'           "--vpc-connector", "{self.__vpc_connector}",\n'
-                f'           "--vpc-egress", "all-traffic"')
-        vpc_connector_tail += ']\n'
-
-        cloudbuild_comp_config = (
-            GENERATED_LICENSE +
-            f'steps:\n'
-            f'# ==============================================================================\n'
-            f'# BUILD CUSTOM IMAGES\n'
-            f'# ==============================================================================\n'
-            f'\n'
-            f'''  # build the component_base image\n'''
-            f'''  - name: "gcr.io/cloud-builders/docker"\n'''
-            f'''    args: [ "build", "-t", "{self.__af_registry_location}-docker.pkg.dev/{self.__project_id}/{self.__af_registry_name}/components/component_base:latest", "." ]\n'''
-            f'''    dir: "{self.__base_dir}components/component_base"\n'''
-            f'''    id: "build_component_base"\n'''
-            f'''    waitFor: ["-"]\n'''
-            f'\n'
-            f'''  # build the run_pipeline image\n'''
-            f'''  - name: 'gcr.io/cloud-builders/docker'\n'''
-            f'''    args: [ "build", "-t", "{self.__af_registry_location}-docker.pkg.dev/{self.__project_id}/{self.__af_registry_name}/run_pipeline:latest", "-f", "cloud_run/run_pipeline/Dockerfile", "." ]\n'''
-            f'''    dir: "{self.__base_dir}"\n'''
-            f'''    id: "build_pipeline_runner_svc"\n'''
-            f'''    waitFor: ['build_component_base']\n''')
-
-        cloudbuild_cloudrun_config = (
-            f'\n'
-            f'# ==============================================================================\n'
-            f'# PUSH & DEPLOY CUSTOM IMAGES\n'
-            f'# ==============================================================================\n'
-            f'\n'
-            f'''  # push the component_base image\n'''
-            f'''  - name: "gcr.io/cloud-builders/docker"\n'''
-            f'''    args: ["push", "{self.__af_registry_location}-docker.pkg.dev/{self.__project_id}/{self.__af_registry_name}/components/component_base:latest"]\n'''
-            f'''    dir: "{self.__base_dir}components/component_base"\n'''
-            f'''    id: "push_component_base"\n'''
-            f'''    waitFor: ["build_pipeline_runner_svc"]\n'''
-            f'\n'
-            f'''  # push the run_pipeline image\n'''
-            f'''  - name: "gcr.io/cloud-builders/docker"\n'''
-            f'''    args: ["push", "{self.__af_registry_location}-docker.pkg.dev/{self.__project_id}/{self.__af_registry_name}/run_pipeline:latest"]\n'''
-            f'''    dir: "{self.__base_dir}"\n'''
-            f'''    id: "push_pipeline_runner_svc"\n'''
-            f'''    waitFor: ["push_component_base"]\n'''
-            f'\n'
-            f'''  # deploy the cloud run service\n'''
-            f'''  - name: "gcr.io/google.com/cloudsdktool/cloud-sdk"\n'''
-            f'''    entrypoint: gcloud\n'''
-            f'''    args: ["run",\n'''
-            f'''           "deploy",\n'''
-            f'''           "{self.__cloud_run_name}",\n'''
-            f'''           "--image",\n'''
-            f'''           "{self.__af_registry_location}-docker.pkg.dev/{self.__project_id}/{self.__af_registry_name}/run_pipeline:latest",\n'''
-            f'''           "--region",\n'''
-            f'''           "{self.__cloud_run_location}",\n'''
-            f'''           "--service-account",\n'''
-            f'''           "{self.__pipeline_runner_service_account}",{vpc_connector_tail}'''
-            f'''    id: "deploy_pipeline_runner_svc"\n'''
-            f'''    waitFor: ["push_pipeline_runner_svc"]\n'''
-            f'\n'
-            f'''  # Copy runtime parameters\n'''
-            f'''  - name: 'gcr.io/cloud-builders/gcloud'\n'''
-            f'''    entrypoint: bash\n'''
-            f'''    args:\n'''
-            f'''      - '-e'\n'''
-            f'''      - '-c'\n'''
-            f'''      - |\n'''
-            f'''        cp -r {self.__base_dir}cloud_run/queueing_svc .\n'''
-            f'''    id: "setup_queueing_svc"\n'''
-            f'''    waitFor: ["deploy_pipeline_runner_svc"]\n'''
-            f'\n'
-            f'''  # Install dependencies\n'''
-            f'''  - name: python\n'''
-            f'''    entrypoint: pip\n'''
-            f'''    args: ["install", "-r", "queueing_svc/requirements.txt", "--user"]\n'''
-            f'''    id: "install_queueing_svc_deps"\n'''
-            f'''    waitFor: ["setup_queueing_svc"]\n'''
-            f'\n'
-            f'''  # Submit to queue\n'''
-            f'''  - name: python\n'''
-            f'''    entrypoint: python\n'''
-            f'''    args: ["queueing_svc/main.py", "--setting", "queue_job"]\n'''
-            f'''    id: "submit_job_to_queue"\n'''
-            f'''    waitFor: ["install_queueing_svc_deps"]\n''')
-
-        cloudbuild_scheduler_config = (
-            '\n'
-            '''  # Create Scheduler Job\n'''
-            '''  - name: python\n'''
-            '''    entrypoint: python\n'''
-            '''    args: ["queueing_svc/main.py", "--setting", "schedule_job"]\n'''
-            '''    id: "schedule_job"\n'''
-            '''    waitFor: ["submit_job_to_queue"]\n''')
-
-        custom_comp_image = (
-            f'\n'
-            f'images:\n'
-            f'''  # custom component images\n'''
-            f'''  - "{self.__af_registry_location}-docker.pkg.dev/{self.__project_id}/{self.__af_registry_name}/components/component_base:latest"\n''')
-
-        cloudrun_image = (
-            f'''  # Cloud Run image\n'''
-            f'''  - "{self.__af_registry_location}-docker.pkg.dev/{self.__project_id}/{self.__af_registry_name}/run_pipeline:latest"\n''')
-
-        if self.__run_local:
-            cb_file_contents = cloudbuild_comp_config + custom_comp_image
-        else:
-            if self.__cloud_schedule_pattern == 'No Schedule Specified':
-                cb_file_contents = cloudbuild_comp_config + cloudbuild_cloudrun_config + custom_comp_image + cloudrun_image
-            else:
-                cb_file_contents = cloudbuild_comp_config + cloudbuild_cloudrun_config + cloudbuild_scheduler_config + custom_comp_image + cloudrun_image
-
-        return cb_file_contents
-
     def _create_dockerfile(self):
         """Creates the content of a Dockerfile to be written to the component_base directory.
 
-        Args:
-            default_image: Default image used for this process.
-
         Returns:
             str: Text content of dockerfile.
         """
         return (
             GENERATED_LICENSE +
-            f'FROM {self.__default_image}\n'
+            f'FROM {self.__base_image}\n'
             f'RUN python -m pip install --upgrade pip\n'
             f'COPY requirements.txt .\n'
             f'RUN python -m pip install -r \ \n'
             f'    requirements.txt --quiet --no-cache-dir \ \n'
             f'    && rm -f requirements.txt\n'
             f'COPY ./src /pipelines/component/src\n'
             f'ENTRYPOINT ["/bin/bash"]\n')
@@ -538,14 +409,15 @@
         return (
             GENERATED_LICENSE +
             f'# These values are descriptive only - do not change.\n'
             f'# Rerun AutoMLOps.generate() to change these values.\n'
             f'gcp:\n'
             f'  af_registry_location: {self.__af_registry_location}\n'
             f'  af_registry_name: {self.__af_registry_name}\n'
+            f'  base_image: {self.__base_image}\n'
             f'  cb_trigger_location: {self.__cb_trigger_location}\n'
             f'  cb_trigger_name: {self.__cb_trigger_name}\n'
             f'  cloud_run_location: {self.__cloud_run_location}\n'
             f'  cloud_run_name: {self.__cloud_run_name}\n'
             f'  cloud_tasks_queue_location: {self.__cloud_tasks_queue_location}\n'
             f'  cloud_tasks_queue_name: {self.__cloud_tasks_queue_name}\n'
             f'  cloud_schedule_location: {self.__cloud_schedule_location}\n'
@@ -606,15 +478,15 @@
             'db_dtypes',
             'pyarrow',
             'gcsfs',
             'fsspec']
         # Infer reqs using pipreqs
         execute_process(f'python3 -m pipreqs.pipreqs {GENERATED_COMPONENT_BASE} --mode no-pin --force', to_null=False)
         pipreqs = read_file(reqs_filename).splitlines()
-        # Get user-inputted requirements from .tmpfiles dir
+        # Get user-inputted requirements from the cache dir
         user_inp_reqs = []
         components_path_list = get_components_list()
         for component_path in components_path_list:
             component_spec = read_yaml_file(component_path)
             reqs = component_spec['implementation']['container']['command'][2]
             formatted_reqs = re.findall('\'([^\']*)\'', reqs)
             user_inp_reqs.extend(formatted_reqs)
```

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/scaffold.py` & `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/scaffold.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 import inspect
 from typing import Callable, List, Optional, TypeVar, Union
 
 import docstring_parser
 
 from AutoMLOps.utils.constants import (
     DEFAULT_PIPELINE_NAME,
-    PIPELINE_TMPFILE,
-    TMPFILES_DIR
+    PLACEHOLDER_IMAGE,
+    PIPELINE_CACHE_FILE,
+    CACHE_DIR
 )
 from AutoMLOps.utils.utils import (
     get_function_source_definition,
     make_dirs,
     update_params,
     write_file,
     write_yaml_file
@@ -61,23 +62,23 @@
     component_spec = {}
     component_spec['name'] = name
     if description:
         component_spec['description'] = description
     component_spec['inputs'] = get_function_parameters(func)
     component_spec['implementation'] = {}
     component_spec['implementation']['container'] = {}
-    component_spec['implementation']['container']['image'] = 'TBD'
+    component_spec['implementation']['container']['image'] = PLACEHOLDER_IMAGE
     component_spec['implementation']['container']['command'] = get_packages_to_install_command(func, packages_to_install)
     component_spec['implementation']['container']['args'] = ['--executor_input',
                                                              {'executorInput': None},
                                                              '--function_to_execute', 
                                                              name]
     # Write component yaml
-    filename = TMPFILES_DIR + f'/{name}.yaml'
-    make_dirs([TMPFILES_DIR])
+    filename = CACHE_DIR + f'/{name}.yaml'
+    make_dirs([CACHE_DIR])
     write_yaml_file(filename, component_spec, 'w')
 
 def get_packages_to_install_command(func: Optional[Callable] = None,
                                     packages_to_install: Optional[List[str]] = None):
     """Returns a list of formatted list of commands, including code for tmp storage.
 
     Args:
@@ -167,16 +168,16 @@
             a plain parameter, or a path to a file).
         name: The name of the pipeline.
         description: Short description of what the pipeline does.
     """
     pipeline_scaffold = (get_pipeline_decorator(name, description) +
                          get_function_source_definition(func) +
                          get_compile_step(func.__name__))
-    make_dirs([TMPFILES_DIR]) # if it doesn't already exist
-    write_file(PIPELINE_TMPFILE, pipeline_scaffold, 'w')
+    make_dirs([CACHE_DIR]) # if it doesn't already exist
+    write_file(PIPELINE_CACHE_FILE, pipeline_scaffold, 'w')
 
 def get_pipeline_decorator(name: Optional[str] = None,
                            description: Optional[str] = None):
     """Creates the kfp pipeline decorator.
 
     Args:
         name: The name of the pipeline.
```

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/utils/__init__.py` & `google-cloud-automlops-1.1.2/AutoMLOps/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/utils/constants.py` & `google-cloud-automlops-1.1.2/AutoMLOps/utils/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,14 @@
 # limitations under the License.
 
 """Sets global constants."""
 
 # pylint: disable=C0103
 # pylint: disable=line-too-long
 
-# temporary files
-TMPFILES_DIR = '.tmpfiles'
-IMPORTS_TMPFILE = f'{TMPFILES_DIR}/imports.py'
-CELL_TMPFILE = f'{TMPFILES_DIR}/cell.py'
-PIPELINE_TMPFILE = f'{TMPFILES_DIR}/pipeline_scaffold.py'
-
 # Apache license
 GENERATED_LICENSE = (
     '# Licensed under the Apache License, Version 2.0 (the "License");\n'
     '# you may not use this file except in compliance with the License.\n'
     '# You may obtain a copy of the License at\n'
     '#\n'
     '#     http://www.apache.org/licenses/LICENSE-2.0\n'
@@ -37,17 +31,19 @@
     '# See the License for the specific language governing permissions and\n'
     '# limitations under the License.\n'
     '#\n'
     '# DISCLAIMER: This code is generated as part of the AutoMLOps output.\n'
     '\n'
 )
 
+# Placeholder
+PLACEHOLDER_IMAGE = 'AutoMLOps_image_tbd'
+
 # AutoMLOps file paths
 BASE_DIR = 'AutoMLOps/'
-DEFAULT_IMAGE = 'python:3.9-slim'
 GENERATED_DEFAULTS_FILE = BASE_DIR + 'configs/defaults.yaml'
 GENERATED_PIPELINE_SPEC_SH_FILE = BASE_DIR + 'scripts/build_pipeline_spec.sh'
 GENERATED_BUILD_COMPONENTS_SH_FILE = BASE_DIR + 'scripts/build_components.sh'
 GENERATED_RUN_PIPELINE_SH_FILE = BASE_DIR + 'scripts/run_pipeline.sh'
 GENERATED_RUN_ALL_SH_FILE = BASE_DIR + 'scripts/run_all.sh'
 GENERATED_RESOURCES_SH_FILE = BASE_DIR + 'scripts/create_resources.sh'
 GENERATED_SUBMIT_JOB_FILE = BASE_DIR + 'scripts/submit_to_runner_svc.sh'
@@ -66,16 +62,20 @@
     BASE_DIR + 'images',
     BASE_DIR + 'pipelines',
     BASE_DIR + 'pipelines/runtime_parameters',
     BASE_DIR + 'scripts',
     BASE_DIR + 'scripts/pipeline_spec'
 ]
 
+# temporary files
+CACHE_DIR = '.AutoMLOps-cache'
+PIPELINE_CACHE_FILE = CACHE_DIR + '/pipeline_scaffold.py'
+
 # KFP Spec output_file location
-OUTPUT_DIR = TMPFILES_DIR
+OUTPUT_DIR = CACHE_DIR
 
 # Generated kfp pipeline metadata name
 DEFAULT_PIPELINE_NAME = 'automlops-pipeline'
 
 # Character substitution constants
 LEFT_BRACKET = '{'
 RIGHT_BRACKET = '}'
```

### Comparing `google-cloud-automlops-1.1.1/AutoMLOps/utils/utils.py` & `google-cloud-automlops-1.1.2/AutoMLOps/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,18 @@
 import subprocess
 
 import itertools
 import textwrap
 from typing import Callable
 import yaml
 
-from AutoMLOps.utils.constants import TMPFILES_DIR
+from AutoMLOps.utils.constants import (
+    CACHE_DIR,
+    PLACEHOLDER_IMAGE
+)
 
 def make_dirs(directories: list):
     """Makes directories with the specified names.
 
     Args:
         directories: Path of the directories to make.
     """
@@ -139,26 +142,26 @@
     """
     try:
         os.remove(filepath)
     except OSError:
         pass
 
 def get_components_list(full_path: bool = True) -> list:
-    """Reads yamls in tmpfiles directory, verifies they are component
+    """Reads yamls in the cache directory, verifies they are component
        yamls, and returns the name of the files.
 
     Args:
         full_path: Boolean; if false, stores only the filename w/o extension.
     Returns:
         list: Contains the names or paths of all component yamls in the dir.
     """
     components_list = []
-    elements = os.listdir(TMPFILES_DIR)
+    elements = os.listdir(CACHE_DIR)
     for file in list(filter(lambda y: ('.yaml' or '.yml') in y, elements)):
-        path = os.path.join(TMPFILES_DIR, file)
+        path = os.path.join(CACHE_DIR, file)
         if is_component_config(path):
             if full_path:
                 components_list.append(path)
             else:
                 components_list.append(os.path.basename(file).split('.')[0])
     return components_list
 
@@ -278,7 +281,18 @@
     right_bracket = '}'
     newline = '\n'
 
     return (
         f'''{left_bracket}\n'''
         f'''    {f'{newline}    '.join(f"   {quote}{k}{quote}: {quote if k != 'component_spec' else ''}{v}{quote if k != 'component_spec' else ''}," for k, v in job_spec.items())}{newline}'''
         f'''    {right_bracket}\n''')
+
+def is_using_kfp_spec(image: str):
+    """Takes in an image string from a component yaml and determines if it came from kfp or not.
+
+    Args:
+        image: image string.
+
+    Returns:
+        bool: is the component using kfp spec.
+    """
+    return image != PLACEHOLDER_IMAGE
```

### Comparing `google-cloud-automlops-1.1.1/LICENSE` & `google-cloud-automlops-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/PKG-INFO` & `google-cloud-automlops-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.1
+Version: 1.1.2
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -99,46 +99,41 @@
 
 # User Guide
 
 For a user-guide, please view these [slides](./AutoMLOps_Implementation_Guide_External.pdf).
 
 # Options
 
-AutoMLOps currently supports 4 different configurations based on the following flags:
-1. `use_kfp_spec`: (Optional) Bool that specifies whether to use Kubeflow definitions or Python custom definitions. Defaults to False. See [user guide](./AutoMLOps_Implementation_Guide_External.pdf).
-    - if True:
-        - The pipeline uses Kubeflow objects and syntax, and will generate all the necessary files in the backend to compile and run the pipeline.
-    - if False:
-        - The pipeline uses a custom defined syntax (through a series of python dictionaries and lists) that effectively removes the need to know Kubeflow syntax to compile and run the pipeline. 
-2. `run_local`: (Optional) Bool that specifies whether to use generate files resources locally or use cloud CI/CD workflow (see below). Defaults to True. See [CI/CD Workflow](#cloud-continuous-integration-and-continuous-deployment-workflow)
+AutoMLOps CI/CD options:
+1. `run_local`: Bool that specifies whether to use generate files resources locally or use cloud CI/CD workflow (see below). Defaults to True. See [CI/CD Workflow](#cloud-continuous-integration-and-continuous-deployment-workflow)
 
 Required parameters:
 1. `project_id: str`
 2. `pipeline_params: dict`
 
 Optional parameters (defaults shown):
 1. `af_registry_location: str = 'us-central1'`
 2. `af_registry_name: str = 'vertex-mlops-af'`
-3. `cb_trigger_location: str = 'us-central1'`
-4. `cb_trigger_name: str = 'automlops-trigger'`
-5. `cloud_run_location: str = 'us-central1'`
-6. `cloud_run_name: str = 'run-pipeline'`
-7. `cloud_tasks_queue_location: str = 'us-central1'`
-8. `cloud_tasks_queue_name: str = 'queueing-svc'`
-9. `csr_branch_name: str = 'automlops'`
-10. `csr_name: str = 'AutoMLOps-repo'`
-11. `custom_training_job_specs: list[dict] = None`
-12. `gs_bucket_location: str = 'us-central1'`
-13. `gs_bucket_name: str = None`
-14. `pipeline_runner_sa: str = None`
-15. `run_local: bool = True`
-16. `schedule_location: str = 'us-central1'`
-17. `schedule_name: str = 'AutoMLOps-schedule'`
-18. `schedule_pattern: str = 'No Schedule Specified'`
-19. `use_kfp_spec: bool = False`
+3. `base_image: str = 'python:3.9-slim'`
+4. `cb_trigger_location: str = 'us-central1'`
+5. `cb_trigger_name: str = 'automlops-trigger'`
+6. `cloud_run_location: str = 'us-central1'`
+7. `cloud_run_name: str = 'run-pipeline'`
+8. `cloud_tasks_queue_location: str = 'us-central1'`
+9. `cloud_tasks_queue_name: str = 'queueing-svc'`
+10. `csr_branch_name: str = 'automlops'`
+11. `csr_name: str = 'AutoMLOps-repo'`
+12. `custom_training_job_specs: list[dict] = None`
+13. `gs_bucket_location: str = 'us-central1'`
+14. `gs_bucket_name: str = None`
+15. `pipeline_runner_sa: str = None`
+16. `run_local: bool = True`
+17. `schedule_location: str = 'us-central1'`
+18. `schedule_name: str = 'AutoMLOps-schedule'`
+19. `schedule_pattern: str = 'No Schedule Specified'`
 20. `vpc_connector: str = None`
 
 AutoMLOps will generate the resources specified by these parameters (e.g. Artifact Registry, Cloud Source Repo, etc.). If run_local is set to False, the AutoMLOps will turn the current working directory of the notebook into a Git repo and use it for the CSR. Additionally, if a cron formatted str is given as an arg for `schedule_pattern` then it will set up a Cloud Schedule to run accordingly.
 
 # Customizations
 
 **Set scheduled run:**
@@ -146,16 +141,17 @@
 Use the `schedule_pattern` parameter to specify a cron job schedule to run the pipeline job on a recurring basis.
 ```
 schedule_pattern = '0 */12 * * *'
 ```
 
 **Set pipeline compute resources:**
 
-Use the `custom_training_job_specs` parameter to specify resources for any custom component in the pipeline.
+Use the `base_image` and `custom_training_job_specs` parameter to specify resources for any custom component in the pipeline.
 ```
+base_image = 'us-docker.pkg.dev/vertex-ai/training/tf-gpu.2-11.py310:latest',
 custom_training_job_specs = [{
     'component_spec': 'train_model',
     'display_name': 'train-model-accelerated',
     'machine_type': 'a2-highgpu-1g',
     'accelerator_type': 'NVIDIA_TESLA_A100',
     'accelerator_count': '1'
 }]
@@ -243,20 +239,28 @@
 - Use [terraform](https://github.com/GoogleCloudPlatform/vertex-pipelines-end-to-end-samples/tree/main/terraform) for the creation of resources.
 - Allow multiple AutoMLOps pipelines within the same directory
 - Adding model monitoring part
 - Alternatives to Pipreqs
 
 # Contributors
 
-[Sean Rastatter](mailto:srastatter@google.com): Technical Lead
+[Sean Rastatter](mailto:srastatter@google.com): Tech Lead
 
 [Tony DiLoreto](mailto:tonydiloreto@google.com): Project Manager
 
 [Allegra Noto](mailto:allegranoto@google.com): Senior Project Engineer
 
+[Ahmad Khan](mailto:ahmadkh@google.com): Engineer
+
+[Jesus Orozco](mailto:jesusfc@google.com): Cloud Engineer
+
+[Erin Horning](mailto:ehorning@google.com): Infrastructure Engineer
+
+[Alex Ho](mailto:alexanderho@google.com): Engineer
+
 # Disclaimer
 
 **This is not an officially supported Google product.**
 
 Copyright 2023 Google LLC. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `google-cloud-automlops-1.1.1/README.md` & `google-cloud-automlops-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -78,46 +78,41 @@
 
 # User Guide
 
 For a user-guide, please view these [slides](./AutoMLOps_Implementation_Guide_External.pdf).
 
 # Options
 
-AutoMLOps currently supports 4 different configurations based on the following flags:
-1. `use_kfp_spec`: (Optional) Bool that specifies whether to use Kubeflow definitions or Python custom definitions. Defaults to False. See [user guide](./AutoMLOps_Implementation_Guide_External.pdf).
-    - if True:
-        - The pipeline uses Kubeflow objects and syntax, and will generate all the necessary files in the backend to compile and run the pipeline.
-    - if False:
-        - The pipeline uses a custom defined syntax (through a series of python dictionaries and lists) that effectively removes the need to know Kubeflow syntax to compile and run the pipeline. 
-2. `run_local`: (Optional) Bool that specifies whether to use generate files resources locally or use cloud CI/CD workflow (see below). Defaults to True. See [CI/CD Workflow](#cloud-continuous-integration-and-continuous-deployment-workflow)
+AutoMLOps CI/CD options:
+1. `run_local`: Bool that specifies whether to use generate files resources locally or use cloud CI/CD workflow (see below). Defaults to True. See [CI/CD Workflow](#cloud-continuous-integration-and-continuous-deployment-workflow)
 
 Required parameters:
 1. `project_id: str`
 2. `pipeline_params: dict`
 
 Optional parameters (defaults shown):
 1. `af_registry_location: str = 'us-central1'`
 2. `af_registry_name: str = 'vertex-mlops-af'`
-3. `cb_trigger_location: str = 'us-central1'`
-4. `cb_trigger_name: str = 'automlops-trigger'`
-5. `cloud_run_location: str = 'us-central1'`
-6. `cloud_run_name: str = 'run-pipeline'`
-7. `cloud_tasks_queue_location: str = 'us-central1'`
-8. `cloud_tasks_queue_name: str = 'queueing-svc'`
-9. `csr_branch_name: str = 'automlops'`
-10. `csr_name: str = 'AutoMLOps-repo'`
-11. `custom_training_job_specs: list[dict] = None`
-12. `gs_bucket_location: str = 'us-central1'`
-13. `gs_bucket_name: str = None`
-14. `pipeline_runner_sa: str = None`
-15. `run_local: bool = True`
-16. `schedule_location: str = 'us-central1'`
-17. `schedule_name: str = 'AutoMLOps-schedule'`
-18. `schedule_pattern: str = 'No Schedule Specified'`
-19. `use_kfp_spec: bool = False`
+3. `base_image: str = 'python:3.9-slim'`
+4. `cb_trigger_location: str = 'us-central1'`
+5. `cb_trigger_name: str = 'automlops-trigger'`
+6. `cloud_run_location: str = 'us-central1'`
+7. `cloud_run_name: str = 'run-pipeline'`
+8. `cloud_tasks_queue_location: str = 'us-central1'`
+9. `cloud_tasks_queue_name: str = 'queueing-svc'`
+10. `csr_branch_name: str = 'automlops'`
+11. `csr_name: str = 'AutoMLOps-repo'`
+12. `custom_training_job_specs: list[dict] = None`
+13. `gs_bucket_location: str = 'us-central1'`
+14. `gs_bucket_name: str = None`
+15. `pipeline_runner_sa: str = None`
+16. `run_local: bool = True`
+17. `schedule_location: str = 'us-central1'`
+18. `schedule_name: str = 'AutoMLOps-schedule'`
+19. `schedule_pattern: str = 'No Schedule Specified'`
 20. `vpc_connector: str = None`
 
 AutoMLOps will generate the resources specified by these parameters (e.g. Artifact Registry, Cloud Source Repo, etc.). If run_local is set to False, the AutoMLOps will turn the current working directory of the notebook into a Git repo and use it for the CSR. Additionally, if a cron formatted str is given as an arg for `schedule_pattern` then it will set up a Cloud Schedule to run accordingly.
 
 # Customizations
 
 **Set scheduled run:**
@@ -125,16 +120,17 @@
 Use the `schedule_pattern` parameter to specify a cron job schedule to run the pipeline job on a recurring basis.
 ```
 schedule_pattern = '0 */12 * * *'
 ```
 
 **Set pipeline compute resources:**
 
-Use the `custom_training_job_specs` parameter to specify resources for any custom component in the pipeline.
+Use the `base_image` and `custom_training_job_specs` parameter to specify resources for any custom component in the pipeline.
 ```
+base_image = 'us-docker.pkg.dev/vertex-ai/training/tf-gpu.2-11.py310:latest',
 custom_training_job_specs = [{
     'component_spec': 'train_model',
     'display_name': 'train-model-accelerated',
     'machine_type': 'a2-highgpu-1g',
     'accelerator_type': 'NVIDIA_TESLA_A100',
     'accelerator_count': '1'
 }]
@@ -222,20 +218,28 @@
 - Use [terraform](https://github.com/GoogleCloudPlatform/vertex-pipelines-end-to-end-samples/tree/main/terraform) for the creation of resources.
 - Allow multiple AutoMLOps pipelines within the same directory
 - Adding model monitoring part
 - Alternatives to Pipreqs
 
 # Contributors
 
-[Sean Rastatter](mailto:srastatter@google.com): Technical Lead
+[Sean Rastatter](mailto:srastatter@google.com): Tech Lead
 
 [Tony DiLoreto](mailto:tonydiloreto@google.com): Project Manager
 
 [Allegra Noto](mailto:allegranoto@google.com): Senior Project Engineer
 
+[Ahmad Khan](mailto:ahmadkh@google.com): Engineer
+
+[Jesus Orozco](mailto:jesusfc@google.com): Cloud Engineer
+
+[Erin Horning](mailto:ehorning@google.com): Infrastructure Engineer
+
+[Alex Ho](mailto:alexanderho@google.com): Engineer
+
 # Disclaimer
 
 **This is not an officially supported Google product.**
 
 Copyright 2023 Google LLC. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -244,8 +248,8 @@
 
 http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
-limitations under the License.
+limitations under the License.
```

### Comparing `google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/PKG-INFO` & `google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.1
+Version: 1.1.2
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -99,46 +99,41 @@
 
 # User Guide
 
 For a user-guide, please view these [slides](./AutoMLOps_Implementation_Guide_External.pdf).
 
 # Options
 
-AutoMLOps currently supports 4 different configurations based on the following flags:
-1. `use_kfp_spec`: (Optional) Bool that specifies whether to use Kubeflow definitions or Python custom definitions. Defaults to False. See [user guide](./AutoMLOps_Implementation_Guide_External.pdf).
-    - if True:
-        - The pipeline uses Kubeflow objects and syntax, and will generate all the necessary files in the backend to compile and run the pipeline.
-    - if False:
-        - The pipeline uses a custom defined syntax (through a series of python dictionaries and lists) that effectively removes the need to know Kubeflow syntax to compile and run the pipeline. 
-2. `run_local`: (Optional) Bool that specifies whether to use generate files resources locally or use cloud CI/CD workflow (see below). Defaults to True. See [CI/CD Workflow](#cloud-continuous-integration-and-continuous-deployment-workflow)
+AutoMLOps CI/CD options:
+1. `run_local`: Bool that specifies whether to use generate files resources locally or use cloud CI/CD workflow (see below). Defaults to True. See [CI/CD Workflow](#cloud-continuous-integration-and-continuous-deployment-workflow)
 
 Required parameters:
 1. `project_id: str`
 2. `pipeline_params: dict`
 
 Optional parameters (defaults shown):
 1. `af_registry_location: str = 'us-central1'`
 2. `af_registry_name: str = 'vertex-mlops-af'`
-3. `cb_trigger_location: str = 'us-central1'`
-4. `cb_trigger_name: str = 'automlops-trigger'`
-5. `cloud_run_location: str = 'us-central1'`
-6. `cloud_run_name: str = 'run-pipeline'`
-7. `cloud_tasks_queue_location: str = 'us-central1'`
-8. `cloud_tasks_queue_name: str = 'queueing-svc'`
-9. `csr_branch_name: str = 'automlops'`
-10. `csr_name: str = 'AutoMLOps-repo'`
-11. `custom_training_job_specs: list[dict] = None`
-12. `gs_bucket_location: str = 'us-central1'`
-13. `gs_bucket_name: str = None`
-14. `pipeline_runner_sa: str = None`
-15. `run_local: bool = True`
-16. `schedule_location: str = 'us-central1'`
-17. `schedule_name: str = 'AutoMLOps-schedule'`
-18. `schedule_pattern: str = 'No Schedule Specified'`
-19. `use_kfp_spec: bool = False`
+3. `base_image: str = 'python:3.9-slim'`
+4. `cb_trigger_location: str = 'us-central1'`
+5. `cb_trigger_name: str = 'automlops-trigger'`
+6. `cloud_run_location: str = 'us-central1'`
+7. `cloud_run_name: str = 'run-pipeline'`
+8. `cloud_tasks_queue_location: str = 'us-central1'`
+9. `cloud_tasks_queue_name: str = 'queueing-svc'`
+10. `csr_branch_name: str = 'automlops'`
+11. `csr_name: str = 'AutoMLOps-repo'`
+12. `custom_training_job_specs: list[dict] = None`
+13. `gs_bucket_location: str = 'us-central1'`
+14. `gs_bucket_name: str = None`
+15. `pipeline_runner_sa: str = None`
+16. `run_local: bool = True`
+17. `schedule_location: str = 'us-central1'`
+18. `schedule_name: str = 'AutoMLOps-schedule'`
+19. `schedule_pattern: str = 'No Schedule Specified'`
 20. `vpc_connector: str = None`
 
 AutoMLOps will generate the resources specified by these parameters (e.g. Artifact Registry, Cloud Source Repo, etc.). If run_local is set to False, the AutoMLOps will turn the current working directory of the notebook into a Git repo and use it for the CSR. Additionally, if a cron formatted str is given as an arg for `schedule_pattern` then it will set up a Cloud Schedule to run accordingly.
 
 # Customizations
 
 **Set scheduled run:**
@@ -146,16 +141,17 @@
 Use the `schedule_pattern` parameter to specify a cron job schedule to run the pipeline job on a recurring basis.
 ```
 schedule_pattern = '0 */12 * * *'
 ```
 
 **Set pipeline compute resources:**
 
-Use the `custom_training_job_specs` parameter to specify resources for any custom component in the pipeline.
+Use the `base_image` and `custom_training_job_specs` parameter to specify resources for any custom component in the pipeline.
 ```
+base_image = 'us-docker.pkg.dev/vertex-ai/training/tf-gpu.2-11.py310:latest',
 custom_training_job_specs = [{
     'component_spec': 'train_model',
     'display_name': 'train-model-accelerated',
     'machine_type': 'a2-highgpu-1g',
     'accelerator_type': 'NVIDIA_TESLA_A100',
     'accelerator_count': '1'
 }]
@@ -243,20 +239,28 @@
 - Use [terraform](https://github.com/GoogleCloudPlatform/vertex-pipelines-end-to-end-samples/tree/main/terraform) for the creation of resources.
 - Allow multiple AutoMLOps pipelines within the same directory
 - Adding model monitoring part
 - Alternatives to Pipreqs
 
 # Contributors
 
-[Sean Rastatter](mailto:srastatter@google.com): Technical Lead
+[Sean Rastatter](mailto:srastatter@google.com): Tech Lead
 
 [Tony DiLoreto](mailto:tonydiloreto@google.com): Project Manager
 
 [Allegra Noto](mailto:allegranoto@google.com): Senior Project Engineer
 
+[Ahmad Khan](mailto:ahmadkh@google.com): Engineer
+
+[Jesus Orozco](mailto:jesusfc@google.com): Cloud Engineer
+
+[Erin Horning](mailto:ehorning@google.com): Infrastructure Engineer
+
+[Alex Ho](mailto:alexanderho@google.com): Engineer
+
 # Disclaimer
 
 **This is not an officially supported Google product.**
 
 Copyright 2023 Google LLC. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/SOURCES.txt` & `google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/setup.py` & `google-cloud-automlops-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as file:
     readme_contents = file.read()
 
 setup(
     name='google-cloud-automlops',
-    version='1.1.1',
+    version='1.1.2',
     description='AutoMLOps is a service that generates a production-style \
         MLOps pipeline from Jupyter Notebooks.',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/automlops',
     author='Sean Rastatter',
     author_email='srastatter@google.com',
```

### Comparing `google-cloud-automlops-1.1.1/tests/__init__.py` & `google-cloud-automlops-1.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/tests/unit/AutoMLOps_test.py` & `google-cloud-automlops-1.1.2/tests/unit/AutoMLOps_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/tests/unit/__init__.py` & `google-cloud-automlops-1.1.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/tests/unit/deployments/__init__.py` & `google-cloud-automlops-1.1.2/tests/unit/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/tests/unit/frameworks/__init__.py` & `google-cloud-automlops-1.1.2/tests/unit/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/tests/unit/frameworks/kfp/__init__.py` & `google-cloud-automlops-1.1.2/tests/unit/frameworks/kfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/tests/unit/utils/__init__.py` & `google-cloud-automlops-1.1.2/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.1/tests/unit/utils/utils_test.py` & `google-cloud-automlops-1.1.2/tests/unit/utils/utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     #with pytest.raises(OSError):
     #    delete_file('invalid_file_path.txt')
 
 # TBD
 # @pytest.mark.parametrize('full_path', [True, False])
 # def test_get_components_list(full_path: bool) -> None:
 #     # Create a temporary directory
-#     tmp_dir = pathlib.Path('.tmpfiles')
+#     tmp_dir = pathlib.Path('.AutoMLOps-cache')
 #     try:
 #         tmp_dir.mkdir()
 #     except FileExistsError:
 #         pass
 
 #     # Create some component yaml files
 #     component_yaml_1 = tmp_dir / 'component_1.yaml'
```

