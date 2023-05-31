# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230531170356.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230531171908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230531170356.tar", last modified: Wed May 31 17:04:37 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230531171908.tar", last modified: Wed May 31 17:19:48 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531170356.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230531171908.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 17:04:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10281 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-05-31 17:03:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:04:37.217104 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-31 17:04:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:19:48.854473 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-31 17:19:02.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 17:19:48.854473 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-05-31 17:19:02.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 17:19:48.854473 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 17:19:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:19:48.850473 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:19:48.854473 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 17:19:02.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10281 2023-05-31 17:19:02.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-31 17:19:02.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:19:48.854473 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 17:19:48.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-31 17:19:48.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 17:19:48.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-31 17:19:48.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-31 17:19:48.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230531171908/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230531171908/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230531170356
+Version: 1.0.0.dev20230531171908
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230531171908/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230531171908/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230531170356",
+  version="1.0.0.dev20230531171908",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda/lambda_handler.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda/lambda_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 
 handler = LambdaExecutor(index_ek60_table_name, bucket_name, calibration_bucket, calibration_key)
 
 
 def handler(sqs_event, context):
     print("Event : " + str(sqs_event))
     print("Context : " + str(context))
-    for record in sqs_event.Records:
-        message = json.loads(record.Body)
+    for record in sqs_event['Records']:
+        message = json.loads(record['body'])
         print("Start Message : " + str(message))
         handler.execute(message)
         print("Done Message : " + str(message))
     print("Done Event : " + str(sqs_event))
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531170356/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230531171908/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230531170356
+Version: 1.0.0.dev20230531171908
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

