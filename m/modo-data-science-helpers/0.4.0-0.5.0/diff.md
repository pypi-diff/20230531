# Comparing `tmp/modo_data_science_helpers-0.4.0.tar.gz` & `tmp/modo_data_science_helpers-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modo_data_science_helpers-0.4.0.tar", max compression
+gzip compressed data, was "modo_data_science_helpers-0.5.0.tar", max compression
```

## Comparing `modo_data_science_helpers-0.4.0.tar` & `modo_data_science_helpers-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1494 2023-05-12 11:08:38.864353 modo_data_science_helpers-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-12 10:39:55.207198 modo_data_science_helpers-0.4.0/modo_data_science_helpers/__init__.py
--rw-r--r--   0        0        0     4101 2023-05-12 14:52:45.858633 modo_data_science_helpers-0.4.0/modo_data_science_helpers/aws_utils.py
--rw-r--r--   0        0        0      456 2023-05-31 14:33:42.578957 modo_data_science_helpers-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 modo_data_science_helpers-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1582 2023-05-31 14:47:34.172075 modo_data_science_helpers-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 10:39:55.207198 modo_data_science_helpers-0.5.0/modo_data_science_helpers/__init__.py
+-rw-r--r--   0        0        0     4346 2023-05-31 14:47:50.212270 modo_data_science_helpers-0.5.0/modo_data_science_helpers/aws_utils.py
+-rw-r--r--   0        0        0      456 2023-05-31 14:53:38.862670 modo_data_science_helpers-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2366 1970-01-01 00:00:00.000000 modo_data_science_helpers-0.5.0/PKG-INFO
```

### Comparing `modo_data_science_helpers-0.4.0/README.md` & `modo_data_science_helpers-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# AWSHandler
+# MODO Data Science Helpers
+
+## AWS utils
+## AWSHandler
 
 AWSHandler es un wrapper para funcionalidades de aws. Autentica automaticamente tomando las credenciales desde el clipboard (solo tienen que copiarlas desde Get credentials --> Command Line or Programatic Access --> Copy Credentials) y luego borra el clipboard
 
 ## Instalacion (local)
 
 ```python
-!pip install -e .
+!pip install modo-data-science-helpers
 ```
 
 ## Ejemplo de uso
 
 ```python
-from aws_handler import AWSHandler
+from modo-data-science-helpers.aws_utils import AWSHandler
 
 # Crear una instancia de AWSHandler (las credenciales se obtendrán del portapapeles, copiarlas desde Command Line or Programatic Access)
 aws_handler = AWSHandler()
 ```
 ### Consultar datos usando Athena
 ```python
 sql = "SELECT * FROM mi_base_de_datos.mi_tabla LIMIT 10"
```

### Comparing `modo_data_science_helpers-0.4.0/modo_data_science_helpers/aws_utils.py` & `modo_data_science_helpers-0.5.0/modo_data_science_helpers/aws_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import clipboard
 import re
 import boto3
 import awswrangler as wr
 import pandas as pd
 from io import BytesIO
 
+
 class AWSHandler:
-    def __init__(self, profile_name='default', region_name='us-east-1'):
-        self.parse_clipboard_credentials()
+    def __init__(self, profile_name='default', region_name='us-east-1', use_sagemaker_role=False):
+        self.use_sagemaker_role = use_sagemaker_role
+        
+        if not self.use_sagemaker_role:
+            self.parse_clipboard_credentials()
         
         self.session = boto3.session.Session(
-            aws_access_key_id=self.aws_access_key_id,
-            aws_secret_access_key=self.aws_secret_access_key,
-            aws_session_token=self.aws_session_token,
+            aws_access_key_id=self.aws_access_key_id if not self.use_sagemaker_role else None,
+            aws_secret_access_key=self.aws_secret_access_key if not self.use_sagemaker_role else None,
+            aws_session_token=self.aws_session_token if not self.use_sagemaker_role else None,
             region_name=region_name
         )       
         
         self.glue_client = self.session.client("glue", region_name=region_name)        
         self.s3 = self.session.client('s3')
         
         print(f"Successfully initialized credentials for {self.profile_name.split('_')[1]}")
@@ -32,15 +36,16 @@
             self.aws_secret_access_key = match.group(3)
             self.aws_session_token = match.group(4)
 
             # Clear the clipboard after parsing the credentials
             clipboard.copy('')
         else:
             raise ValueError("No AWS credentials found in the clipboard.")
-            
+
+
     def query(self, sql: str, database: str):
         return wr.athena.read_sql_query(sql=sql, database=database, boto3_session=self.session)
 
     def list_tables(self, database: str) -> dict:
         tables = []
         views = []
```

### Comparing `modo_data_science_helpers-0.4.0/PKG-INFO` & `modo_data_science_helpers-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: modo-data-science-helpers
-Version: 0.4.0
+Version: 0.5.0
 Summary: Helpers for AWS most common operations. Includes clipboard auth
 Author: Esteban Elia
 Author-email: esteban.elia@modo.com.ar
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: awswrangler (>=2.20.1,<3.0.0)
+Requires-Dist: awswrangler (>=3.1.1,<4.0.0)
 Requires-Dist: boto3 (>=1.26.111,<2.0.0)
 Requires-Dist: clipboard (>=0.0.4,<0.0.5)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: regex (>=2022.10.31,<2023.0.0)
 Description-Content-Type: text/markdown
 
-# AWSHandler
+# MODO Data Science Helpers
+
+## AWS utils
+## AWSHandler
 
 AWSHandler es un wrapper para funcionalidades de aws. Autentica automaticamente tomando las credenciales desde el clipboard (solo tienen que copiarlas desde Get credentials --> Command Line or Programatic Access --> Copy Credentials) y luego borra el clipboard
 
 ## Instalacion (local)
 
 ```python
-!pip install -e .
+!pip install modo-data-science-helpers
 ```
 
 ## Ejemplo de uso
 
 ```python
-from aws_handler import AWSHandler
+from modo-data-science-helpers.aws_utils import AWSHandler
 
 # Crear una instancia de AWSHandler (las credenciales se obtendrán del portapapeles, copiarlas desde Command Line or Programatic Access)
 aws_handler = AWSHandler()
 ```
 ### Consultar datos usando Athena
 ```python
 sql = "SELECT * FROM mi_base_de_datos.mi_tabla LIMIT 10"
```

