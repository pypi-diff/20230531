# Comparing `tmp/google-cloud-run-0.7.1.tar.gz` & `tmp/google-cloud-run-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-run-0.7.1.tar", last modified: Mon Mar 27 16:05:06 2023, max compression
+gzip compressed data, was "google-cloud-run-0.8.0.tar", last modified: Wed May 31 18:48:12 2023, max compression
```

## Comparing `google-cloud-run-0.7.1.tar` & `google-cloud-run-0.8.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.364279 google-cloud-run-0.7.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4478 2023-03-27 16:05:06.364279 google-cloud-run-0.7.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3587 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.344270 google-cloud-run-0.7.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.344270 google-cloud-run-0.7.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.348272 google-cloud-run-0.7.1/google/cloud/run/
--rw-rw-r--   0 root         (0)     1003     4984 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.348272 google-cloud-run-0.7.1/google/cloud/run_v2/
--rw-rw-r--   0 root         (0)     1003     4323 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    11056 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.348272 google-cloud-run-0.7.1/google/cloud/run_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.352274 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/
--rw-rw-r--   0 root         (0)     1003      753 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/__init__.py
--rw-rw-r--   0 root         (0)     1003    32592 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/async_client.py
--rw-rw-r--   0 root         (0)     1003    44778 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/client.py
--rw-rw-r--   0 root         (0)     1003     5724 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.352274 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8120 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17896 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18214 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    38178 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.352274 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/
--rw-rw-r--   0 root         (0)     1003      729 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/__init__.py
--rw-rw-r--   0 root         (0)     1003    62817 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/async_client.py
--rw-rw-r--   0 root         (0)     1003    75369 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/client.py
--rw-rw-r--   0 root         (0)     1003     5454 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.352274 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/
--rw-rw-r--   0 root         (0)     1003     1260 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10638 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24322 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24783 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    74496 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.352274 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/
--rw-rw-r--   0 root         (0)     1003      749 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/__init__.py
--rw-rw-r--   0 root         (0)     1003    32604 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/async_client.py
--rw-rw-r--   0 root         (0)     1003    45650 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/client.py
--rw-rw-r--   0 root         (0)     1003     5679 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.356276 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/
--rw-rw-r--   0 root         (0)     1003     1330 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8080 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17882 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18199 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    38188 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.356276 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/
--rw-rw-r--   0 root         (0)     1003      745 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/__init__.py
--rw-rw-r--   0 root         (0)     1003    61130 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/async_client.py
--rw-rw-r--   0 root         (0)     1003    74285 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/client.py
--rw-rw-r--   0 root         (0)     1003     5634 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.356276 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11098 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23863 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24318 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    70819 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.356276 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/
--rw-rw-r--   0 root         (0)     1003      733 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/__init__.py
--rw-rw-r--   0 root         (0)     1003    27294 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/async_client.py
--rw-rw-r--   0 root         (0)     1003    40166 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/client.py
--rw-rw-r--   0 root         (0)     1003     5499 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.360278 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/
--rw-rw-r--   0 root         (0)     1003     1274 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7324 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15918 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16151 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    30148 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.360278 google-cloud-run-0.7.1/google/cloud/run_v2/types/
--rw-rw-r--   0 root         (0)     1003     3581 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10407 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/condition.py
--rw-rw-r--   0 root         (0)     1003    13148 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/execution.py
--rw-rw-r--   0 root         (0)     1003     3668 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/execution_template.py
--rw-rw-r--   0 root         (0)     1003    17472 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/job.py
--rw-rw-r--   0 root         (0)     1003    24064 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/k8s_min.py
--rw-rw-r--   0 root         (0)     1003    13548 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/revision.py
--rw-rw-r--   0 root         (0)     1003     5552 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/revision_template.py
--rw-rw-r--   0 root         (0)     1003    19256 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/service.py
--rw-rw-r--   0 root         (0)     1003    13587 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/task.py
--rw-rw-r--   0 root         (0)     1003     4155 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/task_template.py
--rw-rw-r--   0 root         (0)     1003     3750 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/traffic_target.py
--rw-rw-r--   0 root         (0)     1003     5608 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/google/cloud/run_v2/types/vendor_settings.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.364279 google-cloud-run-0.7.1/google_cloud_run.egg-info/
--rw-r--r--   0 root         (0)     1003     4478 2023-03-27 16:05:06.000000 google-cloud-run-0.7.1/google_cloud_run.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3882 2023-03-27 16:05:06.000000 google-cloud-run-0.7.1/google_cloud_run.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:05:06.000000 google-cloud-run-0.7.1/google_cloud_run.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:05:06.000000 google-cloud-run-0.7.1/google_cloud_run.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:05:06.000000 google-cloud-run-0.7.1/google_cloud_run.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 16:05:06.000000 google-cloud-run-0.7.1/google_cloud_run.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:05:06.000000 google-cloud-run-0.7.1/google_cloud_run.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:05:06.364279 google-cloud-run-0.7.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2952 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.364279 google-cloud-run-0.7.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.364279 google-cloud-run-0.7.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.364279 google-cloud-run-0.7.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:06.364279 google-cloud-run-0.7.1/tests/unit/gapic/run_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/tests/unit/gapic/run_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   153024 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_executions.py
--rw-rw-r--   0 root         (0)     1003   260303 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_jobs.py
--rw-rw-r--   0 root         (0)     1003   149917 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_revisions.py
--rw-rw-r--   0 root         (0)     1003   245573 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_services.py
--rw-rw-r--   0 root         (0)     1003   130967 2023-03-27 16:03:07.000000 google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.377286 google-cloud-run-0.8.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4478 2023-05-31 18:48:12.377286 google-cloud-run-0.8.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3587 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.357279 google-cloud-run-0.8.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.357279 google-cloud-run-0.8.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run/
+-rw-rw-r--   0 root         (0)     1003     4984 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run_v2/
+-rw-rw-r--   0 root         (0)     1003     4323 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11056 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/
+-rw-rw-r--   0 root         (0)     1003      753 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32592 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44778 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/client.py
+-rw-rw-r--   0 root         (0)     1003     5724 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8120 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17896 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18214 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    38178 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/
+-rw-rw-r--   0 root         (0)     1003      729 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62817 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/async_client.py
+-rw-rw-r--   0 root         (0)     1003    75369 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/client.py
+-rw-rw-r--   0 root         (0)     1003     5454 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/
+-rw-rw-r--   0 root         (0)     1003     1260 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10638 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24322 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24783 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    74496 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/
+-rw-rw-r--   0 root         (0)     1003      749 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32604 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    45650 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/client.py
+-rw-rw-r--   0 root         (0)     1003     5679 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/
+-rw-rw-r--   0 root         (0)     1003     1330 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8080 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17882 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18199 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    38188 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/
+-rw-rw-r--   0 root         (0)     1003      745 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61130 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/async_client.py
+-rw-rw-r--   0 root         (0)     1003    74285 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/client.py
+-rw-rw-r--   0 root         (0)     1003     5634 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.369283 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11098 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23863 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24318 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    70819 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.369283 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/
+-rw-rw-r--   0 root         (0)     1003      733 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27294 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40166 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/client.py
+-rw-rw-r--   0 root         (0)     1003     5499 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.369283 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/
+-rw-rw-r--   0 root         (0)     1003     1274 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7324 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15918 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16151 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    30148 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/google/cloud/run_v2/types/
+-rw-rw-r--   0 root         (0)     1003     3581 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10542 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/condition.py
+-rw-rw-r--   0 root         (0)     1003    13565 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/execution.py
+-rw-rw-r--   0 root         (0)     1003     4307 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/execution_template.py
+-rw-rw-r--   0 root         (0)     1003    18011 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/job.py
+-rw-rw-r--   0 root         (0)     1003    23222 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/k8s_min.py
+-rw-rw-r--   0 root         (0)     1003    14333 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/revision.py
+-rw-rw-r--   0 root         (0)     1003     6438 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/revision_template.py
+-rw-rw-r--   0 root         (0)     1003    19791 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/service.py
+-rw-rw-r--   0 root         (0)     1003    13995 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/task.py
+-rw-rw-r--   0 root         (0)     1003     4207 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/task_template.py
+-rw-rw-r--   0 root         (0)     1003     3750 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/traffic_target.py
+-rw-rw-r--   0 root         (0)     1003     5608 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/vendor_settings.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/google_cloud_run.egg-info/
+-rw-r--r--   0 root         (0)     1003     4478 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3882 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-31 18:48:12.377286 google-cloud-run-0.8.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2952 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.377286 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   153250 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_executions.py
+-rw-rw-r--   0 root         (0)     1003   261385 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_jobs.py
+-rw-rw-r--   0 root         (0)     1003   150387 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_revisions.py
+-rw-rw-r--   0 root         (0)     1003   246727 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_services.py
+-rw-rw-r--   0 root         (0)     1003   131193 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_tasks.py
```

### Comparing `google-cloud-run-0.7.1/LICENSE` & `google-cloud-run-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/MANIFEST.in` & `google-cloud-run-0.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/PKG-INFO` & `google-cloud-run-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-run
-Version: 0.7.1
+Version: 0.8.0
 Summary: Google Cloud Run API client library
 Home-page: https://github.com/googleapis/python-run
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-run-0.7.1/README.rst` & `google-cloud-run-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run/gapic_version.py` & `google-cloud-run-0.8.0/google/cloud/run/gapic_version.py`

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
-__version__ = "0.7.1"  # {x-release-please-version}
+__version__ = "0.8.0"  # {x-release-please-version}
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/gapic_metadata.json` & `google-cloud-run-0.8.0/google/cloud/run_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/gapic_version.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/gapic_version.py`

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
-__version__ = "0.7.1"  # {x-release-please-version}
+__version__ = "0.8.0"  # {x-release-please-version}
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/async_client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/pagers.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/base.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/grpc.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/executions/transports/rest.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/async_client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/pagers.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/base.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/grpc.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/jobs/transports/rest.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/async_client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/pagers.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/base.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/grpc.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/revisions/transports/rest.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/services/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/services/async_client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/services/client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/services/pagers.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/base.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/grpc.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/grpc_asyncio.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/services/transports/rest.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/async_client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/client.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/pagers.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/base.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/grpc.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/services/tasks/transports/rest.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/__init__.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/condition.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,19 +240,23 @@
                 status. System will retry.
             NON_ZERO_EXIT_CODE (2):
                 A task reached its retry limit and the last
                 attempt failed due to the user container exiting
                 with a non-zero exit code.
             CANCELLED (3):
                 The execution was cancelled by users.
+            CANCELLING (4):
+                The execution is in the process of being
+                cancelled.
         """
         EXECUTION_REASON_UNDEFINED = 0
         JOB_STATUS_SERVICE_POLLING_ERROR = 1
         NON_ZERO_EXIT_CODE = 2
         CANCELLED = 3
+        CANCELLING = 4
 
     type_: str = proto.Field(
         proto.STRING,
         number=1,
     )
     state: State = proto.Field(
         proto.ENUM,
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/execution.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/execution.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,25 +166,29 @@
             UUID4 string and guaranteed to remain unchanged
             until the resource is deleted.
         generation (int):
             Output only. A number that monotonically
             increases every time the user modifies the
             desired state.
         labels (MutableMapping[str, str]):
-            KRM-style labels for the resource.
+            Output only. Unstructured key value map that
+            can be used to organize and categorize objects.
             User-provided labels are shared with Google's
             billing system, so they can be used to filter,
             or break down billing charges by team,
             component, environment, state, etc. For more
             information, visit
             https://cloud.google.com/resource-manager/docs/creating-managing-labels
             or
             https://cloud.google.com/run/docs/configuring/labels
         annotations (MutableMapping[str, str]):
-            KRM-style annotations for the resource.
+            Output only. Unstructured key value map that
+            may be set by external tools to store and
+            arbitrary metadata. They are not queryable and
+            should be preserved when modifying objects.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Represents time when the
             execution was acknowledged by the execution
             controller. It is not guaranteed to be set in
             happens-before order across separate operations.
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Represents time when the
@@ -204,36 +208,40 @@
             response to a Delete request.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. For a deleted resource, the time
             after which it will be permamently deleted. It
             is only populated as a response to a Delete
             request.
         launch_stage (google.api.launch_stage_pb2.LaunchStage):
-            Set the launch stage to a preview stage on write to allow
-            use of preview features in that stage. On read, describes
-            whether the resource uses preview features. Launch Stages
-            are defined at `Google Cloud Platform Launch
+            The least stable launch stage needed to create this
+            resource, as defined by `Google Cloud Platform Launch
             Stages <https://cloud.google.com/terms/launch-stages>`__.
+            Cloud Run supports ``ALPHA``, ``BETA``, and ``GA``.
+
+            .. raw:: html
+
+                <p>Note that this value might not be what was used
+                as input. For example, if ALPHA was provided as input in the parent
+                resource, but only BETA and GA-level features are were, this field will be
+                BETA.
         job (str):
             Output only. The name of the parent Job.
         parallelism (int):
             Output only. Specifies the maximum desired number of tasks
             the execution should run at any given time. Must be <=
             task_count. The actual number of tasks running in steady
             state will be less than this number when ((.spec.task_count
             - .status.successful) < .spec.parallelism), i.e. when the
-            work left to do is less than max parallelism. More info:
-            https://kubernetes.io/docs/concepts/workloads/controllers/jobs-run-to-completion/
+            work left to do is less than max parallelism.
         task_count (int):
             Output only. Specifies the desired number of
             tasks the execution should run. Setting to 1
             means that parallelism is limited to 1 and the
             success of that task signals the success of the
-            execution. More info:
-            https://kubernetes.io/docs/concepts/workloads/controllers/jobs-run-to-completion/
+            execution.
         template (google.cloud.run_v2.types.TaskTemplate):
             Output only. The template used to create
             tasks for this execution.
         reconciling (bool):
             Output only. Indicates whether the resource's reconciliation
             is still in progress. See comments in ``Job.reconciling``
             for additional information on reconciliation process in
@@ -261,14 +269,16 @@
             reached phase Cancelled.
         retried_count (int):
             Output only. The number of tasks which have
             retried at least once.
         log_uri (str):
             Output only. URI where logs for this
             execution can be found in Cloud Console.
+        satisfies_pzs (bool):
+            Output only. Reserved for future use.
         etag (str):
             Output only. A system-generated fingerprint
             for this version of the resource. May be used to
             detect modification conflict during updates.
     """
 
     name: str = proto.Field(
@@ -378,14 +388,18 @@
         proto.INT32,
         number=25,
     )
     log_uri: str = proto.Field(
         proto.STRING,
         number=26,
     )
+    satisfies_pzs: bool = proto.Field(
+        proto.BOOL,
+        number=27,
+    )
     etag: str = proto.Field(
         proto.STRING,
         number=99,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/execution_template.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/execution_template.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,47 +31,59 @@
 
 class ExecutionTemplate(proto.Message):
     r"""ExecutionTemplate describes the data an execution should have
     when created from a template.
 
     Attributes:
         labels (MutableMapping[str, str]):
-            KRM-style labels for the resource.
+            Unstructured key value map that can be used to organize and
+            categorize objects. User-provided labels are shared with
+            Google's billing system, so they can be used to filter, or
+            break down billing charges by team, component, environment,
+            state, etc. For more information, visit
+            https://cloud.google.com/resource-manager/docs/creating-managing-labels
+            or https://cloud.google.com/run/docs/configuring/labels.
 
             .. raw:: html
 
                 <p>Cloud Run API v2 does not support labels with `run.googleapis.com`,
                 `cloud.googleapis.com`, `serving.knative.dev`, or `autoscaling.knative.dev`
                 namespaces, and they will be rejected. All system labels in v1 now have a
                 corresponding field in v2 ExecutionTemplate.
         annotations (MutableMapping[str, str]):
-            KRM-style annotations for the resource.
+            Unstructured key value map that may be set by external tools
+            to store and arbitrary metadata. They are not queryable and
+            should be preserved when modifying objects.
 
             .. raw:: html
 
                 <p>Cloud Run API v2 does not support annotations with `run.googleapis.com`,
                 `cloud.googleapis.com`, `serving.knative.dev`, or `autoscaling.knative.dev`
                 namespaces, and they will be rejected. All system annotations in v1 now
                 have a corresponding field in v2 ExecutionTemplate.
+
+            .. raw:: html
+
+                <p>This field follows Kubernetes annotations' namespacing, limits, and
+                rules.
         parallelism (int):
             Specifies the maximum desired number of tasks the execution
             should run at given time. Must be <= task_count. When the
             job is run, if this field is 0 or unset, the maximum
             possible value will be used for that execution. The actual
             number of tasks running in steady state will be less than
             this number when there are fewer tasks waiting to be
             completed remaining, i.e. when the work left to do is less
             than max parallelism.
         task_count (int):
             Specifies the desired number of tasks the
             execution should run. Setting to 1 means that
             parallelism is limited to 1 and the success of
             that task signals the success of the execution.
-            More info:
-            https://kubernetes.io/docs/concepts/workloads/controllers/jobs-run-to-completion/
+            Defaults to 1.
         template (google.cloud.run_v2.types.TaskTemplate):
             Required. Describes the task(s) that will be
             created when executing an execution.
     """
 
     labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/job.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,44 +274,44 @@
             UUID4 string and guaranteed to remain unchanged
             until the resource is deleted.
         generation (int):
             Output only. A number that monotonically
             increases every time the user modifies the
             desired state.
         labels (MutableMapping[str, str]):
-            KRM-style labels for the resource. User-provided labels are
-            shared with Google's billing system, so they can be used to
-            filter, or break down billing charges by team, component,
-            environment, state, etc. For more information, visit
+            Unstructured key value map that can be used to organize and
+            categorize objects. User-provided labels are shared with
+            Google's billing system, so they can be used to filter, or
+            break down billing charges by team, component, environment,
+            state, etc. For more information, visit
             https://cloud.google.com/resource-manager/docs/creating-managing-labels
-            or https://cloud.google.com/run/docs/configuring/labels
+            or https://cloud.google.com/run/docs/configuring/labels.
 
             .. raw:: html
 
                 <p>Cloud Run API v2 does not support labels with `run.googleapis.com`,
                 `cloud.googleapis.com`, `serving.knative.dev`, or `autoscaling.knative.dev`
                 namespaces, and they will be rejected. All system labels in v1 now have a
                 corresponding field in v2 Job.
         annotations (MutableMapping[str, str]):
-            KRM-style annotations for the resource. Unstructured key
-            value map that may be set by external tools to store and
-            arbitrary metadata. They are not queryable and should be
-            preserved when modifying objects.
+            Unstructured key value map that may be set by external tools
+            to store and arbitrary metadata. They are not queryable and
+            should be preserved when modifying objects.
 
             .. raw:: html
 
                 <p>Cloud Run API v2 does not support annotations with `run.googleapis.com`,
                 `cloud.googleapis.com`, `serving.knative.dev`, or `autoscaling.knative.dev`
-                namespaces, and they will be rejected. All system annotations in v1 now
-                have a corresponding field in v2 Job.
+                namespaces, and they will be rejected on new resources. All system
+                annotations in v1 now have a corresponding field in v2 Job.
 
             .. raw:: html
 
                 <p>This field follows Kubernetes annotations' namespacing, limits, and
-                rules. More info: https://kubernetes.io/docs/user-guide/annotations
+                rules.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The creation time.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The last-modified time.
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The deletion time.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -328,15 +328,24 @@
         client_version (str):
             Arbitrary version identifier for the API
             client.
         launch_stage (google.api.launch_stage_pb2.LaunchStage):
             The launch stage as defined by `Google Cloud Platform Launch
             Stages <https://cloud.google.com/terms/launch-stages>`__.
             Cloud Run supports ``ALPHA``, ``BETA``, and ``GA``. If no
-            value is specified, GA is assumed.
+            value is specified, GA is assumed. Set the launch stage to a
+            preview stage on input to allow use of preview features in
+            that stage. On read (or output), describes whether the
+            resource uses preview features.
+
+            .. raw:: html
+
+                <p>
+                For example, if ALPHA is provided as input, but only BETA and GA-level
+                features are used, this field will be BETA on output.
         binary_authorization (google.cloud.run_v2.types.BinaryAuthorization):
             Settings for the Binary Authorization
             feature.
         template (google.cloud.run_v2.types.ExecutionTemplate):
             Required. The template used to create
             executions for this Job.
         observed_generation (int):
@@ -382,14 +391,16 @@
             ``latest_created_execution``.
 
             If reconciliation failed, ``observed_generation`` and
             ``latest_succeeded_execution`` will have the state of the
             last succeeded execution or empty for newly created Job.
             Additional information on the failure can be found in
             ``terminal_condition`` and ``conditions``.
+        satisfies_pzs (bool):
+            Output only. Reserved for future use.
         etag (str):
             Output only. A system-generated fingerprint
             for this version of the resource. May be used to
             detect modification conflict during updates.
     """
 
     name: str = proto.Field(
@@ -488,14 +499,18 @@
         number=22,
         message="ExecutionReference",
     )
     reconciling: bool = proto.Field(
         proto.BOOL,
         number=23,
     )
+    satisfies_pzs: bool = proto.Field(
+        proto.BOOL,
+        number=25,
+    )
     etag: str = proto.Field(
         proto.STRING,
         number=99,
     )
 
 
 class ExecutionReference(proto.Message):
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/k8s_min.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/k8s_min.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,43 +52,29 @@
     Attributes:
         name (str):
             Name of the container specified as a DNS_LABEL (RFC 1123).
         image (str):
             Required. Name of the container image in
             Dockerhub, Google Artifact Registry, or Google
             Container Registry. If the host is not provided,
-            Dockerhub is assumed. More info:
-            https://kubernetes.io/docs/concepts/containers/images
+            Dockerhub is assumed.
         command (MutableSequence[str]):
-            Entrypoint array. Not executed within a shell. The docker
-            image's ENTRYPOINT is used if this is not provided. Variable
-            references $(VAR_NAME) are expanded using the container's
-            environment. If a variable cannot be resolved, the reference
-            in the input string will be unchanged. The $(VAR_NAME)
-            syntax can be escaped with a double $$, ie: $$(VAR_NAME).
-            Escaped references will never be expanded, regardless of
-            whether the variable exists or not. More info:
-            https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container/#running-a-command-in-a-shell
+            Entrypoint array. Not executed within a
+            shell. The docker image's ENTRYPOINT is used if
+            this is not provided.
         args (MutableSequence[str]):
-            Arguments to the entrypoint. The docker image's CMD is used
-            if this is not provided. Variable references $(VAR_NAME) are
-            expanded using the container's environment. If a variable
-            cannot be resolved, the reference in the input string will
-            be unchanged. The $(VAR_NAME) syntax can be escaped with a
-            double $$, ie: $$(VAR_NAME). Escaped references will never
-            be expanded, regardless of whether the variable exists or
-            not. More info:
-            https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container/#running-a-command-in-a-shell
+            Arguments to the entrypoint.
+            The docker image's CMD is used if this is not
+            provided.
         env (MutableSequence[google.cloud.run_v2.types.EnvVar]):
             List of environment variables to set in the
             container.
         resources (google.cloud.run_v2.types.ResourceRequirements):
             Compute Resource requirements by this
-            container. More info:
-            https://kubernetes.io/docs/concepts/storage/persistent-volumes#resources
+            container.
         ports (MutableSequence[google.cloud.run_v2.types.ContainerPort]):
             List of ports to expose from the container.
             Only a single port can be specified. The
             specified ports must be listening on all
             interfaces (0.0.0.0) within the container to be
             accessible.
             If omitted, a port number will be chosen and
@@ -102,24 +88,20 @@
             Container's working directory.
             If not specified, the container runtime's
             default will be used, which might be configured
             in the container image.
         liveness_probe (google.cloud.run_v2.types.Probe):
             Periodic probe of container liveness.
             Container will be restarted if the probe fails.
-            More info:
-            https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes
         startup_probe (google.cloud.run_v2.types.Probe):
             Startup probe of application within the
             container. All other probes are disabled if a
             startup probe is provided, until it succeeds.
             Container will not be added to service endpoints
             if the probe fails.
-            More info:
-            https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     image: str = proto.Field(
@@ -172,34 +154,47 @@
 
 class ResourceRequirements(proto.Message):
     r"""ResourceRequirements describes the compute resource
     requirements.
 
     Attributes:
         limits (MutableMapping[str, str]):
-            Only memory and CPU are supported. Note: The
-            only supported values for CPU are '1', '2',
-            '4', and '8'. Setting 4 CPU requires at least
-            2Gi of memory. The values of the map is string
-            form of the 'quantity' k8s type:
-            https://github.com/kubernetes/kubernetes/blob/master/staging/src/k8s.io/apimachinery/pkg/api/resource/quantity.go
+            Only ´memory´ and 'cpu' are supported.
+
+            .. raw:: html
+
+                <p>Notes:
+                 * The only supported values for CPU are '1', '2', '4', and '8'. Setting 4
+                CPU requires at least 2Gi of memory. For more information, go to
+                https://cloud.google.com/run/docs/configuring/cpu.
+                  * For supported 'memory' values and syntax, go to
+                 https://cloud.google.com/run/docs/configuring/memory-limits
         cpu_idle (bool):
             Determines whether CPU should be throttled or
             not outside of requests.
+        startup_cpu_boost (bool):
+            Determines whether CPU should be boosted on
+            startup of a new container instance above the
+            requested CPU threshold, this can help reduce
+            cold-start latency.
     """
 
     limits: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=1,
     )
     cpu_idle: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
+    startup_cpu_boost: bool = proto.Field(
+        proto.BOOL,
+        number=3,
+    )
 
 
 class EnvVar(proto.Message):
     r"""EnvVar represents an environment variable present in a
     Container.
 
     This message has `oneof`_ fields (mutually exclusive fields).
@@ -352,16 +347,15 @@
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             Required. Volume's name.
         secret (google.cloud.run_v2.types.SecretVolumeSource):
             Secret represents a secret that should
-            populate this volume. More info:
-            https://kubernetes.io/docs/concepts/storage/volumes#secret
+            populate this volume.
 
             This field is a member of `oneof`_ ``volume_type``.
         cloud_sql_instance (google.cloud.run_v2.types.CloudSqlInstance):
             For Cloud SQL volumes, contains the specific
             instances that should be mounted. Visit
             https://cloud.google.com/sql/docs/mysql/connect-run
             for more information on how to connect Cloud SQL
@@ -534,22 +528,19 @@
 
     Attributes:
         initial_delay_seconds (int):
             Number of seconds after the container has
             started before the probe is initiated.
             Defaults to 0 seconds. Minimum value is 0.
             Maximum value for liveness probe is 3600.
-            Maximum value for startup probe is 240. More
-            info:
-            https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes
+            Maximum value for startup probe is 240.
         timeout_seconds (int):
             Number of seconds after which the probe times out. Defaults
             to 1 second. Minimum value is 1. Maximum value is 3600. Must
-            be smaller than period_seconds. More info:
-            https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes
+            be smaller than period_seconds.
         period_seconds (int):
             How often (in seconds) to perform the probe. Default to 10
             seconds. Minimum value is 1. Maximum value for liveness
             probe is 3600. Maximum value for startup probe is 240. Must
             be greater or equal than timeout_seconds.
         failure_threshold (int):
             Minimum consecutive failures for the probe to
@@ -617,25 +608,34 @@
     Attributes:
         path (str):
             Path to access on the HTTP server. Defaults
             to '/'.
         http_headers (MutableSequence[google.cloud.run_v2.types.HTTPHeader]):
             Custom headers to set in the request. HTTP
             allows repeated headers.
+        port (int):
+            Port number to access on the container. Must be in the range
+            1 to 65535. If not specified, defaults to the exposed port
+            of the container, which is the value of
+            container.ports[0].containerPort.
     """
 
     path: str = proto.Field(
         proto.STRING,
         number=1,
     )
     http_headers: MutableSequence["HTTPHeader"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="HTTPHeader",
     )
+    port: int = proto.Field(
+        proto.INT32,
+        number=5,
+    )
 
 
 class HTTPHeader(proto.Message):
     r"""HTTPHeader describes a custom header to be used in HTTP
     probes
 
     Attributes:
@@ -656,33 +656,35 @@
 
 
 class TCPSocketAction(proto.Message):
     r"""TCPSocketAction describes an action based on opening a socket
 
     Attributes:
         port (int):
-            Port number to access on the container. Must
-            be in the range 1 to 65535. If not specified,
-            defaults to 8080.
+            Port number to access on the container. Must be in the range
+            1 to 65535. If not specified, defaults to the exposed port
+            of the container, which is the value of
+            container.ports[0].containerPort.
     """
 
     port: int = proto.Field(
         proto.INT32,
         number=1,
     )
 
 
 class GRPCAction(proto.Message):
     r"""GRPCAction describes an action involving a GRPC port.
 
     Attributes:
         port (int):
-            Port number of the gRPC service. Number must
-            be in the range 1 to 65535. If not specified,
-            defaults to 8080.
+            Port number of the gRPC service. Number must be in the range
+            1 to 65535. If not specified, defaults to the exposed port
+            of the container, which is the value of
+            container.ports[0].containerPort.
         service (str):
             Service is the name of the service to place
             in the gRPC HealthCheckRequest (see
             https://github.com/grpc/grpc/blob/master/doc/health-checking.md).
             If this is not specified, the default behavior
             is defined by gRPC.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/revision.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/revision.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,44 +167,54 @@
             UUID4 string and guaranteed to remain unchanged
             until the resource is deleted.
         generation (int):
             Output only. A number that monotonically
             increases every time the user modifies the
             desired state.
         labels (MutableMapping[str, str]):
-            KRM-style labels for the resource.
+            Output only. Unstructured key value map that
+            can be used to organize and categorize objects.
             User-provided labels are shared with Google's
             billing system, so they can be used to filter,
             or break down billing charges by team,
             component, environment, state, etc. For more
             information, visit
             https://cloud.google.com/resource-manager/docs/creating-managing-labels
             or
-            https://cloud.google.com/run/docs/configuring/labels
+            https://cloud.google.com/run/docs/configuring/labels.
         annotations (MutableMapping[str, str]):
-            KRM-style annotations for the resource.
+            Output only. Unstructured key value map that
+            may be set by external tools to store and
+            arbitrary metadata. They are not queryable and
+            should be preserved when modifying objects.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The creation time.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The last-modified time.
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. For a deleted resource, the
             deletion time. It is only populated as a
             response to a Delete request.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. For a deleted resource, the time
             after which it will be permamently deleted. It
             is only populated as a response to a Delete
             request.
         launch_stage (google.api.launch_stage_pb2.LaunchStage):
-            Set the launch stage to a preview stage on write to allow
-            use of preview features in that stage. On read, describes
-            whether the resource uses preview features. Launch Stages
-            are defined at `Google Cloud Platform Launch
+            The least stable launch stage needed to create this
+            resource, as defined by `Google Cloud Platform Launch
             Stages <https://cloud.google.com/terms/launch-stages>`__.
+            Cloud Run supports ``ALPHA``, ``BETA``, and ``GA``.
+
+            .. raw:: html
+
+                <p>Note that this value might not be what was used
+                as input. For example, if ALPHA was provided as input in the parent
+                resource, but only BETA and GA-level features are were, this field will be
+                BETA.
         service (str):
             Output only. The name of the parent service.
         scaling (google.cloud.run_v2.types.RevisionScaling):
             Scaling settings for this revision.
         vpc_access (google.cloud.run_v2.types.VpcAccess):
             VPC Access configuration for this Revision.
             For more information, visit
@@ -256,14 +266,18 @@
             Output only. The generation of this Revision currently
             serving traffic. See comments in ``reconciling`` for
             additional information on reconciliation process in Cloud
             Run.
         log_uri (str):
             Output only. The Google Console URI to obtain
             logs for the Revision.
+        satisfies_pzs (bool):
+            Output only. Reserved for future use.
+        session_affinity (bool):
+            Enable session affinity.
         etag (str):
             Output only. A system-generated fingerprint
             for this version of the resource. May be used to
             detect modification conflict during updates.
     """
 
     name: str = proto.Field(
@@ -384,14 +398,22 @@
         proto.INT64,
         number=32,
     )
     log_uri: str = proto.Field(
         proto.STRING,
         number=33,
     )
+    satisfies_pzs: bool = proto.Field(
+        proto.BOOL,
+        number=37,
+    )
+    session_affinity: bool = proto.Field(
+        proto.BOOL,
+        number=38,
+    )
     etag: str = proto.Field(
         proto.STRING,
         number=99,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/revision_template.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/revision_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,31 +36,44 @@
 
     Attributes:
         revision (str):
             The unique name for the revision. If this
             field is omitted, it will be automatically
             generated based on the Service name.
         labels (MutableMapping[str, str]):
-            KRM-style labels for the resource.
+            Unstructured key value map that can be used to organize and
+            categorize objects. User-provided labels are shared with
+            Google's billing system, so they can be used to filter, or
+            break down billing charges by team, component, environment,
+            state, etc. For more information, visit
+            https://cloud.google.com/resource-manager/docs/creating-managing-labels
+            or https://cloud.google.com/run/docs/configuring/labels.
 
             .. raw:: html
 
                 <p>Cloud Run API v2 does not support labels with `run.googleapis.com`,
                 `cloud.googleapis.com`, `serving.knative.dev`, or `autoscaling.knative.dev`
                 namespaces, and they will be rejected. All system labels in v1 now have a
                 corresponding field in v2 RevisionTemplate.
         annotations (MutableMapping[str, str]):
-            KRM-style annotations for the resource.
+            Unstructured key value map that may be set by external tools
+            to store and arbitrary metadata. They are not queryable and
+            should be preserved when modifying objects.
 
             .. raw:: html
 
                 <p>Cloud Run API v2 does not support annotations with `run.googleapis.com`,
                 `cloud.googleapis.com`, `serving.knative.dev`, or `autoscaling.knative.dev`
                 namespaces, and they will be rejected. All system annotations in v1 now
                 have a corresponding field in v2 RevisionTemplate.
+
+            .. raw:: html
+
+                <p>This field follows Kubernetes annotations' namespacing, limits, and
+                rules.
         scaling (google.cloud.run_v2.types.RevisionScaling):
             Scaling settings for this Revision.
         vpc_access (google.cloud.run_v2.types.VpcAccess):
             VPC Access configuration to use for this
             Revision. For more information, visit
             https://cloud.google.com/run/docs/configuring/connecting-vpc.
         timeout (google.protobuf.duration_pb2.Duration):
@@ -87,14 +100,16 @@
             A reference to a customer managed encryption
             key (CMEK) to use to encrypt this container
             image. For more information, go to
             https://cloud.google.com/run/docs/securing/using-cmek
         max_instance_request_concurrency (int):
             Sets the maximum number of requests that each
             serving instance can receive.
+        session_affinity (bool):
+            Enable session affinity.
     """
 
     revision: str = proto.Field(
         proto.STRING,
         number=1,
     )
     labels: MutableMapping[str, str] = proto.MapField(
@@ -145,10 +160,14 @@
         proto.STRING,
         number=14,
     )
     max_instance_request_concurrency: int = proto.Field(
         proto.INT32,
         number=15,
     )
+    session_affinity: bool = proto.Field(
+        proto.BOOL,
+        number=19,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/service.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,17 +94,17 @@
         validate_only (bool):
             Indicates that the request should be
             validated and default values populated, without
             persisting the request or updating any
             resources.
         allow_missing (bool):
             If set to true, and if the Service does not
-            exist, it will create a new one. Caller must
-            have both create and update permissions for this
-            call if this is set to true.
+            exist, it will create a new one. The caller must
+            have 'run.services.create' permissions if this
+            is set to true and the Service does not exist.
     """
 
     service: "Service" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Service",
     )
@@ -261,21 +261,21 @@
         generation (int):
             Output only. A number that monotonically increases every
             time the user modifies the desired state. Please note that
             unlike v1, this is an int64 value. As with most Google APIs,
             its JSON representation will be a ``string`` instead of an
             ``integer``.
         labels (MutableMapping[str, str]):
-            Map of string keys and values that can be used to organize
-            and categorize objects. User-provided labels are shared with
+            Unstructured key value map that can be used to organize and
+            categorize objects. User-provided labels are shared with
             Google's billing system, so they can be used to filter, or
             break down billing charges by team, component, environment,
             state, etc. For more information, visit
             https://cloud.google.com/resource-manager/docs/creating-managing-labels
-            or https://cloud.google.com/run/docs/configuring/labels
+            or https://cloud.google.com/run/docs/configuring/labels.
 
             .. raw:: html
 
                 <p>Cloud Run API v2 does not support labels with  `run.googleapis.com`,
                 `cloud.googleapis.com`, `serving.knative.dev`, or `autoscaling.knative.dev`
                 namespaces, and they will be rejected. All system labels in v1 now have a
                 corresponding field in v2 Service.
@@ -284,22 +284,21 @@
             to store and arbitrary metadata. They are not queryable and
             should be preserved when modifying objects.
 
             .. raw:: html
 
                 <p>Cloud Run API v2 does not support annotations with `run.googleapis.com`,
                 `cloud.googleapis.com`, `serving.knative.dev`, or `autoscaling.knative.dev`
-                namespaces, and they will be rejected. All system annotations in v1 now
-                have a corresponding field in v2 Service.
+                namespaces, and they will be rejected in new resources. All system
+                annotations in v1 now have a corresponding field in v2 Service.
 
             .. raw:: html
 
                 <p>This field follows Kubernetes
-                annotations' namespacing, limits, and rules. More info:
-                https://kubernetes.io/docs/user-guide/annotations
+                annotations' namespacing, limits, and rules.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The creation time.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The last-modified time.
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The deletion time.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -320,15 +319,24 @@
             Provides the ingress settings for this Service. On output,
             returns the currently observed ingress settings, or
             INGRESS_TRAFFIC_UNSPECIFIED if no revision is active.
         launch_stage (google.api.launch_stage_pb2.LaunchStage):
             The launch stage as defined by `Google Cloud Platform Launch
             Stages <https://cloud.google.com/terms/launch-stages>`__.
             Cloud Run supports ``ALPHA``, ``BETA``, and ``GA``. If no
-            value is specified, GA is assumed.
+            value is specified, GA is assumed. Set the launch stage to a
+            preview stage on input to allow use of preview features in
+            that stage. On read (or output), describes whether the
+            resource uses preview features.
+
+            .. raw:: html
+
+                <p>
+                For example, if ALPHA is provided as input, but only BETA and GA-level
+                features are used, this field will be BETA on output.
         binary_authorization (google.cloud.run_v2.types.BinaryAuthorization):
             Settings for the Binary Authorization
             feature.
         template (google.cloud.run_v2.types.RevisionTemplate):
             Required. The template used to create
             revisions for this Service.
         traffic (MutableSequence[google.cloud.run_v2.types.TrafficTarget]):
@@ -367,14 +375,16 @@
             Output only. Detailed status information for corresponding
             traffic targets. See comments in ``reconciling`` for
             additional information on reconciliation process in Cloud
             Run.
         uri (str):
             Output only. The main URI in which this
             Service is serving traffic.
+        satisfies_pzs (bool):
+            Output only. Reserved for future use.
         reconciling (bool):
             Output only. Returns true if the Service is currently being
             acted upon by the system to bring it into the desired state.
 
             When a new Service is created, or an existing one is
             updated, Cloud Run will asynchronously perform all necessary
             steps to bring the Service to the desired serving state.
@@ -521,14 +531,18 @@
         number=35,
         message=traffic_target.TrafficTargetStatus,
     )
     uri: str = proto.Field(
         proto.STRING,
         number=36,
     )
+    satisfies_pzs: bool = proto.Field(
+        proto.BOOL,
+        number=38,
+    )
     reconciling: bool = proto.Field(
         proto.BOOL,
         number=98,
     )
     etag: str = proto.Field(
         proto.STRING,
         number=99,
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/task.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,25 +130,29 @@
             string and guaranteed to remain unchanged until
             the resource is deleted.
         generation (int):
             Output only. A number that monotonically
             increases every time the user modifies the
             desired state.
         labels (MutableMapping[str, str]):
-            KRM-style labels for the resource.
+            Output only. Unstructured key value map that
+            can be used to organize and categorize objects.
             User-provided labels are shared with Google's
             billing system, so they can be used to filter,
             or break down billing charges by team,
             component, environment, state, etc. For more
             information, visit
             https://cloud.google.com/resource-manager/docs/creating-managing-labels
             or
             https://cloud.google.com/run/docs/configuring/labels
         annotations (MutableMapping[str, str]):
-            KRM-style annotations for the resource.
+            Output only. Unstructured key value map that
+            may be set by external tools to store and
+            arbitrary metadata. They are not queryable and
+            should be preserved when modifying objects.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Represents time when the task
             was created by the job controller. It is not
             guaranteed to be set in happens-before order
             across separate operations.
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Represents time when the task
@@ -233,14 +237,16 @@
         vpc_access (google.cloud.run_v2.types.VpcAccess):
             Output only. VPC Access configuration to use
             for this Task. For more information, visit
             https://cloud.google.com/run/docs/configuring/connecting-vpc.
         log_uri (str):
             Output only. URI where logs for this
             execution can be found in Cloud Console.
+        satisfies_pzs (bool):
+            Output only. Reserved for future use.
         etag (str):
             Output only. A system-generated fingerprint
             for this version of the resource. May be used to
             detect modification conflict during updates.
     """
 
     name: str = proto.Field(
@@ -366,14 +372,18 @@
         number=29,
         message=vendor_settings.VpcAccess,
     )
     log_uri: str = proto.Field(
         proto.STRING,
         number=32,
     )
+    satisfies_pzs: bool = proto.Field(
+        proto.BOOL,
+        number=33,
+    )
     etag: str = proto.Field(
         proto.STRING,
         number=99,
     )
 
 
 class TaskAttemptResult(proto.Message):
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/task_template.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/task_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,24 @@
             Holds the single container that defines the
             unit of execution for this task.
         volumes (MutableSequence[google.cloud.run_v2.types.Volume]):
             A list of Volumes to make available to
             containers.
         max_retries (int):
             Number of retries allowed per Task, before
-            marking this Task failed.
+            marking this Task failed. Defaults to 3.
 
             This field is a member of `oneof`_ ``retries``.
         timeout (google.protobuf.duration_pb2.Duration):
             Max allowed time duration the Task may be
             active before the system will actively try to
             mark it failed and kill associated containers.
             This applies per attempt of a task, meaning each
-            retry can run for the full timeout.
+            retry can run for the full timeout. Defaults to
+            600 seconds.
         service_account (str):
             Email address of the IAM service account
             associated with the Task of a Job. The service
             account represents the identity of the running
             task, and determines what permissions the task
             has. If not provided, the task will use the
             project's default service account.
```

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/traffic_target.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/traffic_target.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google/cloud/run_v2/types/vendor_settings.py` & `google-cloud-run-0.8.0/google/cloud/run_v2/types/vendor_settings.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/google_cloud_run.egg-info/PKG-INFO` & `google-cloud-run-0.8.0/google_cloud_run.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-run
-Version: 0.7.1
+Version: 0.8.0
 Summary: Google Cloud Run API client library
 Home-page: https://github.com/googleapis/python-run
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-run-0.7.1/google_cloud_run.egg-info/SOURCES.txt` & `google-cloud-run-0.8.0/google_cloud_run.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/setup.py` & `google-cloud-run-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/tests/__init__.py` & `google-cloud-run-0.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/tests/unit/__init__.py` & `google-cloud-run-0.8.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/tests/unit/gapic/__init__.py` & `google-cloud-run-0.8.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/tests/unit/gapic/run_v2/__init__.py` & `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_executions.py` & `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_executions.py`

 * *Files 0% similar despite different names*

```diff
@@ -724,14 +724,15 @@
             observed_generation=2021,
             running_count=1417,
             succeeded_count=1581,
             failed_count=1261,
             cancelled_count=1571,
             retried_count=1399,
             log_uri="log_uri_value",
+            satisfies_pzs=True,
             etag="etag_value",
         )
         response = client.get_execution(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
@@ -750,14 +751,15 @@
     assert response.observed_generation == 2021
     assert response.running_count == 1417
     assert response.succeeded_count == 1581
     assert response.failed_count == 1261
     assert response.cancelled_count == 1571
     assert response.retried_count == 1399
     assert response.log_uri == "log_uri_value"
+    assert response.satisfies_pzs is True
     assert response.etag == "etag_value"
 
 
 def test_get_execution_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ExecutionsClient(
@@ -802,14 +804,15 @@
                 observed_generation=2021,
                 running_count=1417,
                 succeeded_count=1581,
                 failed_count=1261,
                 cancelled_count=1571,
                 retried_count=1399,
                 log_uri="log_uri_value",
+                satisfies_pzs=True,
                 etag="etag_value",
             )
         )
         response = await client.get_execution(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
@@ -829,14 +832,15 @@
     assert response.observed_generation == 2021
     assert response.running_count == 1417
     assert response.succeeded_count == 1581
     assert response.failed_count == 1261
     assert response.cancelled_count == 1571
     assert response.retried_count == 1399
     assert response.log_uri == "log_uri_value"
+    assert response.satisfies_pzs is True
     assert response.etag == "etag_value"
 
 
 @pytest.mark.asyncio
 async def test_get_execution_async_from_dict():
     await test_get_execution_async(request_type=dict)
 
@@ -1660,14 +1664,15 @@
             observed_generation=2021,
             running_count=1417,
             succeeded_count=1581,
             failed_count=1261,
             cancelled_count=1571,
             retried_count=1399,
             log_uri="log_uri_value",
+            satisfies_pzs=True,
             etag="etag_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = execution.Execution.pb(return_value)
@@ -1690,14 +1695,15 @@
     assert response.observed_generation == 2021
     assert response.running_count == 1417
     assert response.succeeded_count == 1581
     assert response.failed_count == 1261
     assert response.cancelled_count == 1571
     assert response.retried_count == 1399
     assert response.log_uri == "log_uri_value"
+    assert response.satisfies_pzs is True
     assert response.etag == "etag_value"
 
 
 def test_get_execution_rest_required_fields(request_type=execution.GetExecutionRequest):
     transport_class = transports.ExecutionsRestTransport
 
     request_init = {}
```

### Comparing `google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_jobs.py` & `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -935,14 +935,15 @@
             last_modifier="last_modifier_value",
             client="client_value",
             client_version="client_version_value",
             launch_stage=launch_stage_pb2.LaunchStage.UNIMPLEMENTED,
             observed_generation=2021,
             execution_count=1628,
             reconciling=True,
+            satisfies_pzs=True,
             etag="etag_value",
         )
         response = client.get_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
@@ -957,14 +958,15 @@
     assert response.last_modifier == "last_modifier_value"
     assert response.client == "client_value"
     assert response.client_version == "client_version_value"
     assert response.launch_stage == launch_stage_pb2.LaunchStage.UNIMPLEMENTED
     assert response.observed_generation == 2021
     assert response.execution_count == 1628
     assert response.reconciling is True
+    assert response.satisfies_pzs is True
     assert response.etag == "etag_value"
 
 
 def test_get_job_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = JobsClient(
@@ -1005,14 +1007,15 @@
                 last_modifier="last_modifier_value",
                 client="client_value",
                 client_version="client_version_value",
                 launch_stage=launch_stage_pb2.LaunchStage.UNIMPLEMENTED,
                 observed_generation=2021,
                 execution_count=1628,
                 reconciling=True,
+                satisfies_pzs=True,
                 etag="etag_value",
             )
         )
         response = await client.get_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
@@ -1028,14 +1031,15 @@
     assert response.last_modifier == "last_modifier_value"
     assert response.client == "client_value"
     assert response.client_version == "client_version_value"
     assert response.launch_stage == launch_stage_pb2.LaunchStage.UNIMPLEMENTED
     assert response.observed_generation == 2021
     assert response.execution_count == 1628
     assert response.reconciling is True
+    assert response.satisfies_pzs is True
     assert response.etag == "etag_value"
 
 
 @pytest.mark.asyncio
 async def test_get_job_async_from_dict():
     await test_get_job_async(request_type=dict)
 
@@ -2850,15 +2854,19 @@
                                     "secret_key_ref": {
                                         "secret": "secret_value",
                                         "version": "version_value",
                                     }
                                 },
                             }
                         ],
-                        "resources": {"limits": {}, "cpu_idle": True},
+                        "resources": {
+                            "limits": {},
+                            "cpu_idle": True,
+                            "startup_cpu_boost": True,
+                        },
                         "ports": [{"name": "name_value", "container_port": 1511}],
                         "volume_mounts": [
                             {"name": "name_value", "mount_path": "mount_path_value"}
                         ],
                         "working_dir": "working_dir_value",
                         "liveness_probe": {
                             "initial_delay_seconds": 2214,
@@ -2866,14 +2874,15 @@
                             "period_seconds": 1489,
                             "failure_threshold": 1812,
                             "http_get": {
                                 "path": "path_value",
                                 "http_headers": [
                                     {"name": "name_value", "value": "value_value"}
                                 ],
+                                "port": 453,
                             },
                             "tcp_socket": {"port": 453},
                             "grpc": {"port": 453, "service": "service_value"},
                         },
                         "startup_probe": {},
                     }
                 ],
@@ -2919,14 +2928,15 @@
         "execution_count": 1628,
         "latest_created_execution": {
             "name": "name_value",
             "create_time": {},
             "completion_time": {},
         },
         "reconciling": True,
+        "satisfies_pzs": True,
         "etag": "etag_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
@@ -3166,15 +3176,19 @@
                                     "secret_key_ref": {
                                         "secret": "secret_value",
                                         "version": "version_value",
                                     }
                                 },
                             }
                         ],
-                        "resources": {"limits": {}, "cpu_idle": True},
+                        "resources": {
+                            "limits": {},
+                            "cpu_idle": True,
+                            "startup_cpu_boost": True,
+                        },
                         "ports": [{"name": "name_value", "container_port": 1511}],
                         "volume_mounts": [
                             {"name": "name_value", "mount_path": "mount_path_value"}
                         ],
                         "working_dir": "working_dir_value",
                         "liveness_probe": {
                             "initial_delay_seconds": 2214,
@@ -3182,14 +3196,15 @@
                             "period_seconds": 1489,
                             "failure_threshold": 1812,
                             "http_get": {
                                 "path": "path_value",
                                 "http_headers": [
                                     {"name": "name_value", "value": "value_value"}
                                 ],
+                                "port": 453,
                             },
                             "tcp_socket": {"port": 453},
                             "grpc": {"port": 453, "service": "service_value"},
                         },
                         "startup_probe": {},
                     }
                 ],
@@ -3235,14 +3250,15 @@
         "execution_count": 1628,
         "latest_created_execution": {
             "name": "name_value",
             "create_time": {},
             "completion_time": {},
         },
         "reconciling": True,
+        "satisfies_pzs": True,
         "etag": "etag_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
@@ -3347,14 +3363,15 @@
             last_modifier="last_modifier_value",
             client="client_value",
             client_version="client_version_value",
             launch_stage=launch_stage_pb2.LaunchStage.UNIMPLEMENTED,
             observed_generation=2021,
             execution_count=1628,
             reconciling=True,
+            satisfies_pzs=True,
             etag="etag_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = job.Job.pb(return_value)
@@ -3373,14 +3390,15 @@
     assert response.last_modifier == "last_modifier_value"
     assert response.client == "client_value"
     assert response.client_version == "client_version_value"
     assert response.launch_stage == launch_stage_pb2.LaunchStage.UNIMPLEMENTED
     assert response.observed_generation == 2021
     assert response.execution_count == 1628
     assert response.reconciling is True
+    assert response.satisfies_pzs is True
     assert response.etag == "etag_value"
 
 
 def test_get_job_rest_required_fields(request_type=job.GetJobRequest):
     transport_class = transports.JobsRestTransport
 
     request_init = {}
@@ -3985,15 +4003,19 @@
                                     "secret_key_ref": {
                                         "secret": "secret_value",
                                         "version": "version_value",
                                     }
                                 },
                             }
                         ],
-                        "resources": {"limits": {}, "cpu_idle": True},
+                        "resources": {
+                            "limits": {},
+                            "cpu_idle": True,
+                            "startup_cpu_boost": True,
+                        },
                         "ports": [{"name": "name_value", "container_port": 1511}],
                         "volume_mounts": [
                             {"name": "name_value", "mount_path": "mount_path_value"}
                         ],
                         "working_dir": "working_dir_value",
                         "liveness_probe": {
                             "initial_delay_seconds": 2214,
@@ -4001,14 +4023,15 @@
                             "period_seconds": 1489,
                             "failure_threshold": 1812,
                             "http_get": {
                                 "path": "path_value",
                                 "http_headers": [
                                     {"name": "name_value", "value": "value_value"}
                                 ],
+                                "port": 453,
                             },
                             "tcp_socket": {"port": 453},
                             "grpc": {"port": 453, "service": "service_value"},
                         },
                         "startup_probe": {},
                     }
                 ],
@@ -4054,14 +4077,15 @@
         "execution_count": 1628,
         "latest_created_execution": {
             "name": "name_value",
             "create_time": {},
             "completion_time": {},
         },
         "reconciling": True,
+        "satisfies_pzs": True,
         "etag": "etag_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
@@ -4277,15 +4301,19 @@
                                     "secret_key_ref": {
                                         "secret": "secret_value",
                                         "version": "version_value",
                                     }
                                 },
                             }
                         ],
-                        "resources": {"limits": {}, "cpu_idle": True},
+                        "resources": {
+                            "limits": {},
+                            "cpu_idle": True,
+                            "startup_cpu_boost": True,
+                        },
                         "ports": [{"name": "name_value", "container_port": 1511}],
                         "volume_mounts": [
                             {"name": "name_value", "mount_path": "mount_path_value"}
                         ],
                         "working_dir": "working_dir_value",
                         "liveness_probe": {
                             "initial_delay_seconds": 2214,
@@ -4293,14 +4321,15 @@
                             "period_seconds": 1489,
                             "failure_threshold": 1812,
                             "http_get": {
                                 "path": "path_value",
                                 "http_headers": [
                                     {"name": "name_value", "value": "value_value"}
                                 ],
+                                "port": 453,
                             },
                             "tcp_socket": {"port": 453},
                             "grpc": {"port": 453, "service": "service_value"},
                         },
                         "startup_probe": {},
                     }
                 ],
@@ -4346,14 +4375,15 @@
         "execution_count": 1628,
         "latest_created_execution": {
             "name": "name_value",
             "create_time": {},
             "completion_time": {},
         },
         "reconciling": True,
+        "satisfies_pzs": True,
         "etag": "etag_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
```

### Comparing `google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_revisions.py` & `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_revisions.py`

 * *Files 0% similar despite different names*

```diff
@@ -719,14 +719,16 @@
             service_account="service_account_value",
             execution_environment=vendor_settings.ExecutionEnvironment.EXECUTION_ENVIRONMENT_GEN1,
             encryption_key="encryption_key_value",
             encryption_key_revocation_action=vendor_settings.EncryptionKeyRevocationAction.PREVENT_NEW,
             reconciling=True,
             observed_generation=2021,
             log_uri="log_uri_value",
+            satisfies_pzs=True,
+            session_affinity=True,
             etag="etag_value",
         )
         response = client.get_revision(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
@@ -749,14 +751,16 @@
     assert (
         response.encryption_key_revocation_action
         == vendor_settings.EncryptionKeyRevocationAction.PREVENT_NEW
     )
     assert response.reconciling is True
     assert response.observed_generation == 2021
     assert response.log_uri == "log_uri_value"
+    assert response.satisfies_pzs is True
+    assert response.session_affinity is True
     assert response.etag == "etag_value"
 
 
 def test_get_revision_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RevisionsClient(
@@ -799,14 +803,16 @@
                 service_account="service_account_value",
                 execution_environment=vendor_settings.ExecutionEnvironment.EXECUTION_ENVIRONMENT_GEN1,
                 encryption_key="encryption_key_value",
                 encryption_key_revocation_action=vendor_settings.EncryptionKeyRevocationAction.PREVENT_NEW,
                 reconciling=True,
                 observed_generation=2021,
                 log_uri="log_uri_value",
+                satisfies_pzs=True,
+                session_affinity=True,
                 etag="etag_value",
             )
         )
         response = await client.get_revision(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
@@ -830,14 +836,16 @@
     assert (
         response.encryption_key_revocation_action
         == vendor_settings.EncryptionKeyRevocationAction.PREVENT_NEW
     )
     assert response.reconciling is True
     assert response.observed_generation == 2021
     assert response.log_uri == "log_uri_value"
+    assert response.satisfies_pzs is True
+    assert response.session_affinity is True
     assert response.etag == "etag_value"
 
 
 @pytest.mark.asyncio
 async def test_get_revision_async_from_dict():
     await test_get_revision_async(request_type=dict)
 
@@ -1553,14 +1561,16 @@
             service_account="service_account_value",
             execution_environment=vendor_settings.ExecutionEnvironment.EXECUTION_ENVIRONMENT_GEN1,
             encryption_key="encryption_key_value",
             encryption_key_revocation_action=vendor_settings.EncryptionKeyRevocationAction.PREVENT_NEW,
             reconciling=True,
             observed_generation=2021,
             log_uri="log_uri_value",
+            satisfies_pzs=True,
+            session_affinity=True,
             etag="etag_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = revision.Revision.pb(return_value)
@@ -1587,14 +1597,16 @@
     assert (
         response.encryption_key_revocation_action
         == vendor_settings.EncryptionKeyRevocationAction.PREVENT_NEW
     )
     assert response.reconciling is True
     assert response.observed_generation == 2021
     assert response.log_uri == "log_uri_value"
+    assert response.satisfies_pzs is True
+    assert response.session_affinity is True
     assert response.etag == "etag_value"
 
 
 def test_get_revision_rest_required_fields(request_type=revision.GetRevisionRequest):
     transport_class = transports.RevisionsRestTransport
 
     request_init = {}
```

### Comparing `google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_services.py` & `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -931,14 +931,15 @@
             client_version="client_version_value",
             ingress=vendor_settings.IngressTraffic.INGRESS_TRAFFIC_ALL,
             launch_stage=launch_stage_pb2.LaunchStage.UNIMPLEMENTED,
             observed_generation=2021,
             latest_ready_revision="latest_ready_revision_value",
             latest_created_revision="latest_created_revision_value",
             uri="uri_value",
+            satisfies_pzs=True,
             reconciling=True,
             etag="etag_value",
         )
         response = client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
@@ -957,14 +958,15 @@
     assert response.client_version == "client_version_value"
     assert response.ingress == vendor_settings.IngressTraffic.INGRESS_TRAFFIC_ALL
     assert response.launch_stage == launch_stage_pb2.LaunchStage.UNIMPLEMENTED
     assert response.observed_generation == 2021
     assert response.latest_ready_revision == "latest_ready_revision_value"
     assert response.latest_created_revision == "latest_created_revision_value"
     assert response.uri == "uri_value"
+    assert response.satisfies_pzs is True
     assert response.reconciling is True
     assert response.etag == "etag_value"
 
 
 def test_get_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
@@ -1009,14 +1011,15 @@
                 client_version="client_version_value",
                 ingress=vendor_settings.IngressTraffic.INGRESS_TRAFFIC_ALL,
                 launch_stage=launch_stage_pb2.LaunchStage.UNIMPLEMENTED,
                 observed_generation=2021,
                 latest_ready_revision="latest_ready_revision_value",
                 latest_created_revision="latest_created_revision_value",
                 uri="uri_value",
+                satisfies_pzs=True,
                 reconciling=True,
                 etag="etag_value",
             )
         )
         response = await client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
@@ -1036,14 +1039,15 @@
     assert response.client_version == "client_version_value"
     assert response.ingress == vendor_settings.IngressTraffic.INGRESS_TRAFFIC_ALL
     assert response.launch_stage == launch_stage_pb2.LaunchStage.UNIMPLEMENTED
     assert response.observed_generation == 2021
     assert response.latest_ready_revision == "latest_ready_revision_value"
     assert response.latest_created_revision == "latest_created_revision_value"
     assert response.uri == "uri_value"
+    assert response.satisfies_pzs is True
     assert response.reconciling is True
     assert response.etag == "etag_value"
 
 
 @pytest.mark.asyncio
 async def test_get_service_async_from_dict():
     await test_get_service_async(request_type=dict)
@@ -2496,15 +2500,19 @@
                                 "secret_key_ref": {
                                     "secret": "secret_value",
                                     "version": "version_value",
                                 }
                             },
                         }
                     ],
-                    "resources": {"limits": {}, "cpu_idle": True},
+                    "resources": {
+                        "limits": {},
+                        "cpu_idle": True,
+                        "startup_cpu_boost": True,
+                    },
                     "ports": [{"name": "name_value", "container_port": 1511}],
                     "volume_mounts": [
                         {"name": "name_value", "mount_path": "mount_path_value"}
                     ],
                     "working_dir": "working_dir_value",
                     "liveness_probe": {
                         "initial_delay_seconds": 2214,
@@ -2512,14 +2520,15 @@
                         "period_seconds": 1489,
                         "failure_threshold": 1812,
                         "http_get": {
                             "path": "path_value",
                             "http_headers": [
                                 {"name": "name_value", "value": "value_value"}
                             ],
+                            "port": 453,
                         },
                         "tcp_socket": {"port": 453},
                         "grpc": {"port": 453, "service": "service_value"},
                     },
                     "startup_probe": {},
                 }
             ],
@@ -2541,14 +2550,15 @@
                         "instances": ["instances_value1", "instances_value2"]
                     },
                 }
             ],
             "execution_environment": 1,
             "encryption_key": "encryption_key_value",
             "max_instance_request_concurrency": 3436,
+            "session_affinity": True,
         },
         "traffic": [
             {
                 "type_": 1,
                 "revision": "revision_value",
                 "percent": 753,
                 "tag": "tag_value",
@@ -2574,14 +2584,15 @@
                 "revision": "revision_value",
                 "percent": 753,
                 "tag": "tag_value",
                 "uri": "uri_value",
             }
         ],
         "uri": "uri_value",
+        "satisfies_pzs": True,
         "reconciling": True,
         "etag": "etag_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
@@ -2830,15 +2841,19 @@
                                 "secret_key_ref": {
                                     "secret": "secret_value",
                                     "version": "version_value",
                                 }
                             },
                         }
                     ],
-                    "resources": {"limits": {}, "cpu_idle": True},
+                    "resources": {
+                        "limits": {},
+                        "cpu_idle": True,
+                        "startup_cpu_boost": True,
+                    },
                     "ports": [{"name": "name_value", "container_port": 1511}],
                     "volume_mounts": [
                         {"name": "name_value", "mount_path": "mount_path_value"}
                     ],
                     "working_dir": "working_dir_value",
                     "liveness_probe": {
                         "initial_delay_seconds": 2214,
@@ -2846,14 +2861,15 @@
                         "period_seconds": 1489,
                         "failure_threshold": 1812,
                         "http_get": {
                             "path": "path_value",
                             "http_headers": [
                                 {"name": "name_value", "value": "value_value"}
                             ],
+                            "port": 453,
                         },
                         "tcp_socket": {"port": 453},
                         "grpc": {"port": 453, "service": "service_value"},
                     },
                     "startup_probe": {},
                 }
             ],
@@ -2875,14 +2891,15 @@
                         "instances": ["instances_value1", "instances_value2"]
                     },
                 }
             ],
             "execution_environment": 1,
             "encryption_key": "encryption_key_value",
             "max_instance_request_concurrency": 3436,
+            "session_affinity": True,
         },
         "traffic": [
             {
                 "type_": 1,
                 "revision": "revision_value",
                 "percent": 753,
                 "tag": "tag_value",
@@ -2908,14 +2925,15 @@
                 "revision": "revision_value",
                 "percent": 753,
                 "tag": "tag_value",
                 "uri": "uri_value",
             }
         ],
         "uri": "uri_value",
+        "satisfies_pzs": True,
         "reconciling": True,
         "etag": "etag_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
@@ -3024,14 +3042,15 @@
             client_version="client_version_value",
             ingress=vendor_settings.IngressTraffic.INGRESS_TRAFFIC_ALL,
             launch_stage=launch_stage_pb2.LaunchStage.UNIMPLEMENTED,
             observed_generation=2021,
             latest_ready_revision="latest_ready_revision_value",
             latest_created_revision="latest_created_revision_value",
             uri="uri_value",
+            satisfies_pzs=True,
             reconciling=True,
             etag="etag_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
@@ -3054,14 +3073,15 @@
     assert response.client_version == "client_version_value"
     assert response.ingress == vendor_settings.IngressTraffic.INGRESS_TRAFFIC_ALL
     assert response.launch_stage == launch_stage_pb2.LaunchStage.UNIMPLEMENTED
     assert response.observed_generation == 2021
     assert response.latest_ready_revision == "latest_ready_revision_value"
     assert response.latest_created_revision == "latest_created_revision_value"
     assert response.uri == "uri_value"
+    assert response.satisfies_pzs is True
     assert response.reconciling is True
     assert response.etag == "etag_value"
 
 
 def test_get_service_rest_required_fields(request_type=service.GetServiceRequest):
     transport_class = transports.ServicesRestTransport
 
@@ -3675,15 +3695,19 @@
                                 "secret_key_ref": {
                                     "secret": "secret_value",
                                     "version": "version_value",
                                 }
                             },
                         }
                     ],
-                    "resources": {"limits": {}, "cpu_idle": True},
+                    "resources": {
+                        "limits": {},
+                        "cpu_idle": True,
+                        "startup_cpu_boost": True,
+                    },
                     "ports": [{"name": "name_value", "container_port": 1511}],
                     "volume_mounts": [
                         {"name": "name_value", "mount_path": "mount_path_value"}
                     ],
                     "working_dir": "working_dir_value",
                     "liveness_probe": {
                         "initial_delay_seconds": 2214,
@@ -3691,14 +3715,15 @@
                         "period_seconds": 1489,
                         "failure_threshold": 1812,
                         "http_get": {
                             "path": "path_value",
                             "http_headers": [
                                 {"name": "name_value", "value": "value_value"}
                             ],
+                            "port": 453,
                         },
                         "tcp_socket": {"port": 453},
                         "grpc": {"port": 453, "service": "service_value"},
                     },
                     "startup_probe": {},
                 }
             ],
@@ -3720,14 +3745,15 @@
                         "instances": ["instances_value1", "instances_value2"]
                     },
                 }
             ],
             "execution_environment": 1,
             "encryption_key": "encryption_key_value",
             "max_instance_request_concurrency": 3436,
+            "session_affinity": True,
         },
         "traffic": [
             {
                 "type_": 1,
                 "revision": "revision_value",
                 "percent": 753,
                 "tag": "tag_value",
@@ -3753,14 +3779,15 @@
                 "revision": "revision_value",
                 "percent": 753,
                 "tag": "tag_value",
                 "uri": "uri_value",
             }
         ],
         "uri": "uri_value",
+        "satisfies_pzs": True,
         "reconciling": True,
         "etag": "etag_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
@@ -3987,15 +4014,19 @@
                                 "secret_key_ref": {
                                     "secret": "secret_value",
                                     "version": "version_value",
                                 }
                             },
                         }
                     ],
-                    "resources": {"limits": {}, "cpu_idle": True},
+                    "resources": {
+                        "limits": {},
+                        "cpu_idle": True,
+                        "startup_cpu_boost": True,
+                    },
                     "ports": [{"name": "name_value", "container_port": 1511}],
                     "volume_mounts": [
                         {"name": "name_value", "mount_path": "mount_path_value"}
                     ],
                     "working_dir": "working_dir_value",
                     "liveness_probe": {
                         "initial_delay_seconds": 2214,
@@ -4003,14 +4034,15 @@
                         "period_seconds": 1489,
                         "failure_threshold": 1812,
                         "http_get": {
                             "path": "path_value",
                             "http_headers": [
                                 {"name": "name_value", "value": "value_value"}
                             ],
+                            "port": 453,
                         },
                         "tcp_socket": {"port": 453},
                         "grpc": {"port": 453, "service": "service_value"},
                     },
                     "startup_probe": {},
                 }
             ],
@@ -4032,14 +4064,15 @@
                         "instances": ["instances_value1", "instances_value2"]
                     },
                 }
             ],
             "execution_environment": 1,
             "encryption_key": "encryption_key_value",
             "max_instance_request_concurrency": 3436,
+            "session_affinity": True,
         },
         "traffic": [
             {
                 "type_": 1,
                 "revision": "revision_value",
                 "percent": 753,
                 "tag": "tag_value",
@@ -4065,14 +4098,15 @@
                 "revision": "revision_value",
                 "percent": 753,
                 "tag": "tag_value",
                 "uri": "uri_value",
             }
         ],
         "uri": "uri_value",
+        "satisfies_pzs": True,
         "reconciling": True,
         "etag": "etag_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
```

### Comparing `google-cloud-run-0.7.1/tests/unit/gapic/run_v2/test_tasks.py` & `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -693,14 +693,15 @@
             execution_environment=vendor_settings.ExecutionEnvironment.EXECUTION_ENVIRONMENT_GEN1,
             reconciling=True,
             observed_generation=2021,
             index=536,
             retried=751,
             encryption_key="encryption_key_value",
             log_uri="log_uri_value",
+            satisfies_pzs=True,
             etag="etag_value",
         )
         response = client.get_task(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
@@ -721,14 +722,15 @@
     )
     assert response.reconciling is True
     assert response.observed_generation == 2021
     assert response.index == 536
     assert response.retried == 751
     assert response.encryption_key == "encryption_key_value"
     assert response.log_uri == "log_uri_value"
+    assert response.satisfies_pzs is True
     assert response.etag == "etag_value"
 
 
 def test_get_task_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = TasksClient(
@@ -772,14 +774,15 @@
                 execution_environment=vendor_settings.ExecutionEnvironment.EXECUTION_ENVIRONMENT_GEN1,
                 reconciling=True,
                 observed_generation=2021,
                 index=536,
                 retried=751,
                 encryption_key="encryption_key_value",
                 log_uri="log_uri_value",
+                satisfies_pzs=True,
                 etag="etag_value",
             )
         )
         response = await client.get_task(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
@@ -801,14 +804,15 @@
     )
     assert response.reconciling is True
     assert response.observed_generation == 2021
     assert response.index == 536
     assert response.retried == 751
     assert response.encryption_key == "encryption_key_value"
     assert response.log_uri == "log_uri_value"
+    assert response.satisfies_pzs is True
     assert response.etag == "etag_value"
 
 
 @pytest.mark.asyncio
 async def test_get_task_async_from_dict():
     await test_get_task_async(request_type=dict)
 
@@ -1405,14 +1409,15 @@
             execution_environment=vendor_settings.ExecutionEnvironment.EXECUTION_ENVIRONMENT_GEN1,
             reconciling=True,
             observed_generation=2021,
             index=536,
             retried=751,
             encryption_key="encryption_key_value",
             log_uri="log_uri_value",
+            satisfies_pzs=True,
             etag="etag_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = task.Task.pb(return_value)
@@ -1437,14 +1442,15 @@
     )
     assert response.reconciling is True
     assert response.observed_generation == 2021
     assert response.index == 536
     assert response.retried == 751
     assert response.encryption_key == "encryption_key_value"
     assert response.log_uri == "log_uri_value"
+    assert response.satisfies_pzs is True
     assert response.etag == "etag_value"
 
 
 def test_get_task_rest_required_fields(request_type=task.GetTaskRequest):
     transport_class = transports.TasksRestTransport
 
     request_init = {}
```

