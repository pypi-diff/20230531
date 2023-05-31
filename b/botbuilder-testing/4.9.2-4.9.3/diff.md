# Comparing `tmp/botbuilder_testing-4.9.2-py3-none-any.whl.zip` & `tmp/botbuilder_testing-4.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9217 bytes, number of entries: 9
--rw-r--r--  2.0 unx      315 b- defN 20-Jul-13 23:01 botbuilder/testing/__init__.py
--rw-r--r--  2.0 unx      485 b- defN 20-Jul-13 23:01 botbuilder/testing/about.py
--rw-r--r--  2.0 unx     4920 b- defN 20-Jul-13 23:01 botbuilder/testing/dialog_test_client.py
--rw-r--r--  2.0 unx     3786 b- defN 20-Jul-13 23:01 botbuilder/testing/dialog_test_logger.py
--rw-r--r--  2.0 unx    12142 b- defN 20-Jul-13 23:01 botbuilder/testing/storage_base_tests.py
--rw-r--r--  2.0 unx     3872 b- defN 20-Jul-13 23:03 botbuilder_testing-4.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Jul-13 23:03 botbuilder_testing-4.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 20-Jul-13 23:03 botbuilder_testing-4.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      803 b- defN 20-Jul-13 23:03 botbuilder_testing-4.9.2.dist-info/RECORD
-9 files, 26426 bytes uncompressed, 7813 bytes compressed:  70.4%
+Zip file size: 9219 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      315 b- defN 20-Dec-04 01:46 botbuilder/testing/__init__.py
+-rw-r--r--  2.0 unx      485 b- defN 20-Dec-04 01:46 botbuilder/testing/about.py
+-rw-r--r--  2.0 unx     4920 b- defN 20-Dec-04 01:46 botbuilder/testing/dialog_test_client.py
+-rw-r--r--  2.0 unx     3786 b- defN 20-Dec-04 01:46 botbuilder/testing/dialog_test_logger.py
+-rw-r--r--  2.0 unx    12142 b- defN 20-Dec-04 01:46 botbuilder/testing/storage_base_tests.py
+-rw-r--r--  2.0 unx     3872 b- defN 20-Dec-04 01:48 botbuilder_testing-4.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 20-Dec-04 01:48 botbuilder_testing-4.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 20-Dec-04 01:48 botbuilder_testing-4.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      803 b- defN 20-Dec-04 01:48 botbuilder_testing-4.9.3.dist-info/RECORD
+9 files, 26426 bytes uncompressed, 7815 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: botbuilder/testing/dialog_test_logger.py
 Comment: 
 
 Filename: botbuilder/testing/storage_base_tests.py
 Comment: 
 
-Filename: botbuilder_testing-4.9.2.dist-info/METADATA
+Filename: botbuilder_testing-4.9.3.dist-info/METADATA
 Comment: 
 
-Filename: botbuilder_testing-4.9.2.dist-info/WHEEL
+Filename: botbuilder_testing-4.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: botbuilder_testing-4.9.2.dist-info/top_level.txt
+Filename: botbuilder_testing-4.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: botbuilder_testing-4.9.2.dist-info/RECORD
+Filename: botbuilder_testing-4.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `botbuilder_testing-4.9.2.dist-info/METADATA` & `botbuilder_testing-4.9.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botbuilder-testing
-Version: 4.9.2
+Version: 4.9.3
 Summary: Microsoft Bot Framework Bot Builder
 Home-page: https://www.github.com/Microsoft/botbuilder-python
 Author: Microsoft
 License: MIT
 Keywords: botbuilder-testing bots ai testing botframework botbuilder
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `botbuilder_testing-4.9.2.dist-info/RECORD` & `botbuilder_testing-4.9.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 botbuilder/testing/__init__.py,sha256=u8FNpTA0RtzZBUyddhX1BTS9xNcD1mnE-BIlm-S_zsM,315
 botbuilder/testing/about.py,sha256=ldd7Ys_lhgkTT2x-BlVYyGzEcJ3Fn34XLf4_WcakavM,485
 botbuilder/testing/dialog_test_client.py,sha256=GLP2VV4AkgLnC1gqCSfY1w9bnBeP3PQ58RzdtjM9_-8,4920
 botbuilder/testing/dialog_test_logger.py,sha256=UwMaGI8DFnxN1PEz3_RJJ9K6RKo1v9rjsCWfVGkfUx8,3786
 botbuilder/testing/storage_base_tests.py,sha256=voUJCO75rJEunZhWNVGqGqIbHeBhEGA8OljKdORV7K4,12142
-botbuilder_testing-4.9.2.dist-info/METADATA,sha256=4K1Qt4n3S55xMFpxexkCwJXGeYFdIy7VzSy5IDe-NJk,3872
-botbuilder_testing-4.9.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-botbuilder_testing-4.9.2.dist-info/top_level.txt,sha256=2p3tapzF5j-vDQrnQjnuJZvvXStR_qu8i9Tqq-0ThZg,11
-botbuilder_testing-4.9.2.dist-info/RECORD,,
+botbuilder_testing-4.9.3.dist-info/METADATA,sha256=g6_wodMkhGP2wf8Jz-qHmfWl8M2wNqHhfx7BCX112oM,3872
+botbuilder_testing-4.9.3.dist-info/WHEEL,sha256=gm79cMopkncyn0iSnI0vQNiDJ8t9on0H4_iz-CrpXMk,92
+botbuilder_testing-4.9.3.dist-info/top_level.txt,sha256=2p3tapzF5j-vDQrnQjnuJZvvXStR_qu8i9Tqq-0ThZg,11
+botbuilder_testing-4.9.3.dist-info/RECORD,,
```

