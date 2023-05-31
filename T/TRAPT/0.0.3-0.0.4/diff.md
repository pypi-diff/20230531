# Comparing `tmp/TRAPT-0.0.3.tar.gz` & `tmp/TRAPT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TRAPT-0.0.3.tar", last modified: Wed May 31 16:14:36 2023, max compression
+gzip compressed data, was "TRAPT-0.0.4.tar", last modified: Wed May 31 16:31:30 2023, max compression
```

## Comparing `TRAPT-0.0.3.tar` & `TRAPT-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:14:36.697060 TRAPT-0.0.3/
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     1071 2023-05-31 09:43:38.000000 TRAPT-0.0.3/LICENSE
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     2080 2023-05-31 16:14:36.697060 TRAPT-0.0.3/PKG-INFO
--rwxrwxrwx   0 tostring  (1000) tostring  (1000)     1444 2023-05-31 16:10:53.000000 TRAPT-0.0.3/README.md
--rw-rw-r--   0 tostring  (1000) tostring  (1000)      747 2023-05-31 15:53:43.000000 TRAPT-0.0.3/pyproject.toml
--rw-rw-r--   0 tostring  (1000) tostring  (1000)       38 2023-05-31 16:14:36.697060 TRAPT-0.0.3/setup.cfg
-drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:14:36.697060 TRAPT-0.0.3/src/
-drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:14:36.697060 TRAPT-0.0.3/src/TRAPT/
--rwxrwxrwx   0 tostring  (1000) tostring  (1000)     3631 2023-05-31 09:18:18.000000 TRAPT-0.0.3/src/TRAPT/CalcSampleRPMatrix.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     1852 2023-05-17 05:42:05.000000 TRAPT-0.0.3/src/TRAPT/CalcTRAUC.py
--rwxrwxrwx   0 tostring  (1000) tostring  (1000)     3918 2023-05-31 09:18:08.000000 TRAPT-0.0.3/src/TRAPT/CalcTRRPMatrix.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     1457 2023-05-31 09:18:02.000000 TRAPT-0.0.3/src/TRAPT/CalcTRSampleRPMatrix.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     6715 2023-05-31 09:17:55.000000 TRAPT-0.0.3/src/TRAPT/DLFS.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)    13559 2023-05-31 09:49:41.000000 TRAPT-0.0.3/src/TRAPT/DLVGAE.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     5141 2023-05-31 10:19:31.000000 TRAPT-0.0.3/src/TRAPT/TRAPT.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)        0 2023-05-31 09:11:06.000000 TRAPT-0.0.3/src/TRAPT/__init__.py
-drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:14:36.697060 TRAPT-0.0.3/src/TRAPT.egg-info/
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     2080 2023-05-31 16:14:36.000000 TRAPT-0.0.3/src/TRAPT.egg-info/PKG-INFO
--rw-rw-r--   0 tostring  (1000) tostring  (1000)      392 2023-05-31 16:14:36.000000 TRAPT-0.0.3/src/TRAPT.egg-info/SOURCES.txt
--rw-rw-r--   0 tostring  (1000) tostring  (1000)        1 2023-05-31 16:14:36.000000 TRAPT-0.0.3/src/TRAPT.egg-info/dependency_links.txt
--rw-rw-r--   0 tostring  (1000) tostring  (1000)       69 2023-05-31 16:14:36.000000 TRAPT-0.0.3/src/TRAPT.egg-info/requires.txt
--rw-rw-r--   0 tostring  (1000) tostring  (1000)        6 2023-05-31 16:14:36.000000 TRAPT-0.0.3/src/TRAPT.egg-info/top_level.txt
+drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:31:30.384137 TRAPT-0.0.4/
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     1071 2023-05-31 09:43:38.000000 TRAPT-0.0.4/LICENSE
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     2090 2023-05-31 16:31:30.384137 TRAPT-0.0.4/PKG-INFO
+-rwxrwxrwx   0 tostring  (1000) tostring  (1000)     1454 2023-05-31 16:29:23.000000 TRAPT-0.0.4/README.md
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)      757 2023-05-31 16:27:36.000000 TRAPT-0.0.4/pyproject.toml
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)       38 2023-05-31 16:31:30.384137 TRAPT-0.0.4/setup.cfg
+drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:31:30.384137 TRAPT-0.0.4/src/
+drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:31:30.384137 TRAPT-0.0.4/src/TRAPT/
+-rwxrwxrwx   0 tostring  (1000) tostring  (1000)     3631 2023-05-31 09:18:18.000000 TRAPT-0.0.4/src/TRAPT/CalcSampleRPMatrix.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     1852 2023-05-17 05:42:05.000000 TRAPT-0.0.4/src/TRAPT/CalcTRAUC.py
+-rwxrwxrwx   0 tostring  (1000) tostring  (1000)     3918 2023-05-31 09:18:08.000000 TRAPT-0.0.4/src/TRAPT/CalcTRRPMatrix.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     1457 2023-05-31 09:18:02.000000 TRAPT-0.0.4/src/TRAPT/CalcTRSampleRPMatrix.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     6715 2023-05-31 09:17:55.000000 TRAPT-0.0.4/src/TRAPT/DLFS.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)    13559 2023-05-31 09:49:41.000000 TRAPT-0.0.4/src/TRAPT/DLVGAE.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     5141 2023-05-31 10:19:31.000000 TRAPT-0.0.4/src/TRAPT/TRAPT.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)        0 2023-05-31 09:11:06.000000 TRAPT-0.0.4/src/TRAPT/__init__.py
+drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:31:30.384137 TRAPT-0.0.4/src/TRAPT.egg-info/
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     2090 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/PKG-INFO
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)      392 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)        1 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)       74 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/requires.txt
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)        6 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/top_level.txt
```

### Comparing `TRAPT-0.0.3/LICENSE` & `TRAPT-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.3/PKG-INFO` & `TRAPT-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TRAPT
-Version: 0.0.3
+Version: 0.0.4
 Summary: A novel deep learning framework for transcription regulators prediction via integraing large-scale epigenomic data.
 Author-email: zhangguorui <mp798378522@gmail.com>
 Project-URL: Homepage, https://github.com/LicLab-bio/TRAPT
 Project-URL: Bug Tracker, https://github.com/LicLab-bio/TRAPT/issues
 Project-URL: Blog, http://www.licpathway.net/TRAPT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,15 @@
 conda activate TRAPT
 pip install TRAPT
 ```
 
 Run TRAPT using a [case](http://www.licpathway.net/TRAPT/static/download/ESR1@DataSet_01_111_down500.txt):
 
 ```python
+import os
 from TRAPT.TRAPT import Args, RP_Matrix, runTRAPT
 
 # library path
 library = 'library'
 # input file path
 input = 'ESR1@DataSet_01_111_down500.txt'
 # output file path
```

### Comparing `TRAPT-0.0.3/README.md` & `TRAPT-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 conda activate TRAPT
 pip install TRAPT
 ```
 
 Run TRAPT using a [case](http://www.licpathway.net/TRAPT/static/download/ESR1@DataSet_01_111_down500.txt):
 
 ```python
+import os
 from TRAPT.TRAPT import Args, RP_Matrix, runTRAPT
 
 # library path
 library = 'library'
 # input file path
 input = 'ESR1@DataSet_01_111_down500.txt'
 # output file path
```

### Comparing `TRAPT-0.0.3/pyproject.toml` & `TRAPT-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "TRAPT"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="zhangguorui", email="mp798378522@gmail.com" },
 ]
 description = "A novel deep learning framework for transcription regulators prediction via integraing large-scale epigenomic data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
+  "tqdm",
   "numba",
   "numpy",
   "pandas",
   "scikit-learn",
   "scipy",
   "anndata",
   "keras",
```

### Comparing `TRAPT-0.0.3/src/TRAPT/CalcSampleRPMatrix.py` & `TRAPT-0.0.4/src/TRAPT/CalcSampleRPMatrix.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.3/src/TRAPT/CalcTRAUC.py` & `TRAPT-0.0.4/src/TRAPT/CalcTRAUC.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.3/src/TRAPT/CalcTRRPMatrix.py` & `TRAPT-0.0.4/src/TRAPT/CalcTRRPMatrix.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.3/src/TRAPT/CalcTRSampleRPMatrix.py` & `TRAPT-0.0.4/src/TRAPT/CalcTRSampleRPMatrix.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.3/src/TRAPT/DLFS.py` & `TRAPT-0.0.4/src/TRAPT/DLFS.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.3/src/TRAPT/DLVGAE.py` & `TRAPT-0.0.4/src/TRAPT/DLVGAE.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.3/src/TRAPT/TRAPT.py` & `TRAPT-0.0.4/src/TRAPT/TRAPT.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.3/src/TRAPT.egg-info/PKG-INFO` & `TRAPT-0.0.4/src/TRAPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TRAPT
-Version: 0.0.3
+Version: 0.0.4
 Summary: A novel deep learning framework for transcription regulators prediction via integraing large-scale epigenomic data.
 Author-email: zhangguorui <mp798378522@gmail.com>
 Project-URL: Homepage, https://github.com/LicLab-bio/TRAPT
 Project-URL: Bug Tracker, https://github.com/LicLab-bio/TRAPT/issues
 Project-URL: Blog, http://www.licpathway.net/TRAPT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,15 @@
 conda activate TRAPT
 pip install TRAPT
 ```
 
 Run TRAPT using a [case](http://www.licpathway.net/TRAPT/static/download/ESR1@DataSet_01_111_down500.txt):
 
 ```python
+import os
 from TRAPT.TRAPT import Args, RP_Matrix, runTRAPT
 
 # library path
 library = 'library'
 # input file path
 input = 'ESR1@DataSet_01_111_down500.txt'
 # output file path
```

