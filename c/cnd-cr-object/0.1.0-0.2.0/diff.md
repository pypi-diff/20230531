# Comparing `tmp/cnd_cr_object-0.1.0-py3-none-any.whl.zip` & `tmp/cnd_cr_object-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2381 bytes, number of entries: 8
--rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-07 22:28 cnd_cr_object/VERSION
--rw-r--r--  2.0 unx      125 b- defN 23-Apr-07 22:28 cnd_cr_object/__init__.py
--rw-r--r--  2.0 unx      122 b- defN 23-Apr-07 22:28 cnd_cr_object/__version__.py
--rw-r--r--  2.0 unx      572 b- defN 23-Apr-07 22:28 cnd_cr_object/cr_object.py
--rw-r--r--  2.0 unx      768 b- defN 23-Apr-07 22:29 cnd_cr_object-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 22:29 cnd_cr_object-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-07 22:29 cnd_cr_object-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      643 b- defN 23-Apr-07 22:29 cnd_cr_object-0.1.0.dist-info/RECORD
-8 files, 2341 bytes uncompressed, 1247 bytes compressed:  46.7%
+Zip file size: 2380 bytes, number of entries: 8
+-rw-rw-rw-  2.0 unx        5 b- defN 23-May-31 11:52 cnd_cr_object/VERSION
+-rw-r--r--  2.0 unx      125 b- defN 23-May-31 11:52 cnd_cr_object/__init__.py
+-rw-r--r--  2.0 unx      122 b- defN 23-May-31 11:52 cnd_cr_object/__version__.py
+-rw-r--r--  2.0 unx      572 b- defN 23-May-31 11:52 cnd_cr_object/cr_object.py
+-rw-r--r--  2.0 unx      768 b- defN 23-May-31 11:52 cnd_cr_object-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 11:52 cnd_cr_object-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-31 11:52 cnd_cr_object-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      643 b- defN 23-May-31 11:52 cnd_cr_object-0.2.0.dist-info/RECORD
+8 files, 2341 bytes uncompressed, 1246 bytes compressed:  46.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: cnd_cr_object/__version__.py
 Comment: 
 
 Filename: cnd_cr_object/cr_object.py
 Comment: 
 
-Filename: cnd_cr_object-0.1.0.dist-info/METADATA
+Filename: cnd_cr_object-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: cnd_cr_object-0.1.0.dist-info/WHEEL
+Filename: cnd_cr_object-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_cr_object-0.1.0.dist-info/top_level.txt
+Filename: cnd_cr_object-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_cr_object-0.1.0.dist-info/RECORD
+Filename: cnd_cr_object-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cnd_cr_object/VERSION

```diff
@@ -1 +1 @@
-0.1.0
+0.2.0
```

## Comparing `cnd_cr_object-0.1.0.dist-info/METADATA` & `cnd_cr_object-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-cr-object
-Version: 0.1.0
+Version: 0.2.0
 Summary: Base for vro Custom Resource Object
 Home-page: https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
```

## Comparing `cnd_cr_object-0.1.0.dist-info/RECORD` & `cnd_cr_object-0.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cnd_cr_object/VERSION,sha256=atlhOkVXmNbZLl9fOQq0uqcFlryGntaxf1zdKyhjXwY,5
+cnd_cr_object/VERSION,sha256=kR_AxIywxwYB21d1qb7xt0DcTMn5tGOJufBWP-frlNc,5
 cnd_cr_object/__init__.py,sha256=QdMe3KLaaBNV6Bwo89FfVBUTwP4B9TEhh3QpeQiI5EM,125
 cnd_cr_object/__version__.py,sha256=n4tz4WCd1Fep5gqyUpB9bFwlfaKKw8zGOTswJoN2Im0,122
 cnd_cr_object/cr_object.py,sha256=TGowGcWgOSNzWR6AqA3DsQtrj92EAZONmyppl7XVcMk,572
-cnd_cr_object-0.1.0.dist-info/METADATA,sha256=dcbpwdYVTIx6AtX8EapbH_qTrdp9OfnLvvWJJpvd2YI,768
-cnd_cr_object-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-cnd_cr_object-0.1.0.dist-info/top_level.txt,sha256=Oe87B8Nvt4Nk3-WONRZZx-3_oh-eRasrhN-_utM6ZD4,14
-cnd_cr_object-0.1.0.dist-info/RECORD,,
+cnd_cr_object-0.2.0.dist-info/METADATA,sha256=80DUi9wf4egWoXTvRZgHO2iFztRUbRjaAlGfhPMvng8,768
+cnd_cr_object-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cnd_cr_object-0.2.0.dist-info/top_level.txt,sha256=Oe87B8Nvt4Nk3-WONRZZx-3_oh-eRasrhN-_utM6ZD4,14
+cnd_cr_object-0.2.0.dist-info/RECORD,,
```

