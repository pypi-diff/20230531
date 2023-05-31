# Comparing `tmp/geti-sdk-1.5.6.tar.gz` & `tmp/geti-sdk-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geti-sdk-1.5.6.tar", last modified: Tue May 23 14:37:51 2023, max compression
+gzip compressed data, was "geti-sdk-1.5.7.tar", last modified: Wed May 31 16:38:43 2023, max compression
```

## Comparing `geti-sdk-1.5.6.tar` & `geti-sdk-1.5.7.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/LICENSE
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/MANIFEST.in
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/README.md
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.632274 geti-sdk-1.5.6/geti_sdk/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.636274 geti-sdk-1.5.6/geti_sdk/annotation_readers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/base_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.636274 geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/geti_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5107 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/algorithms.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/annotation_scene.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/annotations.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/code_deployment_info.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/configurable_parameter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/configurable_parameter_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/configuration.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/configuration_identifiers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/data_models/containers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/containers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/containers/algorithm_list.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/containers/media_list.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/data_models/enums/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/annotation_kind.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/configuration_enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/deployment_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/domain.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/job_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/job_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/media_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/model_status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      979 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/optimization_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/prediction_mode.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/shape_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/task_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/job.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/label.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/media.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/media_identifiers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/model_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/performance.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/predictions.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/project.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/shapes.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/task.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/task_annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3018 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/test_result.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/demos/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/constants.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.632274 geti-sdk-1.5.6/geti_sdk/demos/data/
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/demos/data/example/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data/example/dogs.png
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/anomaly_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/coco_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5727 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/download_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/video_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/anomaly_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/coco_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/deployment/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/deployment/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/data_models/intermediate_inference_result.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/data_models/region_of_interest.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26692 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/deployed_model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/deployment.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/deployment/resources/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/resources/OVMS_README.md
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/resources/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/utils.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55163 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/geti.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/http_session/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/http_session/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/http_session/exception.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/http_session/geti_session.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/http_session/server_config.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6554 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/platform_versions.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/rest_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3723 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2203 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/active_learning_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/configuration_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/dataset_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/deployment_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/image_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16826 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/media_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/video_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/model_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/prediction_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26172 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/project_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/task_templates.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4808 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/testing_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12260 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/training_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_converters/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2163 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6393 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6909 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/configuration_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/job_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/media_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2411 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/model_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/project_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/status_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1545 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/test_result_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/utils/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/algorithm_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/credentials_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/dictionary_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5753 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/job_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/label_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/plot_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/serialization_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/workspace_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.636274 geti-sdk-1.5.6/geti_sdk.egg-info/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5927 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/requires.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/top_level.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/pyproject.toml
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/requirements/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/requirements/requirements-dev.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/requirements/requirements-docs.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/requirements/requirements-notebooks.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/requirements/requirements.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/setup.cfg
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/setup.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/tests/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/tests/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/tests/conftest.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/tests/helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/constants.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/finalizers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/fixtures.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/plotting.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/project_service.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/training.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/vcr_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.130146 geti-sdk-1.5.7/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/LICENSE
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/MANIFEST.in
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-31 16:38:43.130146 geti-sdk-1.5.7/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/README.md
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.114146 geti-sdk-1.5.7/geti_sdk/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.114146 geti-sdk-1.5.7/geti_sdk/annotation_readers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/annotation_readers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/annotation_readers/base_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.114146 geti-sdk-1.5.7/geti_sdk/annotation_readers/datumaro_annotation_reader/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/annotation_readers/geti_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.118146 geti-sdk-1.5.7/geti_sdk/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5107 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/algorithms.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/annotation_scene.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/annotations.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/code_deployment_info.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/configurable_parameter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/configurable_parameter_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/configuration.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/configuration_identifiers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.118146 geti-sdk-1.5.7/geti_sdk/data_models/containers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/containers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/containers/algorithm_list.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/containers/media_list.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.118146 geti-sdk-1.5.7/geti_sdk/data_models/enums/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/annotation_kind.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/configuration_enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/deployment_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/domain.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/job_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/job_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/media_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/model_status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      979 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/optimization_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/prediction_mode.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/shape_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/enums/task_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/job.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/label.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/media.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/media_identifiers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/model_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/performance.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/predictions.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/project.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/shapes.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/task.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/task_annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3018 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/test_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/data_models/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.118146 geti-sdk-1.5.7/geti_sdk/demos/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/constants.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.110146 geti-sdk-1.5.7/geti_sdk/demos/data/
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.118146 geti-sdk-1.5.7/geti_sdk/demos/data/example/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/data/example/dogs.png
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.122146 geti-sdk-1.5.7/geti_sdk/demos/data_helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/data_helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/data_helpers/anomaly_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/data_helpers/coco_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5727 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/data_helpers/download_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/data_helpers/video_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.122146 geti-sdk-1.5.7/geti_sdk/demos/demo_projects/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/demo_projects/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/demo_projects/anomaly_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/demo_projects/coco_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/demos/demo_projects/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.122146 geti-sdk-1.5.7/geti_sdk/deployment/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/deployment/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.122146 geti-sdk-1.5.7/geti_sdk/deployment/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/deployment/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/deployment/data_models/intermediate_inference_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/deployment/data_models/region_of_interest.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26692 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/deployment/deployed_model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    23062 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/deployment/deployment.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.122146 geti-sdk-1.5.7/geti_sdk/deployment/resources/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/deployment/resources/OVMS_README.md
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/deployment/resources/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/deployment/utils.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55582 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/geti.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.122146 geti-sdk-1.5.7/geti_sdk/http_session/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/http_session/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/http_session/exception.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/http_session/geti_session.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/http_session/server_config.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6554 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/platform_versions.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.126146 geti-sdk-1.5.7/geti_sdk/rest_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3723 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2203 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/active_learning_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.126146 geti-sdk-1.5.7/geti_sdk/rest_clients/annotation_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/annotation_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/annotation_clients/annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/configuration_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/dataset_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/deployment_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.126146 geti-sdk-1.5.7/geti_sdk/rest_clients/media_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/media_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8828 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/media_client/image_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16826 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/media_client/media_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/media_client/video_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/model_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/prediction_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.126146 geti-sdk-1.5.7/geti_sdk/rest_clients/project_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/project_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26172 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/project_client/project_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/project_client/task_templates.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4808 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/testing_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12260 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_clients/training_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.126146 geti-sdk-1.5.7/geti_sdk/rest_converters/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2163 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.126146 geti-sdk-1.5.7/geti_sdk/rest_converters/annotation_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6393 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6909 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/configuration_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/job_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/media_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2411 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/model_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.126146 geti-sdk-1.5.7/geti_sdk/rest_converters/prediction_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/project_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/status_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1545 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/rest_converters/test_result_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.130146 geti-sdk-1.5.7/geti_sdk/utils/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/algorithm_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/credentials_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/dictionary_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5753 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/job_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/label_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/plot_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/serialization_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/geti_sdk/utils/workspace_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.114146 geti-sdk-1.5.7/geti_sdk.egg-info/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-31 16:38:43.000000 geti-sdk-1.5.7/geti_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5927 2023-05-31 16:38:43.000000 geti-sdk-1.5.7/geti_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-05-31 16:38:43.000000 geti-sdk-1.5.7/geti_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-31 16:38:43.000000 geti-sdk-1.5.7/geti_sdk.egg-info/requires.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-05-31 16:38:43.000000 geti-sdk-1.5.7/geti_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/pyproject.toml
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.130146 geti-sdk-1.5.7/requirements/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/requirements/requirements-dev.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/requirements/requirements-docs.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/requirements/requirements-notebooks.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/requirements/requirements.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-05-31 16:38:43.130146 geti-sdk-1.5.7/setup.cfg
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/setup.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.130146 geti-sdk-1.5.7/tests/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/conftest.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-31 16:38:43.130146 geti-sdk-1.5.7/tests/helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/constants.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/finalizers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/fixtures.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/plotting.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/project_service.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/training.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-05-31 16:30:11.000000 geti-sdk-1.5.7/tests/helpers/vcr_helpers.py
```

### Comparing `geti-sdk-1.5.6/LICENSE` & `geti-sdk-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/PKG-INFO` & `geti-sdk-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.6
+Version: 1.5.7
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.6/README.md` & `geti-sdk-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/__init__.py` & `geti-sdk-1.5.7/geti_sdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,10 +74,10 @@
 
    .. automethod:: upload_and_predict_media_folder
 
 """
 
 from .geti import Geti
 
-__version__ = "1.5.6"
+__version__ = "1.5.7"
 
 __all__ = ["Geti"]
```

### Comparing `geti-sdk-1.5.6/geti_sdk/annotation_readers/__init__.py` & `geti-sdk-1.5.7/geti_sdk/annotation_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/annotation_readers/base_annotation_reader.py` & `geti-sdk-1.5.7/geti_sdk/annotation_readers/base_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py` & `geti-sdk-1.5.7/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py` & `geti-sdk-1.5.7/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py` & `geti-sdk-1.5.7/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/annotation_readers/directory_tree_annotation_reader.py` & `geti-sdk-1.5.7/geti_sdk/annotation_readers/directory_tree_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/annotation_readers/geti_annotation_reader.py` & `geti-sdk-1.5.7/geti_sdk/annotation_readers/geti_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/__init__.py` & `geti-sdk-1.5.7/geti_sdk/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/algorithms.py` & `geti-sdk-1.5.7/geti_sdk/data_models/algorithms.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/annotation_scene.py` & `geti-sdk-1.5.7/geti_sdk/data_models/annotation_scene.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/annotations.py` & `geti-sdk-1.5.7/geti_sdk/data_models/annotations.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/code_deployment_info.py` & `geti-sdk-1.5.7/geti_sdk/data_models/code_deployment_info.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/configurable_parameter.py` & `geti-sdk-1.5.7/geti_sdk/data_models/configurable_parameter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/configurable_parameter_group.py` & `geti-sdk-1.5.7/geti_sdk/data_models/configurable_parameter_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/configuration.py` & `geti-sdk-1.5.7/geti_sdk/data_models/configuration.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/configuration_identifiers.py` & `geti-sdk-1.5.7/geti_sdk/data_models/configuration_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/containers/__init__.py` & `geti-sdk-1.5.7/geti_sdk/data_models/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/containers/algorithm_list.py` & `geti-sdk-1.5.7/geti_sdk/data_models/containers/algorithm_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/containers/media_list.py` & `geti-sdk-1.5.7/geti_sdk/data_models/containers/media_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/__init__.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/annotation_kind.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/annotation_kind.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/annotation_state.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/configuration_enums.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/configuration_enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/deployment_state.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/deployment_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/domain.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/domain.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/job_state.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/job_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/job_type.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/job_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/media_type.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/media_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/model_status.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/model_status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/optimization_type.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/optimization_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/prediction_mode.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/prediction_mode.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/shape_type.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/shape_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/enums/task_type.py` & `geti-sdk-1.5.7/geti_sdk/data_models/enums/task_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/job.py` & `geti-sdk-1.5.7/geti_sdk/data_models/job.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/label.py` & `geti-sdk-1.5.7/geti_sdk/data_models/label.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/media.py` & `geti-sdk-1.5.7/geti_sdk/data_models/media.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/media_identifiers.py` & `geti-sdk-1.5.7/geti_sdk/data_models/media_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/model.py` & `geti-sdk-1.5.7/geti_sdk/data_models/model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/model_group.py` & `geti-sdk-1.5.7/geti_sdk/data_models/model_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/performance.py` & `geti-sdk-1.5.7/geti_sdk/data_models/performance.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/predictions.py` & `geti-sdk-1.5.7/geti_sdk/data_models/predictions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/project.py` & `geti-sdk-1.5.7/geti_sdk/data_models/project.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/shapes.py` & `geti-sdk-1.5.7/geti_sdk/data_models/shapes.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/status.py` & `geti-sdk-1.5.7/geti_sdk/data_models/status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/task.py` & `geti-sdk-1.5.7/geti_sdk/data_models/task.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/task_annotation_state.py` & `geti-sdk-1.5.7/geti_sdk/data_models/task_annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/test_result.py` & `geti-sdk-1.5.7/geti_sdk/data_models/test_result.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/data_models/utils.py` & `geti-sdk-1.5.7/geti_sdk/data_models/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/__init__.py` & `geti-sdk-1.5.7/geti_sdk/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/constants.py` & `geti-sdk-1.5.7/geti_sdk/demos/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/data/example/dogs.png` & `geti-sdk-1.5.7/geti_sdk/demos/data/example/dogs.png`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/__init__.py` & `geti-sdk-1.5.7/geti_sdk/demos/data_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/anomaly_helpers.py` & `geti-sdk-1.5.7/geti_sdk/demos/data_helpers/anomaly_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/coco_helpers.py` & `geti-sdk-1.5.7/geti_sdk/demos/data_helpers/coco_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/download_helpers.py` & `geti-sdk-1.5.7/geti_sdk/demos/data_helpers/download_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/video_helpers.py` & `geti-sdk-1.5.7/geti_sdk/demos/data_helpers/video_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/demo_projects/__init__.py` & `geti-sdk-1.5.7/geti_sdk/demos/demo_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/demo_projects/anomaly_demos.py` & `geti-sdk-1.5.7/geti_sdk/demos/demo_projects/anomaly_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/demo_projects/coco_demos.py` & `geti-sdk-1.5.7/geti_sdk/demos/demo_projects/coco_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/demos/demo_projects/utils.py` & `geti-sdk-1.5.7/geti_sdk/demos/demo_projects/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/deployment/__init__.py` & `geti-sdk-1.5.7/geti_sdk/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/deployment/data_models/__init__.py` & `geti-sdk-1.5.7/geti_sdk/deployment/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/deployment/data_models/intermediate_inference_result.py` & `geti-sdk-1.5.7/geti_sdk/deployment/data_models/intermediate_inference_result.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/deployment/data_models/region_of_interest.py` & `geti-sdk-1.5.7/geti_sdk/deployment/data_models/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/deployment/deployed_model.py` & `geti-sdk-1.5.7/geti_sdk/deployment/deployed_model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/deployment/deployment.py` & `geti-sdk-1.5.7/geti_sdk/deployment/deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,30 @@
 import logging
 import os
 import shutil
 from typing import Any, Dict, List, Optional, Union
 
 import attr
 import numpy as np
+import otx
 
 from geti_sdk.data_models import (
     Annotation,
     Label,
     Prediction,
     Project,
     ScoredLabel,
     Task,
     TaskType,
 )
+from geti_sdk.data_models.predictions import ResultMedium
 from geti_sdk.data_models.shapes import Polygon, Rectangle, RotatedRectangle
 from geti_sdk.deployment.data_models import ROI, IntermediateInferenceResult
 from geti_sdk.rest_converters import ProjectRESTConverter
 
-from ..data_models.predictions import ResultMedium
 from .deployed_model import DeployedModel
 from .utils import OVMS_README_PATH, generate_ovms_model_name
 
 
 @attr.define(slots=False)
 class Deployment:
     """
@@ -175,16 +176,27 @@
                 # For some reason the `is_anomaly` flag is not set correctly in the
                 # ote_label_schema, which will break loading the prediction converter.
                 # We set the flag here
                 for label in model.ote_label_schema.get_labels(include_empty=True):
                     if label.name == "Anomalous":
                         label.is_anomalous = True
 
+            if otx.__version__ > "1.2.0":
+                configuration = model.openvino_model_parameters
+                if "use_ellipse_shapes" not in configuration.keys():
+                    configuration.update({"use_ellipse_shapes": False})
+                converter_args = {
+                    "labels": model.ote_label_schema,
+                    "configuration": configuration,
+                }
+            else:
+                converter_args = {"labels": model.ote_label_schema}
+
             inference_converter = create_converter(
-                converter_type=task.type.to_ote_domain(), labels=model.ote_label_schema
+                converter_type=task.type.to_ote_domain(), **converter_args
             )
             inference_converters.update({task.title: inference_converter})
 
             # This is a workaround for a backwards incompatible change in later ote
             # versions
             if task.type.is_detection:
                 alternate_inference_converter = DetectionBoxToAnnotationConverter(
```

### Comparing `geti-sdk-1.5.6/geti_sdk/deployment/resources/OVMS_README.md` & `geti-sdk-1.5.7/geti_sdk/deployment/resources/OVMS_README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/deployment/resources/__init__.py` & `geti-sdk-1.5.7/geti_sdk/deployment/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/deployment/utils.py` & `geti-sdk-1.5.7/geti_sdk/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/geti.py` & `geti-sdk-1.5.7/geti_sdk/geti.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,19 +623,27 @@
         configuration_client.set_project_auto_train(auto_train=False)
 
         # Upload images
         image_client = ImageClient(
             session=self.session, workspace_id=self.workspace_id, project=project
         )
         if isinstance(annotation_reader, DatumAnnotationReader):
-            images = image_client.upload_from_list(
-                path_to_folder=path_to_images,
-                image_names=annotation_reader.get_all_image_names(),
-                n_images=number_of_images_to_upload,
-            )
+            if hasattr(annotation_reader, "get_all_image_filepaths"):
+                images = image_client.upload_from_list(
+                    path_to_folder=path_to_images,
+                    image_names=annotation_reader.get_all_image_filepaths(),
+                    n_images=number_of_images_to_upload,
+                    image_names_as_full_paths=True,
+                )
+            else:
+                images = image_client.upload_from_list(
+                    path_to_folder=path_to_images,
+                    image_names=annotation_reader.get_all_image_names(),
+                    n_images=number_of_images_to_upload,
+                )
         else:
             images = image_client.upload_folder(
                 path_to_images, n_images=number_of_images_to_upload
             )
 
         if (
             number_of_images_to_annotate < len(images)
```

### Comparing `geti-sdk-1.5.6/geti_sdk/http_session/__init__.py` & `geti-sdk-1.5.7/geti_sdk/http_session/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/http_session/exception.py` & `geti-sdk-1.5.7/geti_sdk/http_session/exception.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/http_session/geti_session.py` & `geti-sdk-1.5.7/geti_sdk/http_session/geti_session.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/http_session/server_config.py` & `geti-sdk-1.5.7/geti_sdk/http_session/server_config.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/platform_versions.py` & `geti-sdk-1.5.7/geti_sdk/platform_versions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/__init__.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/active_learning_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/active_learning_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/__init__.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/annotation_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/annotation_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/annotation_clients/annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/configuration_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/configuration_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/dataset_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/deployment_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/deployment_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/__init__.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/media_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/image_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/media_client/image_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 
 import datetime
 import glob
 import io
+import logging
 import os
 from typing import List, Optional, Sequence, Union
 
 import cv2
 import numpy as np
 
 from geti_sdk.data_models import Image, MediaType
@@ -154,27 +155,32 @@
             if extension_included:
                 image_filepaths = image_names
             else:
                 for image_name in image_names:
                     for media_extension in media_formats:
                         if os.path.isfile(image_name + media_extension):
                             image_filepaths.append(image_name + media_extension)
+                            break
             image_filepaths = image_filepaths[0:n_to_upload]
 
         else:
+            logging.debug("Retrieving full filepaths for image upload...")
             for image_name in image_names[0:n_to_upload]:
                 if not extension_included:
                     matches: List[str] = []
                     for media_extension in media_formats:
-                        matches += glob.glob(
+                        match_for_item = glob.glob(
                             os.path.join(
                                 path_to_folder, "**", f"{image_name}{media_extension}"
                             ),
                             recursive=True,
                         )
+                        if len(match_for_item) > 0:
+                            matches += match_for_item
+                            break
                 else:
                     matches = glob.glob(
                         os.path.join(path_to_folder, "**", image_name), recursive=True
                     )
                 if not matches:
                     raise ValueError(
                         f"No matching file found for image with name {image_name}"
```

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/media_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/media_client/media_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/video_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/media_client/video_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/model_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/model_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/prediction_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/prediction_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/__init__.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/project_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/project_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/project_client/project_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/task_templates.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/project_client/task_templates.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/testing_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/testing_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_clients/training_client.py` & `geti-sdk-1.5.7/geti_sdk/rest_clients/training_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/__init__.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/__init__.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/annotation_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/configuration_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/configuration_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/job_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/job_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/media_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/media_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/model_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/model_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/__init__.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/prediction_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/project_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/project_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/status_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/status_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/rest_converters/test_result_rest_converter.py` & `geti-sdk-1.5.7/geti_sdk/rest_converters/test_result_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/__init__.py` & `geti-sdk-1.5.7/geti_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/algorithm_helpers.py` & `geti-sdk-1.5.7/geti_sdk/utils/algorithm_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/credentials_helpers.py` & `geti-sdk-1.5.7/geti_sdk/utils/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/dictionary_helpers.py` & `geti-sdk-1.5.7/geti_sdk/utils/dictionary_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/job_helpers.py` & `geti-sdk-1.5.7/geti_sdk/utils/job_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/label_helpers.py` & `geti-sdk-1.5.7/geti_sdk/utils/label_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/plot_helpers.py` & `geti-sdk-1.5.7/geti_sdk/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/project_helpers.py` & `geti-sdk-1.5.7/geti_sdk/utils/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/serialization_helpers.py` & `geti-sdk-1.5.7/geti_sdk/utils/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk/utils/workspace_helpers.py` & `geti-sdk-1.5.7/geti_sdk/utils/workspace_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk.egg-info/PKG-INFO` & `geti-sdk-1.5.7/geti_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.6
+Version: 1.5.7
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.6/geti_sdk.egg-info/SOURCES.txt` & `geti-sdk-1.5.7/geti_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/geti_sdk.egg-info/requires.txt` & `geti-sdk-1.5.7/geti_sdk.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 certifi>=2022.12.7
 joblib>=1.1.1
 protobuf>=3.20.2
 ovmsclient>=2022.3
 orjson==3.8.8
 
 [dev]
-vcrpy==4.2.*
+vcrpy==4.3.*
 pytest==7.3.*
 pytest-recording==0.12.*
 pytest-cov==4.0.*
 pytest-env==0.8.*
 pytest-html==3.2.*
 flake8>=4.0
 pydocstyle>=6.1
```

### Comparing `geti-sdk-1.5.6/setup.py` & `geti-sdk-1.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/__init__.py` & `geti-sdk-1.5.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/conftest.py` & `geti-sdk-1.5.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/__init__.py` & `geti-sdk-1.5.7/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/constants.py` & `geti-sdk-1.5.7/tests/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/enums.py` & `geti-sdk-1.5.7/tests/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/finalizers.py` & `geti-sdk-1.5.7/tests/helpers/finalizers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/fixtures.py` & `geti-sdk-1.5.7/tests/helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/plotting.py` & `geti-sdk-1.5.7/tests/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/project_helpers.py` & `geti-sdk-1.5.7/tests/helpers/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/project_service.py` & `geti-sdk-1.5.7/tests/helpers/project_service.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/training.py` & `geti-sdk-1.5.7/tests/helpers/training.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.6/tests/helpers/vcr_helpers.py` & `geti-sdk-1.5.7/tests/helpers/vcr_helpers.py`

 * *Files identical despite different names*

