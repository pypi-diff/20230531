# Comparing `tmp/mosaicml-cli-0.4.4.tar.gz` & `tmp/mosaicml-cli-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.4.tar", last modified: Thu May 25 21:30:03 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.5.tar", last modified: Wed May 31 00:46:57 2023, max compression
```

## Comparing `mosaicml-cli-0.4.4.tar` & `mosaicml-cli-0.4.5.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.037665 mosaicml-cli-0.4.4/
--rw-r--r--   0 jeffchen   (501) staff       (20)      696 2023-05-25 21:30:03.037473 mosaicml-cli-0.4.4/PKG-INFO
--rw-r--r--   0 jeffchen   (501) staff       (20)     7187 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/README.md
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.952363 mosaicml-cli-0.4.4/mcli/
--rw-r--r--   0 jeffchen   (501) staff       (20)     2092 2023-05-25 21:29:20.000000 mosaicml-cli-0.4.4/mcli/__init__.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.953282 mosaicml-cli-0.4.4/mcli/api/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/api/__init__.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.954009 mosaicml-cli-0.4.4/mcli/api/cluster/
--rw-r--r--   0 jeffchen   (501) staff       (20)      134 2022-10-27 20:22:32.000000 mosaicml-cli-0.4.4/mcli/api/cluster/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     4237 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.954745 mosaicml-cli-0.4.4/mcli/api/engine/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/api/engine/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    25914 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/engine/engine.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    10685 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/exceptions.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.958833 mosaicml-cli-0.4.4/mcli/api/inference_deployments/
--rw-r--r--   0 jeffchen   (501) staff       (20)     1521 2023-05-25 21:29:20.000000 mosaicml-cli-0.4.4/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3301 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     5105 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3603 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     8458 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1277 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1603 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6483 2023-05-25 21:29:20.000000 mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.959555 mosaicml-cli-0.4.4/mcli/api/mint/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/api/mint/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     7759 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/mint/shell.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2676 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/mint/tty.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.961895 mosaicml-cli-0.4.4/mcli/api/model/
--rw-r--r--   0 jeffchen   (501) staff       (20)     1114 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/model/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6322 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/model/cluster_details.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     4611 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/api/model/inference_deployment.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    10439 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/model/run.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.964675 mosaicml-cli-0.4.4/mcli/api/runs/
--rw-r--r--   0 jeffchen   (501) staff       (20)     1199 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/runs/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2804 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/runs/api_create_run.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     4211 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     8405 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    10933 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     5213 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/api/runs/api_start_run.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     5405 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3937 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    10619 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.965184 mosaicml-cli-0.4.4/mcli/api/schema/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/api/schema/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      636 2022-11-11 00:18:38.000000 mosaicml-cli-0.4.4/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.967286 mosaicml-cli-0.4.4/mcli/api/secrets/
--rw-r--r--   0 jeffchen   (501) staff       (20)      309 2022-09-19 22:17:10.000000 mosaicml-cli-0.4.4/mcli/api/secrets/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2386 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3019 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3718 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2354 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/api/typing_future.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.968150 mosaicml-cli-0.4.4/mcli/api/users/
--rw-r--r--   0 jeffchen   (501) staff       (20)      139 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/api/users/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2715 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.968648 mosaicml-cli-0.4.4/mcli/cli/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/cli/__init__.py
--rwxr-xr-x   0 jeffchen   (501) staff       (20)     6387 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/cli.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.969555 mosaicml-cli-0.4.4/mcli/cli/common/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-02-01 21:37:29.000000 mosaicml-cli-0.4.4/mcli/cli/common/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2461 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6874 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.970615 mosaicml-cli-0.4.4/mcli/cli/m_connect/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1694 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.971403 mosaicml-cli-0.4.4/mcli/cli/m_create/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/cli/m_create/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2385 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_create/m_create.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    16874 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.972337 mosaicml-cli-0.4.4/mcli/cli/m_delete/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6184 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_delete/delete.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     5805 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.972746 mosaicml-cli-0.4.4/mcli/cli/m_deploy/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3896 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.976257 mosaicml-cli-0.4.4/mcli/cli/m_describe/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-01-26 01:45:43.000000 mosaicml-cli-0.4.4/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3902 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     9999 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2002 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.983582 mosaicml-cli-0.4.4/mcli/cli/m_get/
--rw-r--r--   0 jeffchen   (501) staff       (20)      467 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_get/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6226 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_get/clusters.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6447 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/cli/m_get/display.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     5642 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     4803 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_get/m_get.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     9790 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_get/runs.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2189 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_get/secrets.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1580 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/cli/m_get/users.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.985053 mosaicml-cli-0.4.4/mcli/cli/m_init/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/cli/m_init/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     4115 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.990615 mosaicml-cli-0.4.4/mcli/cli/m_interactive/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     9325 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    44284 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     9321 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.998526 mosaicml-cli-0.4.4/mcli/cli/m_kube/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     5523 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1398 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2050 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6946 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:02.999464 mosaicml-cli-0.4.4/mcli/cli/m_log/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/cli/m_log/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    10380 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.000049 mosaicml-cli-0.4.4/mcli/cli/m_ping/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2091 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.000593 mosaicml-cli-0.4.4/mcli/cli/m_predict/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2610 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.001324 mosaicml-cli-0.4.4/mcli/cli/m_root/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/cli/m_root/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      536 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.002086 mosaicml-cli-0.4.4/mcli/cli/m_run/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/cli/m_run/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     8099 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.007147 mosaicml-cli-0.4.4/mcli/cli/m_set_unset/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-10-06 23:40:35.000000 mosaicml-cli-0.4.4/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2973 2023-04-18 22:36:16.000000 mosaicml-cli-0.4.4/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1802 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1940 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1421 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      881 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.007635 mosaicml-cli-0.4.4/mcli/cli/m_stop/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-27 01:04:20.000000 mosaicml-cli-0.4.4/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     4047 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.008850 mosaicml-cli-0.4.4/mcli/cli/m_util/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/cli/m_util/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      797 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_util/m_util.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6837 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/cli/m_util/util.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    12590 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/mcli/config.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.011228 mosaicml-cli-0.4.4/mcli/models/
--rw-r--r--   0 jeffchen   (501) staff       (20)     1047 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/models/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2103 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/models/gpu_type.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    10321 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/models/inference_deployment_config.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      427 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/models/mcli_cluster.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      456 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/models/mcli_envvar.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6724 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/models/mcli_secret.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    19547 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/models/run_config.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.011710 mosaicml-cli-0.4.4/mcli/objects/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/objects/__init__.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.015852 mosaicml-cli-0.4.4/mcli/objects/secrets/
--rw-r--r--   0 jeffchen   (501) staff       (20)     1090 2022-12-09 18:28:49.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.018517 mosaicml-cli-0.4.4/mcli/objects/secrets/create/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1646 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/create/base.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2244 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2408 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6377 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3858 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3001 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     5342 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      783 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1017 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/env_var.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      556 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/gcp.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1267 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/mounted.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      967 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/oci.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      961 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/s3.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1718 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.019329 mosaicml-cli-0.4.4/mcli/proto/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/proto/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1477 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.019749 mosaicml-cli-0.4.4/mcli/sdk/
--rw-r--r--   0 jeffchen   (501) staff       (20)     1918 2023-05-25 21:29:20.000000 mosaicml-cli-0.4.4/mcli/sdk/__init__.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.030951 mosaicml-cli-0.4.4/mcli/utils/
--rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/utils/__init__.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     5306 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/utils/utils_cli.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6073 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/utils/utils_config.py
--rw-r--r--   0 jeffchen   (501) staff       (20)      740 2022-09-23 00:37:17.000000 mosaicml-cli-0.4.4/mcli/utils/utils_date.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    10749 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/utils/utils_docker.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2225 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/utils/utils_epilog.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    10774 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/utils/utils_interactive.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     4527 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/utils/utils_logging.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     2160 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6614 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/utils/utils_pypi.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3115 2022-09-08 17:54:07.000000 mosaicml-cli-0.4.4/mcli/utils/utils_rich.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     5035 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/utils/utils_run_status.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     4350 2022-09-09 21:35:49.000000 mosaicml-cli-0.4.4/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1103 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/mcli/utils/utils_spinner.py
--rw-r--r--   0 jeffchen   (501) staff       (20)    10751 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/utils/utils_string_functions.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1677 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/mcli/utils/utils_types.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     1001 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/mcli/utils/utils_yaml.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     3885 2023-05-25 21:29:30.000000 mosaicml-cli-0.4.4/mcli/version.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.035961 mosaicml-cli-0.4.4/mosaicml_cli.egg-info/
--rw-r--r--   0 jeffchen   (501) staff       (20)      696 2023-05-25 21:30:02.000000 mosaicml-cli-0.4.4/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 jeffchen   (501) staff       (20)     4868 2023-05-25 21:30:02.000000 mosaicml-cli-0.4.4/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jeffchen   (501) staff       (20)        1 2023-05-25 21:30:02.000000 mosaicml-cli-0.4.4/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jeffchen   (501) staff       (20)       75 2023-05-25 21:30:02.000000 mosaicml-cli-0.4.4/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 jeffchen   (501) staff       (20)     1655 2023-05-25 21:30:02.000000 mosaicml-cli-0.4.4/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 jeffchen   (501) staff       (20)        5 2023-05-25 21:30:02.000000 mosaicml-cli-0.4.4/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 jeffchen   (501) staff       (20)    31087 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/pyproject.toml
--rw-r--r--   0 jeffchen   (501) staff       (20)       38 2023-05-25 21:30:03.037751 mosaicml-cli-0.4.4/setup.cfg
--rw-r--r--   0 jeffchen   (501) staff       (20)     3057 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.4/setup.py
-drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-25 21:30:03.037072 mosaicml-cli-0.4.4/tests/
--rw-r--r--   0 jeffchen   (501) staff       (20)     5991 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.4/tests/test_config.py
--rw-r--r--   0 jeffchen   (501) staff       (20)       62 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.4/tests/test_simple.py
--rw-r--r--   0 jeffchen   (501) staff       (20)     6116 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.4/tests/test_upgrade.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.685102 mosaicml-cli-0.4.5/
+-rw-r--r--   0 wai        (502) staff       (20)      696 2023-05-31 00:46:57.684329 mosaicml-cli-0.4.5/PKG-INFO
+-rw-r--r--   0 wai        (502) staff       (20)     7187 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/README.md
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.613771 mosaicml-cli-0.4.5/mcli/
+-rw-r--r--   0 wai        (502) staff       (20)     2092 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.614497 mosaicml-cli-0.4.5/mcli/api/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.615218 mosaicml-cli-0.4.5/mcli/api/cluster/
+-rw-r--r--   0 wai        (502) staff       (20)      134 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/cluster/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     4237 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.615758 mosaicml-cli-0.4.5/mcli/api/engine/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/engine/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)    25914 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/engine/engine.py
+-rw-r--r--   0 wai        (502) staff       (20)    10685 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/exceptions.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.628369 mosaicml-cli-0.4.5/mcli/api/inference_deployments/
+-rw-r--r--   0 wai        (502) staff       (20)     1521 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     3301 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 wai        (502) staff       (20)     5105 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 wai        (502) staff       (20)     3603 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 wai        (502) staff       (20)     8458 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 wai        (502) staff       (20)     1277 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 wai        (502) staff       (20)     1603 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 wai        (502) staff       (20)     6483 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.628958 mosaicml-cli-0.4.5/mcli/api/mint/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.4.5/mcli/api/mint/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     7759 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/mint/shell.py
+-rw-r--r--   0 wai        (502) staff       (20)     2676 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/mint/tty.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.629932 mosaicml-cli-0.4.5/mcli/api/model/
+-rw-r--r--   0 wai        (502) staff       (20)     1114 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/model/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     6322 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/model/cluster_details.py
+-rw-r--r--   0 wai        (502) staff       (20)     4611 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 wai        (502) staff       (20)    10439 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/model/run.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.632579 mosaicml-cli-0.4.5/mcli/api/runs/
+-rw-r--r--   0 wai        (502) staff       (20)     1199 2023-05-30 21:28:48.000000 mosaicml-cli-0.4.5/mcli/api/runs/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2804 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 wai        (502) staff       (20)     4211 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     8906 2023-05-30 23:51:22.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 wai        (502) staff       (20)    10933 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     5213 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 wai        (502) staff       (20)     5405 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     3937 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 wai        (502) staff       (20)    10619 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.633205 mosaicml-cli-0.4.5/mcli/api/schema/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/schema/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)      636 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.634190 mosaicml-cli-0.4.5/mcli/api/secrets/
+-rw-r--r--   0 wai        (502) staff       (20)      309 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/secrets/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2386 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 wai        (502) staff       (20)     3019 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 wai        (502) staff       (20)     3718 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 wai        (502) staff       (20)     2354 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/typing_future.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.634785 mosaicml-cli-0.4.5/mcli/api/users/
+-rw-r--r--   0 wai        (502) staff       (20)      139 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/users/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2715 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.635385 mosaicml-cli-0.4.5/mcli/cli/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/__init__.py
+-rwxr-xr-x   0 wai        (502) staff       (20)     6387 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/cli.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.636113 mosaicml-cli-0.4.5/mcli/cli/common/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/common/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2461 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 wai        (502) staff       (20)     6874 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.636471 mosaicml-cli-0.4.5/mcli/cli/m_connect/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     1694 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.637186 mosaicml-cli-0.4.5/mcli/cli/m_create/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2385 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 wai        (502) staff       (20)    16874 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.637827 mosaicml-cli-0.4.5/mcli/cli/m_delete/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     6184 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 wai        (502) staff       (20)     5805 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.638107 mosaicml-cli-0.4.5/mcli/cli/m_deploy/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     3896 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.639247 mosaicml-cli-0.4.5/mcli/cli/m_describe/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     3902 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 wai        (502) staff       (20)     9988 2023-05-30 23:51:22.000000 mosaicml-cli-0.4.5/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     2002 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.640715 mosaicml-cli-0.4.5/mcli/cli/m_get/
+-rw-r--r--   0 wai        (502) staff       (20)      467 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     6226 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 wai        (502) staff       (20)     6447 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/display.py
+-rw-r--r--   0 wai        (502) staff       (20)     5642 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 wai        (502) staff       (20)     4803 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 wai        (502) staff       (20)     9790 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     2189 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 wai        (502) staff       (20)     1580 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/users.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.641076 mosaicml-cli-0.4.5/mcli/cli/m_init/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     4115 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.641709 mosaicml-cli-0.4.5/mcli/cli/m_interactive/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     9325 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 wai        (502) staff       (20)    44284 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 wai        (502) staff       (20)     9321 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.642367 mosaicml-cli-0.4.5/mcli/cli/m_kube/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     5523 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 wai        (502) staff       (20)     1398 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 wai        (502) staff       (20)     2050 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 wai        (502) staff       (20)     6946 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.642623 mosaicml-cli-0.4.5/mcli/cli/m_log/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)    10845 2023-05-30 23:51:22.000000 mosaicml-cli-0.4.5/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.643023 mosaicml-cli-0.4.5/mcli/cli/m_ping/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2091 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.643379 mosaicml-cli-0.4.5/mcli/cli/m_predict/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-04 20:22:39.000000 mosaicml-cli-0.4.5/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2610 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.643628 mosaicml-cli-0.4.5/mcli/cli/m_root/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)      536 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.643904 mosaicml-cli-0.4.5/mcli/cli/m_run/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     8099 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.644938 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2973 2023-04-04 20:22:39.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 wai        (502) staff       (20)     1802 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 wai        (502) staff       (20)     1940 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 wai        (502) staff       (20)     1421 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 wai        (502) staff       (20)      881 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.645305 mosaicml-cli-0.4.5/mcli/cli/m_stop/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     4047 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.645694 mosaicml-cli-0.4.5/mcli/cli/m_util/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)      797 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 wai        (502) staff       (20)     6837 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_util/util.py
+-rw-r--r--   0 wai        (502) staff       (20)    12590 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/config.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.646826 mosaicml-cli-0.4.5/mcli/models/
+-rw-r--r--   0 wai        (502) staff       (20)     1047 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2103 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/gpu_type.py
+-rw-r--r--   0 wai        (502) staff       (20)    10321 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 wai        (502) staff       (20)      427 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/mcli_cluster.py
+-rw-r--r--   0 wai        (502) staff       (20)      456 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/mcli_envvar.py
+-rw-r--r--   0 wai        (502) staff       (20)     6724 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/mcli_secret.py
+-rw-r--r--   0 wai        (502) staff       (20)    19547 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/run_config.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.646994 mosaicml-cli-0.4.5/mcli/objects/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/objects/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.648710 mosaicml-cli-0.4.5/mcli/objects/secrets/
+-rw-r--r--   0 wai        (502) staff       (20)     1090 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.653650 mosaicml-cli-0.4.5/mcli/objects/secrets/create/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     1646 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 wai        (502) staff       (20)     2244 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 wai        (502) staff       (20)     2408 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 wai        (502) staff       (20)     6377 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 wai        (502) staff       (20)     3858 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 wai        (502) staff       (20)     3001 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 wai        (502) staff       (20)     5342 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 wai        (502) staff       (20)      783 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 wai        (502) staff       (20)     1017 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 wai        (502) staff       (20)      556 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 wai        (502) staff       (20)     1267 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 wai        (502) staff       (20)      967 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/oci.py
+-rw-r--r--   0 wai        (502) staff       (20)      961 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/s3.py
+-rw-r--r--   0 wai        (502) staff       (20)     1718 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.656141 mosaicml-cli-0.4.5/mcli/proto/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.4.5/mcli/proto/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     1477 2023-04-18 23:46:04.000000 mosaicml-cli-0.4.5/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.657277 mosaicml-cli-0.4.5/mcli/sdk/
+-rw-r--r--   0 wai        (502) staff       (20)     1918 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/sdk/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.674046 mosaicml-cli-0.4.5/mcli/utils/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     5306 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/utils/utils_cli.py
+-rw-r--r--   0 wai        (502) staff       (20)     6073 2023-04-18 16:53:02.000000 mosaicml-cli-0.4.5/mcli/utils/utils_config.py
+-rw-r--r--   0 wai        (502) staff       (20)      740 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/utils_date.py
+-rw-r--r--   0 wai        (502) staff       (20)    10749 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_docker.py
+-rw-r--r--   0 wai        (502) staff       (20)     2225 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_epilog.py
+-rw-r--r--   0 wai        (502) staff       (20)    10774 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_interactive.py
+-rw-r--r--   0 wai        (502) staff       (20)     4527 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_logging.py
+-rw-r--r--   0 wai        (502) staff       (20)     2160 2023-04-20 18:58:30.000000 mosaicml-cli-0.4.5/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 wai        (502) staff       (20)     6614 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/utils/utils_pypi.py
+-rw-r--r--   0 wai        (502) staff       (20)     3115 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/utils_rich.py
+-rw-r--r--   0 wai        (502) staff       (20)     5035 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_run_status.py
+-rw-r--r--   0 wai        (502) staff       (20)     4350 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 wai        (502) staff       (20)     1103 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/utils/utils_spinner.py
+-rw-r--r--   0 wai        (502) staff       (20)    10751 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 wai        (502) staff       (20)     1677 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_types.py
+-rw-r--r--   0 wai        (502) staff       (20)     1001 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/utils_yaml.py
+-rw-r--r--   0 wai        (502) staff       (20)     3885 2023-05-30 23:51:33.000000 mosaicml-cli-0.4.5/mcli/version.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.680384 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/
+-rw-r--r--   0 wai        (502) staff       (20)      696 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 wai        (502) staff       (20)     4868 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 wai        (502) staff       (20)        1 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 wai        (502) staff       (20)       75 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 wai        (502) staff       (20)     1655 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 wai        (502) staff       (20)        5 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 wai        (502) staff       (20)    31087 2023-05-30 21:24:59.000000 mosaicml-cli-0.4.5/pyproject.toml
+-rw-r--r--   0 wai        (502) staff       (20)       38 2023-05-31 00:46:57.685437 mosaicml-cli-0.4.5/setup.cfg
+-rw-r--r--   0 wai        (502) staff       (20)     3057 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/setup.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.682855 mosaicml-cli-0.4.5/tests/
+-rw-r--r--   0 wai        (502) staff       (20)     5991 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/tests/test_config.py
+-rw-r--r--   0 wai        (502) staff       (20)       62 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/tests/test_simple.py
+-rw-r--r--   0 wai        (502) staff       (20)     6116 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.4/PKG-INFO` & `mosaicml-cli-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.4
+Version: 0.4.5
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.4/README.md` & `mosaicml-cli-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/__init__.py` & `mosaicml-cli-0.4.5/mcli/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.5/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.5/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/exceptions.py` & `mosaicml-cli-0.4.5/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.5/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.5/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.5/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.5/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.5/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.5/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/model/run.py` & `mosaicml-cli-0.4.5/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.5/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.5/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.5/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.5/mcli/api/runs/api_get_run_logs.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,37 +25,40 @@
 def get_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: Literal[False] = False,
     failed: Optional[bool] = False,
+    attempt: Optional[int] = None,
 ) -> Generator[str, None, None]:
     ...
 
 
 @overload
 def get_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
     failed: Optional[bool] = False,
+    attempt: Optional[int] = None,
 ) -> Generator[Future[str], None, None]:
     ...
 
 
 def get_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: bool = False,
     failed: Optional[bool] = False,
+    attempt: Optional[int] = None,
 ) -> Union[Generator[str, None, None], Generator[Future[str], None, None]]:
     """Get the current logs for an active or completed run
 
     Get the current logs for an active or completed run in the MosaicML platform.
     This returns the full logs as a ``str``, as they exist at the time the request is
     made. If you want to follow the logs for an active run line-by-line, use
     :func:`follow_run_logs`.
@@ -69,29 +72,34 @@
             If the the call takes too long, a :exc:`~concurrent.futures.TimeoutError`
             will be raised. If ``future`` is ``True``, this value will be ignored.
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future` . If True, the
             call to :func:`get_run_logs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the log text, use ``return_value.result()`` with an optional
             ``timeout`` argument.
-        failed (``bool``): Return the logs of the first failed rank if ``True``. ``False`` by default.
+        failed (``bool``): Return the logs of the first failed rank for the provided attempt if ``True``.
+            ``False`` by default.
+        attempt (``Optional[int]``): Attempt (0-indexed) of a run to get logs for. Defaults to the last attempt
 
     Returns:
         If future is False:
             The full log text for a run at the time of the request as a :obj:`str`
         Otherwise:
             A :class:`~concurrent.futures.Future` for the log text
     """
     # Convert to strings
     run_name = run.name if isinstance(run, Run) else run
 
     filters: Dict[str, Any] = {'name': run_name, 'follow': False, 'failed': failed}
     if rank is not None:
         filters['nodeRank'] = rank
 
+    if attempt is not None:
+        filters['attemptIndex'] = attempt
+
     cfg = MCLIConfig.load_config(safe=True)
     if cfg.user_id:
         filters['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     variables = {VARIABLE_DATA_NAME: filters}
@@ -108,35 +116,38 @@
 @overload
 def follow_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: Literal[False] = False,
+    attempt: Optional[int] = None,
 ) -> Generator[str, None, None]:
     ...
 
 
 @overload
 def follow_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
+    attempt: Optional[int] = None,
 ) -> Generator[Future[str], None, None]:
     ...
 
 
 def follow_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: bool = False,
+    attempt: Optional[int] = None,
 ) -> Union[Generator[str, None, None], Generator[Future[str], None, None]]:
     """Follow the logs for an active or completed run in the MosaicML platform
 
     This returns a :obj:`generator` of individual log lines, line-by-line, and will wait until
     new lines are produced if the run is still active.
 
     Args:
@@ -166,14 +177,17 @@
     # Convert to strings
     run_name = run.name if isinstance(run, Run) else run
 
     filters: Dict[str, Any] = {'name': run_name, 'follow': True}
     if rank is not None:
         filters['nodeRank'] = rank
 
+    if attempt is not None:
+        filters['attemptIndex'] = attempt
+
     cfg = MCLIConfig.load_config(safe=True)
     if cfg.user_id:
         filters['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     variables = {VARIABLE_DATA_NAME: filters}
@@ -207,22 +221,22 @@
     """
 
     def __init__(self, return_key: str):
         self.return_key = return_key
         super().__init__()
 
     def update_offset(self, variables: Dict[str, Any]) -> Dict[str, Any]:
-        if self.return_key == "getRunLogs":
+        if self.return_key == 'getRunLogs':
             variables['getRunLogsInput']['offset'] = self.num_bytes_read
         else:
             variables['getInferenceDeploymentLogsInput']['offset'] = self.num_bytes_read
         return variables
 
     def parse_message(self, data: Dict[str, str]) -> str:
         """Get the next message from the GraphQL logging subscription
         """
         # Convert from base64 string to a bytestring
-        b64_message = data['getRunLogs'] if self.return_key == "getRunLogs" else data['getInferenceDeploymentLogs']
+        b64_message = data['getRunLogs'] if self.return_key == 'getRunLogs' else data['getInferenceDeploymentLogs']
         b64_bytes = b64_message.encode('utf8')
         message_bytes = base64.b64decode(b64_bytes)
 
         return self.decode(message_bytes)
```

### Comparing `mosaicml-cli-0.4.4/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.5/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.5/mcli/api/runs/api_start_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.5/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.5/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.5/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.5/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.5/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.5/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.5/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/typing_future.py` & `mosaicml-cli-0.4.5/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.5/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/cli.py` & `mosaicml-cli-0.4.5/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.5/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.5/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.5/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.5/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.5/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.5/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.5/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.5/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.5/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.5/mcli/cli/m_describe/describe_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     PRIORITY = 'priority'
 
 
 class DescribeRunOriginalInputColumns(Enum):
     SUBMITTED_CONFIG = 'submitted_config'
 
 
-RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Run ID', 'Last Attempt ID', 'Cluster', 'Image', 'GPU Type', 'GPU Num']
+RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Run ID', 'Last Attempt ID', 'Cluster', 'Image', 'Priority']
 
 RUN_LIFECYCLE_DISPLAY_NAMES = ['Status', 'Reached At', 'Duration', 'Reason']
 RUN_NODES_DISPLAY_NAMES = ['Node Name']
 SUBMITTED_CONFIG = ['Run Config']
 
 
 @dataclass
```

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.5/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.5/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.5/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.5/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.5/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.5/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.5/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.5/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.5/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.5/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.5/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.5/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.4.5/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.4.5/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.4.5/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.4.5/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.5/mcli/cli/m_log/m_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 > mcli logs multinode-run-1234 --rank 1
 
 # Follow the logs for an ongoing run
 > mcli logs run-1234 --follow
 
 # View the logs for a failed run
 > mcli logs run-1234 --failed
+
+# View the logs for the run's first attempt
+> mcli logs run-1234 --attempt-index 0
 """
 
 # pylint: disable-next=invalid-name
 DEPLOYMENT_LOG_EXAMPLES = """
 
 Examples:
 
@@ -56,52 +59,48 @@
 > mcli get deployment logs
 
 # View the logs of a specific restart in a deployment
 > mcli get deployment logs deploy-1234 --restart 5
 """
 
 
-def _get_run_logs(
-    run: Run,
-    follow: bool,
-    rank: Optional[int],
-    failed: bool,
-) -> Tuple[Optional[str], int]:
+def _get_run_logs(run: Run, follow: bool, rank: Optional[int], failed: bool,
+                  attempt: Optional[int]) -> Tuple[Optional[str], int]:
 
     if run.status == RunStatus.FAILED and not failed and rank is None:
         logger.info(f'{INFO} Run {run.name} has failed. Defaulting to show the first failed node rank.')
         failed = True
 
     if follow and run.status.before(RunStatus.RUNNING):
         with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
             run = watcher.follow()
 
     if run.status == RunStatus.FAILED_PULL:
         CommonLog(logger).log_pod_failed_pull(run.name, run.config.image)
-        return "", 1
+        return '', 1
     elif run.status.before(RunStatus.QUEUED, inclusive=True):
         # Pod still waiting to be scheduled. Return
         logger.error(f'{FAIL} Run {run.name} has not been scheduled')
-        return "", 1
+        return '', 1
     elif run.status.before(RunStatus.RUNNING):
         # Pod still not running, probably because follow==False
         logger.error(f'{FAIL} Run has not yet started. You can check the status with `mcli get runs` '
                      'and try again later.')
-        return "", 1
+        return '', 1
 
     last_line: Optional[str] = None
     end: str = ''
     if follow:
-        for line in follow_run_logs(run, rank=rank):
+        for line in follow_run_logs(run, rank=rank, attempt=attempt):
             print(line, end=end)
             if line:
                 last_line = line
         return last_line, int(0)
     else:
-        log_lines = get_run_logs(run, rank=rank, failed=failed)
+        log_lines = get_run_logs(run, rank=rank, failed=failed, attempt=attempt)
         for line in log_lines:
             # When using progress bars we randomly get newlines added. By default,
             # kubernetes does not return empty lines when streaming, which is
             # replicated in `follow_run_logs`. We'll do that here for parity
             if line:
                 last_line = line
                 print(line, end='')
@@ -135,14 +134,15 @@
 def get_logs(
     submission_type: SubmissionType,
     submission_name: Optional[str] = None,
     rank: Optional[int] = None,
     restart: Optional[int] = None,
     follow: bool = False,
     failed: bool = False,
+    attempt: Optional[int] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
     try:
         submission_type_str = submission_type.value.lower()
         with err_console.status(f'Getting {submission_type_str} details...') as spinner:
@@ -160,15 +160,15 @@
                 if not submissions:
                     raise MAPIException(status=HTTPStatus.NOT_FOUND,
                                         message=f'Could not find {submission_type_str}: [red]{submission_name}[/]')
 
         last_line: Optional[str] = None
         #Have to check type to satisfy pyright
         if isinstance(submissions[0], Run):
-            last_line, err = _get_run_logs(submissions[0], follow, rank, failed)
+            last_line, err = _get_run_logs(submissions[0], follow, rank, failed, attempt)
             if err == 1:
                 return 1
         elif isinstance(submissions[0], InferenceDeployment):
             last_line, err = _get_deployment_logs(submissions[0], restart)
             if err == 1:
                 return 1
 
@@ -214,14 +214,20 @@
 
 def configure_runs_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.set_defaults(func=partial(get_logs, SubmissionType.RUN))
     parser.add_argument('submission_name',
                         metavar='RUN',
                         nargs='?',
                         help='The name of the run. If not provided, will return the logs of the latest run')
+    parser.add_argument('--attempt',
+                        type=int,
+                        default=None,
+                        metavar='N',
+                        dest='attempt',
+                        help="Attempt (0-indexed) of the run whose logs you'd like to view.")
     rank_grp = parser.add_mutually_exclusive_group()
     rank_grp.add_argument('--rank',
                           type=int,
                           default=None,
                           metavar='N',
                           help='Rank of the node in a multi-node run whose logs you\'d like to view')
     rank_grp.add_argument('--failed',
```

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.5/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.5/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.5/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.5/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.5/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.5/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.5/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/config.py` & `mosaicml-cli-0.4.5/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/models/__init__.py` & `mosaicml-cli-0.4.5/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.5/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.5/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.5/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/models/run_config.py` & `mosaicml-cli-0.4.5/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.5/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.5/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.5/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.5/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mcli/version.py` & `mosaicml-cli-0.4.5/mcli/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     # pylint: disable=import-outside-toplevel
     from mcli.config import FeatureFlag, MCLIConfig
     from mcli.utils.utils_pypi import get_latest_alpha_package_version, get_latest_package_version
 
     latest_version = current_version = Version.from_string(__version__)
     conf = MCLIConfig.load_config(safe=True)
     is_alpha = current_version.is_alpha or conf.feature_enabled(FeatureFlag.ALPHA_TESTER)
-    version_output = ""
+    version_output = ''
     try:
         if is_alpha:
             latest_version = get_latest_alpha_package_version()
         else:
             latest_version = get_latest_package_version()
     except Exception:  # pylint: disable=broad-except
         return 'Failed to fetch current version from PyPI.'
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.4.4"
+__version__ = '0.4.5'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.4/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.5/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.4
+Version: 0.4.5
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.4/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.5/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.5/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
-furo==2022.9.29
+build>=0.10.0
+radon>=5.1.0
+yapf>=0.33.0
 toml>=0.10.2
-sphinxcontrib-qthelp>=1.0.3
-sphinxcontrib-devhelp>=1.0.2
-pyright>=1.1.256
-sphinx-panels==0.6.0
+sphinx-argparse==0.4.0
 sphinx-markdown-tables==0.0.17
-radon>=5.1.0
-twine>=4.0.2
-isort>=5.9.3
+sphinx-design
 pre-commit>=2.17.0
-yapf>=0.33.0
-sphinx-rtd-theme==1.0.0
+isort>=5.9.3
 pylint>=2.12.2
 sphinx==4.4.0
-sphinxemoji==0.2.0
-sphinx_external_toc==0.3.0
-sphinx-design
-sphinxcontrib-serializinghtml==1.1.5
 pytest>=6.2.5
-sphinxext-opengraph==0.8.2
-build>=0.10.0
-sphinx-argparse==0.4.0
-sphinxcontrib-applehelp>=1.0.2
-myst-parser>=0.16.1
-pytest-mock>=3.7.0
+sphinxcontrib-serializinghtml==1.1.5
+sphinxemoji==0.2.0
 sphinxcontrib-jsmath>=1.0.1
-sphinxcontrib-katex==0.9.4
-docutils>=0.17.0
-sphinxcontrib-images>=0.9.4
+twine>=4.0.2
+sphinx-panels==0.6.0
+furo==2022.9.29
 pytest-cov>=4.0.0
-sphinxcontrib-htmlhelp>=2.0.0
+sphinxcontrib-applehelp>=1.0.2
+sphinxext-opengraph==0.8.2
+sphinxcontrib-katex==0.9.4
+sphinxcontrib-qthelp>=1.0.3
+myst-parser>=0.16.1
 sphinx-copybutton==0.5.2
+pyright>=1.1.256
+sphinxcontrib-htmlhelp>=2.0.0
+sphinxcontrib-images>=0.9.4
+sphinxcontrib-devhelp>=1.0.2
+sphinx-rtd-theme==1.0.0
+docutils>=0.17.0
+sphinx_external_toc==0.3.0
+pytest-mock>=3.7.0
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
```

### Comparing `mosaicml-cli-0.4.4/pyproject.toml` & `mosaicml-cli-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/setup.py` & `mosaicml-cli-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/tests/test_config.py` & `mosaicml-cli-0.4.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.4/tests/test_upgrade.py` & `mosaicml-cli-0.4.5/tests/test_upgrade.py`

 * *Files identical despite different names*

