# Comparing `tmp/CndIO-2.3.1-py3-none-any.whl.zip` & `tmp/CndIO-2.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5480 bytes, number of entries: 11
--rw-rw-rw-  2.0 unx        5 b- defN 22-Nov-11 21:55 cnd_io/VERSION
--rw-r--r--  2.0 unx      281 b- defN 22-Nov-11 21:55 cnd_io/__init__.py
--rw-r--r--  2.0 unx      115 b- defN 22-Nov-11 21:55 cnd_io/__version__.py
--rw-r--r--  2.0 unx     2815 b- defN 22-Nov-11 21:55 cnd_io/cnd_io.py
--rw-r--r--  2.0 unx      826 b- defN 22-Nov-11 21:55 cnd_io/cnd_provider.py
--rw-r--r--  2.0 unx     3935 b- defN 22-Nov-11 21:55 cnd_io/cnd_provider_gitlab.py
--rw-r--r--  2.0 unx     1316 b- defN 22-Nov-11 21:55 cnd_io/cnd_provider_localfile.py
--rw-r--r--  2.0 unx     2312 b- defN 22-Nov-11 21:55 CndIO-2.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-11 21:55 CndIO-2.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Nov-11 21:55 CndIO-2.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      834 b- defN 22-Nov-11 21:55 CndIO-2.3.1.dist-info/RECORD
-11 files, 12538 bytes uncompressed, 4078 bytes compressed:  67.5%
+Zip file size: 5483 bytes, number of entries: 11
+-rw-rw-rw-  2.0 unx        5 b- defN 23-May-31 13:54 cnd_io/VERSION
+-rw-r--r--  2.0 unx      281 b- defN 23-May-31 13:54 cnd_io/__init__.py
+-rw-r--r--  2.0 unx      115 b- defN 23-May-31 13:54 cnd_io/__version__.py
+-rw-r--r--  2.0 unx     2815 b- defN 23-May-31 13:54 cnd_io/cnd_io.py
+-rw-r--r--  2.0 unx      826 b- defN 23-May-31 13:54 cnd_io/cnd_provider.py
+-rw-r--r--  2.0 unx     3935 b- defN 23-May-31 13:54 cnd_io/cnd_provider_gitlab.py
+-rw-r--r--  2.0 unx     1316 b- defN 23-May-31 13:54 cnd_io/cnd_provider_localfile.py
+-rw-r--r--  2.0 unx     2312 b- defN 23-May-31 13:55 CndIO-2.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 13:55 CndIO-2.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-31 13:55 CndIO-2.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      834 b- defN 23-May-31 13:55 CndIO-2.4.0.dist-info/RECORD
+11 files, 12538 bytes uncompressed, 4081 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: cnd_io/cnd_provider_gitlab.py
 Comment: 
 
 Filename: cnd_io/cnd_provider_localfile.py
 Comment: 
 
-Filename: CndIO-2.3.1.dist-info/METADATA
+Filename: CndIO-2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: CndIO-2.3.1.dist-info/WHEEL
+Filename: CndIO-2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: CndIO-2.3.1.dist-info/top_level.txt
+Filename: CndIO-2.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: CndIO-2.3.1.dist-info/RECORD
+Filename: CndIO-2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cnd_io/VERSION

```diff
@@ -1 +1 @@
-2.3.1
+2.4.0
```

## Comparing `CndIO-2.3.1.dist-info/METADATA` & `CndIO-2.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CndIO
-Version: 2.3.1
+Version: 2.4.0
 Summary: Tools to manage In/Out file. Easy to add new class if you need to change source/dest (file system, git ...)
 Home-page: https://gitlab.com/changendevops/cnd-io
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/cnd-io
```

## Comparing `CndIO-2.3.1.dist-info/RECORD` & `CndIO-2.4.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-cnd_io/VERSION,sha256=QMnqu9l4CYa9yCw7RU8htd5EvSML5ilMjcX4DRH03cE,5
+cnd_io/VERSION,sha256=B7cWS4CxDuWfVq1kZeO2ws8Se_7Cb8K3FjgCCxnX9cg,5
 cnd_io/__init__.py,sha256=_M8DOMUI0QFx5X2_qdsK6NIabPYVaFt6G77tP6b5hp8,281
 cnd_io/__version__.py,sha256=vGgcW_O68DrnmB0JEdhl_fntMiwF806WHENuxgDDraQ,115
 cnd_io/cnd_io.py,sha256=HfH4FG8c7T4Z72Wy0lL1JdeYN-2NWpF-rnC7YsqlgAw,2815
 cnd_io/cnd_provider.py,sha256=53rhtSvZ-u5IMUUqzhCLyUVpsDS7bGQ_DDMt90O_m44,826
 cnd_io/cnd_provider_gitlab.py,sha256=nUd-evvKPeimbL3ypox4hYvNe_1cozVCunFhrnFMu5c,3935
 cnd_io/cnd_provider_localfile.py,sha256=Ohn-_JfrpNbiZl21dlgyWhFyAA7QVVieduI4tRrc5fI,1316
-CndIO-2.3.1.dist-info/METADATA,sha256=0odJnSerWvRhW_QIqXh2JSj53KTyfAmaW0Y1Ko93iF4,2312
-CndIO-2.3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-CndIO-2.3.1.dist-info/top_level.txt,sha256=5ODHl5RPET5r26bYiWP5GzZrzSNpp8FBDOIz_sNmrBk,7
-CndIO-2.3.1.dist-info/RECORD,,
+CndIO-2.4.0.dist-info/METADATA,sha256=BX8zaGm85ynzAZlG8RHKsVqRAjp4Lgl5p0F7Ce01HFo,2312
+CndIO-2.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+CndIO-2.4.0.dist-info/top_level.txt,sha256=5ODHl5RPET5r26bYiWP5GzZrzSNpp8FBDOIz_sNmrBk,7
+CndIO-2.4.0.dist-info/RECORD,,
```

