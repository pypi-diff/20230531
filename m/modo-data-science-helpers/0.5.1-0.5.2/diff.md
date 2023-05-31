# Comparing `tmp/modo_data_science_helpers-0.5.1.tar.gz` & `tmp/modo_data_science_helpers-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modo_data_science_helpers-0.5.1.tar", max compression
+gzip compressed data, was "modo_data_science_helpers-0.5.2.tar", max compression
```

## Comparing `modo_data_science_helpers-0.5.1.tar` & `modo_data_science_helpers-0.5.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1582 2023-05-31 14:47:34.172075 modo_data_science_helpers-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-05-12 10:39:55.207198 modo_data_science_helpers-0.5.1/modo_data_science_helpers/__init__.py
--rw-r--r--   0        0        0     4346 2023-05-31 14:47:50.212270 modo_data_science_helpers-0.5.1/modo_data_science_helpers/aws_utils.py
--rw-r--r--   0        0        0      457 2023-05-31 14:59:45.747331 modo_data_science_helpers-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 modo_data_science_helpers-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1582 2023-05-31 14:47:34.172075 modo_data_science_helpers-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 10:39:55.207198 modo_data_science_helpers-0.5.2/modo_data_science_helpers/__init__.py
+-rw-r--r--   0        0        0     4273 2023-05-31 15:06:59.064815 modo_data_science_helpers-0.5.2/modo_data_science_helpers/aws_utils.py
+-rw-r--r--   0        0        0      457 2023-05-31 15:07:34.850225 modo_data_science_helpers-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 modo_data_science_helpers-0.5.2/PKG-INFO
```

### Comparing `modo_data_science_helpers-0.5.1/README.md` & `modo_data_science_helpers-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `modo_data_science_helpers-0.5.1/modo_data_science_helpers/aws_utils.py` & `modo_data_science_helpers-0.5.2/modo_data_science_helpers/aws_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import clipboard
 import re
 import boto3
 import awswrangler as wr
 import pandas as pd
 from io import BytesIO
 
-
 class AWSHandler:
     def __init__(self, profile_name='default', region_name='us-east-1', use_sagemaker_role=False):
-        self.use_sagemaker_role = use_sagemaker_role
-        
-        if not self.use_sagemaker_role:
-            self.parse_clipboard_credentials()
-        
-        self.session = boto3.session.Session(
-            aws_access_key_id=self.aws_access_key_id if not self.use_sagemaker_role else None,
-            aws_secret_access_key=self.aws_secret_access_key if not self.use_sagemaker_role else None,
-            aws_session_token=self.aws_session_token if not self.use_sagemaker_role else None,
-            region_name=region_name
-        )       
-        
-        self.glue_client = self.session.client("glue", region_name=region_name)        
-        self.s3 = self.session.client('s3')
-        
-        print(f"Successfully initialized credentials for {self.profile_name.split('_')[1]}")
+        if use_sagemaker_role:
+            self.session = boto3.session.Session()
+        else:
+            self.parse_clipboard_credentials()            
+            self.session = boto3.session.Session(
+                aws_access_key_id=self.aws_access_key_id,
+                aws_secret_access_key=self.aws_secret_access_key,
+                aws_session_token=self.aws_session_token,
+                region_name=region_name
+            )                   
+            self.glue_client = self.session.client("glue", region_name=region_name)        
+            self.s3 = self.session.client('s3')
+            
+            print(f"Successfully initialized credentials for {self.profile_name.split('_')[1]}")
         
     def parse_clipboard_credentials(self):
         content = clipboard.paste()
         pattern = r'\[(.+)\]\naws_access_key_id=(.+)\naws_secret_access_key=(.+)\naws_session_token=(.+)'
         match = re.search(pattern, content)
 
         if match:
@@ -36,16 +33,15 @@
             self.aws_secret_access_key = match.group(3)
             self.aws_session_token = match.group(4)
 
             # Clear the clipboard after parsing the credentials
             clipboard.copy('')
         else:
             raise ValueError("No AWS credentials found in the clipboard.")
-
-
+            
     def query(self, sql: str, database: str):
         return wr.athena.read_sql_query(sql=sql, database=database, boto3_session=self.session)
 
     def list_tables(self, database: str) -> dict:
         tables = []
         views = []
```

### Comparing `modo_data_science_helpers-0.5.1/PKG-INFO` & `modo_data_science_helpers-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modo-data-science-helpers
-Version: 0.5.1
+Version: 0.5.2
 Summary: Helpers for AWS most common operations. Includes clipboard auth
 Author: Esteban Elia
 Author-email: esteban.elia@modo.com.ar
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

