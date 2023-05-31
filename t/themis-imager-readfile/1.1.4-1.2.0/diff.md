# Comparing `tmp/themis_imager_readfile-1.1.4.tar.gz` & `tmp/themis_imager_readfile-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themis_imager_readfile-1.1.4.tar", max compression
+gzip compressed data, was "themis_imager_readfile-1.2.0.tar", max compression
```

## Comparing `themis_imager_readfile-1.1.4.tar` & `themis_imager_readfile-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.1.4/LICENSE
--rw-r--r--   0        0        0     2763 2023-05-15 18:17:56.997619 themis_imager_readfile-1.1.4/README.md
--rw-r--r--   0        0        0      666 2023-05-15 18:23:59.979989 themis_imager_readfile-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       49 2023-05-15 18:24:00.010990 themis_imager_readfile-1.1.4/themis_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8458 2023-05-15 18:23:45.670699 themis_imager_readfile-1.1.4/themis_imager_readfile/_themis.py
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 themis_imager_readfile-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2763 2023-05-15 18:17:56.997619 themis_imager_readfile-1.2.0/README.md
+-rw-r--r--   0        0        0      666 2023-05-31 15:36:41.261336 themis_imager_readfile-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-05-31 15:36:41.294337 themis_imager_readfile-1.2.0/themis_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     9271 2023-05-31 15:40:04.332431 themis_imager_readfile-1.2.0/themis_imager_readfile/_themis.py
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 themis_imager_readfile-1.2.0/PKG-INFO
```

### Comparing `themis_imager_readfile-1.1.4/LICENSE` & `themis_imager_readfile-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.1.4/README.md` & `themis_imager_readfile-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.1.4/pyproject.toml` & `themis_imager_readfile-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "themis-imager-readfile"
-version = "1.1.4"
+version = "1.2.0"
 description = "Read functions for THEMIS ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `themis_imager_readfile-1.1.4/themis_imager_readfile/_themis.py` & `themis_imager_readfile-1.2.0/themis_imager_readfile/_themis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-# Author: Lukas Vollmerhaus
-# Date: 2020-10-16
-
 import gzip
 import bz2
-import numpy as np
 import signal
+import numpy as np
 from multiprocessing import Pool
 
 # globals
 THEMIS_IMAGE_SIZE_BYTES = 131072
 THEMIS_DT = np.dtype("uint16")
 THEMIS_DT = THEMIS_DT.newbyteorder('>')  # force big endian byte ordering
 THEMIS_EXPECTED_MINUTE_NUM_FRAMES = 20
@@ -31,24 +28,41 @@
     pool = Pool(processes=workers)
     signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
 
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
-    # call readfile function, run each iteration with a single input file from file_list
-    # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
-    data = []
-    try:
-        data = pool.map(__themis_readfile_worker, file_list)
-    except KeyboardInterrupt:
-        pool.terminate()  # gracefully kill children
-        return np.empty((0, 0, 0), dtype=THEMIS_DT), [], []
+    # check workers
+    if (workers > 1):
+        try:
+            # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
+            original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+            pool = Pool(processes=workers)
+            signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+        except ValueError:
+            # likely the read call is being used within a context that doesn't support the usage
+            # of signals in this way, proceed without it
+            pool = Pool(processes=workers)
+
+        # call readfile function, run each iteration with a single input file from file_list
+        # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
+        data = []
+        try:
+            data = pool.map(__themis_readfile_worker, file_list)
+        except KeyboardInterrupt:
+            pool.terminate()  # gracefully kill children
+            return np.empty((0, 0, 0), dtype=THEMIS_DT), [], []
+        else:
+            pool.close()
     else:
-        pool.close()
+        # don't bother using multiprocessing with one worker, just call the worker function directly
+        data = []
+        for f in file_list:
+            data.append(__themis_readfile_worker(f))
 
     # derive number of frames to prepare for
     total_num_frames = 0
     for i in range(0, len(data)):
         if (data[i][2] is True):
             continue
         total_num_frames += data[i][0].shape[2]
```

### Comparing `themis_imager_readfile-1.1.4/PKG-INFO` & `themis_imager_readfile-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themis-imager-readfile
-Version: 1.1.4
+Version: 1.2.0
 Summary: Read functions for THEMIS ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/themis-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

