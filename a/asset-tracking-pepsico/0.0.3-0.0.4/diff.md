# Comparing `tmp/asset_tracking_pepsico-0.0.3.tar.gz` & `tmp/asset_tracking_pepsico-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-0.0.3.tar", last modified: Wed May 31 09:51:42 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-0.0.4.tar", last modified: Wed May 31 12:43:04 2023, max compression
```

## Comparing `asset_tracking_pepsico-0.0.3.tar` & `asset_tracking_pepsico-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 09:51:42.993161 asset_tracking_pepsico-0.0.3/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.3/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-31 09:51:42.992600 asset_tracking_pepsico-0.0.3/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 asset_tracking_pepsico-0.0.3/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 09:51:42.987335 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6723 2023-05-31 09:44:20.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/asset_tracking_devicelogs.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     4792 2023-05-31 09:51:11.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/asset_tracking_ingest.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 09:51:42.991835 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     5772 2023-05-31 09:45:49.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/dto/PostgresSchema.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     3056 2023-05-30 12:33:32.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 09:51:42.990639 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 09:51:42.000000 asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 09:51:11.000000 asset_tracking_pepsico-0.0.3/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 09:51:42.993340 asset_tracking_pepsico-0.0.3/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 12:43:04.098533 asset_tracking_pepsico-0.0.4/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.4/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-31 12:43:04.097385 asset_tracking_pepsico-0.0.4/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 asset_tracking_pepsico-0.0.4/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 12:43:04.090556 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     4815 2023-05-31 12:41:12.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 12:43:04.095544 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     5772 2023-05-31 09:45:49.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     3056 2023-05-30 12:33:32.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 12:43:04.094869 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1585 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 12:43:04.000000 asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 12:42:01.000000 asset_tracking_pepsico-0.0.4/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 12:43:04.098885 asset_tracking_pepsico-0.0.4/setup.cfg
```

### Comparing `asset_tracking_pepsico-0.0.3/LICENSE` & `asset_tracking_pepsico-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.3/PKG-INFO` & `asset_tracking_pepsico-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset_tracking_pepsico
-Version: 0.0.3
+Version: 0.0.4
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.3/README.md` & `asset_tracking_pepsico-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/asset_tracking_devicelogs.py` & `asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/asset_tracking_devicelogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import traceback
-from dto.PostgresSchema import PostgresSchemaDto
+from asset_tracking_pepsico.dto.PostgresSchema import PostgresSchemaDto
 from datetime import datetime, timedelta
 import utilities
 
 
 class PostGresRepository:
 
     # convert the datetime string to extract date and time in the datetime format
```

### Comparing `asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/asset_tracking_ingest.py` & `asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/asset_tracking_ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import traceback
 import json
-from dto.PostgresSchema import PostgresSchemaDto
+from asset_tracking_pepsico.dto.PostgresSchema import PostgresSchemaDto
 import pandas as pd
 from datetime import datetime
 
 
 class AssetTrackingIngest:
     def __init__(self) -> None:
         self.stop_list = [',', '[', ']', '(', ')', '\n', ' ', '"']
```

### Comparing `asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.3/asset_tracking_pepsico/utilities.py` & `asset_tracking_pepsico-0.0.4/asset_tracking_pepsico/utilities.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.3/asset_tracking_pepsico.egg-info/PKG-INFO` & `asset_tracking_pepsico-0.0.4/asset_tracking_pepsico.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset-tracking-pepsico
-Version: 0.0.3
+Version: 0.0.4
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.3/pyproject.toml` & `asset_tracking_pepsico-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
```

