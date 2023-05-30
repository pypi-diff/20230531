# Comparing `tmp/pydndc-1.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/pydndc-1.0.2-cp39-cp39-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 548883 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      202 b- defN 22-Jul-09 00:50 pydndc/__init__.py
--rw-rw-rw-  2.0 fat     6253 b- defN 22-Oct-02 17:46 pydndc/__main__.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-09 00:50 pydndc/py.typed
--rw-rw-rw-  2.0 fat  1229824 b- defN 23-Jan-02 19:22 pydndc/pydndc.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     6741 b- defN 22-Oct-03 04:29 pydndc/pydndc.pyi
--rw-rw-rw-  2.0 fat    28313 b- defN 23-Jan-02 19:22 pydndc-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jan-02 19:22 pydndc-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jan-02 19:22 pydndc-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      679 b- defN 23-Jan-02 19:22 pydndc-1.0.1.dist-info/RECORD
-9 files, 1272119 bytes uncompressed, 547729 bytes compressed:  56.9%
+Zip file size: 1111037 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     6741 b- defN 22-Oct-04 22:00 pydndc/pydndc.pyi
+-rw-r--r--  2.0 unx      202 b- defN 22-Sep-02 03:09 pydndc/__init__.py
+-rwxr-xr-x  2.0 unx  2671640 b- defN 23-May-30 21:50 pydndc/pydndc.cpython-39-darwin.so
+-rw-r--r--  2.0 unx        0 b- defN 22-Sep-02 03:09 pydndc/py.typed
+-rw-r--r--  2.0 unx     6253 b- defN 22-Oct-02 17:43 pydndc/__main__.py
+-rw-rw-r--  2.0 unx      681 b- defN 23-May-30 21:50 pydndc-1.0.2.dist-info/RECORD
+-rw-r--r--  2.0 unx      113 b- defN 23-May-30 21:50 pydndc-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-30 21:50 pydndc-1.0.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    28300 b- defN 23-May-30 21:50 pydndc-1.0.2.dist-info/METADATA
+9 files, 2713937 bytes uncompressed, 1109879 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: pydndc/__init__.py
+Filename: pydndc/pydndc.pyi
 Comment: 
 
-Filename: pydndc/__main__.py
+Filename: pydndc/__init__.py
 Comment: 
 
-Filename: pydndc/py.typed
+Filename: pydndc/pydndc.cpython-39-darwin.so
 Comment: 
 
-Filename: pydndc/pydndc.cp39-win_amd64.pyd
+Filename: pydndc/py.typed
 Comment: 
 
-Filename: pydndc/pydndc.pyi
+Filename: pydndc/__main__.py
 Comment: 
 
-Filename: pydndc-1.0.1.dist-info/METADATA
+Filename: pydndc-1.0.2.dist-info/RECORD
 Comment: 
 
-Filename: pydndc-1.0.1.dist-info/WHEEL
+Filename: pydndc-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pydndc-1.0.1.dist-info/top_level.txt
+Filename: pydndc-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pydndc-1.0.1.dist-info/RECORD
+Filename: pydndc-1.0.2.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## Comparing `pydndc-1.0.1.dist-info/METADATA` & `pydndc-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydndc
-Version: 1.0.1
+Version: 1.0.2
 Summary: dndc, but from python
 Author: David Priver
 Author-email: david@davidpriver.com
 License: Proprietary
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -972,26 +972,25 @@
     grid-row:1;
   }
   * {
     box-sizing: border-box;
   }
   a {
     text-decoration: none;
-    color: black;
+    color: currentcolor;
     border-bottom: 1px grey dotted;
   }
   div.root {
     display: grid;
     grid-template-columns: 15em auto;
     grid-column-gap: 4em;
     padding-bottom: 90vh;
   }
   nav a {
     border-bottom: 0;
-    color: initial;
     text-decoration: none;
   }
   nav li {
     list-style-type: square;
   }
   nav {
     position: fixed;
```

