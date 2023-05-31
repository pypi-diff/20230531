# Comparing `tmp/mb_pandas-1.0.202305311044-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202305311045-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9951 bytes, number of entries: 13
+Zip file size: 9954 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx      162 b- defN 23-May-25 03:48 mb_pandas/src/__init__.py
 -rw-rw-r--  2.0 unx     1612 b- defN 23-May-25 03:36 mb_pandas/src/aio.py
 -rw-rw-r--  2.0 unx      482 b- defN 23-May-25 03:36 mb_pandas/src/convert_data.py
 -rw-rw-r--  2.0 unx     3516 b- defN 23-May-29 10:17 mb_pandas/src/dfload.py
 -rw-rw-r--  2.0 unx     2418 b- defN 23-May-25 03:36 mb_pandas/src/profiler.py
--rw-rw-r--  2.0 unx     8071 b- defN 23-May-31 10:30 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-31 10:44 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1671 b- defN 23-May-31 10:44 mb_pandas-1.0.202305311044.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-May-31 10:44 mb_pandas-1.0.202305311044.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-May-31 10:44 mb_pandas-1.0.202305311044.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-31 10:44 mb_pandas-1.0.202305311044.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-31 10:44 mb_pandas-1.0.202305311044.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1128 b- defN 23-May-31 10:44 mb_pandas-1.0.202305311044.dist-info/RECORD
-13 files, 23465 bytes uncompressed, 8043 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx     8084 b- defN 23-May-31 10:45 mb_pandas/src/transform.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-31 10:45 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1671 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1128 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.dist-info/RECORD
+13 files, 23478 bytes uncompressed, 8046 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202305311044.data/scripts/df_profile
+Filename: mb_pandas-1.0.202305311045.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202305311044.data/scripts/df_view
+Filename: mb_pandas-1.0.202305311045.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202305311044.dist-info/METADATA
+Filename: mb_pandas-1.0.202305311045.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202305311044.dist-info/WHEEL
+Filename: mb_pandas-1.0.202305311045.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202305311044.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202305311045.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202305311044.dist-info/RECORD
+Filename: mb_pandas-1.0.202305311045.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/transform.py

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 import os
 from .dfload import load_any_df
 from mb_utils.src.logging import logger
 import numpy as np
 import cv2
 
-__all__ = ['check_null','remove_unnamed','rename_columns','check_drop_duplicates','get_dftype','merge_chunk']
+__all__ = ['check_null','remove_unnamed','rename_columns','check_drop_duplicates','get_dftype','merge_chunk','merge_dask']
 
 def merge_chunk(df1,df2,chunksize=10000,logger=None,**kwargs):
     """
     Merging 2 DataFrames in chunks
     
     Args:
         df1 : First DataFrame
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
 VERSION_DAY = int('31')
 VERSION_HOUR = int('10')
-VERSION_MINUTE = int('44')
+VERSION_MINUTE = int('45')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202305311044
-version_date = '2023/05/31 10:44'
+PATCH_VERSION = 202305311045
+version_date = '2023/05/31 10:45'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202305311044.data/scripts/df_profile` & `mb_pandas-1.0.202305311045.data/scripts/df_profile`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305311044.data/scripts/df_view` & `mb_pandas-1.0.202305311045.data/scripts/df_view`

 * *Files identical despite different names*

