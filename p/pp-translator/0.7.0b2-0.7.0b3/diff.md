# Comparing `tmp/pp_translator-0.7.0b2-py3-none-any.whl.zip` & `tmp/pp_translator-0.7.0b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 19364 bytes, number of entries: 13
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-24 00:09 pp_creators/__init__.py
--rw-r--r--  2.0 unx    15592 b- defN 23-Jan-24 00:09 pp_creators/basic_creator.py
--rw-r--r--  2.0 unx     5609 b- defN 23-Jan-24 00:09 pp_creators/creator.py
--rw-r--r--  2.0 unx    11681 b- defN 23-Jan-24 00:09 pp_creators/creator_ee.py
--rw-r--r--  2.0 unx     7909 b- defN 23-Jan-24 00:09 pp_creators/error_checking_creator.py
--rw-r--r--  2.0 unx      760 b- defN 23-Jan-24 00:09 pp_creators/utils.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-24 00:09 pp_creators/validators/__init__.py
--rw-r--r--  2.0 unx     4982 b- defN 23-Jan-24 00:09 pp_creators/validators/validator.py
--rw-r--r--  2.0 unx    16725 b- defN 23-Jan-24 00:10 pp_translator-0.7.0b2.dist-info/LICENSE
--rw-r--r--  2.0 unx      951 b- defN 23-Jan-24 00:10 pp_translator-0.7.0b2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-24 00:10 pp_translator-0.7.0b2.dist-info/WHEEL
--rw-r--r--  2.0 unx       83 b- defN 23-Jan-24 00:10 pp_translator-0.7.0b2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1105 b- defN 23-Jan-24 00:10 pp_translator-0.7.0b2.dist-info/RECORD
-13 files, 65981 bytes uncompressed, 17508 bytes compressed:  73.5%
+Zip file size: 19365 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      246 b- defN 23-May-31 07:39 pp_creators/__init__.py
+-rw-r--r--  2.0 unx    15592 b- defN 23-May-31 07:39 pp_creators/basic_creator.py
+-rw-r--r--  2.0 unx     5609 b- defN 23-May-31 07:39 pp_creators/creator.py
+-rw-r--r--  2.0 unx    11681 b- defN 23-May-31 07:39 pp_creators/creator_ee.py
+-rw-r--r--  2.0 unx     7909 b- defN 23-May-31 07:39 pp_creators/error_checking_creator.py
+-rw-r--r--  2.0 unx      760 b- defN 23-May-31 07:39 pp_creators/utils.py
+-rw-r--r--  2.0 unx      246 b- defN 23-May-31 07:39 pp_creators/validators/__init__.py
+-rw-r--r--  2.0 unx     4982 b- defN 23-May-31 07:39 pp_creators/validators/validator.py
+-rw-r--r--  2.0 unx    16725 b- defN 23-May-31 07:39 pp_translator-0.7.0b3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      952 b- defN 23-May-31 07:39 pp_translator-0.7.0b3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 07:39 pp_translator-0.7.0b3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       83 b- defN 23-May-31 07:39 pp_translator-0.7.0b3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1105 b- defN 23-May-31 07:39 pp_translator-0.7.0b3.dist-info/RECORD
+13 files, 65982 bytes uncompressed, 17509 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: pp_creators/validators/__init__.py
 Comment: 
 
 Filename: pp_creators/validators/validator.py
 Comment: 
 
-Filename: pp_translator-0.7.0b2.dist-info/LICENSE
+Filename: pp_translator-0.7.0b3.dist-info/LICENSE
 Comment: 
 
-Filename: pp_translator-0.7.0b2.dist-info/METADATA
+Filename: pp_translator-0.7.0b3.dist-info/METADATA
 Comment: 
 
-Filename: pp_translator-0.7.0b2.dist-info/WHEEL
+Filename: pp_translator-0.7.0b3.dist-info/WHEEL
 Comment: 
 
-Filename: pp_translator-0.7.0b2.dist-info/top_level.txt
+Filename: pp_translator-0.7.0b3.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_translator-0.7.0b2.dist-info/RECORD
+Filename: pp_translator-0.7.0b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pp_translator-0.7.0b2.dist-info/LICENSE` & `pp_translator-0.7.0b3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pp_translator-0.7.0b2.dist-info/METADATA` & `pp_translator-0.7.0b3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pp-translator
-Version: 0.7.0b2
+Version: 0.7.0b3
 Summary: Library for translating Zepben CIM network models to pandapower models
 Home-page: https://github.com/zepben/pp-translator
 Author: Zeppelin Bend
 Author-email: oss@zepben.com
 License: MPL 2.0
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 License-File: LICENSE
-Requires-Dist: zepben.evolve (==0.35.0b9)
+Requires-Dist: zepben.evolve (==0.35.0b17)
 Requires-Dist: pandapower (==2.9.0)
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pytest-cov ; extra == 'test'
 Requires-Dist: pytest-asyncio ; extra == 'test'
 Requires-Dist: hypothesis ; extra == 'test'
```

## Comparing `pp_translator-0.7.0b2.dist-info/RECORD` & `pp_translator-0.7.0b3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 pp_creators/basic_creator.py,sha256=UWnBONNNQuTCN58BnyuFnDiWeDv1fRfKZjPPe2tavD8,15592
 pp_creators/creator.py,sha256=Rvx-5N9gl-Qm4uVPFHPRKQFZBhh3jqar0FbH-FrR6_0,5609
 pp_creators/creator_ee.py,sha256=z3xv5prM3kFlyFCtDixXHNnYf7ag4WRwh0EXEYOfHhg,11681
 pp_creators/error_checking_creator.py,sha256=tuhXdHBxZ2npa_tXT3fJdFhQDEFdxt8nQ-JZJLOQRLk,7909
 pp_creators/utils.py,sha256=seur2PfLyJaIXWVDkM6iSjKPicF8twhcgGvc_cXXbzs,760
 pp_creators/validators/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 pp_creators/validators/validator.py,sha256=l5DNF871JrmEoi6wB-WmLEZOhdbgYO98ErlD-wmNDX8,4982
-pp_translator-0.7.0b2.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
-pp_translator-0.7.0b2.dist-info/METADATA,sha256=ecX9Ka6U1Xn92CyFaI4pLNhdqu9RZgLTmaXgg-7zO9U,951
-pp_translator-0.7.0b2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pp_translator-0.7.0b2.dist-info/top_level.txt,sha256=4BYt4W6C9pWZUqv_QIaMZk0rNJ8ePiRDwiBDSFMp1bs,83
-pp_translator-0.7.0b2.dist-info/RECORD,,
+pp_translator-0.7.0b3.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
+pp_translator-0.7.0b3.dist-info/METADATA,sha256=7NXl5qmuM_jWayjERLMdZuQneNc7jd9kfrs4pnFEQUM,952
+pp_translator-0.7.0b3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pp_translator-0.7.0b3.dist-info/top_level.txt,sha256=4BYt4W6C9pWZUqv_QIaMZk0rNJ8ePiRDwiBDSFMp1bs,83
+pp_translator-0.7.0b3.dist-info/RECORD,,
```

