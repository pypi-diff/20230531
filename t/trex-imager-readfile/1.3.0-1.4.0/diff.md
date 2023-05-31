# Comparing `tmp/trex_imager_readfile-1.3.0.tar.gz` & `tmp/trex_imager_readfile-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex_imager_readfile-1.3.0.tar", max compression
+gzip compressed data, was "trex_imager_readfile-1.4.0.tar", max compression
```

## Comparing `trex_imager_readfile-1.3.0.tar` & `trex_imager_readfile-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      186 2023-04-25 13:48:57.783144 trex_imager_readfile-1.3.0/README.md
--rw-r--r--   0        0        0      693 2023-05-05 12:55:57.394400 trex_imager_readfile-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      397 2023-05-05 12:55:57.428400 trex_imager_readfile-1.3.0/trex_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8497 2023-05-03 20:42:44.563933 trex_imager_readfile-1.3.0/trex_imager_readfile/blueline.py
--rw-r--r--   0        0        0     8447 2023-05-03 20:42:40.512856 trex_imager_readfile-1.3.0/trex_imager_readfile/nir.py
--rw-r--r--   0        0        0    19882 2023-05-04 17:38:07.536838 trex_imager_readfile-1.3.0/trex_imager_readfile/rgb.py
--rw-r--r--   0        0        0     8541 2023-05-03 20:42:47.366986 trex_imager_readfile-1.3.0/trex_imager_readfile/spectrograph.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 trex_imager_readfile-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-04-25 13:48:57.783144 trex_imager_readfile-1.4.0/README.md
+-rw-r--r--   0        0        0      699 2023-05-31 18:09:31.438669 trex_imager_readfile-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      397 2023-05-31 18:09:31.471670 trex_imager_readfile-1.4.0/trex_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8497 2023-05-03 20:42:44.563933 trex_imager_readfile-1.4.0/trex_imager_readfile/blueline.py
+-rw-r--r--   0        0        0     8447 2023-05-03 20:42:40.512856 trex_imager_readfile-1.4.0/trex_imager_readfile/nir.py
+-rw-r--r--   0        0        0    20625 2023-05-31 18:11:41.895299 trex_imager_readfile-1.4.0/trex_imager_readfile/rgb.py
+-rw-r--r--   0        0        0     8541 2023-05-03 20:42:47.366986 trex_imager_readfile-1.4.0/trex_imager_readfile/spectrograph.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 trex_imager_readfile-1.4.0/PKG-INFO
```

### Comparing `trex_imager_readfile-1.3.0/pyproject.toml` & `trex_imager_readfile-1.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trex-imager-readfile"
-version = "1.3.0"
+version = "1.4.0"
 description = "Read functions for TREx ASI raw image files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
@@ -13,15 +13,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 numpy = "^1.21.0"
 opencv-python = "^4.4.0"
 h5py = "^3.1.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
 flake8 = "^6.0.0"
 pylint = "^2.16.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `trex_imager_readfile-1.3.0/trex_imager_readfile/blueline.py` & `trex_imager_readfile-1.4.0/trex_imager_readfile/blueline.py`

 * *Files identical despite different names*

### Comparing `trex_imager_readfile-1.3.0/trex_imager_readfile/nir.py` & `trex_imager_readfile-1.4.0/trex_imager_readfile/nir.py`

 * *Files identical despite different names*

### Comparing `trex_imager_readfile-1.3.0/trex_imager_readfile/rgb.py` & `trex_imager_readfile-1.4.0/trex_imager_readfile/rgb.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,42 +432,57 @@
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
     # set tar path
     if (tar_tempdir is None):
         tar_tempdir = Path("%s/.trex_imager_readfile" % (str(Path.home())))
-
-    # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    pool = Pool(processes=workers)
-    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+    if not (os.path.exists(tar_tempdir)):
+        os.makedirs(tar_tempdir)
 
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
     # convert to object, injecting other data we need for processing
     processing_list = []
     for f in file_list:
         processing_list.append({
             "filename": f,
             "tar_tempdir": tar_tempdir,
             "quiet": quiet,
         })
 
-    # call readfile function, run each iteration with a single input file from file_list
-    pool_data = []
-    try:
-        pool_data = pool.map(__trex_readfile_worker, processing_list)
-    except KeyboardInterrupt:
-        pool.terminate()  # gracefully kill children
-        return np.empty((0, 0, 0)), [], []
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
+        pool_data = []
+        try:
+            pool_data = pool.map(__trex_readfile_worker, processing_list)
+        except KeyboardInterrupt:
+            pool.terminate()  # gracefully kill children
+            return np.empty((0, 0, 0)), [], []
+        else:
+            pool.close()
     else:
-        pool.close()
+        # don't bother using multiprocessing with one worker, just call the worker function directly
+        pool_data = []
+        for p in processing_list:
+            pool_data.append(__trex_readfile_worker(p))
 
     # set sizes
     image_width = pool_data[0][5]
     image_height = pool_data[0][6]
     image_channels = pool_data[0][7]
     image_dtype = pool_data[0][8]
```

### Comparing `trex_imager_readfile-1.3.0/trex_imager_readfile/spectrograph.py` & `trex_imager_readfile-1.4.0/trex_imager_readfile/spectrograph.py`

 * *Files identical despite different names*

### Comparing `trex_imager_readfile-1.3.0/PKG-INFO` & `trex_imager_readfile-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-imager-readfile
-Version: 1.3.0
+Version: 1.4.0
 Summary: Read functions for TREx ASI raw image files
 Home-page: https://github.com/ucalgary-aurora/trex-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

