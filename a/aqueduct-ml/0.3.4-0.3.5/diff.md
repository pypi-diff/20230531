# Comparing `tmp/aqueduct-ml-0.3.4.tar.gz` & `tmp/aqueduct-ml-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-ml-0.3.4.tar", last modified: Wed May 24 22:48:45 2023, max compression
+gzip compressed data, was "aqueduct-ml-0.3.5.tar", last modified: Wed May 31 20:27:13 2023, max compression
```

## Comparing `aqueduct-ml-0.3.4.tar` & `aqueduct-ml-0.3.5.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.305711 aqueduct-ml-0.3.4/aqueduct_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.305711 aqueduct-ml-0.3.4/aqueduct_executor/migrators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.309712 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.309712 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.313712 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.313712 aqueduct-ml-0.3.4/aqueduct_executor/operators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.313712 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.313712 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.321711 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/athena.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2892 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/connector.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16614 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5201 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/parameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/relational.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9602 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7001 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.321711 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5478 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.329712 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.329712 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/extract_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1276 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.333711 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.333711 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/execute_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/execute_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.333711 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7531 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/parse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/timer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5795 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/bin/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29429 2023-05-24 22:27:12.000000 aqueduct-ml-0.3.4/bin/aqueduct
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-24 22:27:12.000000 aqueduct-ml-0.3.4/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-24 22:27:12.000000 aqueduct-ml-0.3.4/version
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.521709 aqueduct-ml-0.3.5/aqueduct_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.525709 aqueduct-ml-0.3.5/aqueduct_executor/migrators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.525709 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.525709 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.529709 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.529709 aqueduct-ml-0.3.5/aqueduct_executor/operators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.529709 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.529709 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.537709 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/athena.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2886 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1820 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/connector.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16596 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5201 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/parameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/relational.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9602 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7001 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.537709 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5463 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2725 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.545709 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.545709 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1276 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.549709 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.549709 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/execute_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/execute_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.549709 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      462 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7519 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/execution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/parse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/storage.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/timer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9245 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5795 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/bin/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29947 2023-05-31 18:17:41.000000 aqueduct-ml-0.3.5/bin/aqueduct
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-31 18:17:41.000000 aqueduct-ml-0.3.5/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-31 18:17:41.000000 aqueduct-ml-0.3.5/version
```

### Comparing `aqueduct-ml-0.3.4/PKG-INFO` & `aqueduct-ml-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.4
+Version: 0.3.5
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/execute.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/spec.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/athena.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/bigquery.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/common.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/config.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import Optional, Union
 
 from aqueduct_executor.operators.connectors.data import models
 from aqueduct_executor.operators.utils.enums import MetaEnum
 from pydantic import Field
 
-"""Duplicated at `aqueduct/integrations/connect_config.py` for now, please keep them in sync."""
+"""Duplicated at `aqueduct/resources/connect_config.py` for now, please keep them in sync."""
 
 
 class BigQueryConfig(models.BaseConfig):
     project_id: str
     service_account_credentials: str
 
 
@@ -52,15 +52,15 @@
     config_file_path: str = ""
     config_file_content: str = ""
     config_file_profile: str = ""
 
     bucket: str = ""
     region: str = ""
 
-    # This is unused for data integrations. It is only used for storage.
+    # This is unused for data resources. It is only used for storage.
     root_dir: str = ""
 
     use_as_storage: str = ""
 
 
 class AthenaConfig(models.BaseConfig):
     # default type to ACCESS_KEY mainly for backward compatibility
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/connector.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,28 +35,28 @@
 
     @abstractmethod
     def delete(  # type: ignore
         self,
         # TODO (ENG-1285): Revisit the typing issue that araises from inheritence
         objects,  # List[str]
     ) -> List[SavedObjectDelete]:
-        """Delete objects from integration.
+        """Delete objects from resource.
 
         Args:
-            objects: List of objects to delete from this integration.
+            objects: List of objects to delete from this resource.
         """
 
     @abstractmethod
     def load(  # type: ignore
         self,
         # TODO (ENG-1285): Revisit the typing issue that araises from inheritence
         params,  # load.Params
         data: Any,
         artifact_type: ArtifactType,
     ) -> None:
-        """Loads data into destination storage integration.
+        """Loads data into destination storage resource.
 
         Args:
             params: Load parameters for the connector.
             data: data to load.
             artifact_type: type of the artifact.
         """
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/execute.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,17 +248,17 @@
             **kwargs,
         )
 
 
 def run_delete_saved_objects(spec: Spec, storage: Storage, exec_state: ExecutionState) -> None:
     results = {}
     assert isinstance(spec.connector_name, dict)
-    for integration in spec.connector_name:
-        op = setup_connector(spec.connector_name[integration], spec.connector_config[integration])
-        results[integration] = op.delete(spec.integration_to_object[integration])
+    for resource in spec.connector_name:
+        op = setup_connector(spec.connector_name[resource], spec.connector_config[resource])
+        results[resource] = op.delete(spec.resource_to_object[resource])
     utils.write_delete_saved_objects_results(storage, spec.output_content_path, results)
 
 
 def run_load(
     spec: LoadSpec,
     op: connector.DataConnector,
     storage: Storage,
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/extract.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/gcs.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/load.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/main.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/models.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/mongodb.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/mysql.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/parameters.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/parameters.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/postgres.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/relational.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/s3.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/snowflake.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/s3.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                     "Unable to read in table at path `%s` with S3 file format `%s`."
                     % (key, params.format)
                 )
             else:
                 raise Exception(
                     "Unknown S3 file format `%s` for file at path `%s`." % (params.format, key)
                 )
-        # Non-table artifacts use same serialization as regular S3 integration.
+        # Non-table artifacts use same serialization as regular S3 resource.
         else:
             return self.fetch_object(key, params)
 
     def extract_spark(self, params: extract.S3Params, spark_session_obj: SparkSession) -> Any:
         path = json.loads(params.filepath)
         if not isinstance(path, List):
             if len(path) == 0:
@@ -102,12 +102,12 @@
             elif params.format == common.S3TableFormat.JSON:
                 data.write.json(data_path)
             elif params.format == common.S3TableFormat.PARQUET:
                 data.write.parquet(data_path)
             else:
                 raise Exception("Unknown S3 file format %s." % params.format)
         else:
-            # data is not a Spark DataFrame, use normal S3 integration's load.
+            # data is not a Spark DataFrame, use normal S3 resource's load.
             self.load(params, data, artifact_type)
 
     def unionAll(self, dfs: Any) -> Any:
         return functools.reduce(lambda df1, df2: df1.union(df2.select(df1.columns)), dfs)
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spec.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     if "connector_name" not in values:
         raise ValueError("Unknown connector name.")
 
     if not isinstance(connector_config, dict):
         raise ValueError("connector_config is not a dictionary.")
 
     if type(values["connector_name"]) == dict:
-        for integration in connector_config:
-            if "conf" in connector_config[integration]:
-                connector_config[integration] = connector_config[integration]["conf"]
+        for resource in connector_config:
+            if "conf" in connector_config[resource]:
+                connector_config[resource] = connector_config[resource]["conf"]
 
         return connector_config
     else:
         if "conf" not in connector_config:
             # There is no inner `conf` dictionary to unwrap
             # This occurs when the spec is serialized in Python to run operators
             # on other engines.
@@ -136,15 +136,15 @@
 class DeleteSavedObjectsSpec(models.BaseSpec):
     name: str
     type: Literal[enums.JobType.DELETESAVEDOBJECTS]
     storage_config: sconfig.StorageConfig
     metadata_path: str
     connector_name: Dict[str, common.Name]
     connector_config: Dict[str, config.Config]
-    integration_to_object: Dict[str, List[str]]
+    resource_to_object: Dict[str, List[str]]
     output_content_path: str
 
     # validators
     _unwrap_connector_config = validator("connector_config", allow_reuse=True, pre=True)(
         unwrap_connector_config
     )
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/sql_server.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/sqlite.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/utils.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,12 +65,12 @@
         # Write a temp file
         return _session_from_config_file_content(config)
     elif config.type == AWSCredentialType.CONFIG_FILE_PATH:
         return _session_from_config_file_path(config)
     elif config.type == AWSCredentialType.ACCESS_KEY:
         return _session_from_access_key(config)
     else:
-        raise Exception("Unsupported integration config type: %s" % config.type)
+        raise Exception("Unsupported resource config type: %s" % config.type)
 
 
 def url_encode(value: str) -> str:
     return urllib.parse.quote_plus(value)
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/conf.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/utils.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/execute.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/extract_function.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/get_extract_path.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/install_requirements.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/main.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/set_conda_version.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/spec.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/execute.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/main.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/spec.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/execute_data.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/execute_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/execute_function.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/execute_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/utils.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/execute.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/main.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/spec.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/enums.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/execution.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/execution.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 TIP_OP_EXECUTION = "Error executing operator. Please refer to the stack trace for fix."
 _TIP_CREATE_BUG_REPORT = (
     f"Please create bug report in github: {_GITHUB_ISSUE_LINK} . "
     "We will get back to you as soon as we can."
 )
 TIP_UNKNOWN_ERROR = f"Sorry, we've run into an unexpected error! {_TIP_CREATE_BUG_REPORT}"
 TIP_INTEGRATION_CONNECTION = (
-    "We were unable to connect to this integration. "
-    "If the stack trace is not helpful, please check your credentials or contact your integration's provider."
+    "We were unable to connect to this resource. "
+    "If the stack trace is not helpful, please check your credentials or contact your resource's provider."
 )
 TIP_DEMO_CONNECTION = f"We have trouble connecting to demo DB. {_TIP_CREATE_BUG_REPORT}"
 
 TIP_EXTRACT = "We couldn't execute the provided query. Please double check your query is correct."
-TIP_LOAD = "We couldn't load to the integration. Please make sure the target exists, or you have the right permission."
-TIP_DISCOVER = "We couldn't list items in the integration. Please make sure your credentials have the right permission."
+TIP_LOAD = "We couldn't load to the resource. Please make sure the target exists, or you have the right permission."
+TIP_DISCOVER = "We couldn't list items in the resource. Please make sure your credentials have the right permission."
 
 # Assumption: only check operators will use this tip.
 TIP_CHECK_DID_NOT_PASS = "The check did not pass (returned False)."
 
 TIP_NOT_NUMERIC = "The computed result is not of type numeric."
 TIP_NOT_BOOL = "The computed result is not of type bool."
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/config.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/file.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/gcs.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/parse.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/s3.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/timer.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/utils.py` & `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,19 +194,19 @@
 ) -> None:
     # `[object].json()`` gives me the json as a string which gets escaped in `json.dumps()``.
     # However, I cannot serialize it directly with `json.dumps()`` so I serialize with
     # `[object].json()` then `json.loads()` to convert it to a dictionary that is serializable
     # by `json.dumps.()`.
     results_str = json.dumps(
         {
-            integration: [
+            resource: [
                 {"name": result.name, "exec_state": json.loads(result.exec_state.json())}
-                for result in results[integration]
+                for result in results[resource]
             ]
-            for integration in results
+            for resource in results
         }
     )
     storage.put(path, bytes(results_str, encoding=DEFAULT_ENCODING))
 
 
 def write_discover_results(storage: Storage, path: str, tables: List[str]) -> None:
     table_names_str = json.dumps(tables)
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_ml.egg-info/PKG-INFO` & `aqueduct-ml-0.3.5/aqueduct_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.4
+Version: 0.3.5
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-ml-0.3.4/aqueduct_ml.egg-info/SOURCES.txt` & `aqueduct-ml-0.3.5/aqueduct_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.4/bin/aqueduct` & `aqueduct-ml-0.3.5/bin/aqueduct`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import distro
 import requests
 import yaml
 from packaging.version import parse as parse_version
 from tqdm import tqdm
 
-SCHEMA_VERSION = "26"
+SCHEMA_VERSION = "27"
 CHUNK_SIZE = 4096
 
 # Connector Package Version Bounds
 PYMONGO_VERSION_BOUND = "<=4.3.3"
 PSYCOPG2_VERSION_BOUND = "<=2.9.5"
 BIGQUERY_VERSION_BOUND = "<=3.5.0"
 DB_DTYPES_VERSION_BOUND = "<=1.1.1"
@@ -34,15 +34,15 @@
 MYSQL_CLIENT_VERSION_BOUND = "<=2.1.1"
 PYODBC_VERSION_BOUND = "<=4.0.35"
 
 base_directory = os.path.join(os.environ["HOME"], ".aqueduct")
 server_directory = os.path.join(os.environ["HOME"], ".aqueduct", "server")
 ui_directory = os.path.join(os.environ["HOME"], ".aqueduct", "ui")
 
-package_version = "0.3.4"
+package_version = "0.3.5"
 aws_credentials_path = os.path.join(os.environ["HOME"], ".aws", "credentials")
 
 default_server_port = 8080
 
 s3_server_prefix = (
     "https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/%s/server" % package_version
 )
@@ -188,15 +188,15 @@
     with open(os.path.join(server_directory, "bin/server"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/{architecture}/server"), f, "Server")
     with open(os.path.join(server_directory, "bin/executor"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/{architecture}/executor"), f, "Executor")
     with open(os.path.join(server_directory, "bin/migrator"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/{architecture}/migrator"), f, "Migrator")
 
-    print("Downloading integration set up scripts...")
+    print("Downloading resource set up scripts...")
     with open(os.path.join(server_directory, "bin/start-function-executor.sh"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/start-function-executor.sh"), f)
     with open(os.path.join(server_directory, "bin/dag.template"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/dag.template"), f)
     with open(os.path.join(server_directory, "bin/install_sqlserver_ubuntu.sh"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/install_sqlserver_ubuntu.sh"), f)
     print("Downloaded server binaries...")
@@ -221,21 +221,30 @@
     else:
         raise Exception(
             "Unsupported operating system and architecture combination: %s, %s" % (system, arch)
         )
 
 
 def download_terraform_template():
+    # EKS template
     terraform_folder = os.path.join(server_directory, "template", "aws", "eks")
     terraform_zip_path = os.path.join(terraform_folder, "eks_terraform.zip")
     with open(terraform_zip_path, "wb") as f:
         _download_file(os.path.join(s3_server_prefix, "template", "aws", "eks", "eks_terraform.zip"), f)
     with zipfile.ZipFile(terraform_zip_path, "r") as zip:
         zip.extractall(terraform_folder)
     os.remove(terraform_zip_path)
+    # GKE template
+    terraform_folder = os.path.join(server_directory, "template", "gke")
+    terraform_zip_path = os.path.join(terraform_folder, "gke_terraform.zip")
+    with open(terraform_zip_path, "wb") as f:
+        _download_file(os.path.join(s3_server_prefix, "template", "gke", "gke_terraform.zip"), f)
+    with zipfile.ZipFile(terraform_zip_path, "r") as zip:
+        zip.extractall(terraform_folder)
+    os.remove(terraform_zip_path)
 
 
 def update_ui_version():
     print("Updating UI version to %s..." % package_version)
     try:
         shutil.rmtree(ui_directory, ignore_errors=True)
         os.mkdir(ui_directory)
@@ -341,14 +350,15 @@
         shutil.rmtree(preview_outputs_directory)
     os.mkdir(preview_outputs_directory)
 
     template_directories = [
         os.path.join(server_directory, "template"),
         os.path.join(server_directory, "template", "aws"),
         os.path.join(server_directory, "template", "aws", "eks"),
+        os.path.join(server_directory, "template", "gke"),
     ]
 
     for directory in template_directories:
         if not os.path.isdir(directory):
             os.mkdir(directory)
 
     server_version_file = os.path.join(server_directory, "__version__")
@@ -699,15 +709,15 @@
         "install",
         help="""Install the required library dependencies for
                              an Aqueduct connector to a third-party system.""",
     )
     install_args.add_argument(
         "system",
         nargs=1,
-        help="Supported integrations: postgres, redshift, mysql, mariadb, sqlserver, azuresql, s3, athena, snowflake, bigquery.",
+        help="Supported resources: postgres, redshift, mysql, mariadb, sqlserver, azuresql, s3, athena, snowflake, bigquery.",
     )
 
     apikey_args = subparsers.add_parser(
         "apikey", help="Display your Aqueduct API key.")
     clear_args = subparsers.add_parser(
         "clear", help="Erase your Aqueduct installation.")
     version_args = subparsers.add_parser(
```

### Comparing `aqueduct-ml-0.3.4/setup.py` & `aqueduct-ml-0.3.5/setup.py`

 * *Files identical despite different names*

