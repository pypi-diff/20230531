# Comparing `tmp/custom-utils-0.0.312.tar.gz` & `tmp/custom-utils-0.0.313.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-utils-0.0.312.tar", last modified: Sun May 28 18:40:59 2023, max compression
+gzip compressed data, was "custom-utils-0.0.313.tar", last modified: Wed May 31 11:30:04 2023, max compression
```

## Comparing `custom-utils-0.0.312.tar` & `custom-utils-0.0.313.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 18:40:59.932113 custom-utils-0.0.312/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2023-05-18 07:57:45.000000 custom-utils-0.0.312/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16421 2023-05-28 18:40:59.932113 custom-utils-0.0.312/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15790 2023-05-28 13:00:24.000000 custom-utils-0.0.312/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 18:40:59.924112 custom-utils-0.0.312/custom_utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-05-18 07:57:45.000000 custom-utils-0.0.312/custom_utils/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 18:40:59.928113 custom-utils-0.0.312/custom_utils/alerter/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.312/custom_utils/alerter/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1258 2023-05-27 14:34:54.000000 custom-utils-0.0.312/custom_utils/alerter/slack.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-05-18 07:57:45.000000 custom-utils-0.0.312/custom_utils/config.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 18:40:59.928113 custom-utils-0.0.312/custom_utils/configurer/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.312/custom_utils/configurer/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2138 2023-05-18 07:57:45.000000 custom-utils-0.0.312/custom_utils/configurer/profiler.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2473 2023-05-18 07:57:45.000000 custom-utils-0.0.312/custom_utils/configurer/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 18:40:59.932113 custom-utils-0.0.312/custom_utils/connector/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.312/custom_utils/connector/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7285 2023-05-18 07:57:45.000000 custom-utils-0.0.312/custom_utils/connector/bigquery.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8750 2023-05-18 07:57:45.000000 custom-utils-0.0.312/custom_utils/connector/mongodb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2382 2023-05-28 18:40:44.000000 custom-utils-0.0.312/custom_utils/connector/mysql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4066 2023-05-27 13:15:15.000000 custom-utils-0.0.312/custom_utils/connector/s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1017 2023-05-27 10:52:53.000000 custom-utils-0.0.312/custom_utils/exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      568 2023-05-27 12:41:24.000000 custom-utils-0.0.312/custom_utils/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 18:40:59.928113 custom-utils-0.0.312/custom_utils.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16421 2023-05-28 18:40:59.000000 custom-utils-0.0.312/custom_utils.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2023-05-28 18:40:59.000000 custom-utils-0.0.312/custom_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-28 18:40:59.000000 custom-utils-0.0.312/custom_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      386 2023-05-28 18:40:59.000000 custom-utils-0.0.312/custom_utils.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-28 18:40:59.000000 custom-utils-0.0.312/custom_utils.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-28 18:40:59.932113 custom-utils-0.0.312/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1327 2023-05-28 18:40:56.000000 custom-utils-0.0.312/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-31 11:30:04.458515 custom-utils-0.0.313/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2023-05-18 07:57:45.000000 custom-utils-0.0.313/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16627 2023-05-31 11:30:04.458515 custom-utils-0.0.313/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15996 2023-05-29 14:02:00.000000 custom-utils-0.0.313/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-31 11:30:04.434515 custom-utils-0.0.313/custom_utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-05-18 07:57:45.000000 custom-utils-0.0.313/custom_utils/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-31 11:30:04.442515 custom-utils-0.0.313/custom_utils/alerter/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.313/custom_utils/alerter/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1235 2023-05-31 11:29:30.000000 custom-utils-0.0.313/custom_utils/alerter/slack.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-05-18 07:57:45.000000 custom-utils-0.0.313/custom_utils/config.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-31 11:30:04.446515 custom-utils-0.0.313/custom_utils/configurer/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.313/custom_utils/configurer/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2138 2023-05-18 07:57:45.000000 custom-utils-0.0.313/custom_utils/configurer/profiler.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2473 2023-05-18 07:57:45.000000 custom-utils-0.0.313/custom_utils/configurer/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-31 11:30:04.454515 custom-utils-0.0.313/custom_utils/connector/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.313/custom_utils/connector/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7285 2023-05-18 07:57:45.000000 custom-utils-0.0.313/custom_utils/connector/bigquery.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8750 2023-05-18 07:57:45.000000 custom-utils-0.0.313/custom_utils/connector/mongodb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2382 2023-05-28 18:40:44.000000 custom-utils-0.0.313/custom_utils/connector/mysql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4066 2023-05-27 13:15:15.000000 custom-utils-0.0.313/custom_utils/connector/s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1017 2023-05-27 10:52:53.000000 custom-utils-0.0.313/custom_utils/exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      568 2023-05-27 12:41:24.000000 custom-utils-0.0.313/custom_utils/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-31 11:30:04.442515 custom-utils-0.0.313/custom_utils.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16627 2023-05-31 11:30:04.000000 custom-utils-0.0.313/custom_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2023-05-31 11:30:04.000000 custom-utils-0.0.313/custom_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-31 11:30:04.000000 custom-utils-0.0.313/custom_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      386 2023-05-31 11:30:04.000000 custom-utils-0.0.313/custom_utils.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-31 11:30:04.000000 custom-utils-0.0.313/custom_utils.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-31 11:30:04.458515 custom-utils-0.0.313/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1327 2023-05-29 13:42:58.000000 custom-utils-0.0.313/setup.py
```

### Comparing `custom-utils-0.0.312/LICENSE` & `custom-utils-0.0.313/LICENSE`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/PKG-INFO` & `custom-utils-0.0.313/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-utils
-Version: 0.0.312
+Version: 0.0.313
 Summary: Utilities for database connectors, slack alerter, loggers etc
 Home-page: https://github.com/RahulnKumar/custom-utils
 Author: Rahul Kumar
 Author-email: rahulnkumar7@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -83,19 +83,25 @@
 
 ## Setup Credentials from pip package
 from custom_utils.configurer.utils import Credential
 Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********")
 
 
 from custom_utils.connector.s3 import S3
+# Upload python object to S3
+S3.push_python_object(python_object, s3_uri)
 
-# Uplaoding data to S3
+# Pull python object from S3
+obj = S3.pull_python_object(s3_uri)
+
+# AWS CLI setup is must to use the following methods 
+# Uplaoding local data to S3
 S3.push_local_data(file_path, s3_uri)
-                             
-# Doownlaoding data from S3
+                                
+# Downloading data from S3
 S3.pull_s3_data(file_path, s3_uri)
 ```
 
 **S3 Connector Documentation**
     
 ```
 class S3(builtins.object)
@@ -435,15 +441,15 @@
     
     
 **Code Snippet Sample :**
 ```python3
 from custom_utils.alerter.slack import Slack
 slack = Slack(token=SLACK_BOT_TOKEN) # OR Slack() with  SLACK_BOT_TOKEN as env variable
 channel="#shield"
-message = "testing"
+message = "testing"    
 uids = ["U03PAP8C1RC", "U03PAP8C1RC"]
 slack.send_alert(channel, message, uids)
 ```
     
 **Alerter Documentation :**
 ```python
 class Slack(builtins.object)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.312 Summary: Utilities
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.313 Summary: Utilities
 for database connectors, slack alerter, loggers etc Home-page: https://
 github.com/RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
 rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown Provides-Extra: slack Provides-Extra:
 mongodb Provides-Extra: s3 Provides-Extra: mysql Provides-Extra: bigquery
@@ -27,35 +27,38 @@
 rahulnkumar/custom-utils.git` `pip install git+https://github.com/rahulnkumar/
 custom-utils.git@` `pip install git+https://github.com/rahulnkumar/custom-
 utils.git@` [pip-cu] --- ## 2. Connector### 1. S3 Connector**Code Snippet
 Sample :** ```python ## To use S3 either setup AWS CLI or set the credentials
 from pip package only ## Setup AWS CLI sudo apt install awscli && aws configure
 ## Setup Credentials from pip package from custom_utils.configurer.utils import
 Credential Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********") from
-custom_utils.connector.s3 import S3 # Uplaoding data to S3 S3.push_local_data
-(file_path, s3_uri) # Doownlaoding data from S3 S3.pull_s3_data(file_path,
-s3_uri) ``` **S3 Connector Documentation** ``` class S3(builtins.object) | AWS
-S3 utility functions | | Static methods defined here: | | pull_python_object
-(s3_uri) | read python object stored in S3 bucket | :param string s3_uri: s3
-uri of the object | :return python_object : python object stored in the S3 | |
-pull_s3_data(file_path, s3_uri) | write data stored in local machine into S3
-bucket from | :param string s3_uri: target s3 uri | :param string file_path:
-local path of the file | :return None | | push_local_data(file_path, s3_uri) |
-write data stored in local machine into S3 bucket from | :param string s3_uri:
-target s3 uri | :param string file_path: local path of the file | :return None
-| | push_python_object(python_object, s3_uri) | write python objects/variables
-etc into S3 bucket | :param string bucket: bucket name | :param string
-sub_bucket: sub-bucket name | :param string file_name: name of the file to be
-written | :return None | | read_csv(s3_uri) | write data stored in local
-machine into S3 bucket from | :param string s3_uri: csv file S3 URI | :return
-df : pandas dataframe | | -----------------------------------------------------
------------------ ``` --- --- ### 2. MySQL Connector**Code Snippet Sample :**
-```python # Query from Custom MySQL Database from custom_utils.connector.mysql
-import MySQL user = "***" password = "***" host = "***" port = "***" database =
-"***" db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/
+custom_utils.connector.s3 import S3 # Upload python object to S3
+S3.push_python_object(python_object, s3_uri) # Pull python object from S3 obj =
+S3.pull_python_object(s3_uri) # AWS CLI setup is must to use the following
+methods # Uplaoding local data to S3 S3.push_local_data(file_path, s3_uri) #
+Downloading data from S3 S3.pull_s3_data(file_path, s3_uri) ``` **S3 Connector
+Documentation** ``` class S3(builtins.object) | AWS S3 utility functions | |
+Static methods defined here: | | pull_python_object(s3_uri) | read python
+object stored in S3 bucket | :param string s3_uri: s3 uri of the object | :
+return python_object : python object stored in the S3 | | pull_s3_data
+(file_path, s3_uri) | write data stored in local machine into S3 bucket from |
+:param string s3_uri: target s3 uri | :param string file_path: local path of
+the file | :return None | | push_local_data(file_path, s3_uri) | write data
+stored in local machine into S3 bucket from | :param string s3_uri: target s3
+uri | :param string file_path: local path of the file | :return None | |
+push_python_object(python_object, s3_uri) | write python objects/variables etc
+into S3 bucket | :param string bucket: bucket name | :param string sub_bucket:
+sub-bucket name | :param string file_name: name of the file to be written | :
+return None | | read_csv(s3_uri) | write data stored in local machine into S3
+bucket from | :param string s3_uri: csv file S3 URI | :return df : pandas
+dataframe | | -----------------------------------------------------------------
+----- ``` --- --- ### 2. MySQL Connector**Code Snippet Sample :** ```python #
+Query from Custom MySQL Database from custom_utils.connector.mysql import MySQL
+user = "***" password = "***" host = "***" port = "***" database = "***"
+db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/
 {database}" query = "select * from table_name limit 10" mysql = MySQL
 (db_string=db_string) df = mysql.pull_data(query = query) ``` **MySQL Connector
 Documentaion** ``` class MySQL(builtins.object) | MySQL(db_string) | | MySQL
 database utility functions | | Methods defined here: | | __init__(self,
 db_string) | initialisation method for MySQL Connector | :param string
 db_string: mysql database connection string | | push_data(self, data,
 table_name, mode='append') | Execute a query in the mysql table | :param
```

### Comparing `custom-utils-0.0.312/README.md` & `custom-utils-0.0.313/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,25 @@
 
 ## Setup Credentials from pip package
 from custom_utils.configurer.utils import Credential
 Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********")
 
 
 from custom_utils.connector.s3 import S3
+# Upload python object to S3
+S3.push_python_object(python_object, s3_uri)
 
-# Uplaoding data to S3
+# Pull python object from S3
+obj = S3.pull_python_object(s3_uri)
+
+# AWS CLI setup is must to use the following methods 
+# Uplaoding local data to S3
 S3.push_local_data(file_path, s3_uri)
-                             
-# Doownlaoding data from S3
+                                
+# Downloading data from S3
 S3.pull_s3_data(file_path, s3_uri)
 ```
 
 **S3 Connector Documentation**
     
 ```
 class S3(builtins.object)
@@ -415,15 +421,15 @@
     
     
 **Code Snippet Sample :**
 ```python3
 from custom_utils.alerter.slack import Slack
 slack = Slack(token=SLACK_BOT_TOKEN) # OR Slack() with  SLACK_BOT_TOKEN as env variable
 channel="#shield"
-message = "testing"
+message = "testing"    
 uids = ["U03PAP8C1RC", "U03PAP8C1RC"]
 slack.send_alert(channel, message, uids)
 ```
     
 **Alerter Documentation :**
 ```python
 class Slack(builtins.object)
```

#### html2text {}

```diff
@@ -19,35 +19,38 @@
 rahulnkumar/custom-utils.git` `pip install git+https://github.com/rahulnkumar/
 custom-utils.git@` `pip install git+https://github.com/rahulnkumar/custom-
 utils.git@` [pip-cu] --- ## 2. Connector### 1. S3 Connector**Code Snippet
 Sample :** ```python ## To use S3 either setup AWS CLI or set the credentials
 from pip package only ## Setup AWS CLI sudo apt install awscli && aws configure
 ## Setup Credentials from pip package from custom_utils.configurer.utils import
 Credential Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********") from
-custom_utils.connector.s3 import S3 # Uplaoding data to S3 S3.push_local_data
-(file_path, s3_uri) # Doownlaoding data from S3 S3.pull_s3_data(file_path,
-s3_uri) ``` **S3 Connector Documentation** ``` class S3(builtins.object) | AWS
-S3 utility functions | | Static methods defined here: | | pull_python_object
-(s3_uri) | read python object stored in S3 bucket | :param string s3_uri: s3
-uri of the object | :return python_object : python object stored in the S3 | |
-pull_s3_data(file_path, s3_uri) | write data stored in local machine into S3
-bucket from | :param string s3_uri: target s3 uri | :param string file_path:
-local path of the file | :return None | | push_local_data(file_path, s3_uri) |
-write data stored in local machine into S3 bucket from | :param string s3_uri:
-target s3 uri | :param string file_path: local path of the file | :return None
-| | push_python_object(python_object, s3_uri) | write python objects/variables
-etc into S3 bucket | :param string bucket: bucket name | :param string
-sub_bucket: sub-bucket name | :param string file_name: name of the file to be
-written | :return None | | read_csv(s3_uri) | write data stored in local
-machine into S3 bucket from | :param string s3_uri: csv file S3 URI | :return
-df : pandas dataframe | | -----------------------------------------------------
------------------ ``` --- --- ### 2. MySQL Connector**Code Snippet Sample :**
-```python # Query from Custom MySQL Database from custom_utils.connector.mysql
-import MySQL user = "***" password = "***" host = "***" port = "***" database =
-"***" db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/
+custom_utils.connector.s3 import S3 # Upload python object to S3
+S3.push_python_object(python_object, s3_uri) # Pull python object from S3 obj =
+S3.pull_python_object(s3_uri) # AWS CLI setup is must to use the following
+methods # Uplaoding local data to S3 S3.push_local_data(file_path, s3_uri) #
+Downloading data from S3 S3.pull_s3_data(file_path, s3_uri) ``` **S3 Connector
+Documentation** ``` class S3(builtins.object) | AWS S3 utility functions | |
+Static methods defined here: | | pull_python_object(s3_uri) | read python
+object stored in S3 bucket | :param string s3_uri: s3 uri of the object | :
+return python_object : python object stored in the S3 | | pull_s3_data
+(file_path, s3_uri) | write data stored in local machine into S3 bucket from |
+:param string s3_uri: target s3 uri | :param string file_path: local path of
+the file | :return None | | push_local_data(file_path, s3_uri) | write data
+stored in local machine into S3 bucket from | :param string s3_uri: target s3
+uri | :param string file_path: local path of the file | :return None | |
+push_python_object(python_object, s3_uri) | write python objects/variables etc
+into S3 bucket | :param string bucket: bucket name | :param string sub_bucket:
+sub-bucket name | :param string file_name: name of the file to be written | :
+return None | | read_csv(s3_uri) | write data stored in local machine into S3
+bucket from | :param string s3_uri: csv file S3 URI | :return df : pandas
+dataframe | | -----------------------------------------------------------------
+----- ``` --- --- ### 2. MySQL Connector**Code Snippet Sample :** ```python #
+Query from Custom MySQL Database from custom_utils.connector.mysql import MySQL
+user = "***" password = "***" host = "***" port = "***" database = "***"
+db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/
 {database}" query = "select * from table_name limit 10" mysql = MySQL
 (db_string=db_string) df = mysql.pull_data(query = query) ``` **MySQL Connector
 Documentaion** ``` class MySQL(builtins.object) | MySQL(db_string) | | MySQL
 database utility functions | | Methods defined here: | | __init__(self,
 db_string) | initialisation method for MySQL Connector | :param string
 db_string: mysql database connection string | | push_data(self, data,
 table_name, mode='append') | Execute a query in the mysql table | :param
```

### Comparing `custom-utils-0.0.312/custom_utils/alerter/slack.py` & `custom-utils-0.0.313/custom_utils/alerter/slack.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,11 +27,10 @@
 
         returns: Nothing
         """
 
         uids = [f"<@{uid}>" for uid in uids]
         uids = " ".join(uids)
         message = f'{uids}  {message}'
-        print(message)
         self.client.chat_postMessage(channel=channel, text=message)
```

### Comparing `custom-utils-0.0.312/custom_utils/configurer/profiler.py` & `custom-utils-0.0.313/custom_utils/configurer/profiler.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/custom_utils/configurer/utils.py` & `custom-utils-0.0.313/custom_utils/configurer/utils.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/custom_utils/connector/bigquery.py` & `custom-utils-0.0.313/custom_utils/connector/bigquery.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/custom_utils/connector/mongodb.py` & `custom-utils-0.0.313/custom_utils/connector/mongodb.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/custom_utils/connector/mysql.py` & `custom-utils-0.0.313/custom_utils/connector/mysql.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/custom_utils/connector/s3.py` & `custom-utils-0.0.313/custom_utils/connector/s3.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/custom_utils/exceptions.py` & `custom-utils-0.0.313/custom_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/custom_utils/utils.py` & `custom-utils-0.0.313/custom_utils/utils.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/custom_utils.egg-info/PKG-INFO` & `custom-utils-0.0.313/custom_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-utils
-Version: 0.0.312
+Version: 0.0.313
 Summary: Utilities for database connectors, slack alerter, loggers etc
 Home-page: https://github.com/RahulnKumar/custom-utils
 Author: Rahul Kumar
 Author-email: rahulnkumar7@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -83,19 +83,25 @@
 
 ## Setup Credentials from pip package
 from custom_utils.configurer.utils import Credential
 Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********")
 
 
 from custom_utils.connector.s3 import S3
+# Upload python object to S3
+S3.push_python_object(python_object, s3_uri)
 
-# Uplaoding data to S3
+# Pull python object from S3
+obj = S3.pull_python_object(s3_uri)
+
+# AWS CLI setup is must to use the following methods 
+# Uplaoding local data to S3
 S3.push_local_data(file_path, s3_uri)
-                             
-# Doownlaoding data from S3
+                                
+# Downloading data from S3
 S3.pull_s3_data(file_path, s3_uri)
 ```
 
 **S3 Connector Documentation**
     
 ```
 class S3(builtins.object)
@@ -435,15 +441,15 @@
     
     
 **Code Snippet Sample :**
 ```python3
 from custom_utils.alerter.slack import Slack
 slack = Slack(token=SLACK_BOT_TOKEN) # OR Slack() with  SLACK_BOT_TOKEN as env variable
 channel="#shield"
-message = "testing"
+message = "testing"    
 uids = ["U03PAP8C1RC", "U03PAP8C1RC"]
 slack.send_alert(channel, message, uids)
 ```
     
 **Alerter Documentation :**
 ```python
 class Slack(builtins.object)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.312 Summary: Utilities
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.313 Summary: Utilities
 for database connectors, slack alerter, loggers etc Home-page: https://
 github.com/RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
 rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown Provides-Extra: slack Provides-Extra:
 mongodb Provides-Extra: s3 Provides-Extra: mysql Provides-Extra: bigquery
@@ -27,35 +27,38 @@
 rahulnkumar/custom-utils.git` `pip install git+https://github.com/rahulnkumar/
 custom-utils.git@` `pip install git+https://github.com/rahulnkumar/custom-
 utils.git@` [pip-cu] --- ## 2. Connector### 1. S3 Connector**Code Snippet
 Sample :** ```python ## To use S3 either setup AWS CLI or set the credentials
 from pip package only ## Setup AWS CLI sudo apt install awscli && aws configure
 ## Setup Credentials from pip package from custom_utils.configurer.utils import
 Credential Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********") from
-custom_utils.connector.s3 import S3 # Uplaoding data to S3 S3.push_local_data
-(file_path, s3_uri) # Doownlaoding data from S3 S3.pull_s3_data(file_path,
-s3_uri) ``` **S3 Connector Documentation** ``` class S3(builtins.object) | AWS
-S3 utility functions | | Static methods defined here: | | pull_python_object
-(s3_uri) | read python object stored in S3 bucket | :param string s3_uri: s3
-uri of the object | :return python_object : python object stored in the S3 | |
-pull_s3_data(file_path, s3_uri) | write data stored in local machine into S3
-bucket from | :param string s3_uri: target s3 uri | :param string file_path:
-local path of the file | :return None | | push_local_data(file_path, s3_uri) |
-write data stored in local machine into S3 bucket from | :param string s3_uri:
-target s3 uri | :param string file_path: local path of the file | :return None
-| | push_python_object(python_object, s3_uri) | write python objects/variables
-etc into S3 bucket | :param string bucket: bucket name | :param string
-sub_bucket: sub-bucket name | :param string file_name: name of the file to be
-written | :return None | | read_csv(s3_uri) | write data stored in local
-machine into S3 bucket from | :param string s3_uri: csv file S3 URI | :return
-df : pandas dataframe | | -----------------------------------------------------
------------------ ``` --- --- ### 2. MySQL Connector**Code Snippet Sample :**
-```python # Query from Custom MySQL Database from custom_utils.connector.mysql
-import MySQL user = "***" password = "***" host = "***" port = "***" database =
-"***" db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/
+custom_utils.connector.s3 import S3 # Upload python object to S3
+S3.push_python_object(python_object, s3_uri) # Pull python object from S3 obj =
+S3.pull_python_object(s3_uri) # AWS CLI setup is must to use the following
+methods # Uplaoding local data to S3 S3.push_local_data(file_path, s3_uri) #
+Downloading data from S3 S3.pull_s3_data(file_path, s3_uri) ``` **S3 Connector
+Documentation** ``` class S3(builtins.object) | AWS S3 utility functions | |
+Static methods defined here: | | pull_python_object(s3_uri) | read python
+object stored in S3 bucket | :param string s3_uri: s3 uri of the object | :
+return python_object : python object stored in the S3 | | pull_s3_data
+(file_path, s3_uri) | write data stored in local machine into S3 bucket from |
+:param string s3_uri: target s3 uri | :param string file_path: local path of
+the file | :return None | | push_local_data(file_path, s3_uri) | write data
+stored in local machine into S3 bucket from | :param string s3_uri: target s3
+uri | :param string file_path: local path of the file | :return None | |
+push_python_object(python_object, s3_uri) | write python objects/variables etc
+into S3 bucket | :param string bucket: bucket name | :param string sub_bucket:
+sub-bucket name | :param string file_name: name of the file to be written | :
+return None | | read_csv(s3_uri) | write data stored in local machine into S3
+bucket from | :param string s3_uri: csv file S3 URI | :return df : pandas
+dataframe | | -----------------------------------------------------------------
+----- ``` --- --- ### 2. MySQL Connector**Code Snippet Sample :** ```python #
+Query from Custom MySQL Database from custom_utils.connector.mysql import MySQL
+user = "***" password = "***" host = "***" port = "***" database = "***"
+db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/
 {database}" query = "select * from table_name limit 10" mysql = MySQL
 (db_string=db_string) df = mysql.pull_data(query = query) ``` **MySQL Connector
 Documentaion** ``` class MySQL(builtins.object) | MySQL(db_string) | | MySQL
 database utility functions | | Methods defined here: | | __init__(self,
 db_string) | initialisation method for MySQL Connector | :param string
 db_string: mysql database connection string | | push_data(self, data,
 table_name, mode='append') | Execute a query in the mysql table | :param
```

### Comparing `custom-utils-0.0.312/custom_utils.egg-info/SOURCES.txt` & `custom-utils-0.0.313/custom_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.312/setup.py` & `custom-utils-0.0.313/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     author="Rahul Kumar",
     author_email="rahulnkumar7@gmail.com",
     name='custom-utils',
     description='Utilities for database connectors, slack alerter, loggers etc',
-    version="0.0.312",
+    version="0.0.313",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RahulnKumar/custom-utils',
     packages=find_packages(),
     python_requires=">=3.6.9",
     install_requires=['python-dotenv', 'subprocess32',],
     extras_require=EXTRAS_REQUIRE,
```

