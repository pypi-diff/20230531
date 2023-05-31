# Comparing `tmp/ga4_data_import-0.1.1-py3-none-any.whl.zip` & `tmp/ga4_data_import-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 30850 bytes, number of entries: 9
+Zip file size: 30826 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 23:00 ga4_data_import/__init__.py
 -rw-r--r--  2.0 unx     1122 b- defN 23-May-24 20:59 ga4_data_import/common.py
--rw-r--r--  2.0 unx     8468 b- defN 23-May-31 11:20 ga4_data_import/compute.py
+-rw-r--r--  2.0 unx     8468 b- defN 23-May-31 13:49 ga4_data_import/compute.py
 -rw-r--r--  2.0 unx      891 b- defN 23-May-24 18:36 ga4_data_import/storage.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    42831 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      756 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/RECORD
-9 files, 89325 bytes uncompressed, 29538 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    42764 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      756 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/RECORD
+9 files, 89258 bytes uncompressed, 29514 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: ga4_data_import/compute.py
 Comment: 
 
 Filename: ga4_data_import/storage.py
 Comment: 
 
-Filename: ga4_data_import-0.1.1.dist-info/LICENSE
+Filename: ga4_data_import-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: ga4_data_import-0.1.1.dist-info/METADATA
+Filename: ga4_data_import-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: ga4_data_import-0.1.1.dist-info/WHEEL
+Filename: ga4_data_import-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: ga4_data_import-0.1.1.dist-info/top_level.txt
+Filename: ga4_data_import-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ga4_data_import-0.1.1.dist-info/RECORD
+Filename: ga4_data_import-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ga4_data_import-0.1.1.dist-info/LICENSE` & `ga4_data_import-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ga4_data_import-0.1.1.dist-info/METADATA` & `ga4_data_import-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ga4-data-import
-Version: 0.1.1
-Summary: Google Analytics 4 Data Import code samples
+Version: 0.1.2
+Summary: Google Analytics 4 Data Import pipeline
 Author-email: Max Ostapenko <ga4_data_import@maxostapenko.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -676,18 +676,17 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://www.maxostapenko.com/projects/ga4_data_import
 Project-URL: Bug Reports, https://github.com/max-ostapenko/ga4_data_import/issues
-Project-URL: Funding, https://maxostapenko.com/donate
-Project-URL: Say Thanks!, https://www.maxostapenko.com/sponsor
+Project-URL: Funding, https://maxostapenko.com/sponsor
 Project-URL: Source, https://github.com/max-ostapenko/ga4_data_import/
-Keywords: Google Analytics 4,Data Import,SFTP
+Keywords: Google Analytics 4,Data Import,SFTP,Google Cloud Storage
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -705,24 +704,23 @@
 Requires-Dist: build ; extra == 'dev'
 Requires-Dist: twine ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage ; extra == 'test'
 
 # Google Analytics 4 Data Import
 
-Automating data uploads from external sources to GA4
+Automated data imports pipeline to GA4
 
-## Import source - SFTP
 
-### Architecture diagram
+## Import source - Google Cloud Storage (via SFTP)
 
 <!-- markdownlint-disable-next-line MD033 -->
-![diagram](https://raw.githubusercontent.com/max-ostapenko/ga4_data_import/init-release/static/Google%20Analytics%204%20Data%20Import%20pipeline.png)
+<a href="https://colab.research.google.com/github/max-ostapenko/ga4_data_import/blob/main/scripts/GCS_to_GA4.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
-### Get started
+Google Colab is an easy to start thanks to its visual interface and Google-ready environment.
 
-<!-- markdownlint-disable-next-line MD033 -->
-<a href="https://colab.research.google.com/github/max-ostapenko/ga4_data_import/blob/main/GA4_Data_Import_from_Google_Cloud_Storage.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+Open it and follow the instructions to get a pipeline ready within a minute.
 
-## Development
+### Architecture diagram:
 
-Google Colab is used for operation due to notebook's visual interface and environment prepared for running code for Google services.
+<!-- markdownlint-disable-next-line MD033 -->
+![diagram](https://raw.githubusercontent.com/max-ostapenko/ga4_data_import/main/static/GCS_to_GA4%20Data%20Import%20pipeline.png)
```

