# Comparing `tmp/refractio-2.0.3.tar.gz` & `tmp/refractio-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.3.tar", last modified: Tue May 30 09:32:44 2023, max compression
+gzip compressed data, was "refractio-2.0.4.tar", last modified: Wed May 31 13:58:04 2023, max compression
```

## Comparing `refractio-2.0.3.tar` & `refractio-2.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-30 09:32:44.233870 refractio-2.0.3/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7440 2023-05-30 09:32:44.233870 refractio-2.0.3/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6771 2023-05-30 09:31:33.000000 refractio-2.0.3/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-30 09:32:44.232870 refractio-2.0.3/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      319 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4717 2023-05-30 09:31:33.000000 refractio-2.0.3/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3875 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13446 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/snowflake.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-30 09:32:44.232870 refractio-2.0.3/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7440 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      367 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-30 09:32:44.233870 refractio-2.0.3/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1807 2023-05-30 09:31:33.000000 refractio-2.0.3/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 13:58:04.122405 refractio-2.0.4/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8634 2023-05-31 13:58:04.122405 refractio-2.0.4/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7939 2023-05-31 13:57:21.000000 refractio-2.0.4/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 13:58:04.120405 refractio-2.0.4/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      376 2023-05-31 13:57:21.000000 refractio-2.0.4/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4717 2023-05-30 09:31:33.000000 refractio-2.0.4/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4250 2023-05-31 13:57:21.000000 refractio-2.0.4/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    15148 2023-05-31 13:57:21.000000 refractio-2.0.4/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/snowflake.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6140 2023-05-31 13:57:21.000000 refractio-2.0.4/refractio/sqlserver.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 13:58:04.121405 refractio-2.0.4/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8634 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      390 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      526 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-31 13:58:04.122405 refractio-2.0.4/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1884 2023-05-31 13:57:21.000000 refractio-2.0.4/setup.py
```

### Comparing `refractio-2.0.3/PKG-INFO` & `refractio-2.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: refractio
-Version: 2.0.3
-Summary: REFRACT-IO: To read and write dataframe from different connectors.
-Home-page: UNKNOWN
-Author: Abhishek Chaurasia
-Author-email: <abhishek1.chaurasia@fosfor.com>
-License: UNKNOWN
-Project-URL: Product, https://www.fosfor.com/refract/
-Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
-Keywords: refractio
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: snowflake
-Provides-Extra: s3
-Provides-Extra: azureblob
-Provides-Extra: local
-Provides-Extra: sftp
-Provides-Extra: mysql
-Provides-Extra: hive
-
 # Installation:
 ## without any dependencies:
 ```commandline
 pip install refractio
 ```
 ## With all dependencies:
 ```commandline
@@ -54,14 +31,18 @@
 ```commandline
 pip install refractio[mysql]
 ```
 ## With hive:
 ```commandline
 pip install refractio[hive]
 ```
+## With sqlserver:
+```commandline
+pip install refractio[sqlserver]
+```
 
 #### Source code is available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git 
 
 # Usage:
 ## To read dataframe with dataset name only -
 ```python
 from refractio import get_dataframe
@@ -122,14 +103,40 @@
 # To execute a user specific query in mysql, with the current connection object or with the default connection for the user.
 mysql.execute_query(query="user_query")
 
 # To close mysql connection, please do close the connection after use!
 mysql.close_connection()
 ```
 
+## To use sqlserver related operations -
+```python
+from refractio import sqlserver
+
+# To get sqlserver connection object with a default sqlserver connection created by the user, if available.
+sqlserver.get_connection()
+
+# To get sqlserver connection object with a specific connection name
+sqlserver.get_connection(connection_name="sqlserver_con_name")
+
+# To read a specific dataset published from a sqlserver connection
+sqlserver.get_dataframe("dataset_name")
+
+# To read a specific dataset published from a sqlserver connection with only top few records.
+sqlserver.get_dataframe("dataset_name", row_count=3)
+
+# To execute a user specific query in sqlserver, with the specified connection name.
+sqlserver.execute_query(query="user_query", database="db_name", connection_name="connection_name")
+
+# To execute a user specific query in sqlserver, with the current connection object or with the default connection for the user.
+sqlserver.execute_query(query="user_query", database="db_name")
+
+# To close sqlserver connection, please do close the connection after use!
+sqlserver.close_connection()
+```
+
 ## To use hive related operations -
 ```python
 from refractio import hive
 
 # To get hive connection object with a default hive connection created by the user, if available. User id is required (1001 is default user_id used).
 hive.get_connection(user_id=1001)
 
@@ -212,9 +219,7 @@
 azure.get_dataframe("dataset_name", row_count=3)
 
 # Use azure connection object c to do any operation related to azure.
 c = azure.get_connection()
 ```
 
 *Note: Usage documentation will be updated in upcoming releases.*
-
-
```

### Comparing `refractio-2.0.3/README.md` & `refractio-2.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: refractio
+Version: 2.0.4
+Summary: REFRACT-IO: To read and write dataframe from different connectors.
+Home-page: UNKNOWN
+Author: Abhishek Chaurasia
+Author-email: <abhishek1.chaurasia@fosfor.com>
+License: UNKNOWN
+Project-URL: Product, https://www.fosfor.com/refract/
+Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
+Keywords: refractio
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: snowflake
+Provides-Extra: s3
+Provides-Extra: azureblob
+Provides-Extra: local
+Provides-Extra: sftp
+Provides-Extra: mysql
+Provides-Extra: hive
+Provides-Extra: sqlserver
+
 # Installation:
 ## without any dependencies:
 ```commandline
 pip install refractio
 ```
 ## With all dependencies:
 ```commandline
@@ -31,14 +55,18 @@
 ```commandline
 pip install refractio[mysql]
 ```
 ## With hive:
 ```commandline
 pip install refractio[hive]
 ```
+## With sqlserver:
+```commandline
+pip install refractio[sqlserver]
+```
 
 #### Source code is available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git 
 
 # Usage:
 ## To read dataframe with dataset name only -
 ```python
 from refractio import get_dataframe
@@ -99,14 +127,40 @@
 # To execute a user specific query in mysql, with the current connection object or with the default connection for the user.
 mysql.execute_query(query="user_query")
 
 # To close mysql connection, please do close the connection after use!
 mysql.close_connection()
 ```
 
+## To use sqlserver related operations -
+```python
+from refractio import sqlserver
+
+# To get sqlserver connection object with a default sqlserver connection created by the user, if available.
+sqlserver.get_connection()
+
+# To get sqlserver connection object with a specific connection name
+sqlserver.get_connection(connection_name="sqlserver_con_name")
+
+# To read a specific dataset published from a sqlserver connection
+sqlserver.get_dataframe("dataset_name")
+
+# To read a specific dataset published from a sqlserver connection with only top few records.
+sqlserver.get_dataframe("dataset_name", row_count=3)
+
+# To execute a user specific query in sqlserver, with the specified connection name.
+sqlserver.execute_query(query="user_query", database="db_name", connection_name="connection_name")
+
+# To execute a user specific query in sqlserver, with the current connection object or with the default connection for the user.
+sqlserver.execute_query(query="user_query", database="db_name")
+
+# To close sqlserver connection, please do close the connection after use!
+sqlserver.close_connection()
+```
+
 ## To use hive related operations -
 ```python
 from refractio import hive
 
 # To get hive connection object with a default hive connection created by the user, if available. User id is required (1001 is default user_id used).
 hive.get_connection(user_id=1001)
 
@@ -189,7 +243,9 @@
 azure.get_dataframe("dataset_name", row_count=3)
 
 # Use azure connection object c to do any operation related to azure.
 c = azure.get_connection()
 ```
 
 *Note: Usage documentation will be updated in upcoming releases.*
+
+
```

### Comparing `refractio-2.0.3/refractio/amazons3.py` & `refractio-2.0.4/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.3/refractio/azure.py` & `refractio-2.0.4/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.3/refractio/hive.py` & `refractio-2.0.4/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.3/refractio/manager.py` & `refractio-2.0.4/refractio/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,7 +98,21 @@
     :return: query
     """
     if int(row_count) > 0:
         print(f"fetching {row_count} records!")
         return f"SELECT * FROM {table_name} LIMIT {row_count}"
     else:
         return f"SELECT * FROM {table_name}"
+
+
+def get_top_dataframe_query(table_name, row_count):
+    """
+    To get the sqlserver query to fetch dataframe
+    :param table_name:
+    :param row_count:
+    :return: query
+    """
+    if int(row_count) > 0:
+        print(f"fetching {row_count} records!")
+        return f"SELECT TOP {row_count} * FROM {table_name}"
+    else:
+        return f"SELECT * FROM {table_name}"
```

### Comparing `refractio-2.0.3/refractio/mysql.py` & `refractio-2.0.4/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.3/refractio/refractio.py` & `refractio-2.0.4/refractio/refractio.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         if connection_details["params"]["READER"]["type"] == "RDBMS":
             if connection_details["params"]["READER"]["sub_type"] == "SNOWFLAKE":
                 data_frame = get_snowflake_df(connection_details, row_count, strategy)
             elif connection_details["params"]["READER"]["sub_type"] == "MYSQL":
                 data_frame = get_mysql_df(connection_details, row_count, strategy)
             elif connection_details["params"]["READER"]["sub_type"] == "HIVE":
                 data_frame = get_hive_df(connection_details, row_count, strategy, user_id)
+            elif connection_details["params"]["READER"]["sub_type"] == "SQLSERVER":
+                data_frame = get_sqlserver_df(connection_details, row_count, strategy)
             else:
                 print("Reading dataframe using connector backend")
                 # Need to install, git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git
                 from connector.mosaicio import MosaicioConnector
                 connector = MosaicioConnector()
                 data_frame = connector.getPandasDataFrame(
                     param=connection_details["params"],
@@ -189,14 +191,48 @@
     # Read data fromm mysql
     data_frame = pd.read_sql(query, con=conn)
     # Close connection
     conn.close()
     return data_frame
 
 
+def get_sqlserver_df(connection_details, row_count, strategy):
+    """
+    Param:
+        connection_details: connection details dict
+        row_count: number of rows to be fetched
+        strategy: top/bottom
+    To read data frame from sql server connection
+    """
+    print("Reading dataframe from sqlserver native connector")
+    import pyodbc
+
+    # This need the OS should have sql server driver installed. Like,
+    # curl https://packages.microsoft.com/config/rhel/9.0/prod.repo > /etc/yum.repos.d/mssql-release.repo
+    # ACCEPT_EULA=Y yum install -y msodbcsql18
+    driver_lib = "/opt/microsoft/msodbcsql18/lib64/libmsodbcsql-18.2.so.1.1"    # sqlserver driver lib path
+    conn = pyodbc.connect(f'DRIVER={driver_lib};'
+                          f'SERVER={connection_details["params"]["READER"]["host"]};'
+                          f'DATABASE={connection_details["params"]["READER"]["database"]};'
+                          f'UID={connection_details["params"]["READER"]["user"]};'
+                          f'PWD={connection_details["params"]["READER"]["password"]};'
+                          f'TrustServerCertificate=yes;')
+
+    if int(row_count) > 0:
+        # Generate query
+        query = f"SELECT TOP {int(row_count)} * FROM {connection_details['params']['READER']['tables']}"
+    else:
+        query = f"SELECT * FROM {connection_details['params']['READER']['tables']}"
+    # Read data from sqlserver
+    data_frame = pd.read_sql(query, con=conn)
+    # Close connection
+    conn.close()
+    return data_frame
+
+
 def get_s3_df(connection_details, row_count, strategy):
     """
     Param:
         connection_details: connection details dict
         row_count: number of rows to be fetched
         strategy: top/bottom
     To read data frame form amazon S3 connection
```

### Comparing `refractio-2.0.3/refractio/sftp.py` & `refractio-2.0.4/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.3/refractio/snowflake.py` & `refractio-2.0.4/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.3/refractio.egg-info/PKG-INFO` & `refractio-2.0.4/refractio.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.3
+Version: 2.0.4
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
@@ -16,14 +16,15 @@
 Provides-Extra: snowflake
 Provides-Extra: s3
 Provides-Extra: azureblob
 Provides-Extra: local
 Provides-Extra: sftp
 Provides-Extra: mysql
 Provides-Extra: hive
+Provides-Extra: sqlserver
 
 # Installation:
 ## without any dependencies:
 ```commandline
 pip install refractio
 ```
 ## With all dependencies:
@@ -54,14 +55,18 @@
 ```commandline
 pip install refractio[mysql]
 ```
 ## With hive:
 ```commandline
 pip install refractio[hive]
 ```
+## With sqlserver:
+```commandline
+pip install refractio[sqlserver]
+```
 
 #### Source code is available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git 
 
 # Usage:
 ## To read dataframe with dataset name only -
 ```python
 from refractio import get_dataframe
@@ -122,14 +127,40 @@
 # To execute a user specific query in mysql, with the current connection object or with the default connection for the user.
 mysql.execute_query(query="user_query")
 
 # To close mysql connection, please do close the connection after use!
 mysql.close_connection()
 ```
 
+## To use sqlserver related operations -
+```python
+from refractio import sqlserver
+
+# To get sqlserver connection object with a default sqlserver connection created by the user, if available.
+sqlserver.get_connection()
+
+# To get sqlserver connection object with a specific connection name
+sqlserver.get_connection(connection_name="sqlserver_con_name")
+
+# To read a specific dataset published from a sqlserver connection
+sqlserver.get_dataframe("dataset_name")
+
+# To read a specific dataset published from a sqlserver connection with only top few records.
+sqlserver.get_dataframe("dataset_name", row_count=3)
+
+# To execute a user specific query in sqlserver, with the specified connection name.
+sqlserver.execute_query(query="user_query", database="db_name", connection_name="connection_name")
+
+# To execute a user specific query in sqlserver, with the current connection object or with the default connection for the user.
+sqlserver.execute_query(query="user_query", database="db_name")
+
+# To close sqlserver connection, please do close the connection after use!
+sqlserver.close_connection()
+```
+
 ## To use hive related operations -
 ```python
 from refractio import hive
 
 # To get hive connection object with a default hive connection created by the user, if available. User id is required (1001 is default user_id used).
 hive.get_connection(user_id=1001)
```

### Comparing `refractio-2.0.3/setup.py` & `refractio-2.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.3'
+VERSION = '2.0.4'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
         "openpyxl==3.1.2",
         "xlrd==2.0.1",
         "pysftp==0.2.9",
         "pymysql==1.0.3",
         "impyla==0.16.2",
         "thrift-sasl==0.4.3",
         "pure-sasl==0.6.2",
-        "PyHive==0.6.3.dev0"
+        "PyHive==0.6.3.dev0",
+        "pyodbc==4.0.39"
     ],
     "snowflake": [
         "snowflake-connector-python[pandas]==3.0.2"
     ],
     "s3": [
         "boto3==1.26.116"
     ],
@@ -42,14 +43,17 @@
         "pymysql==1.0.3"
     ],
     "hive": [
         "impyla==0.16.2",
         "thrift-sasl==0.4.3",
         "pure-sasl==0.6.2",
         "PyHive==0.6.3.dev0"
+    ],
+    "sqlserver": [
+        "pyodbc==4.0.39"
     ]
 }
 
 # Setting up
 setup(
     name="refractio",
     version=VERSION,
```

