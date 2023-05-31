# Comparing `tmp/refractio-2.0.4.tar.gz` & `tmp/refractio-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.4.tar", last modified: Wed May 31 13:58:04 2023, max compression
+gzip compressed data, was "refractio-2.0.5.tar", last modified: Wed May 31 14:07:01 2023, max compression
```

## Comparing `refractio-2.0.4.tar` & `refractio-2.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 13:58:04.122405 refractio-2.0.4/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8634 2023-05-31 13:58:04.122405 refractio-2.0.4/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7939 2023-05-31 13:57:21.000000 refractio-2.0.4/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 13:58:04.120405 refractio-2.0.4/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      376 2023-05-31 13:57:21.000000 refractio-2.0.4/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4717 2023-05-30 09:31:33.000000 refractio-2.0.4/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4250 2023-05-31 13:57:21.000000 refractio-2.0.4/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    15148 2023-05-31 13:57:21.000000 refractio-2.0.4/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-30 09:31:19.000000 refractio-2.0.4/refractio/snowflake.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6140 2023-05-31 13:57:21.000000 refractio-2.0.4/refractio/sqlserver.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 13:58:04.121405 refractio-2.0.4/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8634 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      390 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      526 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-31 13:58:04.000000 refractio-2.0.4/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-31 13:58:04.122405 refractio-2.0.4/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1884 2023-05-31 13:57:21.000000 refractio-2.0.4/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 14:07:01.718990 refractio-2.0.5/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8919 2023-05-31 14:07:01.718990 refractio-2.0.5/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8224 2023-05-31 14:06:39.000000 refractio-2.0.5/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 14:07:01.717990 refractio-2.0.5/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      376 2023-05-31 13:57:21.000000 refractio-2.0.5/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4717 2023-05-30 09:31:33.000000 refractio-2.0.5/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4250 2023-05-31 13:57:21.000000 refractio-2.0.5/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    15148 2023-05-31 13:57:21.000000 refractio-2.0.5/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/snowflake.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6140 2023-05-31 13:57:21.000000 refractio-2.0.5/refractio/sqlserver.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 14:07:01.718990 refractio-2.0.5/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8919 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      390 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      526 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-31 14:07:01.718990 refractio-2.0.5/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1884 2023-05-31 14:06:39.000000 refractio-2.0.5/setup.py
```

### Comparing `refractio-2.0.4/PKG-INFO` & `refractio-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.4
+Version: 2.0.5
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
@@ -128,15 +128,19 @@
 mysql.execute_query(query="user_query")
 
 # To close mysql connection, please do close the connection after use!
 mysql.close_connection()
 ```
 
 ## To use sqlserver related operations -
+### Requires sqlserver driver library
 ```python
+# Create a custom template with the following commands added in "Pre Init Script" section,
+# sudo curl -o /etc/yum.repos.d/mssql-release.repo https://packages.microsoft.com/config/rhel/9.0/prod.repo
+# sudo ACCEPT_EULA=Y yum install -y msodbcsql18
 from refractio import sqlserver
 
 # To get sqlserver connection object with a default sqlserver connection created by the user, if available.
 sqlserver.get_connection()
 
 # To get sqlserver connection object with a specific connection name
 sqlserver.get_connection(connection_name="sqlserver_con_name")
```

### Comparing `refractio-2.0.4/README.md` & `refractio-2.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,19 @@
 mysql.execute_query(query="user_query")
 
 # To close mysql connection, please do close the connection after use!
 mysql.close_connection()
 ```
 
 ## To use sqlserver related operations -
+### Requires sqlserver driver library
 ```python
+# Create a custom template with the following commands added in "Pre Init Script" section,
+# sudo curl -o /etc/yum.repos.d/mssql-release.repo https://packages.microsoft.com/config/rhel/9.0/prod.repo
+# sudo ACCEPT_EULA=Y yum install -y msodbcsql18
 from refractio import sqlserver
 
 # To get sqlserver connection object with a default sqlserver connection created by the user, if available.
 sqlserver.get_connection()
 
 # To get sqlserver connection object with a specific connection name
 sqlserver.get_connection(connection_name="sqlserver_con_name")
```

### Comparing `refractio-2.0.4/refractio/amazons3.py` & `refractio-2.0.5/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/refractio/azure.py` & `refractio-2.0.5/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/refractio/hive.py` & `refractio-2.0.5/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/refractio/manager.py` & `refractio-2.0.5/refractio/manager.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/refractio/mysql.py` & `refractio-2.0.5/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/refractio/refractio.py` & `refractio-2.0.5/refractio/refractio.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/refractio/sftp.py` & `refractio-2.0.5/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/refractio/snowflake.py` & `refractio-2.0.5/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/refractio/sqlserver.py` & `refractio-2.0.5/refractio/sqlserver.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/refractio.egg-info/PKG-INFO` & `refractio-2.0.5/refractio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.4
+Version: 2.0.5
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
@@ -128,15 +128,19 @@
 mysql.execute_query(query="user_query")
 
 # To close mysql connection, please do close the connection after use!
 mysql.close_connection()
 ```
 
 ## To use sqlserver related operations -
+### Requires sqlserver driver library
 ```python
+# Create a custom template with the following commands added in "Pre Init Script" section,
+# sudo curl -o /etc/yum.repos.d/mssql-release.repo https://packages.microsoft.com/config/rhel/9.0/prod.repo
+# sudo ACCEPT_EULA=Y yum install -y msodbcsql18
 from refractio import sqlserver
 
 # To get sqlserver connection object with a default sqlserver connection created by the user, if available.
 sqlserver.get_connection()
 
 # To get sqlserver connection object with a specific connection name
 sqlserver.get_connection(connection_name="sqlserver_con_name")
```

### Comparing `refractio-2.0.4/refractio.egg-info/requires.txt` & `refractio-2.0.5/refractio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `refractio-2.0.4/setup.py` & `refractio-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.4'
+VERSION = '2.0.5'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

