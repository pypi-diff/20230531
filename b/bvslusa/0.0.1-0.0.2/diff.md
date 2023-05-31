# Comparing `tmp/bvslusa-0.0.1.tar.gz` & `tmp/bvslusa-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bvslusa-0.0.1.tar", last modified: Wed May 31 14:49:24 2023, max compression
+gzip compressed data, was "bvslusa-0.0.2.tar", last modified: Wed May 31 16:39:10 2023, max compression
```

## Comparing `bvslusa-0.0.1.tar` & `bvslusa-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-31 14:49:24.919937 bvslusa-0.0.1/
--rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 bvslusa-0.0.1/LICENSE
--rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-04-27 10:12:58.000000 bvslusa-0.0.1/MANIFEST.in
--rw-r--r--   0 joaonogueira   (501) staff       (20)     4782 2023-05-31 14:49:24.919788 bvslusa-0.0.1/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)     3994 2023-05-31 14:42:33.000000 bvslusa-0.0.1/README.md
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-31 14:49:24.918112 bvslusa-0.0.1/bvslusa/
--rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-05-31 14:44:36.000000 bvslusa-0.0.1/bvslusa/__init__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      787 2023-05-31 14:44:36.000000 bvslusa-0.0.1/bvslusa/_modidx.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      954 2023-05-31 14:44:36.000000 bvslusa-0.0.1/bvslusa/evaluate.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     1528 2023-05-31 14:44:36.000000 bvslusa-0.0.1/bvslusa/metrics.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      780 2023-05-31 14:44:36.000000 bvslusa-0.0.1/bvslusa/validate.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-31 14:49:24.919568 bvslusa-0.0.1/bvslusa.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)     4782 2023-05-31 14:49:24.000000 bvslusa-0.0.1/bvslusa.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      367 2023-05-31 14:49:24.000000 bvslusa-0.0.1/bvslusa.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-31 14:49:24.000000 bvslusa-0.0.1/bvslusa.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       36 2023-05-31 14:49:24.000000 bvslusa-0.0.1/bvslusa.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-31 13:42:09.000000 bvslusa-0.0.1/bvslusa.egg-info/not-zip-safe
--rw-r--r--   0 joaonogueira   (501) staff       (20)       42 2023-05-31 14:49:24.000000 bvslusa-0.0.1/bvslusa.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        8 2023-05-31 14:49:24.000000 bvslusa-0.0.1/bvslusa.egg-info/top_level.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)      988 2023-05-31 14:03:29.000000 bvslusa-0.0.1/settings.ini
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-31 14:49:24.919985 bvslusa-0.0.1/setup.cfg
--rw-rw-r--   0 joaonogueira   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 bvslusa-0.0.1/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-31 16:39:10.856897 bvslusa-0.0.2/
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 bvslusa-0.0.2/LICENSE
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-04-27 10:12:58.000000 bvslusa-0.0.2/MANIFEST.in
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     7443 2023-05-31 16:39:10.856732 bvslusa-0.0.2/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     6655 2023-05-31 16:24:47.000000 bvslusa-0.0.2/README.md
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-31 16:39:10.854883 bvslusa-0.0.2/bvslusa/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-05-31 16:34:09.000000 bvslusa-0.0.2/bvslusa/__init__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      903 2023-05-31 16:34:09.000000 bvslusa-0.0.2/bvslusa/_modidx.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      954 2023-05-31 16:34:09.000000 bvslusa-0.0.2/bvslusa/evaluate.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1528 2023-05-31 16:34:09.000000 bvslusa-0.0.2/bvslusa/metrics.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      709 2023-05-31 16:34:09.000000 bvslusa-0.0.2/bvslusa/ratings.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      780 2023-05-31 16:34:09.000000 bvslusa-0.0.2/bvslusa/validate.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-31 16:39:10.856505 bvslusa-0.0.2/bvslusa.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     7443 2023-05-31 16:39:10.000000 bvslusa-0.0.2/bvslusa.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      386 2023-05-31 16:39:10.000000 bvslusa-0.0.2/bvslusa.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-31 16:39:10.000000 bvslusa-0.0.2/bvslusa.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       36 2023-05-31 16:39:10.000000 bvslusa-0.0.2/bvslusa.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-31 13:42:09.000000 bvslusa-0.0.2/bvslusa.egg-info/not-zip-safe
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       53 2023-05-31 16:39:10.000000 bvslusa-0.0.2/bvslusa.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        8 2023-05-31 16:39:10.000000 bvslusa-0.0.2/bvslusa.egg-info/top_level.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      872 2023-05-31 16:34:09.000000 bvslusa-0.0.2/settings.ini
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-31 16:39:10.856944 bvslusa-0.0.2/setup.cfg
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 bvslusa-0.0.2/setup.py
```

### Comparing `bvslusa-0.0.1/LICENSE` & `bvslusa-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bvslusa-0.0.1/PKG-INFO` & `bvslusa-0.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: bvslusa
-Version: 0.0.1
-Summary: Functions to work with BVS enriched data
-Home-page: https://github.com/datarisk-io/bvslusa
-Author: João Nogueira
-Author-email: joao.nogueira@datarisk.io
-License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # bvslusa
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
 ``` sh
@@ -32,14 +10,15 @@
 
 ## How to use
 
 ``` python
 import pandas as pd
 from bvslusa.validate import remove_restritivos, target_mapping
 from bvslusa.evaluate import evaluate_bvs_scores
+from bvslusa.ratings import get_ratings
 ```
 
 ``` python
 df = pd.read_csv('../data/AVZA_FB727003.csv', sep=';')
 df
 ```
 
@@ -70,17 +49,17 @@
 | 35737 | 668323     | 202203 | 0        | 0       | 0       | 4            | 911         | 1               | 484          | 767          | 513          | 969          | 902          | MAU                  |
 | 35738 | 140483     | 202203 | 0        | 0       | 0       | 2            | 5285        | 1               | 487          | 767          | 531          | 956          | 131          | BOM                  |
 
 <p>35739 rows × 14 columns</p>
 </div>
 
 ``` python
-df.pipe(remove_restritivos) \
-    .pipe(target_mapping) \
-    .pipe(evaluate_bvs_scores)
+df = remove_restritivos(df)
+df = target_mapping(df, target='PERF_MERC_60D6M_EVER', map_dict={'BOM': 0, 'MAU': 1})
+df.pipe(evaluate_bvs_scores)
 ```
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
@@ -97,7 +76,49 @@
 | 0   | SCRCRDMERPJ5 | 0.694770 | 30.86 |
 | 1   | SCRCRDATACAD | 0.666147 | 28.28 |
 | 2   | SCRCRDMERMEI | 0.610453 | 19.22 |
 | 3   | SCRCRDMERPJ3 | 0.598126 | 16.93 |
 | 4   | SCRCRDMERPJ4 | 0.574876 | 13.56 |
 
 </div>
+
+As the SCRCRDMERPJ5 is the best bvs score, let’s proceed to build
+ratings with it:
+
+``` python
+df_ratings = get_ratings(df, target='PERF_MERC_60D6M_EVER', score='SCRCRDMERPJ5')
+```
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+&#10;    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+&#10;    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+
+|        | Bin               | Count | Count (%) | Non-event | Event | Event rate | WoE       | IV       | JS           |
+|--------|-------------------|-------|-----------|-----------|-------|------------|-----------|----------|--------------|
+| 0      | (-inf, 294.50)    | 3341  | 0.142900  | 2709      | 632   | 0.189165   | -0.892188 | 0.163145 | 1.974255e-02 |
+| 1      | \[294.50, 357.50) | 1336  | 0.057143  | 1107      | 229   | 0.171407   | -0.771947 | 0.046611 | 5.685828e-03 |
+| 2      | \[357.50, 405.50) | 1380  | 0.059025  | 1184      | 196   | 0.142029   | -0.549094 | 0.022291 | 2.751878e-03 |
+| 3      | \[405.50, 457.50) | 1469  | 0.062831  | 1299      | 170   | 0.115725   | -0.314082 | 0.007055 | 8.782459e-04 |
+| 4      | \[457.50, 491.50) | 1406  | 0.060137  | 1275      | 131   | 0.093172   | -0.072129 | 0.000322 | 4.028209e-05 |
+| 5      | \[491.50, 535.50) | 1547  | 0.066168  | 1413      | 134   | 0.086619   | 0.007997  | 0.000004 | 5.272191e-07 |
+| 6      | \[535.50, 570.50) | 1189  | 0.050855  | 1095      | 94    | 0.079058   | 0.107581  | 0.000563 | 7.034663e-05 |
+| 7      | \[570.50, 597.50) | 1276  | 0.054577  | 1200      | 76    | 0.059561   | 0.41171   | 0.007813 | 9.698149e-04 |
+| 8      | \[597.50, 629.50) | 1345  | 0.057528  | 1269      | 76    | 0.056506   | 0.467618  | 0.010386 | 1.286575e-03 |
+| 9      | \[629.50, 682.50) | 2340  | 0.100086  | 2223      | 117   | 0.050000   | 0.596806  | 0.027941 | 3.441700e-03 |
+| 10     | \[682.50, 748.50) | 3183  | 0.136142  | 3068      | 115   | 0.036129   | 0.936216  | 0.081821 | 9.869692e-03 |
+| 11     | \[748.50, inf)    | 3568  | 0.152609  | 3498      | 70    | 0.019619   | 1.563818  | 0.202677 | 2.303251e-02 |
+| 12     | Special           | 0     | 0.000000  | 0         | 0     | 0.000000   | 0.0       | 0.000000 | 0.000000e+00 |
+| 13     | Missing           | 0     | 0.000000  | 0         | 0     | 0.000000   | 0.0       | 0.000000 | 0.000000e+00 |
+| Totals |                   | 23380 | 1.000000  | 21340     | 2040  | 0.087254   |           | 0.570628 | 6.776995e-02 |
+
+</div>
+
+![](index_files/figure-commonmark/cell-5-output-2.png)
```

### Comparing `bvslusa-0.0.1/bvslusa/_modidx.py` & `bvslusa-0.0.2/bvslusa/_modidx.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,9 +3,10 @@
 d = { 'settings': { 'branch': 'master',
                 'doc_baseurl': '/bvslusa',
                 'doc_host': 'https://datarisk-io.github.io',
                 'git_url': 'https://github.com/datarisk-io/bvslusa',
                 'lib_path': 'bvslusa'},
   'syms': { 'bvslusa.evaluate': {'bvslusa.evaluate.evaluate_bvs_scores': ('evaluate.html#evaluate_bvs_scores', 'bvslusa/evaluate.py')},
             'bvslusa.metrics': {'bvslusa.metrics.ks_score': ('metrics.html#ks_score', 'bvslusa/metrics.py')},
+            'bvslusa.ratings': {'bvslusa.ratings.get_ratings': ('ratings.html#get_ratings', 'bvslusa/ratings.py')},
             'bvslusa.validate': { 'bvslusa.validate.remove_restritivos': ('validate.html#remove_restritivos', 'bvslusa/validate.py'),
                                   'bvslusa.validate.target_mapping': ('validate.html#target_mapping', 'bvslusa/validate.py')}}}
```

### Comparing `bvslusa-0.0.1/bvslusa/evaluate.py` & `bvslusa-0.0.2/bvslusa/evaluate.py`

 * *Files identical despite different names*

### Comparing `bvslusa-0.0.1/bvslusa/metrics.py` & `bvslusa-0.0.2/bvslusa/metrics.py`

 * *Files identical despite different names*

### Comparing `bvslusa-0.0.1/bvslusa/validate.py` & `bvslusa-0.0.2/bvslusa/validate.py`

 * *Files identical despite different names*

### Comparing `bvslusa-0.0.1/setup.py` & `bvslusa-0.0.2/setup.py`

 * *Files identical despite different names*

