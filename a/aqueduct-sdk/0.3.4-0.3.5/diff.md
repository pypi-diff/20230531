# Comparing `tmp/aqueduct-sdk-0.3.4.tar.gz` & `tmp/aqueduct-sdk-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-sdk-0.3.4.tar", last modified: Wed May 24 22:48:10 2023, max compression
+gzip compressed data, was "aqueduct-sdk-0.3.5.tar", last modified: Wed May 31 20:26:22 2023, max compression
```

## Comparing `aqueduct-sdk-0.3.4.tar` & `aqueduct-sdk-0.3.5.tar`

### file list

```diff
@@ -1,118 +1,119 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.905607 aqueduct-sdk-0.3.4/aqueduct/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.909607 aqueduct-sdk-0.3.4/aqueduct/artifacts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/base_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/bool_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/generic_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/numeric_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6599 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/preview.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/system_metric.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24895 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/table_artifact.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.909607 aqueduct-sdk-0.3.4/aqueduct/backend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/backend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24525 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/backend/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/backend/response_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39473 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.909607 aqueduct-sdk-0.3.4/aqueduct/constants/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/constants/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6626 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/constants/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/constants/exports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/constants/metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52868 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/decorator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3930 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5525 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/flow_run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/github.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.909607 aqueduct-sdk-0.3.4/aqueduct/globals/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/globals/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/globals/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/globals/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/globals/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8506 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/llm_wrapper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/logger.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.913607 aqueduct-sdk-0.3.4/aqueduct/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21114 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/dag_rules.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/execution_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3061 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7786 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/operators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13906 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/response_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.913607 aqueduct-sdk-0.3.4/aqueduct/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/airflow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/aws.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      464 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/aws_lambda.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13077 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/connect_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/databricks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/dynamic_k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/ecr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4878 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/google_sheets.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8993 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4866 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/parameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9364 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5519 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/salesforce.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3528 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/save.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/spark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13323 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      738 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/schedule.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.917607 aqueduct-sdk-0.3.4/aqueduct/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/connect_config_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/dag_delta_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/dag_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/decorator_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/decorators_with_without_parentheses_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/enum_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      909 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/flow_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/helpers_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/metric_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/naming_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15641 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/serialization_test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.917607 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.917607 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/python_function.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.917607 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/test_dependency_folder/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/type_annotations.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/aqueduct/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10726 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/dag_deltas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/utils/describe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/format.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/function_packaging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/integration_validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/local_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/naming.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16574 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/type_inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8220 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/requirements/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/requirements/python-3-10.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/requirements/python-3-7.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/requirements/python-3-8.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/requirements/python-3-9.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-24 22:27:12.000000 aqueduct-sdk-0.3.4/version
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.505823 aqueduct-sdk-0.3.5/aqueduct/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.509823 aqueduct-sdk-0.3.5/aqueduct/artifacts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/base_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/bool_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/generic_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/numeric_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6593 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/preview.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/system_metric.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24892 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/table_artifact.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.509823 aqueduct-sdk-0.3.5/aqueduct/backend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/backend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28105 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/backend/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/backend/response_helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39325 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.509823 aqueduct-sdk-0.3.5/aqueduct/constants/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/constants/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6903 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/constants/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/constants/exports.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/constants/metrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52838 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/decorator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3900 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/error.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5523 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/flow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/flow_run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/github.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.513823 aqueduct-sdk-0.3.5/aqueduct/globals/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/globals/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/globals/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/globals/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/globals/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8506 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/llm_wrapper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/logger.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.513823 aqueduct-sdk-0.3.5/aqueduct/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1976 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21114 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/dag_rules.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/execution_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8353 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/operators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3046 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/resource.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14933 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/response_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.517823 aqueduct-sdk-0.3.5/aqueduct/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/airflow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/aws.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/aws_lambda.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16165 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/connect_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/databricks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7470 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/dynamic_k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1777 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/ecr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1691 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/gar.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4854 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/google_sheets.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      449 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8963 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4866 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/parameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9337 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5492 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/salesforce.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3431 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/save.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/spark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13293 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      726 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/schedule.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.521824 aqueduct-sdk-0.3.5/aqueduct/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/connect_config_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/dag_delta_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/dag_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/decorator_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/decorators_with_without_parentheses_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/enum_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      909 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/flow_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/helpers_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/metric_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/naming_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15527 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/serialization_test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.521824 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.521824 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/python_function.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.521824 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/test_dependency_folder/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6065 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/type_annotations.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/aqueduct/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10726 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/dag_deltas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/utils/describe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/format.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/function_packaging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/local_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/naming.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1416 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/resource_validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16574 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/type_inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8059 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3144 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/requirements/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/requirements/python-3-10.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/requirements/python-3-7.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/requirements/python-3-8.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/requirements/python-3-9.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-31 18:17:41.000000 aqueduct-sdk-0.3.5/version
```

### Comparing `aqueduct-sdk-0.3.4/PKG-INFO` & `aqueduct-sdk-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/__init__.py` & `aqueduct-sdk-0.3.5/aqueduct/__init__.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/artifacts/_create.py` & `aqueduct-sdk-0.3.5/aqueduct/artifacts/_create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/artifacts/base_artifact.py` & `aqueduct-sdk-0.3.5/aqueduct/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/artifacts/bool_artifact.py` & `aqueduct-sdk-0.3.5/aqueduct/artifacts/bool_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/artifacts/create.py` & `aqueduct-sdk-0.3.5/aqueduct/artifacts/create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/artifacts/generic_artifact.py` & `aqueduct-sdk-0.3.5/aqueduct/artifacts/generic_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/artifacts/numeric_artifact.py` & `aqueduct-sdk-0.3.5/aqueduct/artifacts/numeric_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/artifacts/preview.py` & `aqueduct-sdk-0.3.5/aqueduct/artifacts/preview.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,20 @@
     subgraph.set_engine_config(global_engine_config=global_engine_config)
 
     engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status_by_dag(dag=subgraph)
     for name in engine_statuses:
         engine_status = engine_statuses[name]
         if engine_status.status != K8sClusterStatusType.ACTIVE:
             print(
-                "Your preview request makes use of dynamic k8s integration %s, but the k8s cluster is in %s state. It could take 12-15 minutes for the cluster to be ready..."
+                "Your preview request makes use of dynamic k8s resource %s, but the k8s cluster is in %s state. It could take 12-15 minutes for the cluster to be ready..."
                 % (engine_status.name, engine_status.status.value)
             )
         else:
             print(
-                "Your preview request makes use of dynamic k8s integration %s and the k8s cluster is in %s state, so you are good to go!"
+                "Your preview request makes use of dynamic k8s resource %s and the k8s cluster is in %s state, so you are good to go!"
                 % (engine_status.name, engine_status.status.value)
             )
 
     preview_resp = globals.__GLOBAL_API_CLIENT__.preview(dag=subgraph)
 
     # Process all the target artifacts first. Assumption: the preview response contains a result entry
     # for each target artifact.
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/artifacts/system_metric.py` & `aqueduct-sdk-0.3.5/aqueduct/artifacts/system_metric.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/artifacts/table_artifact.py` & `aqueduct-sdk-0.3.5/aqueduct/artifacts/table_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         >>> @op
         >>> def predict(df):
         >>>     return predictions
         >>>
         >>> output_artifact = predict(input_artifact)
 
         The contents of these artifacts can be manifested locally or written to an
-        integration:
+        resource:
 
         >>> df = output_artifact.get()
         >>> print(df.head())
         >>> warehouse.save(output_artifact, table_name="output_table", update_mode="replace")
     """
 
     def __init__(
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/backend/api_client.py` & `aqueduct-sdk-0.3.5/aqueduct/backend/api_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,50 @@
+import datetime
 import io
 import json
 import uuid
 from typing import IO, Any, DefaultDict, Dict, List, Optional, Tuple, Union
 
 import requests
 from aqueduct.constants.enums import ExecutionStatus, K8sClusterActionType, RuntimeType, ServiceType
 from aqueduct.error import (
     AqueductError,
     ClientValidationError,
     InternalServerError,
     InvalidRequestError,
     InvalidUserActionException,
-    NoConnectedIntegrationsException,
+    NoConnectedResourcesException,
     ResourceNotFoundError,
     UnprocessableEntityError,
 )
 from aqueduct.logger import logger
-from aqueduct.models.dag import DAG
-from aqueduct.models.integration import BaseResource, ResourceInfo
-from aqueduct.models.operators import ParamSpec
+from aqueduct.models.artifact import ArtifactMetadata
+from aqueduct.models.dag import DAG, Metadata
+from aqueduct.models.operators import Operator, ParamSpec
+from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.models.response_models import (
     DeleteWorkflowResponse,
     DynamicEngineStatusResponse,
+    GetDagResponse,
+    GetDagResultResponse,
     GetImageURLResponse,
+    GetNodeArtifactResponse,
+    GetNodeOperatorResponse,
     GetVersionResponse,
     GetWorkflowDagResultResponse,
     GetWorkflowResponse,
+    GetWorkflowV1Response,
     ListWorkflowResponseEntry,
     ListWorkflowSavedObjectsResponse,
     PreviewResponse,
     RegisterAirflowWorkflowResponse,
     RegisterWorkflowResponse,
     SavedObjectUpdate,
+    WorkflowDagResponse,
+    WorkflowDagResultResponse,
 )
 from aqueduct.utils.serialization import deserialize
 from pkg_resources import get_distribution, parse_version
 
 from ..resources.connect_config import DynamicK8sConfig, ResourceConfig
 from .response_helpers import (
     _construct_preview_response,
@@ -52,39 +61,46 @@
     """
     Internal client class used to send requests to the aqueduct cluster.
     """
 
     HTTP_PREFIX = "http://"
     HTTPS_PREFIX = "https://"
 
+    # V2
+    GET_WORKFLOW_TEMPLATE = "/api/v2/workflow/%s"
+    GET_DAGS_TEMPLATE = "/api/v2/workflow/%s/dags"
+    GET_DAG_RESULTS_TEMPLATE = "/api/v2/workflow/%s/results"
+    GET_NODES_TEMPLATE = "/api/v2/workflow/%s/dag/%s/nodes"
+
+    # V1
     GET_VERSION_ROUTE = "/api/version"
-    CONNECT_INTEGRATION_ROUTE = "/api/integration/connect"
-    DELETE_INTEGRATION_ROUTE_TEMPLATE = "/api/integration/%s/delete"
+    CONNECT_RESOURCE_ROUTE = "/api/resource/connect"
+    DELETE_RESOURCE_ROUTE_TEMPLATE = "/api/resource/%s/delete"
     PREVIEW_ROUTE = "/api/preview"
     REGISTER_WORKFLOW_ROUTE = "/api/workflow/register"
     REGISTER_AIRFLOW_WORKFLOW_ROUTE = "/api/workflow/register/airflow"
-    LIST_INTEGRATIONS_ROUTE = "/api/integrations"
-    LIST_INTEGRATION_OBJECTS_ROUTE_TEMPLATE = "/api/integration/%s/objects"
+    LIST_RESOURCES_ROUTE = "/api/resources"
+    LIST_RESOURCE_OBJECTS_ROUTE_TEMPLATE = "/api/resource/%s/objects"
     GET_WORKFLOW_ROUTE_TEMPLATE = "/api/workflow/%s"
     GET_WORKFLOW_DAG_RESULT_TEMPLATE = "/api/workflow/%s/result/%s"
     LIST_WORKFLOW_SAVED_OBJECTS_ROUTE = "/api/workflow/%s/objects"
     GET_ARTIFACT_RESULT_TEMPLATE = "/api/artifact/%s/%s/result"
 
     LIST_WORKFLOWS_ROUTE = "/api/workflows"
     REFRESH_WORKFLOW_ROUTE_TEMPLATE = "/api/workflow/%s/refresh"
     DELETE_WORKFLOW_ROUTE_TEMPLATE = "/api/workflow/%s/delete"
-    LIST_GITHUB_REPO_ROUTE = "/api/integrations/github/repos"
-    LIST_GITHUB_BRANCH_ROUTE = "/api/integrations/github/branches"
+    LIST_GITHUB_REPO_ROUTE = "/api/resources/github/repos"
+    LIST_GITHUB_BRANCH_ROUTE = "/api/resources/github/branches"
     NODE_POSITION_ROUTE = "/api/positioning"
     EXPORT_FUNCTION_ROUTE = "/api/function/%s/export"
 
-    GET_DYNAMIC_ENGINE_STATUS_ROUTE = "/api/integration/dynamic-engine/status"
-    EDIT_DYNAMIC_ENGINE_ROUTE_TEMPLATE = "/api/integration/dynamic-engine/%s/edit"
+    GET_DYNAMIC_ENGINE_STATUS_ROUTE = "/api/resource/dynamic-engine/status"
+    EDIT_DYNAMIC_ENGINE_ROUTE_TEMPLATE = "/api/resource/dynamic-engine/%s/edit"
 
-    GET_IMAGE_URL_ROUTE = "/api/integration/container-registry/url"
+    GET_IMAGE_URL_ROUTE = "/api/resource/container-registry/url"
 
     # Auth header
     API_KEY_HEADER = "api-key"
 
     configured = False
 
     def raise_errors(self, response: requests.Response) -> None:
@@ -220,26 +236,25 @@
         return GetVersionResponse(**resp.json()).version
 
     def url_prefix(self) -> str:
         self._check_config()
         return self.HTTPS_PREFIX if self.use_https else self.HTTP_PREFIX
 
     def list_resources(self) -> Dict[str, ResourceInfo]:
-        url = self.construct_full_url(self.LIST_INTEGRATIONS_ROUTE)
+        url = self.construct_full_url(self.LIST_RESOURCES_ROUTE)
         headers = self._generate_auth_headers()
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
         if len(resp.json()) == 0:
-            raise NoConnectedIntegrationsException(
-                "Unable to create flow. Must be connected to at least one integration!"
+            raise NoConnectedResourcesException(
+                "Unable to create flow. Must be connected to at least one resource!"
             )
 
         return {
-            integration_info["name"]: ResourceInfo(**integration_info)
-            for integration_info in resp.json()
+            resource_info["name"]: ResourceInfo(**resource_info) for resource_info in resp.json()
         }
 
     def list_github_repos(self) -> List[str]:
         url = self.construct_full_url(self.LIST_GITHUB_REPO_ROUTE)
         headers = self._generate_auth_headers()
 
         resp = requests.get(url, headers=headers)
@@ -249,118 +264,118 @@
         url = self.construct_full_url(self.LIST_GITHUB_BRANCH_ROUTE)
         headers = self._generate_auth_headers()
         headers["github-repo"] = repo_url
 
         resp = requests.get(url, headers=headers)
         return [x for x in resp.json()["branches"]]
 
-    def list_tables(self, integration_id: str) -> List[str]:
-        """Returns a list of the tables in the specified integration.
-        If the integration is not a relational database, it will throw an error.
+    def list_tables(self, resource_id: str) -> List[str]:
+        """Returns a list of the tables in the specified resource.
+        If the resource is not a relational database, it will throw an error.
         """
-        url = self.construct_full_url(self.LIST_INTEGRATION_OBJECTS_ROUTE_TEMPLATE % integration_id)
+        url = self.construct_full_url(self.LIST_RESOURCE_OBJECTS_ROUTE_TEMPLATE % resource_id)
         headers = self._generate_auth_headers()
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
 
         return [x for x in resp.json()["object_names"]]
 
-    def connect_integration(
+    def connect_resource(
         self, name: str, service: Union[str, ServiceType], config: ResourceConfig
     ) -> None:
-        integration_service = service
-        if isinstance(integration_service, ServiceType):
+        resource_service = service
+        if isinstance(resource_service, ServiceType):
             # The enum value needs to be used
-            integration_service = integration_service.value
+            resource_service = resource_service.value
 
         headers = self._generate_auth_headers()
         headers.update(
             {
-                "integration-name": name,
-                "integration-service": integration_service,
+                "resource-name": name,
+                "resource-service": resource_service,
                 # `by_alias` is necessary to get this to use `schema` as a key for SnowflakeConfig.
                 # `exclude_none` is necessary to exclude `role` when None as SnowflakeConfig.
-                "integration-config": config.json(exclude_none=True, by_alias=True),
+                "resource-config": config.json(exclude_none=True, by_alias=True),
             }
         )
         url = self.construct_full_url(
-            self.CONNECT_INTEGRATION_ROUTE,
+            self.CONNECT_RESOURCE_ROUTE,
         )
         resp = requests.post(url, url, headers=headers)
         self.raise_errors(resp)
 
     def get_dynamic_engine_status_by_dag(
         self,
         dag: DAG,
     ) -> Dict[str, DynamicEngineStatusResponse]:
-        """Makes a request against the /api/integration/dynamic-engine/status endpoint.
-           If an integration id does not correspond to a dynamic integration, the response won't
-           have an entry for that integration.
+        """Makes a request against the /api/resource/dynamic-engine/status endpoint.
+           If an resource id does not correspond to a dynamic resource, the response won't
+           have an entry for that resource.
 
         Args:
             dag:
-                The DAG object. We will extract the engine integration IDs and send them
+                The DAG object. We will extract the engine resource IDs and send them
                 to the backend to retrieve their status. Currently, we are only interested in
                 the status of dynamic engines.
 
         Returns:
             A DynamicEngineStatusResponse object, parsed from the backend endpoint's response.
         """
-        engine_integration_ids = set()
+        engine_resource_ids = set()
 
         dag_engine_config = dag.engine_config
         if dag_engine_config.type == RuntimeType.K8S:
             assert dag_engine_config.k8s_config is not None
-            engine_integration_ids.add(str(dag_engine_config.k8s_config.integration_id))
+            engine_resource_ids.add(str(dag_engine_config.k8s_config.resource_id))
         for op in dag.operators.values():
             if op.spec.engine_config and op.spec.engine_config.type == RuntimeType.K8S:
                 assert op.spec.engine_config.k8s_config is not None
-                engine_integration_ids.add(str(op.spec.engine_config.k8s_config.integration_id))
+                engine_resource_ids.add(str(op.spec.engine_config.k8s_config.resource_id))
 
-        return self.get_dynamic_engine_status(list(engine_integration_ids))
+        return self.get_dynamic_engine_status(list(engine_resource_ids))
 
     def get_dynamic_engine_status(
         self,
-        engine_integration_ids: List[str],
+        engine_resource_ids: List[str],
     ) -> Dict[str, DynamicEngineStatusResponse]:
-        """Makes a request against the /api/integration/dynamic-engine/status endpoint.
-           If an integration id does not correspond to a dynamic integration, the response won't
-           have an entry for that integration.
+        """Makes a request against the /api/resource/dynamic-engine/status endpoint.
+           If an resource id does not correspond to a dynamic resource, the response won't
+           have an entry for that resource.
 
         Args:
-            engine_integration_ids:
-                A list of engine integration IDs. Currently, we are only interested in
+            engine_resource_ids:
+                A list of engine resource IDs. Currently, we are only interested in
                 the status of dynamic engines.
 
         Returns:
             A DynamicEngineStatusResponse object, parsed from the backend endpoint's response.
         """
         headers = self._generate_auth_headers()
-        headers["integration-ids"] = json.dumps(engine_integration_ids)
+        headers["resource-ids"] = json.dumps(engine_resource_ids)
 
         url = self.construct_full_url(self.GET_DYNAMIC_ENGINE_STATUS_ROUTE)
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
 
         return {
             dynamic_engine_status["name"]: DynamicEngineStatusResponse(**dynamic_engine_status)
             for dynamic_engine_status in resp.json()
         }
 
     def edit_dynamic_engine(
         self,
         action: K8sClusterActionType,
-        integration_id: str,
+        resource_id: str,
         config_delta: Optional[DynamicK8sConfig] = None,
     ) -> None:
-        """Makes a request against the /api/integration/dynamic-engine/{integrationId}/edit endpoint.
+        """Makes a request against the /api/resource/dynamic-engine/{resourceId}/edit endpoint.
 
         Args:
-            integration_id:
-                The engine integration ID.
+            resource_id:
+                The engine resource ID.
         """
         if action not in [
             K8sClusterActionType.CREATE,
             K8sClusterActionType.UPDATE,
             K8sClusterActionType.DELETE,
             K8sClusterActionType.FORCE_DELETE,
         ]:
@@ -372,29 +387,29 @@
             config_delta = DynamicK8sConfig()
 
         assert isinstance(config_delta, DynamicK8sConfig)
 
         headers = self._generate_auth_headers()
         headers["action"] = action.value
 
-        url = self.construct_full_url(self.EDIT_DYNAMIC_ENGINE_ROUTE_TEMPLATE % integration_id)
+        url = self.construct_full_url(self.EDIT_DYNAMIC_ENGINE_ROUTE_TEMPLATE % resource_id)
 
         body = {
             "config_delta": config_delta.json(exclude_none=True),
         }
 
         resp = requests.post(url, headers=headers, data=body)
 
         self.raise_errors(resp)
 
-    def delete_integration(
+    def delete_resource(
         self,
-        integration_id: uuid.UUID,
+        resource_id: uuid.UUID,
     ) -> None:
-        url = self.construct_full_url(self.DELETE_INTEGRATION_ROUTE_TEMPLATE % integration_id)
+        url = self.construct_full_url(self.DELETE_RESOURCE_ROUTE_TEMPLATE % resource_id)
         headers = self._generate_auth_headers()
         resp = requests.post(url, headers=headers)
         self.raise_errors(resp)
 
     def preview(
         self,
         dag: DAG,
@@ -406,16 +421,18 @@
                 The DAG object to be serialized into the request header. Preview will
                 execute this entire DAG object.
 
         Returns:
             A PreviewResponse object, parsed from the preview endpoint's response.
         """
         headers = self._generate_auth_headers()
+
+        # TODO(ENG-2994): `by_alias` is required until this naming inconsistency is resolved.
         body = {
-            "dag": dag.json(exclude_none=True),
+            "dag": dag.json(exclude_none=True, by_alias=True),
         }
 
         if len(body["dag"]) > MAX_REQUEST_BODY_SIZE and any(
             artifact_metadata.from_local_data for artifact_metadata in list(dag.artifacts.values())
         ):
             raise InvalidUserActionException(
                 "Local Data after serialization is too large. Aqueduct uses json serialization. The maximum size of workflow with local data is %s in bytes, the current size is %s in bytes."
@@ -463,16 +480,17 @@
         self,
         dag: DAG,
         run_now: bool,
     ) -> Tuple[Dict[str, str], Dict[str, str], Dict[str, IO[Any]]]:
         headers = self._generate_auth_headers()
         # This header value will be string "True" or "False"
         headers.update({"run-now": str(run_now)})
+        # TODO(ENG-2994): `by_alias` is required until this naming inconsistency is resolved.
         body = {
-            "dag": dag.json(exclude_none=True),
+            "dag": dag.json(exclude_none=True, by_alias=True),
         }
 
         if len(body["dag"]) > MAX_REQUEST_BODY_SIZE and any(
             artifact_metadata.from_local_data for artifact_metadata in list(dag.artifacts.values())
         ):
             raise InvalidUserActionException(
                 "Local Data after serialization is too large. Aqueduct uses json serialization. The maximum size of workflow with local data is %s in bytes, the current size is %s in bytes."
@@ -513,29 +531,103 @@
         saved_objects_to_delete: DefaultDict[Union[str, BaseResource], List[SavedObjectUpdate]],
         force: bool,
     ) -> DeleteWorkflowResponse:
         headers = self._generate_auth_headers()
         url = self.construct_full_url(self.DELETE_WORKFLOW_ROUTE_TEMPLATE % flow_id)
         body = {
             "external_delete": {
-                str(integration): [obj.spec.json() for obj in saved_objects_to_delete[integration]]
-                for integration in saved_objects_to_delete
+                # TODO(ENG-2994): `by_alias` is required until this naming inconsistency is resolved.
+                str(resource): [
+                    obj.spec.json(by_alias=True) for obj in saved_objects_to_delete[resource]
+                ]
+                for resource in saved_objects_to_delete
             },
             "force": force,
         }
         response = requests.post(url, headers=headers, json=body)
         self.raise_errors(response)
         return DeleteWorkflowResponse(**response.json())
 
-    def get_workflow(self, flow_id: str) -> GetWorkflowResponse:
+    def get_workflow(self, flow_id: str) -> GetWorkflowV1Response:
         headers = self._generate_auth_headers()
-        url = self.construct_full_url(self.GET_WORKFLOW_ROUTE_TEMPLATE % flow_id)
-        resp = requests.get(url, headers=headers)
-        self.raise_errors(resp)
-        return GetWorkflowResponse(**resp.json())
+
+        url = self.construct_full_url(self.GET_WORKFLOW_TEMPLATE % flow_id)
+        flow_response = requests.get(url, headers=headers)
+        self.raise_errors(flow_response)
+        resp_flow = GetWorkflowResponse(**flow_response.json())
+        metadata = Metadata(
+            name=resp_flow.name,
+            description=resp_flow.description,
+            schedule=resp_flow.schedule,
+            retention_policy=resp_flow.retention_policy,
+        )
+
+        url = self.construct_full_url(self.GET_DAGS_TEMPLATE % flow_id)
+        dags_response = requests.get(url, headers=headers)
+        self.raise_errors(dags_response)
+        resp_dags = {dag["id"]: GetDagResponse(**dag) for dag in dags_response.json()}
+        # Metadata from WorkflowResponse so it is the same for all DAG.
+        dags = {}
+        for dag in resp_dags.values():
+            url = self.construct_full_url(self.GET_NODES_TEMPLATE % (flow_id, dag.id))
+            nodes_resp = requests.get(url, headers=headers)
+            self.raise_errors(nodes_resp)
+            resp_nodes = nodes_resp.json()
+
+            ops = {}
+            for operator in resp_nodes["operators"]:
+                op = GetNodeOperatorResponse(**operator)
+                ops[str(op.id)] = Operator(
+                    id=op.id,
+                    name=op.name,
+                    description=op.description,
+                    spec=op.spec,
+                    inputs=op.inputs,
+                    outputs=op.outputs,
+                )
+
+            artfs = {}
+            for artifact in resp_nodes["artifacts"]:
+                artf = GetNodeArtifactResponse(**artifact)
+                artfs[str(artf.id)] = ArtifactMetadata(
+                    id=artf.id,
+                    name=artf.name,
+                    type=artf.type,
+                )
+
+            dags[dag.id] = WorkflowDagResponse(
+                id=dag.id,
+                workflow_id=dag.workflow_id,
+                metadata=metadata,
+                operators=ops,
+                artifacts=artfs,
+            )
+
+        url = self.construct_full_url(self.GET_DAG_RESULTS_TEMPLATE % flow_id)
+        results_resp = requests.get(url, headers=headers)
+        self.raise_errors(results_resp)
+        dag_results = [GetDagResultResponse(**dag_result) for dag_result in results_resp.json()]
+        workflow_dag_results = [
+            WorkflowDagResultResponse(
+                id=dag_result.id,
+                created_at=int(
+                    datetime.datetime.strptime(
+                        resp_dags[str(dag_result.dag_id)].created_at[:-4],
+                        "%Y-%m-%dT%H:%M:%S.%f"
+                        if resp_dags[str(dag_result.dag_id)].created_at[-1] == "Z"
+                        else "%Y-%m-%dT%H:%M:%S.%f%z",
+                    ).timestamp()
+                ),
+                status=dag_result.exec_state.status,
+                exec_state=dag_result.exec_state,
+                workflow_dag_id=dag_result.dag_id,
+            )
+            for dag_result in dag_results
+        ]
+        return GetWorkflowV1Response(workflow_dags=dags, workflow_dag_results=workflow_dag_results)
 
     def get_workflow_dag_result(self, flow_id: str, result_id: str) -> GetWorkflowDagResultResponse:
         headers = self._generate_auth_headers()
         url = self.construct_full_url(self.GET_WORKFLOW_DAG_RESULT_TEMPLATE % (flow_id, result_id))
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
         return GetWorkflowDagResultResponse(**resp.json())
@@ -580,33 +672,33 @@
         if execution_status != ExecutionStatus.SUCCEEDED:
             logger().warning("Artifact result unavailable due to unsuccessful execution.")
 
         return (return_value, execution_status)
 
     def get_image_url(
         self,
-        integration_id: str,
+        resource_id: str,
         service: ServiceType,
         image_name: str,
     ) -> GetImageURLResponse:
-        """Makes a request against the /api/integration/container-registry/url endpoint.
+        """Makes a request against the /api/resource/container-registry/url endpoint.
 
         Args:
-            integration_id:
-                Container registry integration ID.
+            resource_id:
+                Container registry resource ID.
             service:
                 Container registry service type.
             image_name:
                 Image name to get the URL for.
 
         Returns:
             GetImageURLResponse that contains the URL to the image.
         """
         headers = self._generate_auth_headers()
-        headers["integration-id"] = integration_id
+        headers["resource-id"] = resource_id
         headers["service"] = service.value
         headers["image-name"] = image_name
 
         url = self.construct_full_url(self.GET_IMAGE_URL_ROUTE)
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/backend/response_helpers.py` & `aqueduct-sdk-0.3.5/aqueduct/backend/response_helpers.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/client.py` & `aqueduct-sdk-0.3.5/aqueduct/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,39 +17,39 @@
     ArtifactType,
     ExecutionStatus,
     RelationalDBServices,
     RuntimeType,
     ServiceType,
 )
 from aqueduct.error import (
-    InvalidIntegrationException,
+    InvalidResourceException,
     InvalidUserActionException,
     InvalidUserArgumentException,
 )
 from aqueduct.flow import Flow
 from aqueduct.github import Github
 from aqueduct.logger import logger
 from aqueduct.models.dag import Metadata, RetentionPolicy
-from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import ParamSpec, S3LoadParams
+from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.models.response_models import SavedObjectUpdate
 from aqueduct.resources.airflow import AirflowResource
 from aqueduct.resources.aws import AWSResource
 from aqueduct.resources.aws_lambda import LambdaResource
 from aqueduct.resources.connect_config import (
     BaseConnectionConfig,
     ResourceConfig,
-    convert_dict_to_integration_connect_config,
-    prepare_integration_config,
+    convert_dict_to_resource_connect_config,
+    prepare_resource_config,
 )
 from aqueduct.resources.databricks import DatabricksResource
 from aqueduct.resources.dynamic_k8s import DynamicK8sResource
 from aqueduct.resources.ecr import ECRResource
+from aqueduct.resources.gar import GARResource
 from aqueduct.resources.google_sheets import GoogleSheetsResource
-from aqueduct.resources.k8s import K8sResource
 from aqueduct.resources.mongodb import MongoDBResource
 from aqueduct.resources.parameters import USER_TAG_PATTERN
 from aqueduct.resources.s3 import S3Resource
 from aqueduct.resources.salesforce import SalesforceResource
 from aqueduct.resources.spark import SparkResource
 from aqueduct.resources.sql import RelationalDBResource
 from aqueduct.utils.dag_deltas import (
@@ -78,30 +78,30 @@
         config_dict:
             A dict from the configuration key to its new value.
 
     Available configuration keys:
         "lazy":
             A boolean indicating whether any new functions will be constructed lazily (True) or eagerly (False).
         "engine":
-            The name of the default compute integration to run all functions against.
+            The name of the default compute resource to run all functions against.
             This can still be overriden by the `engine` argument in `client.publish_flow()` or
             on the @op spec. To set this to run against the Aqueduct engine, use "aqueduct" (case-insensitive).
     """
 
     if globals.GLOBAL_LAZY_KEY in config_dict:
         lazy_val = config_dict[globals.GLOBAL_LAZY_KEY]
         if not isinstance(lazy_val, bool):
             raise InvalidUserArgumentException("Must supply a boolean for the lazy key.")
         globals.__GLOBAL_CONFIG__.lazy = lazy_val
 
     if globals.GLOBAL_ENGINE_KEY in config_dict:
         engine_name = config_dict[globals.GLOBAL_ENGINE_KEY]
         if not isinstance(engine_name, str):
             raise InvalidUserArgumentException(
-                "Engine should be the string name of your compute integration."
+                "Engine should be the string name of your compute resource."
             )
         globals.__GLOBAL_CONFIG__.engine = engine_name
 
 
 def get_apikey() -> str:
     """
     Get the API key if the server is running locally.
@@ -155,15 +155,15 @@
         # We must call basicConfig() here so messages show up in Jupyter notebooks.
         logging.basicConfig(format="%(levelname)s:%(message)s", level=logging_level)
 
         if api_key == "":
             api_key = get_apikey()
 
         globals.__GLOBAL_API_CLIENT__.configure(api_key, aqueduct_address)
-        self._connected_integrations: Dict[
+        self._connected_resources: Dict[
             str, ResourceInfo
         ] = globals.__GLOBAL_API_CLIENT__.list_resources()
         self._dag = globals.__GLOBAL_DAG__
 
         # Will show graph if in an ipynb or Python console, but not if running a Python script.
         self._in_notebook_or_console_context = (not hasattr(main, "__file__")) and (
             not "PYTEST_CURRENT_TEST" in os.environ
@@ -178,15 +178,15 @@
         Args:
             repo:
                 The full github repo URL, e.g. "my_organization/my_repo"
             branch:
                 Optional branch name. The default main branch will be used if not specified.
 
         Returns:
-            A github integration object linked to the repo and branch.
+            A github resource object linked to the repo and branch.
 
         """
         return Github(repo_url=repo, branch=branch)
 
     def create_param(
         self,
         name: str,
@@ -239,61 +239,61 @@
         self,
         name: str,
         service: Union[str, ServiceType],
         config: Union[Dict[str, str], ResourceConfig],
     ) -> None:
         """Deprecated. Use `client.connect_resource()` instead."""
         logger().warning(
-            "client.connect_integration() will be deprecated soon. Use `client.connect_resource() instead."
+            "client.connect_resource() will be deprecated soon. Use `client.connect_resource() instead."
         )
         return self.connect_resource(name, service, config)
 
     def connect_resource(
         self,
         name: str,
         service: Union[str, ServiceType],
         config: Union[Dict[str, str], ResourceConfig],
     ) -> None:
-        """Connects the Aqueduct server to an integration.
+        """Connects the Aqueduct server to an resource.
 
         Args:
             name:
-                The name to assign this integration. Will error if an integration with that name
+                The name to assign this resource. Will error if an resource with that name
                 already exists.
             service:
-                The type of integration to connect to.
+                The type of resource to connect to.
             config:
-                Either a dictionary or an IntegrationConnectConfig object that contains the
+                Either a dictionary or an ResourceConnectConfig object that contains the
                 configuration credentials needed to connect.
         """
         if service not in ServiceType:
             raise InvalidUserArgumentException(
                 "Service argument must match exactly one of the enum values in ServiceType (case-sensitive)."
             )
 
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
-        if name in self._connected_integrations.keys():
+        self._connected_resources = globals.__GLOBAL_API_CLIENT__.list_resources()
+        if name in self._connected_resources.keys():
             raise InvalidUserActionException(
-                "Cannot connect a new integration with name `%s`. An integration with this name already exists."
+                "Cannot connect a new resource with name `%s`. An resource with this name already exists."
                 % name
             )
 
         if not isinstance(config, dict) and not isinstance(config, BaseConnectionConfig):
             raise InvalidUserArgumentException(
-                "`config` argument must be either a dict or IntegrationConnectConfig."
+                "`config` argument must be either a dict or ResourceConnectConfig."
             )
 
         if isinstance(config, dict):
-            config = convert_dict_to_integration_connect_config(service, config)
+            config = convert_dict_to_resource_connect_config(service, config)
         assert isinstance(config, BaseConnectionConfig)
 
-        config = prepare_integration_config(service, config)
+        config = prepare_resource_config(service, config)
 
-        logger().info("Connecting to new %s integration `%s`..." % (service, name))
-        globals.__GLOBAL_API_CLIENT__.connect_integration(name, service, config)
+        logger().info("Connecting to new %s resource `%s`..." % (service, name))
+        globals.__GLOBAL_API_CLIENT__.connect_resource(name, service, config)
 
     def delete_integration(
         self,
         name: str,
     ) -> None:
         """Deprecated. Use `client.delete_resource()` instead."""
         logger().warning(
@@ -301,185 +301,188 @@
         )
         return self.delete_resource(name)
 
     def delete_resource(
         self,
         name: str,
     ) -> None:
-        """Deletes the integration from Aqueduct.
+        """Deletes the resource from Aqueduct.
 
         Args:
             name:
-                The name of the integration to delete.
+                The name of the resource to delete.
         """
-        existing_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
+        existing_resources = globals.__GLOBAL_API_CLIENT__.list_resources()
 
         # If the user uses the deprecated demo name, and there isn't a resource for this, that means they actually
         # want to use the new demo name.
         if (
             name == DEPRECATED_AQUEDUCT_DEMO_DB_NAME
-            and DEPRECATED_AQUEDUCT_DEMO_DB_NAME not in existing_integrations.keys()
+            and DEPRECATED_AQUEDUCT_DEMO_DB_NAME not in existing_resources.keys()
         ) or name == AQUEDUCT_DEMO_DB_NAME:
             raise InvalidUserActionException("Cannot delete the Aqueduct demo database: %s" % name)
-        if name not in existing_integrations.keys():
-            raise InvalidIntegrationException("Not connected to integration %s!" % name)
+        if name not in existing_resources.keys():
+            raise InvalidResourceException("Not connected to resource %s!" % name)
 
-        # Update the connected integrations cached on this object.
-        globals.__GLOBAL_API_CLIENT__.delete_integration(existing_integrations[name].id)
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
+        # Update the connected resources cached on this object.
+        globals.__GLOBAL_API_CLIENT__.delete_resource(existing_resources[name].id)
+        self._connected_resources = globals.__GLOBAL_API_CLIENT__.list_resources()
 
     def list_integrations(self) -> Dict[str, ResourceInfo]:
         """Deprecated. Use `client.list_resources()` instead."""
         logger().warning(
-            "client.list_integrations() will be deprecated soon. Use `client.list_resources() instead."
+            "client.list_resources() will be deprecated soon. Use `client.list_resources() instead."
         )
         return self.list_resources()
 
     def list_resources(self) -> Dict[str, ResourceInfo]:
-        """Retrieves a dictionary of integrations the client can use.
+        """Retrieves a dictionary of resources the client can use.
 
         Returns:
-            A dictionary mapping from integration name to additional info.
+            A dictionary mapping from resource name to additional info.
         """
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
-        return self._connected_integrations
+        self._connected_resources = globals.__GLOBAL_API_CLIENT__.list_resources()
+        return self._connected_resources
 
     def integration(
         self,
         name: str,
     ) -> Union[
         SalesforceResource,
         S3Resource,
         GoogleSheetsResource,
         RelationalDBResource,
         AirflowResource,
-        K8sResource,
         LambdaResource,
         MongoDBResource,
         DatabricksResource,
         SparkResource,
         AWSResource,
         ECRResource,
+        DynamicK8sResource,
+        GARResource,
     ]:
         """Deprecated. Use `client.resource()` instead."""
         logger().warning(
-            "client.integration() will be deprecated soon. Use `client.resource() instead."
+            "client.resource() will be deprecated soon. Use `client.resource() instead."
         )
         return self.resource(name)
 
     def resource(
         self, name: str
     ) -> Union[
         SalesforceResource,
         S3Resource,
         GoogleSheetsResource,
         RelationalDBResource,
         AirflowResource,
-        K8sResource,
         LambdaResource,
         MongoDBResource,
         DatabricksResource,
         SparkResource,
         AWSResource,
         ECRResource,
+        DynamicK8sResource,
+        GARResource,
     ]:
-        """Retrieves a connected integration object.
+        """Retrieves a connected resource object.
 
         Args:
             name:
-                The name of the integration
+                The name of the resource
 
         Returns:
-            The integration object with the given name.
+            The resource object with the given name.
 
         Raises:
-            InvalidIntegrationException:
+            InvalidResourceException:
                 An error occurred because the cluster is not connected to the
-                provided integration or the provided integration is of an
+                provided resource or the provided resource is of an
                 incompatible type.
         """
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
-        connected_names = self._connected_integrations.keys()
+        self._connected_resources = globals.__GLOBAL_API_CLIENT__.list_resources()
+        connected_names = self._connected_resources.keys()
 
         if name == DEPRECATED_AQUEDUCT_DEMO_DB_NAME:
             # If the user uses the deprecated demo name, and there isn't a resource for this, that means they actually
             # want to use the new demo name. We implicitly convert this for them, with a warning.
             if DEPRECATED_AQUEDUCT_DEMO_DB_NAME not in connected_names:
                 logger().warning(
                     "`%s` is the deprecated name for the aqueduct demo db. Please use `%s` instead."
                     % (DEPRECATED_AQUEDUCT_DEMO_DB_NAME, AQUEDUCT_DEMO_DB_NAME)
                 )
                 name = AQUEDUCT_DEMO_DB_NAME
 
         if name not in connected_names:
-            raise InvalidIntegrationException("Not connected to integration %s!" % name)
+            raise InvalidResourceException("Not connected to resource %s!" % name)
 
-        integration_info = self._connected_integrations[name]
-        if integration_info.service in RelationalDBServices:
+        resource_info = self._connected_resources[name]
+        if resource_info.service in RelationalDBServices:
             return RelationalDBResource(
                 dag=self._dag,
-                metadata=integration_info,
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.SALESFORCE:
+        elif resource_info.service == ServiceType.SALESFORCE:
             return SalesforceResource(
                 dag=self._dag,
-                metadata=integration_info,
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.GOOGLE_SHEETS:
+        elif resource_info.service == ServiceType.GOOGLE_SHEETS:
             return GoogleSheetsResource(
                 dag=self._dag,
-                metadata=integration_info,
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.S3:
+        elif resource_info.service == ServiceType.S3:
             return S3Resource(
                 dag=self._dag,
-                metadata=integration_info,
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.AIRFLOW:
+        elif resource_info.service == ServiceType.AIRFLOW:
             return AirflowResource(
-                metadata=integration_info,
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.K8S:
-            return K8sResource(
-                metadata=integration_info,
+        elif resource_info.service == ServiceType.K8S:
+            return DynamicK8sResource(
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.LAMBDA:
+        elif resource_info.service == ServiceType.LAMBDA:
             return LambdaResource(
-                metadata=integration_info,
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.MONGO_DB:
+        elif resource_info.service == ServiceType.MONGO_DB:
             return MongoDBResource(
                 dag=self._dag,
-                metadata=integration_info,
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.DATABRICKS:
+        elif resource_info.service == ServiceType.DATABRICKS:
             return DatabricksResource(
-                metadata=integration_info,
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.SPARK:
+        elif resource_info.service == ServiceType.SPARK:
             return SparkResource(
-                metadata=integration_info,
+                metadata=resource_info,
             )
-        elif integration_info.service == ServiceType.AWS:
-            dynamic_k8s_integration_name = "%s:aqueduct_ondemand_k8s" % name
-            dynamic_k8s_integration_info = self._connected_integrations[
-                dynamic_k8s_integration_name
-            ]
+        elif resource_info.service == ServiceType.AWS:
+            dynamic_k8s_resource_name = "%s:aqueduct_ondemand_k8s" % name
+            dynamic_k8s_resource_info = self._connected_resources[dynamic_k8s_resource_name]
             return AWSResource(
-                metadata=integration_info,
-                k8s_integration_metadata=dynamic_k8s_integration_info,
+                metadata=resource_info,
+                k8s_resource_metadata=dynamic_k8s_resource_info,
             )
-        elif integration_info.service == ServiceType.ECR:
+        elif resource_info.service == ServiceType.ECR:
             return ECRResource(
-                metadata=integration_info,
+                metadata=resource_info,
+            )
+        elif resource_info.service == ServiceType.GAR:
+            return GARResource(
+                metadata=resource_info,
             )
         else:
-            raise InvalidIntegrationException(
-                "This method does not support loading integration of type %s"
-                % integration_info.service
+            raise InvalidResourceException(
+                "This method does not support loading resource of type %s" % resource_info.service
             )
 
     def list_flows(self) -> List[Dict[str, str]]:
         """Lists the flows that are accessible by this client.
 
         Returns:
             A list of flows, each represented as a dictionary providing essential
@@ -557,30 +560,30 @@
         to this new state.
 
         The default execution engine of the flow is Aqueduct. In order to specify which
         execution engine the flow will be running on, use "config" parameter. Eg:
         >>> flow = client.publish_flow(
         >>>     name="k8s_example",
         >>>     artifacts=[output],
-        >>>     engine="k8s_integration",
+        >>>     engine="k8s_resource",
         >>> )
 
         Args:
             name:
                 The name of the newly created flow.
             description:
                 A description for the new flow.
             schedule:
                 A cron expression specifying the cadence that this flow
                 will run on. If empty, the flow will only execute manually.
                 For example, to run at the top of every hour:
 
                 >> schedule = aqueduct.hourly(minute: 0)
             engine:
-                The name of the compute integration (eg. "my_lambda_integration") this the flow will
+                The name of the compute resource (eg. "my_lambda_resource") this the flow will
                 be computed on.
             artifacts:
                 All the artifacts that you care about computing. These artifacts are guaranteed
                 to be computed. Additional artifacts may also be computed if they are upstream
                 dependencies.
             metrics:
                 All the metrics that you would like to compute. If not supplied, we include by default
@@ -719,18 +722,18 @@
             name=name,
             description=description,
             schedule=flow_schedule,
             retention_policy=retention_policy,
         )
         dag.set_engine_config(
             global_engine_config=generate_engine_config(
-                self._connected_integrations,
+                self._connected_resources,
                 globals.__GLOBAL_CONFIG__.engine,
             ),
-            publish_flow_engine_config=generate_engine_config(self._connected_integrations, engine),
+            publish_flow_engine_config=generate_engine_config(self._connected_resources, engine),
         )
 
         dag.validate_and_resolve_artifact_names()
 
         if dag.engine_config.type == RuntimeType.AIRFLOW:
             if run_now is not None:
                 raise InvalidUserArgumentException(
@@ -875,15 +878,15 @@
                 If both are specified, they must correspond to the same flow.
             flow_name:
                 Used to identify the flow to fetch from the system.
 
             flow_identifier takes precedence over flow_id or flow_name arguments
 
             saved_objects_to_delete:
-                The tables or storage paths to delete grouped by integration name.
+                The tables or storage paths to delete grouped by resource name.
             force:
                 Force the deletion even though some workflow-written objects in the writes_to_delete argument had UpdateMode=append
 
         Raises:
             InvalidRequestError:
                 An error occurred when attempting to fetch the workflow to
                 delete. The provided `flow_id` may be malformed.
@@ -911,56 +914,56 @@
         s3_parameterized_filepaths: List[Tuple[str, str]] = []
         for saved_obj_list in saved_objects_to_delete.values():
             for saved_obj_to_delete in saved_obj_list:
                 if isinstance(saved_obj_to_delete.spec.parameters, S3LoadParams):
                     filepath = saved_obj_to_delete.spec.parameters.filepath
                     if len(re.findall(USER_TAG_PATTERN, filepath)) > 0:
                         s3_parameterized_filepaths.append(
-                            (saved_obj_to_delete.integration_name, filepath)
+                            (saved_obj_to_delete.resource_name, filepath)
                         )
 
         if len(s3_parameterized_filepaths) > 0:
             raise InvalidUserArgumentException(
                 "Deleting objects at parameterized filepaths in S3 is currently unsupported. The following resource-filepath "
                 "combinations in `saved_objects_to_delete` are parameterized: \n"
                 + ", ".join(
                     [
-                        f"{integration_name}: {filepath}"
-                        for integration_name, filepath in s3_parameterized_filepaths
+                        f"{resource_name}: {filepath}"
+                        for resource_name, filepath in s3_parameterized_filepaths
                     ]
                 )
             )
 
         flows = [(flow.id, flow.name) for flow in globals.__GLOBAL_API_CLIENT__.list_workflows()]
         flow_id_key = find_flow_with_user_supplied_id_and_name(flows, flow_identifier)
 
         # TODO(ENG-410): This method gives no indication as to whether the flow
         #  was successfully deleted.
         resp = globals.__GLOBAL_API_CLIENT__.delete_workflow(
             flow_id_key, saved_objects_to_delete, force
         )
 
         failures = []
-        for integration in resp.saved_object_deletion_results:
-            for obj in resp.saved_object_deletion_results[integration]:
+        for resource in resp.saved_object_deletion_results:
+            for obj in resp.saved_object_deletion_results[resource]:
                 if obj.exec_state.status == ExecutionStatus.FAILED:
                     trace = ""
                     if obj.exec_state.error:
                         context = obj.exec_state.error.context.strip().replace("\n", "\n>\t")
                         trace = f">\t{context}\n{obj.exec_state.error.tip}"
-                    failure_string = f"[{integration}] {obj.name}\n{trace}"
+                    failure_string = f"[{resource}] {obj.name}\n{trace}"
                     failures.append(failure_string)
         if len(failures) > 0:
             failures_string = "\n".join(failures)
             raise Exception(
                 f"Failed to delete {len(failures)} saved objects.\nFailures\n{failures_string}"
             )
 
     def describe(self) -> None:
         """Prints out info about this client in a human-readable format."""
         print("============================= Aqueduct Client =============================")
         print("Connected endpoint: %s" % globals.__GLOBAL_API_CLIENT__.aqueduct_address)
         print("Log Level: %s" % logging.getLevelName(logging.root.level))
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
-        print("Current Integrations:")
-        for integrations in self._connected_integrations:
-            print("\t -" + integrations)
+        self._connected_resources = globals.__GLOBAL_API_CLIENT__.list_resources()
+        print("Current Resources:")
+        for resources in self._connected_resources:
+            print("\t -" + resources)
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/constants/enums.py` & `aqueduct-sdk-0.3.5/aqueduct/constants/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,20 @@
     DATABRICKS = "Databricks"
     EMAIL = "Email"
     SLACK = "Slack"
     SPARK = "Spark"
     AWS = "AWS"
     ECR = "ECR"
     FILESYSTEM = "Filesystem"
+    GAR = "GAR"
+
+
+class CloudProviderType(str, Enum, metaclass=MetaEnum):
+    AWS = "AWS"
+    GCP = "GCP"
 
 
 class RelationalDBServices(str, Enum, metaclass=MetaEnum):
     """Must match the corresponding entries in `ServiceType` exactly."""
 
     POSTGRES = "Postgres"
     SNOWFLAKE = "Snowflake"
@@ -103,14 +109,22 @@
     RUNNING = "running"
     FAILED = "failed"
     PENDING = "pending"
     REGISTERED = "registered"
     CANCELED = "canceled"
 
 
+class NotificationLogLevel(str, Enum, metaclass=MetaEnum):
+    SUCCESS = "success"
+    WARNING = "warning"
+    ERROR = "error"
+    INFO = "info"
+    NEUTRAL = "neutral"
+
+
 class FailureType(Enum, metaclass=MetaEnum):
     SYSTEM = 1
     USER_FATAL = 2
     # For failures that don't stop execution.
     # Eg. check operator with WARNING severity fails.
     USER_NON_FATAL = 3
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/decorator.py` & `aqueduct-sdk-0.3.5/aqueduct/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,16 +533,16 @@
         url = image.get("url")
 
         if registry_name is None:
             raise InvalidUserArgumentException(
                 "`registry_name` must be specified when `image` is set."
             )
 
-        connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
-        if registry_name not in connected_integrations.keys():
+        connected_resources = globals.__GLOBAL_API_CLIENT__.list_resources()
+        if registry_name not in connected_resources.keys():
             raise InvalidUserArgumentException(
                 "Registry name `%s` is not one of the connected resources." % registry_name,
             )
 
         if url is None:
             raise InvalidUserArgumentException("`url` must be specified when `image` is set.")
 
@@ -552,16 +552,16 @@
             else:
                 raise InvalidUserArgumentException(
                     "Image URL must be in the form of `endpoint/repo:tag`. "
                     "Such as 123456789012.dkr.ecr.us-east-1.amazonaws.com/my-image:latest."
                 )
 
         spec.image = ImageConfig(
-            registry_id=str(connected_integrations[registry_name].id),
-            service=connected_integrations[registry_name].service,
+            registry_id=str(connected_resources[registry_name].id),
+            service=connected_resources[registry_name].service,
             url=url,
         )
 
 
 def op(
     name: Optional[Union[str, UserFunction]] = None,
     description: Optional[str] = None,
@@ -583,15 +583,15 @@
 
     Args:
         name:
             Operator name. Defaults to the function name if not provided (or is of a non-string type).
         description:
             A description for the operator.
         engine:
-            The name of the compute integration this operator will run on. Defaults to the Aqueduct engine.
+            The name of the compute resource this operator will run on. Defaults to the Aqueduct engine.
         file_dependencies:
             A list of relative paths to files that the function needs to access.
             Python classes/methods already imported within the function's file
             need not be included.
         requirements:
             Defines the python package requirements that this operator will run with.
             Can be either a path to the requirements.txt file or a list of pip requirements specifiers.
@@ -629,15 +629,15 @@
                 For example, the following value is valid: "nvidia.com/gpu".
             "cuda_version" (str):
                 Version of CUDA to use with GPU (only applicable for Kubernetes engine). The currently supported
                 values are "11.4.1" and "11.8.0".
         image:
             A dictionary containing the custom image configurations that this operator will run with.
             The dictionary needs to contain the following keys:
-            "registry_name" (str): The name of the registry integration to use.
+            "registry_name" (str): The name of the registry resource to use.
             "url" (str): The full URL of the image to use. Example: "123456789012.dkr.ecr.us-east-1.amazonaws.com/my-image:latest"
             It is recommended to get the dictionary via `client.resource("my_registry_name").image("my-image:latest")`
 
     Examples:
         The op name is inferred from the function name. The description is pulled from the function
         docstring or can be explicitly set in the decorator.
 
@@ -798,15 +798,15 @@
             (eg. ["transformers==4.21.0", "numpy==1.22.4"]. If not supplied, we'll first
             look for a `requirements.txt` file in the same directory as the decorated function
             and install those. Otherwise, the method raises RequirementsMissingError exception.
         output:
             An optional custom name for the output metric artifact. Otherwise, the default naming scheme
             will be used.
         engine:
-            The name of the compute integration this operator will run on.
+            The name of the compute resource this operator will run on.
         resources:
             A dictionary containing the custom resource configurations that this operator will run with.
             These configurations are guaranteed to be followed, we will not silently ignore any of them.
             If a resource configuration is unsupported by a particular execution engine, we will fail at
             execution time. The supported keys are:
 
             "num_cpus" (int):
@@ -827,15 +827,15 @@
                 For example, the following value is valid: "nvidia.com/gpu".
             "cuda_version" (str):
                 Version of CUDA to use with GPU (only applicable for Kubernetes engine). The currently supported
                 values are "11.4.1" and "11.8.0".
         image:
             A dictionary containing the custom image configurations that this operator will run with.
             The dictionary needs to contain the following keys:
-            "registry_name" (str): The name of the registry integration to use.
+            "registry_name" (str): The name of the registry resource to use.
             "url" (str): The full URL of the image to use. Example: "123456789012.dkr.ecr.us-east-1.amazonaws.com/my-image:latest"
             It is recommended to get the dictionary via `client.resource("my_registry_name").image("my-image:latest")`
 
     Examples:
         The metric name is inferred from the function name. The description is pulled from the function
         docstring or can be explicitly set in the decorator.
 
@@ -1001,15 +1001,15 @@
             (eg. ["transformers==4.21.0", "numpy==1.22.4"]. If not supplied, we'll first
             look for a `requirements.txt` file in the same directory as the decorated function
             and install those. Otherwise, the method raises RequirementsMissingError exception.
         output:
             An optional custom name for the output metric artifact. Otherwise, the default naming scheme
             will be used.
         engine:
-            The name of the compute integration this operator will run on.
+            The name of the compute resource this operator will run on.
         resources:
             A dictionary containing the custom resource configurations that this operator will run with.
             These configurations are guaranteed to be followed, we will not silently ignore any of them.
             If a resource configuration is unsupported by a particular execution engine, we will fail at
             execution time. The supported keys are:
 
             "num_cpus" (int):
@@ -1030,15 +1030,15 @@
                 For example, the following value is valid: "nvidia.com/gpu".
             "cuda_version" (str):
                 Version of CUDA to use with GPU (only applicable for Kubernetes engine). The currently supported
                 values are "11.4.1" and "11.8.0".
         image:
             A dictionary containing the custom image configurations that this operator will run with.
             The dictionary needs to contain the following keys:
-            "registry_name" (str): The name of the registry integration to use.
+            "registry_name" (str): The name of the registry resource to use.
             "url" (str): The full URL of the image to use. Example: "123456789012.dkr.ecr.us-east-1.amazonaws.com/my-image:latest"
             It is recommended to get the dictionary via `client.resource("my_registry_name").image("my-image:latest")`
 
     Examples:
         The check name is inferred from the function name. The description is pulled from the function
         docstring or can be explicitly set in the decorator.
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/error.py` & `aqueduct-sdk-0.3.5/aqueduct/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,27 +58,27 @@
 
 
 """
 BELOW: Errors that are raised by the Python SDK code, not the backend.
 """
 
 
-# Exception raised when trying to create flow without connecting to integration
-class NoConnectedIntegrationsException(Error):
+# Exception raised when trying to create flow without connecting to resource
+class NoConnectedResourcesException(Error):
     pass
 
 
-# Exception raised when referencing an integration that doesn't exist or the wrong
-# integration type.
-class InvalidIntegrationException(Error):
+# Exception raised when referencing an resource that doesn't exist or the wrong
+# resource type.
+class InvalidResourceException(Error):
     pass
 
 
 # Exception raised when checking a flow that doesn't write to any destination store.
-class NoDestinationIntegrationException(Error):
+class NoDestinationResourceException(Error):
     pass
 
 
 # Exception raised when the user misconfigures something when running a function.
 class InvalidFunctionException(Error):
     pass
 
@@ -133,15 +133,15 @@
 
 
 # Exception raised when requirements.txt file is missing
 class RequirementsMissingError(Error):
     pass
 
 
-# Exception raised when the user attempts to use an integration that has failed to connected.
-class IntegrationFailedToConnect(Error):
+# Exception raised when the user attempts to use an resource that has failed to connected.
+class ResourceFailedToConnect(Error):
     pass
 
 
-# Exception raised when the user attempts to use an integration that is still connecting.
-class IntegrationConnectionInProgress(Error):
+# Exception raised when the user attempts to use an resource that is still connecting.
+class ResourceConnectionInProgress(Error):
     pass
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/flow.py` & `aqueduct-sdk-0.3.5/aqueduct/flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import uuid
 from collections import defaultdict
 from typing import DefaultDict, Dict, List, Optional, Union
 
 from aqueduct.error import InvalidUserArgumentException
 from aqueduct.flow_run import FlowRun
 from aqueduct.models.response_models import (
-    GetWorkflowResponse,
+    GetWorkflowV1Response,
     SavedObjectUpdate,
     WorkflowDagResponse,
 )
 from aqueduct.utils.utils import format_header_for_print, generate_ui_url, parse_user_supplied_id
 
 from aqueduct import globals
 
@@ -31,15 +31,15 @@
         self._id = flow_id
         self._in_notebook_or_console_context = in_notebook_or_console_context
 
     def id(self) -> uuid.UUID:
         """Returns the id of the flow."""
         return uuid.UUID(self._id)
 
-    def _get_workflow_resp(self) -> GetWorkflowResponse:
+    def _get_workflow_resp(self) -> GetWorkflowV1Response:
         resp = globals.__GLOBAL_API_CLIENT__.get_workflow(self._id)
         return resp
 
     def name(self) -> str:
         """Returns the latest name of the flow."""
         latest_workflow_dag = self._get_latest_dag_resp()
         assert latest_workflow_dag.metadata.name is not None
@@ -107,25 +107,25 @@
             in_notebook_or_console_context=self._in_notebook_or_console_context,
         )
 
     def list_saved_objects(self) -> DefaultDict[str, List[SavedObjectUpdate]]:
         """Get everything saved by the flow.
 
         Returns:
-            A dictionary mapping the integration id to the list of table names/storage path.
+            A dictionary mapping the resource id to the list of table names/storage path.
         """
         object_mapping: DefaultDict[str, List[SavedObjectUpdate]] = defaultdict(list)
 
         workflow_objects = globals.__GLOBAL_API_CLIENT__.list_saved_objects(self._id).object_details
         if workflow_objects is None:
             return object_mapping  # Empty map
 
         object_mapping = defaultdict(list)
         for item in workflow_objects:
-            object_mapping[item.integration_name].append(item)
+            object_mapping[item.resource_name].append(item)
         return object_mapping
 
     def describe(self) -> None:
         """Prints out a human-readable description of the flow."""
         latest_workflow_dag = self._get_latest_dag_resp()
 
         latest_metadata = latest_workflow_dag.metadata
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/flow_run.py` & `aqueduct-sdk-0.3.5/aqueduct/flow_run.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/github.py` & `aqueduct-sdk-0.3.5/aqueduct/github.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/llm_wrapper.py` & `aqueduct-sdk-0.3.5/aqueduct/llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/models/artifact.py` & `aqueduct-sdk-0.3.5/aqueduct/models/artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/models/dag.py` & `aqueduct-sdk-0.3.5/aqueduct/models/dag.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/models/dag_rules.py` & `aqueduct-sdk-0.3.5/aqueduct/models/dag_rules.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/models/execution_state.py` & `aqueduct-sdk-0.3.5/aqueduct/models/execution_state.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/models/integration.py` & `aqueduct-sdk-0.3.5/aqueduct/models/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,19 @@
                 "Tip": exec_state.error.tip,
                 "Context": exec_state.error.context,
             }
 
         return json.dumps(description_map, sort_keys=False, indent=4)
 
     def describe(self) -> None:
-        """Prints out a human-readable description of the integration."""
+        """Prints out a human-readable description of the resource."""
         print(repr(self))
 
     def is_relational(self) -> bool:
-        """Returns whether the integration connects to a relational data store."""
+        """Returns whether the resource connects to a relational data store."""
         return self.service in [
             ServiceType.POSTGRES,
             ServiceType.SNOWFLAKE,
             ServiceType.MYSQL,
             ServiceType.REDSHIFT,
             ServiceType.MARIADB,
             ServiceType.SQLSERVER,
@@ -57,37 +57,37 @@
             ServiceType.SQLITE,
             ServiceType.ATHENA,
         ]
 
 
 class BaseResource(ABC):
     """
-    Base class for the various integrations Aqueduct interacts with.
+    Base class for the various resources Aqueduct interacts with.
     """
 
     _metadata: ResourceInfo
 
     def id(self) -> uuid.UUID:
         return self._metadata.id
 
     def name(self) -> str:
         return self._metadata.name
 
     def type(self) -> ServiceType:
         return self._metadata.service
 
     def __hash__(self) -> int:
-        """An integration is uniquely identified by its name.
+        """An resource is uniquely identified by its name.
         Ref: https://docs.python.org/3.5/reference/datamodel.html#object.__hash__
         """
         return hash(self._metadata.name)
 
     def __eq__(self, other: Any) -> bool:
         """The string and resource object representation are equivalent allowing
         the user to access a dictionary keyed by the BaseResource object with the
-        integration name as a string and vice versa
+        resource name as a string and vice versa
         """
         if type(other) == type(self) and "name" in other._metadata.__dict__:
             return bool(self._metadata.name == other._metadata.name)
         elif type(other) == str:
             return bool(self._metadata.name == other)
         return False
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/models/operators.py` & `aqueduct-sdk-0.3.5/aqueduct/models/operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,20 @@
     S3TableFormat,
     SalesforceExtractType,
     SerializationType,
     ServiceType,
 )
 from aqueduct.error import AqueductError, UnsupportedFeatureException
 from aqueduct.models.config import EngineConfig
-from aqueduct.models.integration import ResourceInfo
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, Extra, Field
 
 
 class GithubMetadata(BaseModel):
     """
-    Specifies a destination in github integration.
+    Specifies a destination in github resource.
     There are two ways to specify the content:
     -   by `path`, which points to a file or dir in the github repo.
     -   from `repo_config_content_type` and `repo_config_content_name`, which points to
         information stored in the repo's `.aqconfig`.
     If using `repo_config` content, backend will ignore `path` and overwrite it with
     the `path` specified in `.aqconfig`.
     """
@@ -86,16 +85,23 @@
     MongoExtractParams,
     RelationalDBExtractParams,
 ]
 
 
 class ExtractSpec(BaseModel):
     service: ServiceType
-    integration_id: uuid.UUID
-    parameters: UnionExtractParams
+
+    # TODO(ENG-2994): This spec is parsed into a golang struct that still expects
+    #  the "integration" terminology.
+    resource_id: uuid.UUID = Field(alias="integration_id")
+    parameters: Union[str, UnionExtractParams]
+
+    class Config:
+        # Prevents any validation errors due to the alias when setting the `resource_id` field.
+        allow_population_by_field_name = True
 
 
 class RelationalDBLoadParams(BaseModel):
     # If this field is parameterized, then it is expected to be empty.
     # Instead, we will feed the parameter artifact into the save operator.
     table: str
     update_mode: LoadUpdateMode
@@ -123,35 +129,41 @@
     SalesforceLoadParams, S3LoadParams, GoogleSheetsLoadParams, RelationalDBLoadParams
 ]
 
 
 # Class expected by backend for a load operator.
 class LoadSpec(BaseModel):
     service: ServiceType
-    integration_id: uuid.UUID
+
+    # TODO(ENG-2994): This spec is parsed into a golang struct that still expects
+    #  the "integration" terminology.
+    resource_id: uuid.UUID = Field(alias="integration_id")
     parameters: UnionLoadParams
 
+    class Config:
+        # Prevents any validation errors due to the alias when setting the `resource_id` field.
+        allow_population_by_field_name = True
+
     def identifier(self) -> str:
         if isinstance(self.parameters, RelationalDBLoadParams):
             return self.parameters.table
         elif isinstance(self.parameters, S3LoadParams):
             return self.parameters.filepath
         raise UnsupportedFeatureException(
-            "identifier() is currently unsupported for data integration type %s."
-            % self.service.value
+            "identifier() is currently unsupported for data resource type %s." % self.service.value
         )
 
     def set_identifier(self, new_obj_identifier: str) -> None:
         if isinstance(self.parameters, RelationalDBLoadParams):
             self.parameters.table = new_obj_identifier
         elif isinstance(self.parameters, S3LoadParams):
             self.parameters.filepath = new_obj_identifier
         else:
             raise UnsupportedFeatureException(
-                "set_identifier() is currently unsupported for data integration type %s."
+                "set_identifier() is currently unsupported for data resource type %s."
                 % self.service.value
             )
 
 
 class EntryPoint(BaseModel):
     file: str
     class_name: Optional[str]
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/models/response_models.py` & `aqueduct-sdk-0.3.5/aqueduct/models/response_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime
 from typing import Dict, List, Optional, Union
 
 from aqueduct.constants.enums import (
     ArtifactType,
     ExecutionStatus,
     K8sClusterStatusType,
+    NotificationLogLevel,
     SerializationType,
 )
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import EngineConfig, Metadata, RetentionPolicy, Schedule
 from aqueduct.models.execution_state import ExecutionState
 from aqueduct.models.operators import LoadSpec, Operator, OperatorSpec
 from aqueduct.models.utils import human_readable_timestamp
@@ -19,14 +20,53 @@
 class ArtifactResult(BaseModel):
     serialization_type: SerializationType
     artifact_type: ArtifactType
     content: bytes
 
 
 # V2 Responses
+class NotificationSettings(BaseModel):
+    """Represents the notification settings associated with a workflow."""
+
+    settings: Optional[Dict[str, NotificationLogLevel]]
+
+
+class GetWorkflowResponse(BaseModel):
+    """Represents a single workflow.
+
+    Attributes:
+        id:
+            The id of the artifact node.
+        user_id:
+            The user id of the owner.
+        name:
+            The name of the workflow.
+        description:
+            The description of the workflow.
+        schedule:
+            The schedule of the workflow.
+        created_at:
+            When the workflow is created.
+        retention_policy:
+            Workflow retention policy regarding number of DAGs to save.
+        notification_settings:
+            Notification setting of workflow.
+
+    """
+
+    id: uuid.UUID
+    user_id: uuid.UUID
+    name: str
+    description: str
+    schedule: Schedule
+    created_at: str
+    retention_policy: RetentionPolicy
+    notification_settings: NotificationSettings
+
+
 class GetDagResponse(BaseModel):
     id: uuid.UUID
     workflow_id: uuid.UUID
     created_at: str
     engine_config: EngineConfig
 
 
@@ -332,15 +372,15 @@
             "status": self.status.value,
         }
         if self.exec_state.error is not None:
             readable["error"] = self.exec_state.error.tip + "\n" + self.exec_state.error.context
         return readable
 
 
-class GetWorkflowResponse(BaseModel):
+class GetWorkflowV1Response(BaseModel):
     """This is the response object returned by api_client.get_workflow().
 
     Attributes:
         workflow_dags:
             All the historical workflow dags.
         workflow_dag_results:
             All the historical workflow results.
@@ -446,26 +486,26 @@
 class DeleteWorkflowResponse(BaseModel):
     """This is the response object returned by api_client.delete_workflow().
 
     Attributes:
         saved_object_deletion_results:
             Results of deleting saved objects.
             Key: Resource name
-            Value: List of SavedObjectDelete belonging to that integration
+            Value: List of SavedObjectDelete belonging to that resource
     """
 
     saved_object_deletion_results: Dict[str, List[SavedObjectDelete]]
 
 
 class SavedObjectUpdate(BaseModel):
     """This is an item in the list returned by ListWorkflowSavedObjectsResponse."""
 
     operator_name: str
     modified_at: str
-    integration_name: str
+    resource_name: str
     spec: LoadSpec
 
 
 class ListWorkflowSavedObjectsResponse(BaseModel):
     """This is the response object returned by api_client.get_workflow_writes().
 
     Attributes:
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/aws.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/aws.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from aqueduct.models.integration import BaseResource, ResourceInfo
+from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.resources.dynamic_k8s import DynamicK8sResource
 
 
 class AWSResource(BaseResource):
     """
-    Class for AWS integration.
+    Class for AWS resource.
     """
 
-    def __init__(self, metadata: ResourceInfo, k8s_integration_metadata: ResourceInfo):
+    def __init__(self, metadata: ResourceInfo, k8s_resource_metadata: ResourceInfo):
         self._metadata = metadata
-        self.k8s = DynamicK8sResource(k8s_integration_metadata)
+        self.k8s = DynamicK8sResource(k8s_resource_metadata)
 
     def describe(self) -> None:
-        """Prints out a human-readable description of the K8s integration."""
+        """Prints out a human-readable description of the K8s resource."""
         print("==================== AWS Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/connect_config.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/connect_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union, cast
 
-from aqueduct.constants.enums import MetaEnum, NotificationLevel, ServiceType
+from aqueduct.constants.enums import CloudProviderType, MetaEnum, NotificationLevel, ServiceType
 from aqueduct.error import InternalAqueductError, InvalidUserArgumentException
 from pydantic import BaseModel, Extra, Field
 
 """Copied mostly over from `aqueduct_executor/operators/connectors/data/config.py` for now, please keep them in sync."""
 
 
 class BaseConnectionConfig(BaseModel):
@@ -17,15 +17,15 @@
 
     class Config:
         extra = Extra.forbid
 
 
 class BigQueryConfig(BaseConnectionConfig):
     """
-    BigQueryConfig defines the Pydantic Config for a BigQuery integration.
+    BigQueryConfig defines the Pydantic Config for a BigQuery resource.
     One of the following between `service_account_credentials` and
     `service_account_credentials_path` must be specified. If `service_account_credentials_path`
     is specified, it takes priority.
     """
 
     project_id: str
     service_account_credentials: Optional[str] = None
@@ -82,15 +82,15 @@
     # Config credentials
     config_file_path: str = ""
     config_file_profile: str = ""
 
     bucket: str
     region: str
 
-    # When connecting a new integration, we allow both leading or trailing slashes here.
+    # When connecting a new resource, we allow both leading or trailing slashes here.
     # The path will be sanitized before being stored in the database.
     root_dir: str = ""
 
     use_as_storage: str = "false"
 
 
 class GCSConfig(BaseConnectionConfig):
@@ -195,25 +195,37 @@
     secret_access_key: str = ""
     region: str = ""
     config_file_path: str = ""
     config_file_profile: str = ""
     k8s: Optional[DynamicK8sConfig]
 
 
+class GCPConfig(BaseConnectionConfig):
+    region: str
+    zone: str
+    service_account_key_path: str = ""
+    service_account_key: str = ""
+
+
 class ECRConfig(BaseConnectionConfig):
     # Either 1) all of access_key_id, secret_access_key, region, or 2) both config_file_path and
     # config_file_profile need to be specified. Any other cases will be rejected by the server's
     # config validation process.
     access_key_id: str = ""
     secret_access_key: str = ""
     region: str = ""
     config_file_path: str = ""
     config_file_profile: str = ""
 
 
+class GARConfig(BaseConnectionConfig):
+    service_account_key_path: str = ""
+    service_account_key: str = ""
+
+
 class _AWSConfigWithSerializedConfig(BaseConnectionConfig):
     access_key_id: str = ""
     secret_access_key: str = ""
     region: str = ""
     config_file_path: str = ""
     config_file_profile: str = ""
     k8s_serialized: Optional[
@@ -261,19 +273,41 @@
     workspace_url: str
     access_token: str
     s3_instance_profile_arn: str
     instance_pool_id: Optional[str] = None
 
 
 class K8sConfig(BaseConnectionConfig):
+    kubeconfig_path: str = ""
+    cluster_name: str = ""
+    use_same_cluster: str = "false"
+    cloud_provider: Optional[CloudProviderType]
+    gcp_config: Optional[GCPConfig]
+    cluster_config: Optional[DynamicK8sConfig]
+
+
+class _K8sConfigWithSerializedConfig(BaseConnectionConfig):
     kubeconfig_path: str
     cluster_name: str
     use_same_cluster: str = "false"
-    dynamic: str = "false"
-    cloud_integration_id: str = ""
+    cloud_provider: Optional[CloudProviderType]
+    gcp_config_serialized: Optional[str]  # this is a json-serialized string of GCPConfig
+    # add fields from DynamicK8sConfig
+    keepalive: Optional[Union[str, int]]
+    cpu_node_type: Optional[str]
+    gpu_node_type: Optional[str]
+    min_cpu_node: Optional[Union[str, int]]
+    max_cpu_node: Optional[Union[str, int]]
+    min_gpu_node: Optional[Union[str, int]]
+    max_gpu_node: Optional[Union[str, int]]
+
+    # This converts all int fields to string during json serialization. We need to do this becasue our
+    # backend assumes all config fields must be string.
+    class Config:
+        json_encoders = {int: str}
 
 
 ResourceConfig = Union[
     BigQueryConfig,
     EmailConfig,
     _EmailConfigWithStringField,
     MySQLConfig,
@@ -283,25 +317,27 @@
     AthenaConfig,
     SnowflakeConfig,
     SqlServerConfig,
     SQLiteConfig,
     SlackConfig,
     AWSConfig,
     ECRConfig,
+    GARConfig,
     _AWSConfigWithSerializedConfig,
     _SlackConfigWithStringField,
     AirflowConfig,
     SparkConfig,
     DatabricksConfig,
     K8sConfig,
     CondaConfig,
+    _K8sConfigWithSerializedConfig,
 ]
 
 
-def convert_dict_to_integration_connect_config(
+def convert_dict_to_resource_connect_config(
     service: Union[str, ServiceType], config_dict: Dict[str, str]
 ) -> ResourceConfig:
     if service == ServiceType.BIGQUERY:
         return BigQueryConfig(**config_dict)
     elif service in [ServiceType.MARIADB, ServiceType.MYSQL]:
         return MySQLConfig(**config_dict)
     elif service == ServiceType.MONGO_DB:
@@ -334,35 +370,43 @@
         return DatabricksConfig(**config_dict)
     elif service == ServiceType.AWS:
         return AWSConfig(**config_dict)
     elif service == ServiceType.K8S:
         return K8sConfig(**config_dict)
     elif service == ServiceType.ECR:
         return ECRConfig(**config_dict)
+    elif service == ServiceType.GAR:
+        return GARConfig(**config_dict)
     raise InternalAqueductError("Unexpected Service Type: %s" % service)
 
 
-def prepare_integration_config(
+def prepare_resource_config(
     service: Union[str, ServiceType], config: ResourceConfig
 ) -> ResourceConfig:
     """Prepares the ResourceConfig object to be sent to the backend
-    as part of a request to connect a new integration.
+    as part of a request to connect a new resource.
     """
     if service == ServiceType.BIGQUERY:
         return _prepare_big_query_config(cast(BigQueryConfig, config))
 
     if service == ServiceType.SLACK:
         return _prepare_slack_config(cast(SlackConfig, config))
 
     if service == ServiceType.EMAIL:
         return _prepare_email_config(cast(EmailConfig, config))
 
     if service == ServiceType.AWS:
         return _prepare_aws_config(cast(AWSConfig, config))
 
+    if service == ServiceType.K8S:
+        return _prepare_k8s_config(cast(K8sConfig, config))
+
+    if service == ServiceType.GAR:
+        return _prepare_gar_config(cast(GARConfig, config))
+
     return config
 
 
 def _prepare_email_config(config: EmailConfig) -> _EmailConfigWithStringField:
     return _EmailConfigWithStringField(
         user=config.user,
         password=config.password,
@@ -390,14 +434,45 @@
         region=config.region,
         config_file_path=config.config_file_path,
         config_file_profile=config.config_file_profile,
         k8s_serialized=(None if config.k8s is None else config.k8s.json(exclude_none=True)),
     )
 
 
+def _prepare_k8s_config(config: K8sConfig) -> _K8sConfigWithSerializedConfig:
+    if config.gcp_config is not None and config.gcp_config.service_account_key_path is not None:
+        with open(config.gcp_config.service_account_key_path, "r") as f:
+            config.gcp_config.service_account_key = f.read()
+
+    return _K8sConfigWithSerializedConfig(
+        kubeconfig_path=config.kubeconfig_path,
+        cluster_name=config.cluster_name,
+        use_same_cluster=config.use_same_cluster,
+        cloud_provider=config.cloud_provider,
+        gcp_config_serialized=(
+            None if config.gcp_config is None else config.gcp_config.json(exclude_none=True)
+        ),
+        # add fields from DynamicK8sConfig
+        keepalive=config.cluster_config.keepalive if config.cluster_config else None,
+        cpu_node_type=config.cluster_config.cpu_node_type if config.cluster_config else None,
+        gpu_node_type=config.cluster_config.gpu_node_type if config.cluster_config else None,
+        min_cpu_node=config.cluster_config.min_cpu_node if config.cluster_config else None,
+        max_cpu_node=config.cluster_config.max_cpu_node if config.cluster_config else None,
+        min_gpu_node=config.cluster_config.min_gpu_node if config.cluster_config else None,
+        max_gpu_node=config.cluster_config.max_gpu_node if config.cluster_config else None,
+    )
+
+
+def _prepare_gar_config(config: GARConfig) -> GARConfig:
+    if config.service_account_key_path is not None:
+        with open(config.service_account_key_path, "r") as f:
+            config.service_account_key = f.read()
+    return config
+
+
 def _prepare_big_query_config(config: BigQueryConfig) -> BigQueryConfig:
     """Prepares the BigQueryConfig object by reading the service account
     credentials into a string field if the filepath is specified.
     """
     if not config.service_account_credentials and not config.service_account_credentials_path:
         raise InvalidUserArgumentException(
             "At least one of `service_account_credentials` or `service_account_credentials_path` must be set for a BigQueryConfig."
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/dynamic_k8s.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/dynamic_k8s.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Union
 
 from aqueduct.constants.enums import K8sClusterActionType, K8sClusterStatusType
-from aqueduct.error import InvalidIntegrationException, InvalidUserArgumentException
-from aqueduct.models.integration import BaseResource, ResourceInfo
+from aqueduct.error import InvalidResourceException, InvalidUserArgumentException
+from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.models.response_models import DynamicEngineStatusResponse
 from aqueduct.resources.connect_config import DynamicK8sConfig
 from aqueduct.resources.validation import validate_is_connected
 
 
 def parse_dynamic_k8s_config(
     config_delta: Union[Dict[str, Union[int, str]], DynamicK8sConfig]
@@ -22,35 +22,35 @@
     return config_delta
 
 
 def validate_engine_record(
     name: str, engine_statuses: Dict[str, DynamicEngineStatusResponse]
 ) -> None:
     if len(engine_statuses) == 0:
-        raise InvalidIntegrationException("Dynamic engine %s does not exist!" % name)
+        raise InvalidResourceException("Dynamic engine %s does not exist!" % name)
 
     if len(engine_statuses) > 1:
-        raise InvalidIntegrationException("Duplicate dynamic engine with name %s!" % name)
+        raise InvalidResourceException("Duplicate dynamic engine with name %s!" % name)
 
 
 class DynamicK8sResource(BaseResource):
     """
-    Class for Dynamic K8s integration.
+    Class for Dynamic K8s resource.
     """
 
     def __init__(self, metadata: ResourceInfo):
         self._metadata = metadata
 
     @validate_is_connected()
     def status(self) -> str:
         """Get the current status of the dynamic Kubernetes cluster."""
         from aqueduct import globals
 
         engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status(
-            engine_integration_ids=[str(self._metadata.id)]
+            engine_resource_ids=[str(self._metadata.id)]
         )
 
         validate_engine_record(self._metadata.name, engine_statuses)
 
         return engine_statuses[self._metadata.name].status.value
 
     @validate_is_connected()
@@ -62,25 +62,25 @@
         Args:
             config_delta (optional):
                 This field contains new config values to be used in creating the cluster.
                 These new values will overwrite existing ones from that point on. Any config values
                 that are identical to the current ones do not need to be included in config_delta.
 
         Raises:
-            InvalidIntegrationException:
+            InvalidResourceException:
                 An error occurred when the dynamic engine doesn't exist.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
         config_delta = parse_dynamic_k8s_config(config_delta)
 
         from aqueduct import globals
 
         engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status(
-            engine_integration_ids=[str(self._metadata.id)]
+            engine_resource_ids=[str(self._metadata.id)]
         )
 
         validate_engine_record(self._metadata.name, engine_statuses)
 
         status = engine_statuses[self._metadata.name].status
         if status == K8sClusterStatusType.ACTIVE and all(
             value is None for value in config_delta.dict().values()
@@ -90,15 +90,15 @@
 
         print(
             "Cluster is currently in %s status. It could take 12-15 minutes for the cluster to be created or updated..."
             % status.value
         )
         globals.__GLOBAL_API_CLIENT__.edit_dynamic_engine(
             action=K8sClusterActionType.CREATE,
-            integration_id=str(self._metadata.id),
+            resource_id=str(self._metadata.id),
             config_delta=config_delta,
         )
 
     @validate_is_connected()
     def update(self, config_delta: Union[Dict[str, Union[int, str]], DynamicK8sConfig]) -> None:
         """Update the dynamic Kubernetes cluster. This can only be done when the cluster is in
             Active status.
@@ -106,25 +106,25 @@
         Args:
             config_delta:
                 This field contains new config values to be used in creating the cluster.
                 These new values will overwrite existing ones from that point on. Any config values
                 that are identical to the current ones do not need to be included in config_delta.
 
         Raises:
-            InvalidIntegrationException:
+            InvalidResourceException:
                 An error occurred when the dynamic engine doesn't exist.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
         config_delta = parse_dynamic_k8s_config(config_delta)
 
         from aqueduct import globals
 
         engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status(
-            engine_integration_ids=[str(self._metadata.id)]
+            engine_resource_ids=[str(self._metadata.id)]
         )
 
         validate_engine_record(self._metadata.name, engine_statuses)
 
         status = engine_statuses[self._metadata.name].status
         if status != K8sClusterStatusType.ACTIVE:
             print(
@@ -135,38 +135,38 @@
 
         print(
             "Cluster is currently in %s status. It could take 12-15 minutes for the cluster to be updated..."
             % status.value
         )
         globals.__GLOBAL_API_CLIENT__.edit_dynamic_engine(
             action=K8sClusterActionType.UPDATE,
-            integration_id=str(self._metadata.id),
+            resource_id=str(self._metadata.id),
             config_delta=config_delta,
         )
 
     @validate_is_connected()
     def delete(self, force: bool = False) -> None:
         """Deletes the dynamic Kubernetes cluster if it is running, ignoring the keepalive period.
 
         Args:
             force:
                 By default, if there are any pods in the "Running" or "ContainerCreating" status,
                 the deletion process will fail. However, if the flag is set to "True", this check
                 will be skipped, allowing the cluster to be deleted despite the presence of such pods.
 
         Raises:
-            InvalidIntegrationException:
+            InvalidResourceException:
                 An error occurred when the dynamic engine doesn't exist.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
         from aqueduct import globals
 
         engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status(
-            engine_integration_ids=[str(self._metadata.id)]
+            engine_resource_ids=[str(self._metadata.id)]
         )
 
         validate_engine_record(self._metadata.name, engine_statuses)
 
         status = engine_statuses[self._metadata.name].status
         if status == K8sClusterStatusType.TERMINATED:
             print("Cluster is already in %s status." % status.value)
@@ -178,14 +178,14 @@
         )
 
         action = K8sClusterActionType.DELETE
         if force:
             action = K8sClusterActionType.FORCE_DELETE
 
         globals.__GLOBAL_API_CLIENT__.edit_dynamic_engine(
-            action=action, integration_id=str(self._metadata.id)
+            action=action, resource_id=str(self._metadata.id)
         )
 
     def describe(self) -> None:
-        """Prints out a human-readable description of the K8s integration."""
+        """Prints out a human-readable description of the K8s resource."""
         print("==================== Dynamic K8s Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/ecr.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/ecr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Dict
 
 from aqueduct.error import InvalidUserArgumentException
-from aqueduct.models.integration import BaseResource, ResourceInfo
+from aqueduct.models.resource import BaseResource, ResourceInfo
 
 from aqueduct import globals
 
 
 class ECRResource(BaseResource):
     """
-    Class for ECR integration.
+    Class for ECR resource.
     """
 
     def __init__(self, metadata: ResourceInfo):
         self._metadata = metadata
 
     def describe(self) -> None:
-        """Prints out a human-readable description of the ECR integration."""
+        """Prints out a human-readable description of the ECR resource."""
         print("==================== ECR Resource =============================")
         self._metadata.describe()
 
     def image(self, image_name: str) -> Dict[str, str]:
         """
         Returns a dictionary with the name of the ECR resource and the image URL, which can be
         used as input to the `image` field of an operator's decorator. This method also verifies
@@ -35,15 +35,15 @@
         if len(image_name.split(":")) != 2:
             if len(image_name.split(":")) == 1:
                 image_name = image_name + ":latest"
             else:
                 raise InvalidUserArgumentException("Image name must be of the form `image:tag`.")
 
         response = globals.__GLOBAL_API_CLIENT__.get_image_url(
-            integration_id=str(self._metadata.id),
+            resource_id=str(self._metadata.id),
             service=self._metadata.service,
             image_name=image_name,
         )
 
         return {
             "registry_name": self._metadata.name,
             "url": response.url,
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/google_sheets.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/google_sheets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import Optional
 
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.table_artifact import TableArtifact
 from aqueduct.constants.enums import ArtifactType, GoogleSheetsSaveMode
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     GoogleSheetsExtractParams,
     GoogleSheetsLoadParams,
     Operator,
     OperatorSpec,
 )
+from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.utils import generate_uuid
 
 from ..utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
 from .save import _save_artifact
 
 
 class GoogleSheetsResource(BaseResource):
     """
-    Class for Google Sheets integration.
+    Class for Google Sheets resource.
     """
 
     def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
     @validate_is_connected()
@@ -35,15 +35,15 @@
         self,
         spreadsheet_id: str,
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
     ) -> TableArtifact:
         """
-        Retrieves a spreadsheet from the Google Sheets integration.
+        Retrieves a spreadsheet from the Google Sheets resource.
 
         Args:
             spreadsheet_id:
                 Id of spreadsheet to retrieve. This can be found in the URL of the spreadsheet, e.g.
                 https://docs.google.com/spreadsheets/d/{SPREADSHEET_ID}/edit#gid=0
             name:
                 Name of the query.
@@ -51,15 +51,15 @@
                 Name to assign the output artifact. If not set, the default naming scheme will be used.
             description:
                 Description of the query.
 
         Returns:
             TableArtifact representing the Google Sheet.
         """
-        integration_info = self._metadata
+        resource_info = self._metadata
 
         op_name = name or "%s query" % self.name()
         artifact_name = output or default_artifact_name_from_op_name(op_name)
 
         operator_id = generate_uuid()
         output_artifact_id = generate_uuid()
         apply_deltas_to_dag(
@@ -68,16 +68,16 @@
                 AddOperatorDelta(
                     op=Operator(
                         id=operator_id,
                         name=op_name,
                         description=description,
                         spec=OperatorSpec(
                             extract=ExtractSpec(
-                                service=integration_info.service,
-                                integration_id=integration_info.id,
+                                service=resource_info.service,
+                                resource_id=resource_info.id,
                                 parameters=GoogleSheetsExtractParams(
                                     spreadsheet_id=spreadsheet_id,
                                 ),
                             )
                         ),
                         outputs=[output_artifact_id],
                     ),
@@ -124,10 +124,10 @@
             artifact.id(),
             self._dag,
             self._metadata,
             save_params=GoogleSheetsLoadParams(filepath=filepath, save_mode=save_mode),
         )
 
     def describe(self) -> None:
-        """Prints out a human-readable description of the google sheets integration."""
+        """Prints out a human-readable description of the google sheets resource."""
         print("==================== Google Sheets Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/mongodb.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/mongodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 
 from aqueduct.artifacts import preview as artifact_utils
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.table_artifact import TableArtifact
 from aqueduct.constants.enums import ArtifactType, ExecutionMode, LoadUpdateMode
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     MongoExtractParams,
     Operator,
     OperatorSpec,
     RelationalDBLoadParams,
 )
+from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.resources.parameters import _validate_parameters
 from aqueduct.resources.save import _save_artifact
 from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
 from aqueduct.utils.utils import generate_uuid
 
 from aqueduct import globals
 
 
-class MongoDBCollectionIntegration(BaseResource):
+class MongoDBCollectionResource(BaseResource):
     _collection_name: str
     _dag: DAG
 
     def __init__(self, dag: DAG, metadata: ResourceInfo, collection_name: str) -> None:
         self._metadata = metadata
         self._dag = dag
         self._collection_name = collection_name
@@ -63,15 +63,15 @@
                 An optional list of string parameters to use in the query.  We use the Postgres syntax of $1, $2 for placeholders.
                 The number denotes which parameter in the list to use (one-indexed). These parameters feed into the
                 sql query operator and will fill in the placeholders in the query with the actual values.
 
                 Example:
                     country1 = client.create_param("UK", default=" United Kingdom ")
                     country2 = client.create_param("Thailand", default=" Thailand ")
-                    mongo_db_integration.collection("hotel_reviews").find(
+                    mongo_db_resource.collection("hotel_reviews").find(
                         {
                             "reviewer_nationality": {
                                 "$in": [$1, $2],
                            }
                         },
                         parameters=[country1, country2],
                     )
@@ -126,15 +126,15 @@
                     op=Operator(
                         id=op_id,
                         name=op_name,
                         description=description,
                         spec=OperatorSpec(
                             extract=ExtractSpec(
                                 service=self.type(),
-                                integration_id=self.id(),
+                                resource_id=self.id(),
                                 parameters=mongo_extract_params,
                             )
                         ),
                         inputs=param_artf_ids,
                         outputs=[output_artf_id],
                     ),
                     output_artifacts=[
@@ -177,37 +177,37 @@
                 table=self._collection_name, update_mode=update_mode
             ),
         )
 
 
 class MongoDBResource(BaseResource):
     """
-    Class for MongoDB integration. This works similar to mongo's `Database` object:
+    Class for MongoDB resource. This works similar to mongo's `Database` object:
 
-    mongo_integration = client.resource("my_resource_name")
-    my_table_artifact = mongo_integration.collection("my_collection").find({})
+    mongo_resource = client.resource("my_resource_name")
+    my_table_artifact = mongo_resource.collection("my_collection").find({})
     """
 
     def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
     @validate_is_connected()
-    def collection(self, name: str) -> MongoDBCollectionIntegration:
+    def collection(self, name: str) -> MongoDBCollectionResource:
         """Returns a specific collection object to call `.find()` method.
 
         Example:
 
         mongo_resource = client.resource("my_resource_name")
         my_table_artifact = mongo_resource.collection("my_collection").find({})
         """
-        return MongoDBCollectionIntegration(self._dag, self._metadata, name)
+        return MongoDBCollectionResource(self._dag, self._metadata, name)
 
     def describe(self) -> None:
-        """Prints out a human-readable description of the MongoDB integration."""
+        """Prints out a human-readable description of the MongoDB resource."""
         print("==================== MongoDB Resource =============================")
         self._metadata.describe()
 
     @validate_is_connected()
     def save(self, artifact: BaseArtifact, collection: str, update_mode: LoadUpdateMode) -> None:
         """Registers a save operator of the given artifact, to be executed when it's computed in a published flow.
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/parameters.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/parameters.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/s3.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from typing import List, Optional, Union
 
 from aqueduct.artifacts import preview as artifact_utils
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.constants.enums import ArtifactType, ExecutionMode, S3TableFormat
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     Operator,
     OperatorSpec,
     S3ExtractParams,
     S3LoadParams,
 )
+from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.utils import generate_uuid
 
 from aqueduct import globals
 
 from ..artifacts.create import to_artifact_class
@@ -42,15 +42,15 @@
     else:
         raise InvalidUserArgumentException("Unsupported S3 file format `%s`." % format)
     return format_enum
 
 
 class S3Resource(BaseResource):
     """
-    Class for S3 integration.
+    Class for S3 resource.
     """
 
     def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
     @validate_is_connected()
@@ -62,15 +62,15 @@
         merge: Optional[bool] = None,
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
         lazy: bool = False,
     ) -> BaseArtifact:
         """
-        Reads one or more files from the S3 integration.
+        Reads one or more files from the S3 resource.
 
         Args:
             filepaths:
                 Filepath to retrieve from. The filepaths can either be:
                 1) a single string that represents a file name or a directory name. The directory
                 name must ends with a `/`. In case of a file name, we attempt to retrieve that file.
                 In case of a directory name, we do a prefix search on the directory and retrieve
@@ -110,15 +110,15 @@
         if format and artifact_type != ArtifactType.TABLE:
             raise InvalidUserArgumentException(
                 "Format argument is only applicable to table artifact type, found %s instead."
                 % artifact_type
             )
         format_enum = _convert_to_s3_table_format(format)
 
-        integration_info = self._metadata
+        resource_info = self._metadata
         op_name = name or "%s query" % self.name()
         artifact_name = output or default_artifact_name_from_op_name(op_name)
 
         operator_id = generate_uuid()
         output_artifact_id = generate_uuid()
 
         def _is_directory_search() -> bool:
@@ -139,16 +139,16 @@
                 AddOperatorDelta(
                     op=Operator(
                         id=operator_id,
                         name=op_name,
                         description=description,
                         spec=OperatorSpec(
                             extract=ExtractSpec(
-                                service=integration_info.service,
-                                integration_id=integration_info.id,
+                                service=resource_info.service,
+                                resource_id=resource_info.id,
                                 parameters=S3ExtractParams(
                                     filepath=json.dumps(filepaths),
                                     artifact_type=artifact_type,
                                     format=format_enum,
                                     merge=merge,
                                 ),
                             )
@@ -184,15 +184,15 @@
             filepath:
                 The S3 path to save to. Will overwrite any existing object at that path.
             format:
                 Only required if saving a table artifact. Options are case-insensitive "json", "csv", "parquet".
         """
         if artifact.type() == ArtifactType.TABLE and format is None:
             raise InvalidUserArgumentException(
-                "You must supply a file format when saving tabular data into S3 integration `%s`."
+                "You must supply a file format when saving tabular data into S3 resource `%s`."
                 % self.name(),
             )
         elif (
             artifact.type() != ArtifactType.TABLE
             and artifact.type() != ArtifactType.UNTYPED
             and format is not None
         ):
@@ -211,10 +211,10 @@
             artifact_ids,
             self._dag,
             self._metadata,
             save_params=S3LoadParams(filepath=filepath, format=_convert_to_s3_table_format(format)),
         )
 
     def describe(self) -> None:
-        """Prints out a human-readable description of the S3 integration."""
+        """Prints out a human-readable description of the S3 resource."""
         print("==================== S3 Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/salesforce.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/salesforce.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 from typing import Optional
 
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.table_artifact import TableArtifact
 from aqueduct.constants.enums import ArtifactType, SalesforceExtractType
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     Operator,
     OperatorSpec,
     SalesforceExtractParams,
     SalesforceLoadParams,
 )
+from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.utils import generate_uuid
 
 from ..utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
 from .save import _save_artifact
 
 
 class SalesforceResource(BaseResource):
     """
-    Class for Salesforce integration.
+    Class for Salesforce resource.
     """
 
     def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
     @validate_is_connected()
@@ -36,15 +36,15 @@
         self,
         search_query: str,
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
     ) -> TableArtifact:
         """
-        Runs a search against the Salesforce integration.
+        Runs a search against the Salesforce resource.
 
         Args:
             search_query:
                 The search query to run.
             name:
                 Name of the query.
            output:
@@ -76,15 +76,15 @@
         self,
         query: str,
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
     ) -> TableArtifact:
         """
-        Runs a query against the Salesforce integration.
+        Runs a query against the Salesforce resource.
 
         Args:
             query:
                 The query to run.
             name:
                 Name of the query.
             output:
@@ -126,31 +126,31 @@
         self,
         op_name: str,
         output: Optional[str],
         description: str,
         query: str,
         extract_type: SalesforceExtractType,
     ) -> uuid.UUID:
-        integration_info = self._metadata
+        resource_info = self._metadata
 
         artifact_name = output or default_artifact_name_from_op_name(op_name)
         operator_id = generate_uuid()
         output_artifact_id = generate_uuid()
         apply_deltas_to_dag(
             self._dag,
             deltas=[
                 AddOperatorDelta(
                     op=Operator(
                         id=operator_id,
                         name=op_name,
                         description=description,
                         spec=OperatorSpec(
                             extract=ExtractSpec(
-                                service=integration_info.service,
-                                integration_id=integration_info.id,
+                                service=resource_info.service,
+                                resource_id=resource_info.id,
                                 parameters=SalesforceExtractParams(type=extract_type, query=query),
                             )
                         ),
                         outputs=[output_artifact_id],
                     ),
                     output_artifacts=[
                         ArtifactMetadata(
@@ -163,10 +163,10 @@
                 )
             ],
         )
 
         return output_artifact_id
 
     def describe(self) -> None:
-        """Prints out a human-readable description of the Salesforce integration."""
+        """Prints out a human-readable description of the Salesforce resource."""
         print("==================== Salesforce Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/save.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/save.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,88 @@
 import uuid
 from typing import List, Union
 
 from aqueduct.constants.enums import OperatorType
-from aqueduct.error import InvalidIntegrationException
+from aqueduct.error import InvalidResourceException
 from aqueduct.globals import __GLOBAL_API_CLIENT__ as global_api_client
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import ResourceInfo
 from aqueduct.models.operators import LoadSpec, Operator, OperatorSpec, UnionLoadParams
+from aqueduct.models.resource import ResourceInfo
 from aqueduct.utils.dag_deltas import (
     AddOperatorDelta,
     DAGDelta,
     RemoveOperatorDelta,
     apply_deltas_to_dag,
 )
 from aqueduct.utils.utils import generate_uuid
 
 
 def _save_artifact(
     artifact_ids: Union[uuid.UUID, List[uuid.UUID]],
     dag: DAG,
-    integration_info: ResourceInfo,
+    resource_info: ResourceInfo,
     save_params: UnionLoadParams,
 ) -> None:
-    """Configures the given artifact to be written to a specific integration after it's computed in a published flow.
+    """Configures the given artifact to be written to a specific resource after it's computed in a published flow.
 
     Args:
         artifact_ids:
             Can either be a single ID, or any number of IDs. In the latter case, that means that the first n-1 artifacts
             are parameters to the save operators. The nth artifact is the one that will be saved.
         dag:
             The dag object that we will attach the load operator to.
-        integration_info:
-            Config info for the destination integration.
+        resource_info:
+            Config info for the destination resource.
         save_params:
             Save configuration info (eg. table name, update mode).
 
     Raises:
-        InvalidIntegrationException:
-            An error occurred because the requested integration could not be
+        InvalidResourceException:
+            An error occurred because the requested resource could not be
             found.
         InvalidUserActionException:
-            An error occurred because you are trying to load non-relational data into a relational integration.
+            An error occurred because you are trying to load non-relational data into a relational resource.
         InvalidUserArgumentException:
             An error occurred because some necessary fields are missing in the SaveParams.
     """
     if not isinstance(artifact_ids, list):
         artifact_ids = [artifact_ids]
 
-    integrations_map = global_api_client.list_resources()
-    if integration_info.name not in integrations_map:
-        raise InvalidIntegrationException(
-            "Not connected to integration %s!" % integration_info.name
-        )
-
-    # We currently do not allow multiple save operators on the same artifact to the same integration.
-    # We do allow multiple artifacts to write to the same integration, as well as a single artifact
-    # to write to multiple integrations.
-    save_op_name = "save to %s" % integration_info.name
+    resources_map = global_api_client.list_resources()
+    if resource_info.name not in resources_map:
+        raise InvalidResourceException("Not connected to resource %s!" % resource_info.name)
+
+    # We currently do not allow multiple save operators on the same artifact to the same resource.
+    # We do allow multiple artifacts to write to the same resource, as well as a single artifact
+    # to write to multiple resources.
+    save_op_name = "save to %s" % resource_info.name
 
-    # Replace any existing save operator on this artifact that goes to the same integration.
+    # Replace any existing save operator on this artifact that goes to the same resource.
     artifact_id_to_save = artifact_ids[-1]
 
     deltas: List[DAGDelta] = []
     existing_save_ops = dag.list_operators(
         filter_to=[OperatorType.LOAD],
         on_artifact_id=artifact_id_to_save,
     )
     for op in existing_save_ops:
         assert op.spec.load is not None
-        if op.spec.load.integration_id == integration_info.id:
+        if op.spec.load.resource_id == resource_info.id:
             deltas.append(RemoveOperatorDelta(op.id))
 
     deltas.append(
         AddOperatorDelta(
             op=Operator(
                 id=generate_uuid(),
                 name=save_op_name,
                 description="",
                 spec=OperatorSpec(
                     load=LoadSpec(
-                        service=integration_info.service,
-                        integration_id=integration_info.id,
+                        service=resource_info.service,
+                        resource_id=resource_info.id,
                         parameters=save_params,
                     )
                 ),
                 inputs=artifact_ids,
             ),
             output_artifacts=[],
         )
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/resources/sql.py` & `aqueduct-sdk-0.3.5/aqueduct/resources/sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.preview import preview_artifact
 from aqueduct.artifacts.table_artifact import TableArtifact
 from aqueduct.constants.enums import ArtifactType, ExecutionMode, LoadUpdateMode, ServiceType
 from aqueduct.error import InvalidUserActionException, InvalidUserArgumentException
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     Operator,
     OperatorSpec,
     RelationalDBExtractParams,
     RelationalDBLoadParams,
 )
+from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.resources.parameters import (
     _validate_artifact_is_string,
     _validate_builtin_expansions,
     _validate_parameters,
 )
 from aqueduct.resources.save import _save_artifact
 from aqueduct.resources.validation import validate_is_connected
@@ -40,32 +40,32 @@
 GET_TABLE_QUERY = "select * from %s"
 LIST_TABLES_QUERY_SQLITE = "SELECT name AS tablename FROM sqlite_master WHERE type='table';"
 LIST_TABLES_QUERY_ATHENA = "AQUEDUCT_ATHENA_LIST_TABLE"
 
 
 class RelationalDBResource(BaseResource):
     """
-    Class for Relational integrations.
+    Class for Relational resources.
     """
 
     def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
     @validate_is_connected()
     def list_tables(self) -> pd.DataFrame:
         """
-        Lists the tables available in the RelationalDB integration.
+        Lists the tables available in the RelationalDB resource.
 
         Returns:
             pd.DataFrame of available tables.
         """
 
         if self.type() in [ServiceType.BIGQUERY, ServiceType.SNOWFLAKE]:
-            # Use the list integration objects endpoint instead of
+            # Use the list resource objects endpoint instead of
             # providing a hardcoded SQL query to execute
             tables = globals.__GLOBAL_API_CLIENT__.list_tables(str(self.id()))
             return pd.DataFrame(tables, columns=["tablename"])
 
         if self.type() in [
             ServiceType.POSTGRES,
             ServiceType.REDSHIFT,
@@ -84,15 +84,15 @@
 
         sql_artifact = self.sql(query=list_tables_query)
         return sql_artifact.get()
 
     @validate_is_connected()
     def table(self, name: str) -> pd.DataFrame:
         """
-        Retrieves a table from a RelationalDB integration.
+        Retrieves a table from a RelationalDB resource.
 
         Args:
             name:
                 The name of the table to retrieve.
 
         Returns:
             pd.DataFrame of the table to retrieve.
@@ -107,15 +107,15 @@
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
         parameters: Optional[List[BaseArtifact]] = None,
         lazy: bool = False,
     ) -> TableArtifact:
         """
-        Runs a SQL query against the RelationalDB integration.
+        Runs a SQL query against the RelationalDB resource.
 
         Args:
             query:
                 The query to run. When a list is provided, we run the list
                 in a chain and return the result of the final query.
             name:
                 Name of the query.
@@ -208,15 +208,15 @@
                     op=Operator(
                         id=sql_operator_id,
                         name=op_name,
                         description=description,
                         spec=OperatorSpec(
                             extract=ExtractSpec(
                                 service=self.type(),
-                                integration_id=self.id(),
+                                resource_id=self.id(),
                                 parameters=extract_params,
                             )
                         ),
                         inputs=sql_input_artifact_ids,
                         outputs=[sql_output_artifact_id],
                     ),
                     output_artifacts=[
@@ -247,15 +247,15 @@
         table_name: Union[str, BaseArtifact],
         update_mode: LoadUpdateMode,
     ) -> None:
         """Registers a save operator of the given artifact, to be executed when it's computed in a published flow.
 
         Args:
             artifact:
-                The artifact to save into this sql integration.
+                The artifact to save into this sql resource.
             table_name:
                 The table to save the artifact to. You can also parameterize this field by passing
                 a string parameter here. When this save is parameterized, the table name parameter
                 will always be ordered before the artifact in the save operator's input list.
             update_mode:
                 Defines the semantics of the save if a table already exists.
                 Options are "replace", "append" (row-wise), or "fail" (if table already exists).
@@ -297,20 +297,20 @@
             self._dag,
             self._metadata,
             save_params=RelationalDBLoadParams(table=table_name_str, update_mode=update_mode),
         )
 
     def describe(self) -> None:
         """
-        Prints out a human-readable description of the SQL integration.
+        Prints out a human-readable description of the SQL resource.
         """
         print("==================== SQL Resource =============================")
         print("Resource Information:")
         self._metadata.describe()
 
-        # Only list the tables if the integration is connected.
+        # Only list the tables if the resource is connected.
         try:
             print("Resource Table List Preview:")
             print(self.list_tables()["name"].head().to_string())
             print("(only first 5 tables are shown)")
         except:
             pass
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/schedule.py` & `aqueduct-sdk-0.3.5/aqueduct/schedule.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/tests/dag_delta_test.py` & `aqueduct-sdk-0.3.5/aqueduct/tests/dag_delta_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/tests/dag_test.py` & `aqueduct-sdk-0.3.5/aqueduct/tests/dag_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/tests/decorator_test.py` & `aqueduct-sdk-0.3.5/aqueduct/tests/decorator_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/tests/decorators_with_without_parentheses_test.py` & `aqueduct-sdk-0.3.5/aqueduct/tests/decorators_with_without_parentheses_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/tests/flow_test.py` & `aqueduct-sdk-0.3.5/aqueduct/tests/flow_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/tests/helpers_test.py` & `aqueduct-sdk-0.3.5/aqueduct/tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/tests/metric_test.py` & `aqueduct-sdk-0.3.5/aqueduct/tests/metric_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/tests/serialization_test.py` & `aqueduct-sdk-0.3.5/aqueduct/tests/serialization_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,37 +165,37 @@
         metadata=Metadata(),
     )
 
 
 def test_extract_serialization():
     op_id = uuid.uuid4()
     other_ids = [uuid.uuid4(), uuid.uuid4()]
-    integration_id = uuid.uuid4()
+    resource_id = uuid.uuid4()
     extract_operator = Operator(
         id=op_id,
         name="Extract Operator",
         description="",
         spec=OperatorSpec(
             extract=ExtractSpec(
                 service=ServiceType.POSTGRES,
-                integration_id=integration_id,
+                resource_id=resource_id,
                 parameters=RelationalDBExtractParams(query="SELECT * FROM hotel_reviews;"),
             ),
         ),
         outputs=[other_ids[1]],
     )
     assert extract_operator.json(exclude_none=True) == json.dumps(
         {
             "id": str(op_id),
             "name": "Extract Operator",
             "description": "",
             "spec": {
                 "extract": {
                     "service": ServiceType.POSTGRES,
-                    "integration_id": str(integration_id),
+                    "resource_id": str(resource_id),
                     "parameters": {
                         "query": "SELECT * FROM hotel_reviews;",
                     },
                 }
             },
             "inputs": [],
             "outputs": [str(other_ids[1])],
@@ -205,15 +205,15 @@
     extract_operator_sf = Operator(
         id=op_id,
         name="Extract Operator Salesforce",
         description="",
         spec=OperatorSpec(
             extract=ExtractSpec(
                 service=ServiceType.SALESFORCE,
-                integration_id=integration_id,
+                resource_id=resource_id,
                 parameters=SalesforceExtractParams(
                     type=SalesforceExtractType.SEARCH, query="FIND joe;"
                 ),
             ),
         ),
         outputs=[other_ids[1]],
     )
@@ -221,15 +221,15 @@
         {
             "id": str(op_id),
             "name": "Extract Operator Salesforce",
             "description": "",
             "spec": {
                 "extract": {
                     "service": ServiceType.SALESFORCE,
-                    "integration_id": str(integration_id),
+                    "resource_id": str(resource_id),
                     "parameters": {
                         "type": "search",
                         "query": "FIND joe;",
                     },
                 }
             },
             "inputs": [],
@@ -240,29 +240,29 @@
     extract_operator_gs = Operator(
         id=op_id,
         name="Extract Operator Google Sheets",
         description="",
         spec=OperatorSpec(
             extract=ExtractSpec(
                 service=ServiceType.GOOGLE_SHEETS,
-                integration_id=integration_id,
+                resource_id=resource_id,
                 parameters=GoogleSheetsExtractParams(spreadsheet_id="0"),
             ),
         ),
         outputs=[other_ids[1]],
     )
     assert extract_operator_gs.json(exclude_none=True) == json.dumps(
         {
             "id": str(op_id),
             "name": "Extract Operator Google Sheets",
             "description": "",
             "spec": {
                 "extract": {
                     "service": ServiceType.GOOGLE_SHEETS,
-                    "integration_id": str(integration_id),
+                    "resource_id": str(resource_id),
                     "parameters": {
                         "spreadsheet_id": "0",
                     },
                 }
             },
             "inputs": [],
             "outputs": [str(other_ids[1])],
@@ -272,15 +272,15 @@
     extract_operator_s3 = Operator(
         id=op_id,
         name="Extract Operator S3",
         description="",
         spec=OperatorSpec(
             extract=ExtractSpec(
                 service=ServiceType.S3,
-                integration_id=integration_id,
+                resource_id=resource_id,
                 parameters=S3ExtractParams(
                     filepath=json.dumps("test.csv"),
                     artifact_type=ArtifactType.TABLE,
                     format=S3TableFormat.CSV,
                 ),
             ),
         ),
@@ -290,15 +290,15 @@
         {
             "id": str(op_id),
             "name": "Extract Operator S3",
             "description": "",
             "spec": {
                 "extract": {
                     "service": ServiceType.S3,
-                    "integration_id": str(integration_id),
+                    "resource_id": str(resource_id),
                     "parameters": {
                         "filepath": json.dumps("test.csv"),
                         "artifact_type": ArtifactType.TABLE,
                         "format": "CSV",
                     },
                 }
             },
@@ -307,23 +307,23 @@
         }
     )
 
 
 def test_load_serialization():
     op_id = uuid.uuid4()
     other_ids = [uuid.uuid4(), uuid.uuid4()]
-    integration_id = uuid.uuid4()
+    resource_id = uuid.uuid4()
     load_operator = Operator(
         id=op_id,
         name="Load Operator",
         description="",
         spec=OperatorSpec(
             load=LoadSpec(
                 service=ServiceType.POSTGRES,
-                integration_id=integration_id,
+                resource_id=resource_id,
                 parameters=RelationalDBLoadParams(
                     table="hotel_reviews", update_mode=LoadUpdateMode.REPLACE
                 ),
             ),
         ),
         inputs=[other_ids[0]],
     )
@@ -331,15 +331,15 @@
         {
             "id": str(op_id),
             "name": "Load Operator",
             "description": "",
             "spec": {
                 "load": {
                     "service": ServiceType.POSTGRES,
-                    "integration_id": str(integration_id),
+                    "resource_id": str(resource_id),
                     "parameters": {
                         "table": "hotel_reviews",
                         "update_mode": "replace",
                     },
                 }
             },
             "inputs": [str(other_ids[0])],
@@ -350,29 +350,29 @@
     load_operator_sf = Operator(
         id=op_id,
         name="Load Operator Salesforce",
         description="",
         spec=OperatorSpec(
             load=LoadSpec(
                 service=ServiceType.SALESFORCE,
-                integration_id=integration_id,
+                resource_id=resource_id,
                 parameters=SalesforceLoadParams(object="hotel_reviews"),
             ),
         ),
         inputs=[other_ids[0]],
     )
     assert load_operator_sf.json(exclude_none=True) == json.dumps(
         {
             "id": str(op_id),
             "name": "Load Operator Salesforce",
             "description": "",
             "spec": {
                 "load": {
                     "service": ServiceType.SALESFORCE,
-                    "integration_id": str(integration_id),
+                    "resource_id": str(resource_id),
                     "parameters": {
                         "object": "hotel_reviews",
                     },
                 }
             },
             "inputs": [str(other_ids[0])],
             "outputs": [],
@@ -382,15 +382,15 @@
     load_operator_gs = Operator(
         id=op_id,
         name="Load Operator Google Sheets",
         description="",
         spec=OperatorSpec(
             load=LoadSpec(
                 service=ServiceType.GOOGLE_SHEETS,
-                integration_id=integration_id,
+                resource_id=resource_id,
                 parameters=GoogleSheetsLoadParams(
                     filepath="test_sheet.csv",
                     save_mode=GoogleSheetsSaveMode.OVERWRITE,
                 ),
             ),
         ),
         inputs=[other_ids[0]],
@@ -399,15 +399,15 @@
         {
             "id": str(op_id),
             "name": "Load Operator Google Sheets",
             "description": "",
             "spec": {
                 "load": {
                     "service": ServiceType.GOOGLE_SHEETS,
-                    "integration_id": str(integration_id),
+                    "resource_id": str(resource_id),
                     "parameters": {
                         "filepath": "test_sheet.csv",
                         "save_mode": "overwrite",
                     },
                 }
             },
             "inputs": [str(other_ids[0])],
@@ -418,15 +418,15 @@
     load_operator_s3 = Operator(
         id=op_id,
         name="Load Operator S3",
         description="",
         spec=OperatorSpec(
             load=LoadSpec(
                 service=ServiceType.S3,
-                integration_id=integration_id,
+                resource_id=resource_id,
                 parameters=S3LoadParams(
                     filepath="test.json",
                     format=S3TableFormat.JSON,
                 ),
             ),
         ),
         inputs=[other_ids[0]],
@@ -435,15 +435,15 @@
         {
             "id": str(op_id),
             "name": "Load Operator S3",
             "description": "",
             "spec": {
                 "load": {
                     "service": ServiceType.S3,
-                    "integration_id": str(integration_id),
+                    "resource_id": str(resource_id),
                     "parameters": {
                         "filepath": "test.json",
                         "format": S3TableFormat.JSON,
                     },
                 }
             },
             "inputs": [str(other_ids[0])],
@@ -454,15 +454,15 @@
     load_operator_s3_without_format = Operator(
         id=op_id,
         name="Load Operator S3",
         description="",
         spec=OperatorSpec(
             load=LoadSpec(
                 service=ServiceType.S3,
-                integration_id=integration_id,
+                resource_id=resource_id,
                 parameters=S3LoadParams(
                     filepath="test.json",
                 ),
             ),
         ),
         inputs=[other_ids[0]],
     )
@@ -470,15 +470,15 @@
         {
             "id": str(op_id),
             "name": "Load Operator S3",
             "description": "",
             "spec": {
                 "load": {
                     "service": ServiceType.S3,
-                    "integration_id": str(integration_id),
+                    "resource_id": str(resource_id),
                     "parameters": {
                         "filepath": "test.json",
                     },
                 }
             },
             "inputs": [str(other_ids[0])],
             "outputs": [],
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/tests/utils.py` & `aqueduct-sdk-0.3.5/aqueduct/tests/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     )
 
 
 def default_extract_spec() -> OperatorSpec:
     return OperatorSpec(
         extract=ExtractSpec(
             service=ServiceType.POSTGRES,
-            integration_id=generate_uuid(),
+            resource_id=generate_uuid(),
             parameters=RelationalDBExtractParams(query="This is a SQL Query"),
         )
     )
 
 
 def default_function_spec() -> OperatorSpec:
     return OperatorSpec(
@@ -123,15 +123,15 @@
     )
 
 
 def default_load_spec() -> OperatorSpec:
     return OperatorSpec(
         load=LoadSpec(
             service=ServiceType.POSTGRES,
-            integration_id=generate_uuid(),
+            resource_id=generate_uuid(),
             parameters=RelationalDBLoadParams(table="output", update_mode=LoadUpdateMode.REPLACE),
         )
     )
 
 
 def default_artifact(id: uuid.UUID, name: str) -> ArtifactMetadata:
     return ArtifactMetadata(id=id, name=name, type=ArtifactType.TABLE, explicitly_named=True)
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/utils/dag_deltas.py` & `aqueduct-sdk-0.3.5/aqueduct/utils/dag_deltas.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/utils/describe.py` & `aqueduct-sdk-0.3.5/aqueduct/utils/describe.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/utils/function_packaging.py` & `aqueduct-sdk-0.3.5/aqueduct/utils/function_packaging.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/utils/integration_validation.py` & `aqueduct-sdk-0.3.5/aqueduct/utils/resource_validation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Optional
 
 from aqueduct.constants.enums import ExecutionStatus
-from aqueduct.error import IntegrationConnectionInProgress, IntegrationFailedToConnect
+from aqueduct.error import ResourceConnectionInProgress, ResourceFailedToConnect
 from aqueduct.models.execution_state import ExecutionState
 
 
-def validate_integration_is_connected(name: str, exec_state: Optional[ExecutionState]) -> None:
-    """Method used to determine if this integration was successfully connected to or not.
+def validate_resource_is_connected(name: str, exec_state: Optional[ExecutionState]) -> None:
+    """Method used to determine if this resource was successfully connected to or not.
     If not successfully connected (or pending), we will raise an Exception.
     """
     # TODO(ENG-2813): Remove the assumption that a missing `exec_state` means success.
     if exec_state is None or exec_state.status == ExecutionStatus.SUCCEEDED:
         return
 
     if exec_state.status == ExecutionStatus.FAILED:
         assert exec_state.error is not None
-        raise IntegrationFailedToConnect(
-            "Cannot use integration %s because it has not been successfully connected to: "
-            "%s\n%s\n\n Please see the /integrations page on the UI for more details."
+        raise ResourceFailedToConnect(
+            "Cannot use resource %s because it has not been successfully connected to: "
+            "%s\n%s\n\n Please see the /resources page on the UI for more details."
             % (
                 name,
                 exec_state.error.tip,
                 exec_state.error.context,
             )
         )
     else:
         # The assumption is that we are in the running state here.
-        raise IntegrationConnectionInProgress(
-            "Cannot use integration %s because it is still in the process of connecting."
-            "Please see the /integrations page on the UI for more details." % name
+        raise ResourceConnectionInProgress(
+            "Cannot use resource %s because it is still in the process of connecting."
+            "Please see the /resources page on the UI for more details." % name
         )
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct/utils/local_data.py` & `aqueduct-sdk-0.3.5/aqueduct/utils/local_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/utils/naming.py` & `aqueduct-sdk-0.3.5/aqueduct/utils/naming.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/utils/serialization.py` & `aqueduct-sdk-0.3.5/aqueduct/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/utils/type_inference.py` & `aqueduct-sdk-0.3.5/aqueduct/utils/type_inference.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.4/aqueduct/utils/utils.py` & `aqueduct-sdk-0.3.5/aqueduct/utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     DatabricksEngineConfig,
     EngineConfig,
     K8sEngineConfig,
     LambdaEngineConfig,
     SparkEngineConfig,
 )
 from aqueduct.models.dag import Schedule
-from aqueduct.models.integration import ResourceInfo
 from aqueduct.models.operators import ParamSpec
+from aqueduct.models.resource import ResourceInfo
 from aqueduct.resources.dynamic_k8s import DynamicK8sResource
-from aqueduct.utils.integration_validation import validate_integration_is_connected
+from aqueduct.utils.resource_validation import validate_resource_is_connected
 from croniter import croniter
 
 from ..models.execution_state import Logs
 from .serialization import artifact_type_to_serialization_type, serialize_val
 from .type_inference import _bytes_to_base64_string
 
 
@@ -38,15 +38,15 @@
 
 
 def generate_uuid() -> uuid.UUID:
     return uuid.uuid4()
 
 
 WORKFLOW_UI_ROUTE_TEMPLATE = "/workflow/%s"
-WORKFLOW_RUN_UI_ROUTE_TEMPLATE = "?workflowDagResultId=%s"
+WORKFLOW_RUN_UI_ROUTE_TEMPLATE = "/result/%s"
 
 
 def generate_ui_url(
     aqueduct_base_address: str, workflow_id: str, result_id: Optional[str] = None
 ) -> str:
     if result_id:
         url = "%s%s%s" % (
@@ -143,73 +143,71 @@
     return ParamSpec(
         val=_bytes_to_base64_string(serialize_val(val, serialization_type, derived_from_bson)),
         serialization_type=serialization_type,
     )
 
 
 def generate_engine_config(
-    integrations: Dict[str, ResourceInfo],
-    integration_name: Optional[Union[str, DynamicK8sResource]],
+    resources: Dict[str, ResourceInfo],
+    resource_name: Optional[Union[str, DynamicK8sResource]],
 ) -> Optional[EngineConfig]:
-    """Generates an EngineConfig from an integration info object.
+    """Generates an EngineConfig from an resource info object.
 
     Both None and "Aqueduct" (case-insensitive) map to the Aqueduct Engine.
     """
-    if isinstance(integration_name, DynamicK8sResource):
-        integration_name = integration_name.name()
+    if isinstance(resource_name, DynamicK8sResource):
+        resource_name = resource_name.name()
 
-    if integration_name is None or integration_name.lower() == "aqueduct":
+    if resource_name is None or resource_name.lower() == "aqueduct":
         return None
 
-    if integration_name not in integrations.keys():
-        raise InvalidIntegrationException(
-            "Not connected to compute integration `%s`!" % integration_name
-        )
+    if resource_name not in resources.keys():
+        raise InvalidResourceException("Not connected to compute resource `%s`!" % resource_name)
 
-    integration = integrations[integration_name]
-    validate_integration_is_connected(integration_name, integration.exec_state)
+    resource = resources[resource_name]
+    validate_resource_is_connected(resource_name, resource.exec_state)
 
-    if integration.service == ServiceType.AIRFLOW:
+    if resource.service == ServiceType.AIRFLOW:
         return EngineConfig(
             type=RuntimeType.AIRFLOW,
-            name=integration_name,
+            name=resource_name,
             airflow_config=AirflowEngineConfig(
-                integration_id=integration.id,
+                resource_id=resource.id,
             ),
         )
-    elif integration.service == ServiceType.K8S:
+    elif resource.service == ServiceType.K8S:
         return EngineConfig(
             type=RuntimeType.K8S,
-            name=integration_name,
+            name=resource_name,
             k8s_config=K8sEngineConfig(
-                integration_id=integration.id,
+                resource_id=resource.id,
             ),
         )
-    elif integration.service == ServiceType.LAMBDA:
+    elif resource.service == ServiceType.LAMBDA:
         return EngineConfig(
             type=RuntimeType.LAMBDA,
-            name=integration_name,
+            name=resource_name,
             lambda_config=LambdaEngineConfig(
-                integration_id=integration.id,
+                resource_id=resource.id,
             ),
         )
-    elif integration.service == ServiceType.DATABRICKS:
+    elif resource.service == ServiceType.DATABRICKS:
         return EngineConfig(
             type=RuntimeType.DATABRICKS,
-            name=integration_name,
+            name=resource_name,
             databricks_config=DatabricksEngineConfig(
-                integration_id=integration.id,
+                resource_id=resource.id,
             ),
         )
-    elif integration.service == ServiceType.SPARK:
+    elif resource.service == ServiceType.SPARK:
         return EngineConfig(
             type=RuntimeType.SPARK,
-            name=integration_name,
+            name=resource_name,
             spark_config=SparkEngineConfig(
-                integration_id=integration.id,
+                resource_id=resource.id,
             ),
         )
     else:
         raise AqueductError("Unsupported engine configuration.")
 
 
 def find_flow_with_user_supplied_id_and_name(
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/PKG-INFO` & `aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/SOURCES.txt` & `aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,27 @@
 aqueduct/globals/dag.py
 aqueduct/models/__init__.py
 aqueduct/models/artifact.py
 aqueduct/models/config.py
 aqueduct/models/dag.py
 aqueduct/models/dag_rules.py
 aqueduct/models/execution_state.py
-aqueduct/models/integration.py
 aqueduct/models/operators.py
+aqueduct/models/resource.py
 aqueduct/models/response_models.py
 aqueduct/models/utils.py
 aqueduct/resources/__init__.py
 aqueduct/resources/airflow.py
 aqueduct/resources/aws.py
 aqueduct/resources/aws_lambda.py
 aqueduct/resources/connect_config.py
 aqueduct/resources/databricks.py
 aqueduct/resources/dynamic_k8s.py
 aqueduct/resources/ecr.py
+aqueduct/resources/gar.py
 aqueduct/resources/google_sheets.py
 aqueduct/resources/k8s.py
 aqueduct/resources/mongodb.py
 aqueduct/resources/parameters.py
 aqueduct/resources/s3.py
 aqueduct/resources/salesforce.py
 aqueduct/resources/save.py
@@ -80,17 +81,17 @@
 aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
 aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
 aqueduct/utils/__init__.py
 aqueduct/utils/dag_deltas.py
 aqueduct/utils/describe.py
 aqueduct/utils/format.py
 aqueduct/utils/function_packaging.py
-aqueduct/utils/integration_validation.py
 aqueduct/utils/local_data.py
 aqueduct/utils/naming.py
+aqueduct/utils/resource_validation.py
 aqueduct/utils/serialization.py
 aqueduct/utils/type_inference.py
 aqueduct/utils/utils.py
 aqueduct_sdk.egg-info/PKG-INFO
 aqueduct_sdk.egg-info/SOURCES.txt
 aqueduct_sdk.egg-info/dependency_links.txt
 aqueduct_sdk.egg-info/requires.txt
```

### Comparing `aqueduct-sdk-0.3.4/setup.py` & `aqueduct-sdk-0.3.5/setup.py`

 * *Files identical despite different names*

