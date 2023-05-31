# Comparing `tmp/zepben.edith-0.3.0b3-py3-none-any.whl.zip` & `tmp/zepben.edith-0.3.0b4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 16144 bytes, number of entries: 8
--rw-r--r--  2.0 unx    12393 b- defN 23-Jan-18 06:42 zepben/edith/__init__.py
--rw-r--r--  2.0 unx    11753 b- defN 23-Jan-18 06:42 zepben/edith/linecode_catalogue.py
--rw-r--r--  2.0 unx    45381 b- defN 23-Jan-18 06:42 zepben/edith/transformer_catalogue.py
--rw-r--r--  2.0 unx    16725 b- defN 23-Jan-18 06:42 zepben.edith-0.3.0b3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1202 b- defN 23-Jan-18 06:42 zepben.edith-0.3.0b3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-18 06:42 zepben.edith-0.3.0b3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-18 06:42 zepben.edith-0.3.0b3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      690 b- defN 23-Jan-18 06:42 zepben.edith-0.3.0b3.dist-info/RECORD
-8 files, 88243 bytes uncompressed, 14936 bytes compressed:  83.1%
+Zip file size: 16146 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    12393 b- defN 23-May-31 07:53 zepben/edith/__init__.py
+-rw-r--r--  2.0 unx    11753 b- defN 23-May-31 07:53 zepben/edith/linecode_catalogue.py
+-rw-r--r--  2.0 unx    45381 b- defN 23-May-31 07:53 zepben/edith/transformer_catalogue.py
+-rw-r--r--  2.0 unx    16725 b- defN 23-May-31 07:53 zepben.edith-0.3.0b4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1203 b- defN 23-May-31 07:53 zepben.edith-0.3.0b4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 07:53 zepben.edith-0.3.0b4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-31 07:53 zepben.edith-0.3.0b4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      690 b- defN 23-May-31 07:53 zepben.edith-0.3.0b4.dist-info/RECORD
+8 files, 88244 bytes uncompressed, 14938 bytes compressed:  83.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: zepben/edith/linecode_catalogue.py
 Comment: 
 
 Filename: zepben/edith/transformer_catalogue.py
 Comment: 
 
-Filename: zepben.edith-0.3.0b3.dist-info/LICENSE
+Filename: zepben.edith-0.3.0b4.dist-info/LICENSE
 Comment: 
 
-Filename: zepben.edith-0.3.0b3.dist-info/METADATA
+Filename: zepben.edith-0.3.0b4.dist-info/METADATA
 Comment: 
 
-Filename: zepben.edith-0.3.0b3.dist-info/WHEEL
+Filename: zepben.edith-0.3.0b4.dist-info/WHEEL
 Comment: 
 
-Filename: zepben.edith-0.3.0b3.dist-info/top_level.txt
+Filename: zepben.edith-0.3.0b4.dist-info/top_level.txt
 Comment: 
 
-Filename: zepben.edith-0.3.0b3.dist-info/RECORD
+Filename: zepben.edith-0.3.0b4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `zepben.edith-0.3.0b3.dist-info/LICENSE` & `zepben.edith-0.3.0b4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zepben.edith-0.3.0b3.dist-info/METADATA` & `zepben.edith-0.3.0b4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zepben.edith
-Version: 0.3.0b3
+Version: 0.3.0b4
 Summary: Python SDK extensions for the Edith project
 Home-page: https://github.com/zepben/edith-sdk
 Author: Kurt Greaves
 Author-email: kurt.greaves@zepben.com
 License: MPL 2.0
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: zepben.evolve (==0.35.0b9)
+Requires-Dist: zepben.evolve (==0.35.0b17)
 Requires-Dist: dataclassy (==0.6.2)
 Requires-Dist: mock (==4.0.3)
 Provides-Extra: test
 Requires-Dist: pytest (==7.1.2) ; extra == 'test'
 Requires-Dist: pytest-cov (==2.10.1) ; extra == 'test'
 Requires-Dist: pytest-asyncio (==0.19.0) ; extra == 'test'
 Requires-Dist: pytest-timeout (==1.4.2) ; extra == 'test'
```

## Comparing `zepben.edith-0.3.0b3.dist-info/RECORD` & `zepben.edith-0.3.0b4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 zepben/edith/__init__.py,sha256=RCgU24JM5hxT57O3i_dPCfI6WWJ0MNLAKzp5wOXU97w,12393
 zepben/edith/linecode_catalogue.py,sha256=TwgJ9zxwCuonG7KyTXQbU6El6zaPUzP4bWsoB2hVtmU,11753
 zepben/edith/transformer_catalogue.py,sha256=Tn7sBNW245u3O95htsa3TfVYl9Y3LD8XeVHzaBeB7kQ,45381
-zepben.edith-0.3.0b3.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
-zepben.edith-0.3.0b3.dist-info/METADATA,sha256=0owwS7elGROBuGIM1lC-XWqG8qARO3y_zA7ObzbNwSc,1202
-zepben.edith-0.3.0b3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-zepben.edith-0.3.0b3.dist-info/top_level.txt,sha256=eVLDJiO6FGjL_Z7KdmFE-R8uf1Q07aaVLGe9Ee4kmBw,7
-zepben.edith-0.3.0b3.dist-info/RECORD,,
+zepben.edith-0.3.0b4.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
+zepben.edith-0.3.0b4.dist-info/METADATA,sha256=0mWCZ3SxnE3y-zrRWsHH1uZopmyBqCO9QmO7kEJyXuQ,1203
+zepben.edith-0.3.0b4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+zepben.edith-0.3.0b4.dist-info/top_level.txt,sha256=eVLDJiO6FGjL_Z7KdmFE-R8uf1Q07aaVLGe9Ee4kmBw,7
+zepben.edith-0.3.0b4.dist-info/RECORD,,
```

