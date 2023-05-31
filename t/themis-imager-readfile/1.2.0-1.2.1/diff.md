# Comparing `tmp/themis_imager_readfile-1.2.0.tar.gz` & `tmp/themis_imager_readfile-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themis_imager_readfile-1.2.0.tar", max compression
+gzip compressed data, was "themis_imager_readfile-1.2.1.tar", max compression
```

## Comparing `themis_imager_readfile-1.2.0.tar` & `themis_imager_readfile-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.2.0/LICENSE
--rw-r--r--   0        0        0     2763 2023-05-15 18:17:56.997619 themis_imager_readfile-1.2.0/README.md
--rw-r--r--   0        0        0      666 2023-05-31 15:36:41.261336 themis_imager_readfile-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       49 2023-05-31 15:36:41.294337 themis_imager_readfile-1.2.0/themis_imager_readfile/__init__.py
--rw-r--r--   0        0        0     9271 2023-05-31 15:40:04.332431 themis_imager_readfile-1.2.0/themis_imager_readfile/_themis.py
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 themis_imager_readfile-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2763 2023-05-15 18:17:56.997619 themis_imager_readfile-1.2.1/README.md
+-rw-r--r--   0        0        0      666 2023-05-31 15:56:15.011026 themis_imager_readfile-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-05-31 15:56:15.045027 themis_imager_readfile-1.2.1/themis_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8971 2023-05-31 15:54:47.371259 themis_imager_readfile-1.2.1/themis_imager_readfile/_themis.py
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 themis_imager_readfile-1.2.1/PKG-INFO
```

### Comparing `themis_imager_readfile-1.2.0/LICENSE` & `themis_imager_readfile-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.2.0/README.md` & `themis_imager_readfile-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.2.0/pyproject.toml` & `themis_imager_readfile-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "themis-imager-readfile"
-version = "1.2.0"
+version = "1.2.1"
 description = "Read functions for THEMIS ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `themis_imager_readfile-1.2.0/themis_imager_readfile/_themis.py` & `themis_imager_readfile-1.2.1/themis_imager_readfile/_themis.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,14 @@
     :type file_list: str
     :param workers: number of worker processes to spawn, defaults to 1
     :type workers: int, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
-    # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    pool = Pool(processes=workers)
-    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
-
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
     # check workers
     if (workers > 1):
         try:
```

### Comparing `themis_imager_readfile-1.2.0/PKG-INFO` & `themis_imager_readfile-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themis-imager-readfile
-Version: 1.2.0
+Version: 1.2.1
 Summary: Read functions for THEMIS ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/themis-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

