# Comparing `tmp/kedro-datasets-1.3.0.tar.gz` & `tmp/kedro-datasets-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-datasets-1.3.0.tar", last modified: Mon May 22 20:35:33 2023, max compression
+gzip compressed data, was "kedro-datasets-1.4.0.tar", last modified: Wed May 31 12:03:29 2023, max compression
```

## Comparing `kedro-datasets-1.3.0.tar` & `kedro-datasets-1.4.0.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/api/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/api/api_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/biosequence/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/biosequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/dask/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/databricks/managed_table_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/email/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/email/message_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/holoviews/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/json/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/json/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/networkx/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/networkx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/networkx/gml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/networkx/graphml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/networkx/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/feather_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/gbq_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/generic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/hdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/sql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/pillow/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pillow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pillow/image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/plotly/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/polars/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/polars/csv_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/redis/redis_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/snowflake/snowpark_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/spark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/spark_jdbc_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/svmlight/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/svmlight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/text/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/text/text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tracking/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/video/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/video/video_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/api/api_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/biosequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/biosequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/databricks/managed_table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/email/message_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/json/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/networkx/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/networkx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/networkx/gml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/networkx/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/feather_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/pillow/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pillow/image_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/plotly/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/polars/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/polars/csv_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/redis/redis_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/snowflake/snowpark_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/spark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/spark_jdbc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/spark_streaming_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/svmlight/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/svmlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/text/text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/kedro_datasets/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tracking/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/kedro_datasets/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/video/video_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/kedro_datasets/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/setup.py
```

### Comparing `kedro-datasets-1.3.0/PKG-INFO` & `kedro-datasets-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.3.0
+Version: 1.4.0
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: api
 Provides-Extra: biosequence
 Provides-Extra: dask
 Provides-Extra: databricks
-Provides-Extra: docs
 Provides-Extra: geopandas
 Provides-Extra: holoviews
 Provides-Extra: matplotlib
 Provides-Extra: networkx
 Provides-Extra: pandas
 Provides-Extra: pillow
 Provides-Extra: plotly
@@ -59,14 +58,15 @@
 Provides-Extra: spark.SparkJDBCDataSet
 Provides-Extra: spark.DeltaTableDataSet
 Provides-Extra: svmlight.SVMLightDataSet
 Provides-Extra: tensorflow.TensorFlowModelDataSet
 Provides-Extra: video.VideoDataSet
 Provides-Extra: yaml.YAMLDataSet
 Provides-Extra: all
+Provides-Extra: docs
 
 # Kedro-Datasets
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-datasets/)
 [![PyPI Version](https://badge.fury.io/py/kedro-datasets.svg)](https://pypi.org/project/kedro-datasets/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
```

### Comparing `kedro-datasets-1.3.0/README.md` & `kedro-datasets-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/api/api_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/api/api_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         >>>         }
         >>>     },
         >>>     credentials=("username", "password")
         >>> )
         >>> data = data_set.load()
 
     ``APIDataSet`` can also be used to save output on a remote server using HTTP(S)
-    methods.
+    methods. ::
 
         >>> example_table = '{"col1":["val1", "val2"], "col2":["val3", "val4"]}'
 
         >>> data_set = APIDataSet(
                 method = "POST",
                 url = "url_of_remote_server",
                 save_args = {"chunk_size":1}
@@ -112,15 +112,15 @@
                 Expected format is ``('login', 'password')`` if given as a tuple or
                 list. An ``AuthBase`` instance can be provided for more complex cases.
             metadata: Any arbitrary metadata.
                 This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             ValueError: if both ``auth`` and ``credentials`` are specified or used
-            unsupported RESTful API method.
+                unsupported RESTful API method.
         """
         super().__init__()
 
         # GET method means load
         if method == "GET":
             self._params = load_args or {}
```

### Comparing `kedro-datasets-1.3.0/kedro_datasets/biosequence/biosequence_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/biosequence/biosequence_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/dask/parquet_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/dask/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/databricks/managed_table_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/databricks/managed_table_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/email/message_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/email/message_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/geopandas/geojson_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/geopandas/geojson_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/holoviews/holoviews_writer.py` & `kedro-datasets-1.4.0/kedro_datasets/holoviews/holoviews_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/json/json_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/json/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/matplotlib/matplotlib_writer.py` & `kedro-datasets-1.4.0/kedro_datasets/matplotlib/matplotlib_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/networkx/gml_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/networkx/gml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/networkx/graphml_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/networkx/graphml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/networkx/json_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/networkx/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/__init__.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/csv_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/excel_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/feather_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/feather_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/gbq_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/gbq_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/generic_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/generic_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/hdf_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/hdf_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/json_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/parquet_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/sql_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/sql_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pandas/xml_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pandas/xml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pickle/pickle_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pickle/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/pillow/image_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/pillow/image_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/plotly/json_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/plotly/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/plotly/plotly_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/plotly/plotly_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/polars/csv_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/polars/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/redis/redis_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/redis/redis_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/snowflake/snowpark_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/snowflake/snowpark_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/spark/deltatable_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/spark/deltatable_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/spark/spark_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/spark/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/spark/spark_hive_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/spark/spark_hive_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/spark/spark_jdbc_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/spark/spark_jdbc_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/svmlight/svmlight_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/svmlight/svmlight_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/text/text_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/text/text_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/tracking/json_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/tracking/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/tracking/metrics_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/tracking/metrics_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/video/video_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/video/video_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets/yaml/yaml_dataset.py` & `kedro-datasets-1.4.0/kedro_datasets/yaml/yaml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/kedro_datasets.egg-info/PKG-INFO` & `kedro-datasets-1.4.0/kedro_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.3.0
+Version: 1.4.0
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: api
 Provides-Extra: biosequence
 Provides-Extra: dask
 Provides-Extra: databricks
-Provides-Extra: docs
 Provides-Extra: geopandas
 Provides-Extra: holoviews
 Provides-Extra: matplotlib
 Provides-Extra: networkx
 Provides-Extra: pandas
 Provides-Extra: pillow
 Provides-Extra: plotly
@@ -59,14 +58,15 @@
 Provides-Extra: spark.SparkJDBCDataSet
 Provides-Extra: spark.DeltaTableDataSet
 Provides-Extra: svmlight.SVMLightDataSet
 Provides-Extra: tensorflow.TensorFlowModelDataSet
 Provides-Extra: video.VideoDataSet
 Provides-Extra: yaml.YAMLDataSet
 Provides-Extra: all
+Provides-Extra: docs
 
 # Kedro-Datasets
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-datasets/)
 [![PyPI Version](https://badge.fury.io/py/kedro-datasets.svg)](https://pypi.org/project/kedro-datasets/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
```

### Comparing `kedro-datasets-1.3.0/kedro_datasets.egg-info/SOURCES.txt` & `kedro-datasets-1.4.0/kedro_datasets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 kedro_datasets/snowflake/__init__.py
 kedro_datasets/snowflake/snowpark_dataset.py
 kedro_datasets/spark/__init__.py
 kedro_datasets/spark/deltatable_dataset.py
 kedro_datasets/spark/spark_dataset.py
 kedro_datasets/spark/spark_hive_dataset.py
 kedro_datasets/spark/spark_jdbc_dataset.py
+kedro_datasets/spark/spark_streaming_dataset.py
 kedro_datasets/svmlight/__init__.py
 kedro_datasets/svmlight/svmlight_dataset.py
 kedro_datasets/tensorflow/__init__.py
 kedro_datasets/tensorflow/tensorflow_model_dataset.py
 kedro_datasets/text/__init__.py
 kedro_datasets/text/text_dataset.py
 kedro_datasets/tracking/__init__.py
```

### Comparing `kedro-datasets-1.3.0/kedro_datasets.egg-info/requires.txt` & `kedro-datasets-1.4.0/kedro_datasets.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,19 @@
 Pillow~=9.0
 PyYAML<7.0,>=4.2
 SQLAlchemy<3.0,>=1.4
 biopython~=1.73
 dask[complete]~=2021.10
 delta-spark<3.0,>=1.0
 delta-spark~=1.2.1
-docutils==0.16
 geopandas<1.0,>=0.6.0
 hdfs<3.0,>=2.5.8
 holoviews~=1.13.0
-ipykernel<7.0,>=5.3
 lxml~=4.6
 matplotlib<4.0,>=3.0.3
-myst-parser~=0.17.2
-nbsphinx==0.8.1
-nbstripout~=0.4
 networkx~=2.4
 opencv-python~=4.5.5.64
 openpyxl<4.0,>=3.0.6
 pandas-gbq<0.18.0,>=0.12.0
 pandas<3.0,>=1.3
 plotly<6.0,>=4.8.0
 polars~=0.17.0
@@ -32,18 +27,14 @@
 pyspark<4.0,>=2.2
 redis~=4.1
 requests~=2.20
 s3fs<0.5,>=0.3.0
 scikit-learn~=1.0.2
 scipy~=1.7.3
 snowflake-snowpark-python~=1.0.0
-sphinx-autodoc-typehints==1.11.1
-sphinx_copybutton==0.3.1
-sphinx_rtd_theme==0.4.1
-sphinx~=3.4.3
 triad<1.0,>=0.6.7
 
 [all:platform_system != "Darwin" or platform_machine != "arm64"]
 tensorflow~=2.0
 
 [all:platform_system != "Windows"]
 tables~=3.6
```

### Comparing `kedro-datasets-1.3.0/pyproject.toml` & `kedro-datasets-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.3.0/setup.py` & `kedro-datasets-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,23 @@
     "pandas.GenericDataSet": [PANDAS],
 }
 pillow_require = {"pillow.ImageDataSet": ["Pillow~=9.0"]}
 plotly_require = {
     "plotly.PlotlyDataSet": [PANDAS, "plotly>=4.8.0, <6.0"],
     "plotly.JSONDataSet": ["plotly>=4.8.0, <6.0"],
 }
-polars_require = {"polars.CSVDataSet": [POLARS],}
+polars_require = {
+    "polars.CSVDataSet": [POLARS]
+}
 redis_require = {"redis.PickleDataSet": ["redis~=4.1"]}
 snowflake_require = {
-    "snowflake.SnowparkTableDataSet": ["snowflake-snowpark-python~=1.0.0", "pyarrow~=8.0"]
+    "snowflake.SnowparkTableDataSet": [
+        "snowflake-snowpark-python~=1.0.0",
+        "pyarrow~=8.0",
+    ]
 }
 spark_require = {
     "spark.SparkDataSet": [SPARK, HDFS, S3FS],
     "spark.SparkHiveDataSet": [SPARK, HDFS, S3FS],
     "spark.SparkJDBCDataSet": [SPARK, HDFS, S3FS],
     "spark.DeltaTableDataSet": [SPARK, HDFS, S3FS, "delta-spark>=1.0, <3.0"],
 }
@@ -67,35 +72,22 @@
         # currently only TensorFlow V2 supported for saving and loading.
         # V1 requires HDF5 and serialises differently
         "tensorflow~=2.0; platform_system != 'Darwin' or platform_machine != 'arm64'",
         # https://developer.apple.com/metal/tensorflow-plugin/
         "tensorflow-macos~=2.0; platform_system == 'Darwin' and platform_machine == 'arm64'",
     ]
 }
-video_require = {
-    "video.VideoDataSet": ["opencv-python~=4.5.5.64"]
-}
+video_require = {"video.VideoDataSet": ["opencv-python~=4.5.5.64"]}
 yaml_require = {"yaml.YAMLDataSet": [PANDAS, "PyYAML>=4.2, <7.0"]}
 
 extras_require = {
     "api": _collect_requirements(api_require),
     "biosequence": _collect_requirements(biosequence_require),
     "dask": _collect_requirements(dask_require),
     "databricks": _collect_requirements(databricks_require),
-    "docs": [
-        "docutils==0.16",
-        "sphinx~=3.4.3",
-        "sphinx_rtd_theme==0.4.1",
-        "nbsphinx==0.8.1",
-        "nbstripout~=0.4",
-        "sphinx-autodoc-typehints==1.11.1",
-        "sphinx_copybutton==0.3.1",
-        "ipykernel>=5.3, <7.0",
-        "myst-parser~=0.17.2",
-    ],
     "geopandas": _collect_requirements(geopandas_require),
     "holoviews": _collect_requirements(holoviews_require),
     "matplotlib": _collect_requirements(matplotlib_require),
     "networkx": _collect_requirements(networkx_require),
     "pandas": _collect_requirements(pandas_require),
     "pillow": _collect_requirements(pillow_require),
     "plotly": _collect_requirements(plotly_require),
@@ -124,11 +116,22 @@
     **svmlight_require,
     **tensorflow_require,
     **video_require,
     **yaml_require,
 }
 
 extras_require["all"] = _collect_requirements(extras_require)
+extras_require["docs"] = [
+    "docutils==0.16",
+    "sphinx~=3.4.3",
+    "sphinx_rtd_theme==0.4.1",
+    "nbsphinx==0.8.1",
+    "nbstripout~=0.4",
+    "sphinx-autodoc-typehints==1.11.1",
+    "sphinx_copybutton==0.3.1",
+    "ipykernel>=5.3, <7.0",
+    "myst-parser~=0.17.2",
+]
 
 setup(
     extras_require=extras_require,
 )
```

