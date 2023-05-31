# Comparing `tmp/pandasklar-0.2.5.tar.gz` & `tmp/pandasklar-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasklar-0.2.5.tar", last modified: Wed Mar 15 10:54:01 2023, max compression
+gzip compressed data, was "pandasklar-0.3.1.tar", last modified: Wed May 31 19:38:45 2023, max compression
```

## Comparing `pandasklar-0.2.5.tar` & `pandasklar-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-03-15 10:54:01.467371 pandasklar-0.2.5/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.2.5/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)     9805 2023-03-15 10:54:01.467371 pandasklar-0.2.5/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     9297 2023-03-15 10:53:32.000000 pandasklar-0.2.5/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1301 2023-03-15 10:53:20.000000 pandasklar-0.2.5/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-03-15 10:54:01.467371 pandasklar-0.2.5/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-03-15 10:54:01.467371 pandasklar-0.2.5/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-03-15 10:54:01.467371 pandasklar-0.2.5/src/pandasklar/
--rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.2.5/src/pandasklar/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.2.5/src/pandasklar/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)    18166 2023-02-20 15:41:30.000000 pandasklar-0.2.5/src/pandasklar/aggregate.py
--rw-r--r--   0 me        (1000) me        (1000)    27390 2023-02-12 20:16:51.000000 pandasklar-0.2.5/src/pandasklar/analyse.py
--rw-r--r--   0 me        (1000) me        (1000)    10330 2023-02-12 20:17:03.000000 pandasklar-0.2.5/src/pandasklar/compare.py
--rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.2.5/src/pandasklar/config.py
--rw-r--r--   0 me        (1000) me        (1000)    26803 2023-02-20 15:41:11.000000 pandasklar-0.2.5/src/pandasklar/content.py
--rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.2.5/src/pandasklar/develop.py
--rw-r--r--   0 me        (1000) me        (1000)    32300 2023-03-15 09:45:06.000000 pandasklar-0.2.5/src/pandasklar/pandas.py
--rw-r--r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.2.5/src/pandasklar/plot.py
--rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.2.5/src/pandasklar/rank.py
--rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.2.5/src/pandasklar/scale.py
--rw-r--r--   0 me        (1000) me        (1000)     8718 2023-02-12 20:19:30.000000 pandasklar-0.2.5/src/pandasklar/string.py
--rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.2.5/src/pandasklar/subsets.py
--rw-r--r--   0 me        (1000) me        (1000)     5653 2022-11-09 21:26:08.000000 pandasklar-0.2.5/src/pandasklar/type_info.py
--rw-r--r--   0 me        (1000) me        (1000)     5467 2022-11-09 07:00:35.000000 pandasklar-0.2.5/src/pandasklar/values_info.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-03-15 10:54:01.467371 pandasklar-0.2.5/src/pandasklar.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     9805 2023-03-15 10:54:01.000000 pandasklar-0.2.5/src/pandasklar.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      677 2023-03-15 10:54:01.000000 pandasklar-0.2.5/src/pandasklar.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2023-03-15 10:54:01.000000 pandasklar-0.2.5/src/pandasklar.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       56 2023-03-15 10:54:01.000000 pandasklar-0.2.5/src/pandasklar.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       47 2023-03-15 10:54:01.000000 pandasklar-0.2.5/src/pandasklar.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)       11 2023-03-15 10:54:01.000000 pandasklar-0.2.5/src/pandasklar.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-31 19:38:45.489691 pandasklar-0.3.1/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.3.1/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)     9805 2023-05-31 19:38:45.489691 pandasklar-0.3.1/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     9297 2023-05-31 19:38:05.000000 pandasklar-0.3.1/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1301 2023-05-31 19:37:55.000000 pandasklar-0.3.1/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-05-31 19:38:45.489691 pandasklar-0.3.1/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-31 19:38:45.365693 pandasklar-0.3.1/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-31 19:38:45.481691 pandasklar-0.3.1/src/pandasklar/
+-rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.3.1/src/pandasklar/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.3.1/src/pandasklar/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)    19899 2023-05-12 20:23:55.000000 pandasklar-0.3.1/src/pandasklar/aggregate.py
+-rw-r--r--   0 me        (1000) me        (1000)    27540 2023-04-11 17:22:24.000000 pandasklar-0.3.1/src/pandasklar/analyse.py
+-rw-r--r--   0 me        (1000) me        (1000)    10330 2023-02-12 20:17:03.000000 pandasklar-0.3.1/src/pandasklar/compare.py
+-rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.3.1/src/pandasklar/config.py
+-rw-r--r--   0 me        (1000) me        (1000)    26803 2023-02-20 15:41:11.000000 pandasklar-0.3.1/src/pandasklar/content.py
+-rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.3.1/src/pandasklar/develop.py
+-rw-r--r--   0 me        (1000) me        (1000)    32239 2023-03-16 08:54:51.000000 pandasklar-0.3.1/src/pandasklar/pandas.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.3.1/src/pandasklar/plot.py
+-rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.3.1/src/pandasklar/rank.py
+-rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.3.1/src/pandasklar/scale.py
+-rw-r--r--   0 me        (1000) me        (1000)     8975 2023-04-10 20:10:39.000000 pandasklar-0.3.1/src/pandasklar/string.py
+-rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.3.1/src/pandasklar/subsets.py
+-rw-r--r--   0 me        (1000) me        (1000)     5653 2022-11-09 21:26:08.000000 pandasklar-0.3.1/src/pandasklar/type_info.py
+-rw-r--r--   0 me        (1000) me        (1000)     5467 2022-11-09 07:00:35.000000 pandasklar-0.3.1/src/pandasklar/values_info.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-31 19:38:45.489691 pandasklar-0.3.1/src/pandasklar.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)     9805 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      677 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       56 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       47 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)       11 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/top_level.txt
```

### Comparing `pandasklar-0.2.5/LICENSE` & `pandasklar-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/PKG-INFO` & `pandasklar-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.2.5
+Version: 0.3.1
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandasklar-0.2.5/README.md` & `pandasklar-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/pyproject.toml` & `pandasklar-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyproject.toml
 
 
 [project]
 name            = "pandasklar"
-version         = "0.2.5"    
+version         = "0.3.1"    
 
 requires-python = ">=3.8"
 dependencies    = ['pandas','numpy','perlin_noise','termcolor','bpyth','blab',]
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
 description     = "Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL."
 readme          = "README.md"
```

### Comparing `pandasklar-0.2.5/src/pandasklar/__init__.py` & `pandasklar-0.3.1/src/pandasklar/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/aggregate.py` & `pandasklar-0.3.1/src/pandasklar/aggregate.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,35 +6,97 @@
 import numpy  as np
 import bpyth  as bpy
    
 from collections import Counter, defaultdict 
 
 from .config     import Config
 from .pandas     import dataframe, reset_index, drop_cols, rename_col, move_cols, drop_multiindex, quicksample, add_rows, move_rows
+from .rank       import rank
 from .type_info  import type_info
 
 
+
 ###############################################################################################
 # .............................................................................................
 # Aggregation ...
 # .............................................................................................
 ###############################################################################################
 
 
+
+def partial_pivot( df, col_pivot=None, col_score=None, cols_group=None,  width_max=None):
+    
+    result = df.copy()
+        
+    # col_score
+    if col_score is None:
+        col_score = 'temp_score_gRwdnr'
+        result[col_score] = 0
+    result[col_score] = result[col_score].fillna(result[col_score].min()-1 )
+    
+    # cols_group
+    if cols_group is None:
+        cols_group = [ c for c in list(result.columns) if c != col_score and c != col_pivot ]
+    elif type(cols_group) is str:
+        cols_group = [cols_group] #let the command take a string or list          
+    
+    # isnull
+    if result.isnull().values.any():
+        raise ValueError('Works without NaNs only')
+    
+    # ranken
+    result = rank(result, col_score=col_score, cols_group=cols_group, col_target='pivot_rank', verbose=False)
+
+    # max_i
+    max_i = result.pivot_rank.max()
+    if width_max is not None and width_max < max_i:
+        max_i = width_max
+    
+    # group_and_agg vorbereiten
+    col_origins = cols_group.copy()    
+    col_funcs   = [''] * len(col_origins)
+    col_names   = [''] * len(col_origins)    
+    
+    # eintragen
+    for i in range(0,max_i):
+        #print(i)
+        c = col_pivot + '_' + str(i)
+        col_origins += [c]
+        col_funcs   += ['first']    
+        col_names   += [c]               
+        mask = result.pivot_rank == i+1
+        result.loc[mask,c] = result[mask][col_pivot]
+
+
+    result = group_and_agg( result, col_origins, col_funcs, col_names, verbose=False)
+
+    return result
+
+
+
+
+
+
+
+
+
+
+
 def group_and_agg(df, col_origins, col_funcs=None, col_names=None, dropna=True, optimize=False, verbose=None): 
     '''
     Groups and aggregates. Provides a user interface similar to that of MS Access.
     * col_origins: list of all columns to process
     * col_funcs:   list of all functions to apply to the columns above. 
                    Sometimes you have to use strings, sometimes function names.
                    'group' or '' = grouping. 
     * col_names:   list of new names for the result columns. Optional. Space = default name will be taken.
     * dropna:      Parameter for groupby.
     * optimize:    True to handle duplicated rows seperatly. 
                    Useful in situations with not many duplicated rows and slow functions in col_funcs.
+                   There is a known bug with default names with optimize=True, you should use col_names explicitly for col_funcs other than 'group'.
     
     Example:
     df = pak.people()
     pak.group_and_agg( df, 
                        col_origins=['age_class', 'birthplace', 'first_name',  'age', 'age', 'first_name'],
                        col_funcs  =['group',     'group',      pak.agg_words, 'min', 'max', 'min'],
                  )    
@@ -69,16 +131,16 @@
     reihenfolge = list(steuer.name_new)
 
     if col_names:
         mask = (steuer['col_names'].str.len() == 0)
         steuer.loc[mask,'col_names'] = steuer[mask].name_new # Standardnamen übernehmen
         
     if optimize:
-        if df.isnull().values.any():
-            raise ValueError('Works without NaNs only')
+        if df[col_origins].isnull().values.any():
+            raise ValueError('Works without NaNs in col_origins only')
         mask = df.duplicated(subset=cols_group, keep=False)
         df_unique, df_withdups = move_rows(df, mask, msg=None, verbose=False)
         if verbose:
             print( '{0} unique rows and {1} rows with duplicates'.format(df_unique.shape[0] , df_withdups.shape[0])  )
         assert df_unique.shape[0] + df_withdups.shape[0] == df.shape[0]
         result = group_and_agg( df_withdups, col_origins=col_origins, col_funcs=col_funcs, col_names=col_names, dropna=dropna, optimize=False, verbose=False)
         result = add_rows(result,df_unique[col_origins],verbose=False)
```

### Comparing `pandasklar-0.2.5/src/pandasklar/analyse.py` & `pandasklar-0.3.1/src/pandasklar/analyse.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     changedatatype:       Should the datatypes get optimized?
     verbose:              True if messages are wanted.
     '''
     
     if verbose is None:
         verbose = Config.get('VERBOSE')  
         
-    result = bpy.load_pickle(filename)
+    result = pd.read_pickle(filename)
     if resetindex == True:
         result = result.reset_index()
     elif resetindex == 'AUTO':
         result = result.reset_index()    
         result = drop_cols(result, 'index')       
     
     if changedatatype:     
@@ -68,16 +68,25 @@
     '''
     
     if verbose is None:
         verbose = Config.get('VERBOSE')  
         
     if changedatatype:       
         df = change_datatype(df, verbose=False)
-    bpy.dump_pickle(df,filename)
+        
+    pd.to_pickle(df,filename)    
+    
+    if verbose:
+        print(df.shape[0], 'rows written')      
+    
+        
 
+to_pickle   = dump_pickle
+read_pickle = load_pickle
+    
     
     
     
 #################################################################################
 # ...............................................................................
 # Spalten auf datatype untersuchen
 # ...............................................................................
```

### Comparing `pandasklar-0.2.5/src/pandasklar/compare.py` & `pandasklar-0.3.1/src/pandasklar/compare.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/config.py` & `pandasklar-0.3.1/src/pandasklar/config.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/content.py` & `pandasklar-0.3.1/src/pandasklar/content.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/develop.py` & `pandasklar-0.3.1/src/pandasklar/develop.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/pandas.py` & `pandasklar-0.3.1/src/pandasklar/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,15 @@
         elif cond == 'null':
             mask = result[col_new].notnull()   &   (  result[col_rename].isnull()   |   (result[col_rename]=='')   )        
         else:         
             mask = result[col_new].notnull() 
         if verbose:
             print('update_col:', result[mask].shape[0], 'cells written into existing column')
         with warnings.catch_warnings():
-            warnings.simplefilter(action='ignore', category=FutureWarning)   
+            warnings.simplefilter('ignore')    
             result.loc[mask, col_rename] = result.loc[mask, col_new]
         result = copy_datatype( result, df_to )    # datatypes restaurieren               
         #result[col_rename] = copy_datatype( result[col_rename], df_to[col_rename] )    # datatype restaurieren
         result = drop_cols(result,[col_new])
         result_mask = mask.copy()
     
     # Die Spalte ist neu
@@ -348,15 +348,15 @@
         result_mask = result[col_rename].notnull()
         if verbose:
             print('update_col:', result[result_mask].shape[0], 'cells written into new column')        
     
     if keep:
         mask = result[col_rename+keep] == result[col_rename]
         with warnings.catch_warnings():
-            warnings.simplefilter(action='ignore', category=FutureWarning)           
+            warnings.simplefilter('ignore')           
             result.loc[mask,col_rename+keep] = np.NaN
         
     if df_to.shape[0] != result.shape[0]:
         print('update_col:','WARNING: df_from identifier not unique.','I call this again with func="max"')
         return update_col(df_to, df_from, left_on=left_on, right_on=right_on, col=col, col_rename=col_rename, func='max', keep=keep, verbose=verbose)
     
     if return_mask:
```

### Comparing `pandasklar-0.2.5/src/pandasklar/plot.py` & `pandasklar-0.3.1/src/pandasklar/plot.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/rank.py` & `pandasklar-0.3.1/src/pandasklar/rank.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/scale.py` & `pandasklar-0.3.1/src/pandasklar/scale.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/string.py` & `pandasklar-0.3.1/src/pandasklar/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     Removes a list of unwanted substrings from a Series of strings.
     * remove_list: list of substrings to remove
     * safemode:    Selects the algorithm.
                    safemode=True:  Each substring is removed separately
                    safemode=False: Works with one regular expression.
                                    Special characters such as asterisks must be backslashed.    
     '''
+    
+    # sort by len
+    remove_list = sorted(remove_list, key=len, reverse=True)
+    
     if safemode:
         for r in remove_list:
             series = series.str.replace(r, '', regex=False)
         return series.str.strip()    
     
     else:
         remove_list = [re.escape(w) for w in remove_list]
@@ -41,14 +45,17 @@
     
     
 def remove_words(series, remove_list):
     '''
     Removes a list of unwanted words from a Series of strings.
     Works by regular expression, so special characters such as asterisks must be backslashed.  
     '''
+    # sort by len
+    remove_list = sorted(remove_list, key=len, reverse=True)
+    
     pat = r'\b(?:{})\b'.format('|'.join(remove_list))   # 
     return series.str.replace( pat, '', regex=True ).str.strip()        
     
     
     
 def replace_str(series, translationtable):
     '''
@@ -187,24 +194,26 @@
     
     # startswith alternative, works only if all strings in searchme have the same length. Also returns the matching fragment
     def startwiths(data, searchme, find_identical):
         prefix = searchme[bisect_right(searchme, data)-1]
         if ((data!=prefix) or find_identical ) and data.startswith(prefix): 
             return prefix    
     
+
     search = pd.DataFrame(searchfor)
     search.columns = ['searchstring'] 
     search['len'] = search.searchstring.str.len()
     grouped = search.groupby('len')
     lengroups = grouped.agg(list).reset_index().sort_values('len', ascending=find_longest)  
     result = df.copy()
     result[col_found] = None
- 
-    for index, row in lengroups.iterrows():
-        result[col_found].update(result[col_search].apply(startwiths, searchme=sorted(row.searchstring), find_identical=find_identical)  )  
+        
+    with pd.option_context("mode.copy_on_write", False):           
+        for index, row in lengroups.iterrows():
+            result[col_found].update(result[col_search].apply(startwiths, searchme=sorted(row.searchstring), find_identical=find_identical)  )  
         
     result[col_found] = result[col_found].astype('string')    
     return result
```

### Comparing `pandasklar-0.2.5/src/pandasklar/subsets.py` & `pandasklar-0.3.1/src/pandasklar/subsets.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/type_info.py` & `pandasklar-0.3.1/src/pandasklar/type_info.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar/values_info.py` & `pandasklar-0.3.1/src/pandasklar/values_info.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.2.5/src/pandasklar.egg-info/PKG-INFO` & `pandasklar-0.3.1/src/pandasklar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.2.5
+Version: 0.3.1
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandasklar-0.2.5/src/pandasklar.egg-info/SOURCES.txt` & `pandasklar-0.3.1/src/pandasklar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

