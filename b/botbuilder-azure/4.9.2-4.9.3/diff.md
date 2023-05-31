# Comparing `tmp/botbuilder_azure-4.9.2-py3-none-any.whl.zip` & `tmp/botbuilder_azure-4.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 11648 bytes, number of entries: 9
--rw-r--r--  2.0 unx      824 b- defN 20-Jul-13 23:01 botbuilder/azure/__init__.py
--rw-r--r--  2.0 unx      481 b- defN 20-Jul-13 23:01 botbuilder/azure/about.py
--rw-r--r--  2.0 unx     4082 b- defN 20-Jul-13 23:01 botbuilder/azure/blob_storage.py
--rw-r--r--  2.0 unx    12403 b- defN 20-Jul-13 23:01 botbuilder/azure/cosmosdb_partitioned_storage.py
--rw-r--r--  2.0 unx    13228 b- defN 20-Jul-13 23:01 botbuilder/azure/cosmosdb_storage.py
--rw-r--r--  2.0 unx     3897 b- defN 20-Jul-13 23:03 botbuilder_azure-4.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Jul-13 23:03 botbuilder_azure-4.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 20-Jul-13 23:03 botbuilder_azure-4.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      788 b- defN 20-Jul-13 23:03 botbuilder_azure-4.9.2.dist-info/RECORD
+-rw-r--r--  2.0 unx      824 b- defN 20-Dec-04 01:46 botbuilder/azure/__init__.py
+-rw-r--r--  2.0 unx      481 b- defN 20-Dec-04 01:46 botbuilder/azure/about.py
+-rw-r--r--  2.0 unx     4082 b- defN 20-Dec-04 01:46 botbuilder/azure/blob_storage.py
+-rw-r--r--  2.0 unx    12403 b- defN 20-Dec-04 01:46 botbuilder/azure/cosmosdb_partitioned_storage.py
+-rw-r--r--  2.0 unx    13228 b- defN 20-Dec-04 01:46 botbuilder/azure/cosmosdb_storage.py
+-rw-r--r--  2.0 unx     3897 b- defN 20-Dec-04 01:48 botbuilder_azure-4.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 20-Dec-04 01:48 botbuilder_azure-4.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 20-Dec-04 01:48 botbuilder_azure-4.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      788 b- defN 20-Dec-04 01:48 botbuilder_azure-4.9.3.dist-info/RECORD
 9 files, 35806 bytes uncompressed, 10276 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: botbuilder/azure/cosmosdb_partitioned_storage.py
 Comment: 
 
 Filename: botbuilder/azure/cosmosdb_storage.py
 Comment: 
 
-Filename: botbuilder_azure-4.9.2.dist-info/METADATA
+Filename: botbuilder_azure-4.9.3.dist-info/METADATA
 Comment: 
 
-Filename: botbuilder_azure-4.9.2.dist-info/WHEEL
+Filename: botbuilder_azure-4.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: botbuilder_azure-4.9.2.dist-info/top_level.txt
+Filename: botbuilder_azure-4.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: botbuilder_azure-4.9.2.dist-info/RECORD
+Filename: botbuilder_azure-4.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `botbuilder_azure-4.9.2.dist-info/METADATA` & `botbuilder_azure-4.9.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botbuilder-azure
-Version: 4.9.2
+Version: 4.9.3
 Summary: Microsoft Bot Framework Bot Builder
 Home-page: https://www.github.com/Microsoft/botbuilder-python
 Author: Microsoft
 License: MIT
 Keywords: BotBuilderAzure,bots,ai,botframework,botbuilder,azure
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `botbuilder_azure-4.9.2.dist-info/RECORD` & `botbuilder_azure-4.9.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 botbuilder/azure/__init__.py,sha256=GMnwbK-UfjhELh9Y2xBpM4yREBaiN1asA0LVjUJ37uk,824
 botbuilder/azure/about.py,sha256=iJH6M1Vt92FzjfLsLDA03UXdKWV5voNj9GzSVV6h1LQ,481
 botbuilder/azure/blob_storage.py,sha256=Evgmb1jTbj92HV2whtR6-1YsAwaNGQ2SEcrFVo8Mkew,4082
 botbuilder/azure/cosmosdb_partitioned_storage.py,sha256=3QkSIOzvfxbfv8pnzGWyRNMaWvVrF_1C2juyIoPRFLM,12403
 botbuilder/azure/cosmosdb_storage.py,sha256=mwlzytMYW5eeur-bmDyhoLlqnvYp2sVGwGwofegIupY,13228
-botbuilder_azure-4.9.2.dist-info/METADATA,sha256=oxc3DxaCE42oD4JPmDT0DFVpaMfMKCPSbotVjB5mEY4,3897
-botbuilder_azure-4.9.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-botbuilder_azure-4.9.2.dist-info/top_level.txt,sha256=2p3tapzF5j-vDQrnQjnuJZvvXStR_qu8i9Tqq-0ThZg,11
-botbuilder_azure-4.9.2.dist-info/RECORD,,
+botbuilder_azure-4.9.3.dist-info/METADATA,sha256=uj1YSj1km31Cc23Ah5vl3JLrkYThb8qhPwmQFWaNFRg,3897
+botbuilder_azure-4.9.3.dist-info/WHEEL,sha256=gm79cMopkncyn0iSnI0vQNiDJ8t9on0H4_iz-CrpXMk,92
+botbuilder_azure-4.9.3.dist-info/top_level.txt,sha256=2p3tapzF5j-vDQrnQjnuJZvvXStR_qu8i9Tqq-0ThZg,11
+botbuilder_azure-4.9.3.dist-info/RECORD,,
```

