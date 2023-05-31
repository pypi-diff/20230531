# Comparing `tmp/mb_pandas-1.0.202305301635-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202305311026-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9750 bytes, number of entries: 13
+Zip file size: 9924 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx      162 b- defN 23-May-25 03:48 mb_pandas/src/__init__.py
 -rw-rw-r--  2.0 unx     1612 b- defN 23-May-25 03:36 mb_pandas/src/aio.py
 -rw-rw-r--  2.0 unx      482 b- defN 23-May-25 03:36 mb_pandas/src/convert_data.py
 -rw-rw-r--  2.0 unx     3516 b- defN 23-May-29 10:17 mb_pandas/src/dfload.py
 -rw-rw-r--  2.0 unx     2418 b- defN 23-May-25 03:36 mb_pandas/src/profiler.py
--rw-rw-r--  2.0 unx     7226 b- defN 23-May-30 16:35 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-30 16:35 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1671 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1128 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.dist-info/RECORD
-13 files, 22620 bytes uncompressed, 7842 bytes compressed:  65.3%
+-rw-rw-r--  2.0 unx     7891 b- defN 23-May-31 10:26 mb_pandas/src/transform.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-31 10:26 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1671 b- defN 23-May-31 10:26 mb_pandas-1.0.202305311026.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-May-31 10:26 mb_pandas-1.0.202305311026.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-May-31 10:26 mb_pandas-1.0.202305311026.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-31 10:26 mb_pandas-1.0.202305311026.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-31 10:26 mb_pandas-1.0.202305311026.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1128 b- defN 23-May-31 10:26 mb_pandas-1.0.202305311026.dist-info/RECORD
+13 files, 23285 bytes uncompressed, 8016 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202305301635.data/scripts/df_profile
+Filename: mb_pandas-1.0.202305311026.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202305301635.data/scripts/df_view
+Filename: mb_pandas-1.0.202305311026.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202305301635.dist-info/METADATA
+Filename: mb_pandas-1.0.202305311026.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202305301635.dist-info/WHEEL
+Filename: mb_pandas-1.0.202305311026.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202305301635.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202305311026.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202305301635.dist-info/RECORD
+Filename: mb_pandas-1.0.202305311026.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/transform.py

```diff
@@ -45,14 +45,39 @@
     # for chunk in list_df:
     #     merged_chunk = pd.merge(df1,chunk,**kwargs)
     #     res = pd.concat([res, merged_chunk])
     
     # res = res.reset_index(drop=True)
     # return res
     
+ 
+def merge_dusk(df1,df2,logger=None,**kwargs):
+    """
+    Use dusk to merge 2 DataFrames
+    
+    Args:
+        df1 : First DataFrame : pandas DataFrame
+        df2 : Second DataFrame :  pandas DataFrame
+    Returns:
+        df : merged DataFrame : pandas DataFrame
+    """
+    
+    import dask.dataframe as dd
+    
+    #Convert pandas DataFrames to Dask DataFrames
+    ddf1 = dd.from_pandas(df1, npartitions=2)
+    ddf2 = dd.from_pandas(df2, npartitions=2)
+
+    # Merge Dask DataFrames
+    merged_ddf = dd.merge(ddf1, ddf2, **kwargs)
+
+    # Compute the result and convert back to a pandas DataFrame
+    merged_df = merged_ddf.compute()
+    return merged_df
+    
 
 def check_null(file_path,fillna=False,logger=None) -> pd.DataFrame:
     """
     Pandas file checker. Checks Null values
     Input: 
         file_path (csv): path to csv file
         fillna (bool): fillna with False
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
-VERSION_DAY = int('30')
-VERSION_HOUR = int('16')
-VERSION_MINUTE = int('35')
+VERSION_DAY = int('31')
+VERSION_HOUR = int('10')
+VERSION_MINUTE = int('26')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202305301635
-version_date = '2023/05/30 16:35'
+PATCH_VERSION = 202305311026
+version_date = '2023/05/31 10:26'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202305301635.data/scripts/df_profile` & `mb_pandas-1.0.202305311026.data/scripts/df_profile`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305301635.data/scripts/df_view` & `mb_pandas-1.0.202305311026.data/scripts/df_view`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305301635.dist-info/RECORD` & `mb_pandas-1.0.202305311026.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mb_pandas/src/__init__.py,sha256=WU80RSEXwgPXneLCZV_JyaMkKzAGEvYo9Icq0QzfBJE,162
 mb_pandas/src/aio.py,sha256=UK3o2TMFDeNQvhiFAulAyd1fKJPjrShEbK-Y-85tlsM,1612
 mb_pandas/src/convert_data.py,sha256=Wp1yDT9Ie-lBZGE7WmsMXB7nN3mv0MwbiloInr1aoc0,482
 mb_pandas/src/dfload.py,sha256=Yet5dq8R0NDi69UXiUAfQMwbWqhLRGjXqhUvJI5pBSw,3516
 mb_pandas/src/profiler.py,sha256=iX_nAksh-HzjyhQLnbutvEtNVGfVwja2CsQ1zaYZbeA,2418
-mb_pandas/src/transform.py,sha256=shaD06A5eZcPMy7YIncntPVC41sQf952gi9bIyAQC-w,7226
-mb_pandas/src/version.py,sha256=vHFiYS09rKHxsUto9h9shzKvxTq2DLZft_TUDCRJCbk,396
-mb_pandas-1.0.202305301635.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
-mb_pandas-1.0.202305301635.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
-mb_pandas-1.0.202305301635.dist-info/METADATA,sha256=l5k1E7HADdx7AzlfqE0TbM8xEQ3bIcjQxB1D2kelboM,224
-mb_pandas-1.0.202305301635.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_pandas-1.0.202305301635.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
-mb_pandas-1.0.202305301635.dist-info/RECORD,,
+mb_pandas/src/transform.py,sha256=-QTlxbHWLwuk5Ih2Z78CATcKwHqVKShvRLI9WRi7Jtc,7891
+mb_pandas/src/version.py,sha256=yppBZ8_8uWQG1_DNBOJlSQgaInetL1aencvjam_NnGM,396
+mb_pandas-1.0.202305311026.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
+mb_pandas-1.0.202305311026.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
+mb_pandas-1.0.202305311026.dist-info/METADATA,sha256=qr4lgf3eRSyvkOIl1hrL4y4z5lula3_s0qhZ1QYCUXw,224
+mb_pandas-1.0.202305311026.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_pandas-1.0.202305311026.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
+mb_pandas-1.0.202305311026.dist-info/RECORD,,
```

