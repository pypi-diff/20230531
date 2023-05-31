# Comparing `tmp/h2o_mlops_scoring_client-0.0.7b1-py3-none-any.whl.zip` & `tmp/h2o_mlops_scoring_client-0.0.8b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8741 bytes, number of entries: 8
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 18:14 h2o_mlops_scoring_client/VERSION
--rw-r--r--  2.0 unx     9746 b- defN 23-May-18 21:02 h2o_mlops_scoring_client/__init__.py
+Zip file size: 8752 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        8 b- defN 23-May-31 16:47 h2o_mlops_scoring_client/VERSION
+-rw-r--r--  2.0 unx     9820 b- defN 23-May-31 16:46 h2o_mlops_scoring_client/__init__.py
 -rw-r--r--  2.0 unx    14230 b- defN 23-May-18 21:02 h2o_mlops_scoring_client/_utils.py
 -rw-r--r--  2.0 unx      228 b- defN 23-May-18 21:02 h2o_mlops_scoring_client/_version.py
--rw-r--r--  2.0 unx     3032 b- defN 23-May-22 18:14 h2o_mlops_scoring_client-0.0.7b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 18:14 h2o_mlops_scoring_client-0.0.7b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 18:14 h2o_mlops_scoring_client-0.0.7b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      737 b- defN 23-May-22 18:14 h2o_mlops_scoring_client-0.0.7b1.dist-info/RECORD
-8 files, 28098 bytes uncompressed, 7427 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx     3044 b- defN 23-May-31 16:47 h2o_mlops_scoring_client-0.0.8b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 16:47 h2o_mlops_scoring_client-0.0.8b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-May-31 16:47 h2o_mlops_scoring_client-0.0.8b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      737 b- defN 23-May-31 16:47 h2o_mlops_scoring_client-0.0.8b1.dist-info/RECORD
+8 files, 28184 bytes uncompressed, 7438 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: h2o_mlops_scoring_client/_utils.py
 Comment: 
 
 Filename: h2o_mlops_scoring_client/_version.py
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.7b1.dist-info/METADATA
+Filename: h2o_mlops_scoring_client-0.0.8b1.dist-info/METADATA
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.7b1.dist-info/WHEEL
+Filename: h2o_mlops_scoring_client-0.0.8b1.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.7b1.dist-info/top_level.txt
+Filename: h2o_mlops_scoring_client-0.0.8b1.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.7b1.dist-info/RECORD
+Filename: h2o_mlops_scoring_client-0.0.8b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_mlops_scoring_client/VERSION

```diff
@@ -1 +1 @@
-0.0.7b1
+0.0.8b1
```

## h2o_mlops_scoring_client/__init__.py

```diff
@@ -98,15 +98,15 @@
             after scoring
         mini_batch_size: number of rows per scorer call
         spark_config_overrides: pass Spark configuration options to the Spark context
     """
     try:
         start = _datetime.datetime.now().replace(microsecond=0)
 
-        if spark_conf_dir:
+        if spark_master.startswith("local") and spark_conf_dir:
             _utils.preflight(spark_conf_dir)
             _os.environ["SPARK_CONF_DIR"] = _os.path.abspath(spark_conf_dir)
 
         logger.info("Starting Spark context")
         spark = _utils.get_spark_session(
             app_name="h2o_mlops_scoring_client",
             master=spark_master,
@@ -222,15 +222,15 @@
     mini_batch_size: int = 1000,
     passphrase: _typing.Optional[str] = None,
     spark_config_overrides: _typing.Optional[_typing.Dict[str, str]] = None,
 ) -> _pandas.DataFrame:
     try:
         start = _datetime.datetime.now().replace(microsecond=0)
 
-        if spark_conf_dir:
+        if spark_master.startswith("local") and spark_conf_dir:
             _utils.preflight(spark_conf_dir)
             _os.environ["SPARK_CONF_DIR"] = _os.path.abspath(spark_conf_dir)
 
         logger.info("Starting Spark context")
         spark = _utils.get_spark_session(
             app_name="h2o_mlops_scoring_client",
             master=spark_master,
```

## Comparing `h2o_mlops_scoring_client-0.0.7b1.dist-info/METADATA` & `h2o_mlops_scoring_client-0.0.8b1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-mlops-scoring-client
-Version: 0.0.7b1
+Version: 0.0.8b1
 Summary: A Python client library to simplify robust mini-batch scoring against an H2O MLOps scoring endpoint.
 Author: H2O.ai
 Author-email: support@h2o.ai
 License: Proprietary License
 Project-URL: Documentation, https://docs.h2o.ai/mlops/mlops-scoring-client/overview
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
@@ -73,14 +73,15 @@
 The MLOps scoring client can support many source/sinks, including:
 
 - ADLS Gen 2
 - Databases with a JDBC driver
 - Local file system
 - GBQ
 - S3
+- Snowflake
 
 ### What file types are supported?
 
 The MLOps scoring client can read and write:
 
 - CSV
 - Parquet
```

