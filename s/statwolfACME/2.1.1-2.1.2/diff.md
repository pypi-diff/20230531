# Comparing `tmp/statwolfACME-2.1.1-py2.py3-none-any.whl.zip` & `tmp/statwolfACME-2.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13665 bytes, number of entries: 10
--rw-r--r--  2.0 unx    18067 b- defN 23-Feb-06 08:57 ACME/ACME.py
--rw-r--r--  2.0 unx     3993 b- defN 23-Feb-06 08:57 ACME/ACME_anomaly_detection.py
--rw-r--r--  2.0 unx    15589 b- defN 23-Feb-06 08:57 ACME/ACME_function.py
--rw-r--r--  2.0 unx     8172 b- defN 23-Feb-06 08:57 ACME/ACME_plot.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-06 08:57 ACME/__init__.py
--rw-r--r--  2.0 unx      596 b- defN 23-Feb-06 08:57 ACME/utils.py
--rw-r--r--  2.0 unx      765 b- defN 23-Feb-06 09:00 statwolfACME-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-06 09:00 statwolfACME-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Feb-06 09:00 statwolfACME-2.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      766 b- defN 23-Feb-06 09:00 statwolfACME-2.1.1.dist-info/RECORD
-10 files, 48063 bytes uncompressed, 12369 bytes compressed:  74.3%
+Zip file size: 13669 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    18082 b- defN 23-May-31 14:59 ACME/ACME.py
+-rw-r--r--  2.0 unx     3993 b- defN 23-Feb-02 14:51 ACME/ACME_anomaly_detection.py
+-rw-r--r--  2.0 unx    15589 b- defN 23-Feb-06 08:58 ACME/ACME_function.py
+-rw-r--r--  2.0 unx     8172 b- defN 23-May-31 14:36 ACME/ACME_plot.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 08:44 ACME/__init__.py
+-rw-r--r--  2.0 unx      596 b- defN 23-Jan-31 08:44 ACME/utils.py
+-rw-r--r--  2.0 unx      765 b- defN 23-May-31 15:02 statwolfACME-2.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-31 15:02 statwolfACME-2.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-31 15:02 statwolfACME-2.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      766 b- defN 23-May-31 15:02 statwolfACME-2.1.2.dist-info/RECORD
+10 files, 48078 bytes uncompressed, 12373 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: ACME/__init__.py
 Comment: 
 
 Filename: ACME/utils.py
 Comment: 
 
-Filename: statwolfACME-2.1.1.dist-info/METADATA
+Filename: statwolfACME-2.1.2.dist-info/METADATA
 Comment: 
 
-Filename: statwolfACME-2.1.1.dist-info/WHEEL
+Filename: statwolfACME-2.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: statwolfACME-2.1.1.dist-info/top_level.txt
+Filename: statwolfACME-2.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: statwolfACME-2.1.1.dist-info/RECORD
+Filename: statwolfACME-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ACME/ACME.py

```diff
@@ -333,15 +333,15 @@
                 meta['index'] = self._local_explain['local_name']
                 meta['baseline'] = self._local_explain['baseline_pred']
             else:
                 table = self._global_explain['meta']
                 meta['local'] = False
 
             # prepare for the plotting
-            plot_df = table.sort_values('original').reset_index().rename(columns={'index':'feature'}).copy()
+            plot_df = table.sort_values(['importance','original']).reset_index().rename(columns={'index':'feature'}).copy()
 
             # if local set the refering x to the local values observation
             # for the global set to 0
             if local:
                 meta['x'] = table['baseline_prediction'].values[0]
             else: 
                 meta['x'] = 0
```

## Comparing `statwolfACME-2.1.1.dist-info/METADATA` & `statwolfACME-2.1.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statwolfACME
-Version: 2.1.1
+Version: 2.1.2
 Summary: ACME - Accelerated Model Explainability
 Home-page: https://github.com/dandolodavid/ACME
 Author: Dandolo David
 Author-email: dandolodavid@gmail.com
 License: BSD 4-clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

