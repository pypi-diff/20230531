# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230531161853.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230531170356.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230531161853.tar", last modified: Wed May 31 16:19:34 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230531170356.tar", last modified: Wed May 31 17:04:37 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531161853.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230531170356.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 16:19:34.744202 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-31 16:18:47.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 16:19:34.744202 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-05-31 16:18:47.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 16:19:34.744202 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 16:19:32.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 16:19:34.744202 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 16:19:34.744202 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 16:18:47.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10281 2023-05-31 16:18:47.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-05-31 16:18:47.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 16:19:34.744202 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 16:19:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-31 16:19:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 16:19:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-31 16:19:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-31 16:19:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 17:04:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10281 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531161853/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531161853/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230531161853
+Version: 1.0.0.dev20230531170356
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531161853/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531161853/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230531161853",
+  version="1.0.0.dev20230531170356",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda/lambda_handler.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/lambda_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 When run locally, all boto3.Sessions will need to have a profile enabled.
 To enable the default profile have export AWS_DEFAULT_PROFILE=echofish set in your bashrc
 """
 
 import os
 import json
-from lambda_executor import LambdaExecutor
+from .lambda_executor import LambdaExecutor
 
 index_ek60_table_name = os.environ.get('INDEX_EK60_TABLE_NAME')
 bucket_name = os.environ.get('BUCKET_NAME')
 calibration_bucket = os.environ.get('CALIBRATION_BUCKET')
 calibration_key = os.environ.get('CALIBRATION_KEY')
 
 handler = LambdaExecutor(index_ek60_table_name, bucket_name, calibration_bucket, calibration_key)
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531161853/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230531161853
+Version: 1.0.0.dev20230531170356
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

