# Comparing `tmp/gulagcleaner-0.5.0.tar.gz` & `tmp/gulagcleaner-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulagcleaner-0.5.0.tar", last modified: Wed May 31 21:34:32 2023, max compression
+gzip compressed data, was "gulagcleaner-0.5.1.tar", last modified: Wed May 31 21:42:51 2023, max compression
```

## Comparing `gulagcleaner-0.5.0.tar` & `gulagcleaner-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 21:34:32.593029 gulagcleaner-0.5.0/
--rw-rw-rw-   0        0        0    71644 2023-02-12 15:01:11.000000 gulagcleaner-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     2437 2023-05-31 21:34:32.593091 gulagcleaner-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2023-05-31 21:24:37.000000 gulagcleaner-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 21:34:32.564420 gulagcleaner-0.5.0/gulagcleaner/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:01:11.000000 gulagcleaner-0.5.0/gulagcleaner/__init__.py
--rw-rw-rw-   0        0        0     2757 2023-05-31 21:16:23.000000 gulagcleaner-0.5.0/gulagcleaner/command_line.py
--rw-rw-rw-   0        0        0     5886 2023-05-31 21:17:33.000000 gulagcleaner-0.5.0/gulagcleaner/gulagcleaner_extract.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:34:32.590421 gulagcleaner-0.5.0/gulagcleaner.egg-info/
--rw-rw-rw-   0        0        0     2437 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-02-12 15:01:11.000000 gulagcleaner-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      857 2023-05-31 21:34:32.600419 gulagcleaner-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 21:42:51.379112 gulagcleaner-0.5.1/
+-rw-rw-rw-   0        0        0    71644 2023-02-12 15:01:11.000000 gulagcleaner-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     2437 2023-05-31 21:42:51.379112 gulagcleaner-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2023-05-31 21:24:37.000000 gulagcleaner-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 21:42:51.349077 gulagcleaner-0.5.1/gulagcleaner/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:01:11.000000 gulagcleaner-0.5.1/gulagcleaner/__init__.py
+-rw-rw-rw-   0        0        0     2757 2023-05-31 21:39:11.000000 gulagcleaner-0.5.1/gulagcleaner/command_line.py
+-rw-rw-rw-   0        0        0     5889 2023-05-31 21:40:21.000000 gulagcleaner-0.5.1/gulagcleaner/gulagcleaner_extract.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:42:51.377076 gulagcleaner-0.5.1/gulagcleaner.egg-info/
+-rw-rw-rw-   0        0        0     2437 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-02-12 15:01:11.000000 gulagcleaner-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      857 2023-05-31 21:42:51.386081 gulagcleaner-0.5.1/setup.cfg
```

### Comparing `gulagcleaner-0.5.0/LICENSE` & `gulagcleaner-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.5.0/PKG-INFO` & `gulagcleaner-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.5.0
+Version: 0.5.1
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162,KosmicKatXV,pgalinanes
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gulagcleaner-0.5.0/README.md` & `gulagcleaner-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.5.0/gulagcleaner/command_line.py` & `gulagcleaner-0.5.1/gulagcleaner/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         print("  -r            replaces the original file with the deembedded file.")
         print("  -o            uses the old deembeding method (for files older than 18/05/2023).")
         print("  -v            shows the version of the program.")
         return
 
     # Check for the -v argument
     if '-v' in sys.argv:
-        print("actual version: 0.5.0")
+        print("actual version: 0.5.1")
         return
 
     # Get the filename argument
     if len(sys.argv) < 2:
         print('Usage: gulagcleaner [-h] [-r] [-o] [-v] <filename>')
         return
     filename = sys.argv[-1]
```

### Comparing `gulagcleaner-0.5.0/gulagcleaner/gulagcleaner_extract.py` & `gulagcleaner-0.5.1/gulagcleaner/gulagcleaner_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         except Exception as e:
             print("Failed to extract metadata:", e)
 
         pdf = PdfReader(intermediate_pdf_path)
 
         if method=="old":
             xobjs = list(find_objects(pdf.pages, valid_subtypes=(PdfName.Form, PdfName.Dummy)))
-            pages = [wrap_object(item, 1000, 0.5 * 72) for item in xobjs]
+            newpages = [wrap_object(item, 1000, 0.5 * 72) for item in xobjs]
 
             if not xobjs:
                 os.remove(intermediate_pdf_path)
                 return {
                     "Success": False,
                     "return_path": "",
                     "Error": "No embedded pages found.",
```

### Comparing `gulagcleaner-0.5.0/gulagcleaner.egg-info/PKG-INFO` & `gulagcleaner-0.5.1/gulagcleaner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.5.0
+Version: 0.5.1
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162,KosmicKatXV,pgalinanes
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gulagcleaner-0.5.0/setup.cfg` & `gulagcleaner-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 756c 6167 636c 6561 6e65 720d   = gulagcleaner.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e30  .version = 0.5.0
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e31  .version = 0.5.1
 00000030: 0d0a 6175 7468 6f72 203d 2059 4d31 3632  ..author = YM162
 00000040: 2c4b 6f73 6d69 634b 6174 5856 2c70 6761  ,KosmicKatXV,pga
 00000050: 6c69 6e61 6e65 730d 0a61 7574 686f 725f  linanes..author_
 00000060: 656d 6169 6c20 3d20 6461 7669 642e 666f  email = david.fo
 00000070: 6e74 616e 6564 6131 3640 676d 6169 6c2e  ntaneda16@gmail.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 6420 7265 6d6f 7661 6c20 746f   = Ad removal to
```

