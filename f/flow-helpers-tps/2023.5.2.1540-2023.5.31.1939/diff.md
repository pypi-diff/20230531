# Comparing `tmp/flow_helpers_tps-2023.5.2.1540.tar.gz` & `tmp/flow_helpers_tps-2023.5.31.1939.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_helpers_tps-2023.5.2.1540.tar", max compression
+gzip compressed data, was "flow_helpers_tps-2023.5.31.1939.tar", max compression
```

## Comparing `flow_helpers_tps-2023.5.2.1540.tar` & `flow_helpers_tps-2023.5.31.1939.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2023-05-02 15:40:07.963458 flow_helpers_tps-2023.5.2.1540/LICENSE
--rw-r--r--   0        0        0        0 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/__init__.py
--rw-r--r--   0        0        0     4868 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_bingwmt.py
--rw-r--r--   0        0        0      657 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_covidtracking.py
--rw-r--r--   0        0        0     3893 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_dcm.py
--rw-r--r--   0        0        0     3230 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_facebook.py
--rw-r--r--   0        0        0      488 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_file.py
--rw-r--r--   0        0        0     9315 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_firebasetransform.py
--rw-r--r--   0        0        0    10574 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_funneltransform.py
--rw-r--r--   0        0        0    24475 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gatransform.py
--rw-r--r--   0        0        0     6953 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gbq.py
--rw-r--r--   0        0        0     4308 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gcs.py
--rw-r--r--   0        0        0     2639 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gdrive.py
--rw-r--r--   0        0        0    11001 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_googleanalytics.py
--rw-r--r--   0        0        0     4408 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gsc.py
--rw-r--r--   0        0        0      631 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gsheet.py
--rw-r--r--   0        0        0      981 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_impact.py
--rw-r--r--   0        0        0     7255 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_journera.py
--rw-r--r--   0        0        0     2986 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_listen360.py
--rw-r--r--   0        0        0     6403 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_mssql.py
--rw-r--r--   0        0        0      505 2023-05-02 15:40:07.975458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_s3.py
--rw-r--r--   0        0        0     7919 2023-05-02 15:40:07.979458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_sa360.py
--rw-r--r--   0        0        0    18284 2023-05-02 15:40:07.979458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_salesforce.py
--rw-r--r--   0        0        0     2615 2023-05-02 15:40:07.979458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_scrapinghub.py
--rw-r--r--   0        0        0     6739 2023-05-02 15:40:07.979458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_sftp.py
--rw-r--r--   0        0        0     6113 2023-05-02 15:40:07.979458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_sharepoint.py
--rw-r--r--   0        0        0    11579 2023-05-02 15:40:07.979458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_snowflake.py
--rw-r--r--   0        0        0     2264 2023-05-02 15:40:07.979458 flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_time.py
--rw-r--r--   0        0        0      622 2023-05-02 15:40:48.352430 flow_helpers_tps-2023.5.2.1540/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 flow_helpers_tps-2023.5.2.1540/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-31 19:39:00.850031 flow_helpers_tps-2023.5.31.1939/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/__init__.py
+-rw-r--r--   0        0        0     4868 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_bingwmt.py
+-rw-r--r--   0        0        0      657 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_covidtracking.py
+-rw-r--r--   0        0        0     3893 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_dcm.py
+-rw-r--r--   0        0        0     3230 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_facebook.py
+-rw-r--r--   0        0        0      488 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_file.py
+-rw-r--r--   0        0        0     9315 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_firebasetransform.py
+-rw-r--r--   0        0        0    10574 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_funneltransform.py
+-rw-r--r--   0        0        0    24475 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gatransform.py
+-rw-r--r--   0        0        0     6953 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gbq.py
+-rw-r--r--   0        0        0     4308 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gcs.py
+-rw-r--r--   0        0        0     2639 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gdrive.py
+-rw-r--r--   0        0        0    11001 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_googleanalytics.py
+-rw-r--r--   0        0        0     4408 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gsc.py
+-rw-r--r--   0        0        0      631 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gsheet.py
+-rw-r--r--   0        0        0      981 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_impact.py
+-rw-r--r--   0        0        0     7255 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_journera.py
+-rw-r--r--   0        0        0     2986 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_listen360.py
+-rw-r--r--   0        0        0     6403 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_mssql.py
+-rw-r--r--   0        0        0      505 2023-05-31 19:39:00.858031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_s3.py
+-rw-r--r--   0        0        0     7919 2023-05-31 19:39:00.862031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_sa360.py
+-rw-r--r--   0        0        0    18284 2023-05-31 19:39:00.862031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_salesforce.py
+-rw-r--r--   0        0        0     2615 2023-05-31 19:39:00.862031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_scrapinghub.py
+-rw-r--r--   0        0        0     6739 2023-05-31 19:39:00.862031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_sftp.py
+-rw-r--r--   0        0        0     6113 2023-05-31 19:39:00.862031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_sharepoint.py
+-rw-r--r--   0        0        0    11579 2023-05-31 19:39:00.862031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_snowflake.py
+-rw-r--r--   0        0        0     2264 2023-05-31 19:39:00.862031 flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_time.py
+-rw-r--r--   0        0        0      621 2023-05-31 19:39:31.070660 flow_helpers_tps-2023.5.31.1939/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 flow_helpers_tps-2023.5.31.1939/PKG-INFO
```

### Comparing `flow_helpers_tps-2023.5.2.1540/LICENSE` & `flow_helpers_tps-2023.5.31.1939/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_bingwmt.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_bingwmt.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_covidtracking.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_covidtracking.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_dcm.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_dcm.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_facebook.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_facebook.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_firebasetransform.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_firebasetransform.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_funneltransform.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_funneltransform.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gatransform.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gatransform.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gbq.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gbq.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gcs.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gcs.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gdrive.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gdrive.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_googleanalytics.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_googleanalytics.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gsc.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gsc.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_gsheet.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_gsheet.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_impact.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_impact.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_journera.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_journera.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_listen360.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_listen360.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_mssql.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_mssql.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_sa360.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_sa360.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_salesforce.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_salesforce.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_scrapinghub.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_scrapinghub.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_sftp.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_sftp.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_sharepoint.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_sharepoint.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_snowflake.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_snowflake.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/flow_helpers_tps/_time.py` & `flow_helpers_tps-2023.5.31.1939/flow_helpers_tps/_time.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.2.1540/PKG-INFO` & `flow_helpers_tps-2023.5.31.1939/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: flow-helpers-tps
-Version: 2023.5.2.1540
+Version: 2023.5.31.1939
 Summary: Handy helpers for ETL and API interfacing.
 License: MIT
 Author: joshliu3
 Author-email: jliu@theparkingspot.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Office365-REST-Python-Client (>=2.4.0,<3.0.0)
+Requires-Dist: Office365-REST-Python-Client (==2.3.3)
 Requires-Dist: SQLAlchemy (>=2.0.9,<3.0.0)
 Requires-Dist: boto3 (>=1.26.110,<2.0.0)
 Requires-Dist: facebook-business (>=16.0.2,<17.0.0)
 Requires-Dist: flatdict (==4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=2.85.0,<3.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

