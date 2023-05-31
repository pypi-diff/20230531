# Comparing `tmp/nascam_imager_readfile-1.2.1.tar.gz` & `tmp/nascam_imager_readfile-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nascam_imager_readfile-1.2.1.tar", max compression
+gzip compressed data, was "nascam_imager_readfile-1.3.0.tar", max compression
```

## Comparing `nascam_imager_readfile-1.2.1.tar` & `nascam_imager_readfile-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.2.1/LICENSE
--rw-r--r--   0        0        0     2513 2023-05-04 21:39:35.746033 nascam_imager_readfile-1.2.1/README.md
--rw-r--r--   0        0        0       49 2023-05-05 13:27:03.375086 nascam_imager_readfile-1.2.1/nascam_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8183 2023-05-04 21:33:12.222821 nascam_imager_readfile-1.2.1/nascam_imager_readfile/_nascam.py
--rw-r--r--   0        0        0      687 2023-05-05 13:27:03.338086 nascam_imager_readfile-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2801 2023-05-31 17:29:41.564429 nascam_imager_readfile-1.3.0/README.md
+-rw-r--r--   0        0        0       49 2023-05-31 17:29:51.092622 nascam_imager_readfile-1.3.0/nascam_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     9089 2023-05-31 18:07:17.540970 nascam_imager_readfile-1.3.0/nascam_imager_readfile/_nascam.py
+-rw-r--r--   0        0        0      687 2023-05-31 17:29:51.032621 nascam_imager_readfile-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.3.0/PKG-INFO
```

### Comparing `nascam_imager_readfile-1.2.1/LICENSE` & `nascam_imager_readfile-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nascam_imager_readfile-1.2.1/README.md` & `nascam_imager_readfile-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import nascam_imager_readfile`
 
+**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
+
 ### Read a single file
 
 ```python
 >>> import nascam_imager_readfile
 >>> filename = "path/to/data/2010/01/01/atha_nascam-iccd04/ut06/20100101_0600_atha_nascam-iccd04.png.tar"
 >>> img, meta, problematic_files = nascam_imager_readfile.read(filename)
 ```
```

### Comparing `nascam_imager_readfile-1.2.1/nascam_imager_readfile/_nascam.py` & `nascam_imager_readfile-1.3.0/nascam_imager_readfile/_nascam.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import signal
 import cv2
 import tarfile
 import os
 import datetime
 import numpy as np
+from pathlib import Path
 from multiprocessing import Pool
 
 # static globals
 __EXPECTED_FRAME_COUNT = 20
 __PNG_METADATA_PROJECT_UID = "nascam"
 
 
@@ -21,15 +22,15 @@
     image_height = 0
     image_dtype = np.dtype("uint16")
     image_dtype = image_dtype.newbyteorder('>')
 
     # check file extension to know how to process
     try:
         if (file_obj["filename"].endswith("png") or file_obj["filename"].endswith("png.tar")):
-            return __nascam_readfile_worker_png(file_obj["filename"])
+            return __nascam_readfile_worker_png(file_obj)
         else:
             print("Unrecognized file type: %s" % (file_obj["filename"]))
     except Exception as e:
         import traceback
         traceback.print_exc()
         print("Failed to process file '%s' " % (file_obj["filename"]))
         problematic = True
@@ -134,55 +135,74 @@
             os.remove(f)
 
     # return
     return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
         image_width, image_height, image_dtype
 
 
-def read(file_list, workers=1, tar_tempdir=os.getcwd()):
+def read(file_list, workers=1, tar_tempdir=None):
     """
     Read in a single PNG.TAR file, or an array of them. All files
     must be the same type.
 
     :param file_list: filename or list of filenames
     :type file_list: str
     :param workers: number of worker processes to spawn, defaults to 1
     :type workers: int, optional
-    :param tar_tempdir: path to untar to, defaults to '.'
+    :param tar_tempdir: path to untar to, defaults to '~/.nascam_imager_readfile'
     :type tar_tempdir: str, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
-    # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    pool = Pool(processes=workers)
-    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+    # set tar path
+    if (tar_tempdir is None):
+        tar_tempdir = Path("%s/.nascam_imager_readfile" % (str(Path.home())))
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
         })
 
-    # call readfile function, run each iteration with a single input file from file_list
-    pool_data = []
-    try:
-        pool_data = pool.map(__nascam_readfile_worker, processing_list)
-    except KeyboardInterrupt:
-        pool.terminate()  # gracefully kill children
-        return np.empty((0, 0)), [], []
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
+            pool_data = pool.map(__nascam_readfile_worker, processing_list)
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
+            pool_data.append(__nascam_readfile_worker(p))
 
     # set sizes
     image_width = pool_data[0][5]
     image_height = pool_data[0][6]
     image_dtype = pool_data[0][7]
 
     # pre-allocate array sizes (optimization)
```

### Comparing `nascam_imager_readfile-1.2.1/pyproject.toml` & `nascam_imager_readfile-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nascam-imager-readfile"
-version = "1.2.1"
+version = "1.3.0"
 description = "Read functions for NASCAM ASI raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `nascam_imager_readfile-1.2.1/PKG-INFO` & `nascam_imager_readfile-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nascam-imager-readfile
-Version: 1.2.1
+Version: 1.3.0
 Summary: Read functions for NASCAM ASI raw files
 Home-page: https://github.com/ucalgary-aurora/nascam-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -46,14 +46,16 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import nascam_imager_readfile`
 
+**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
+
 ### Read a single file
 
 ```python
 >>> import nascam_imager_readfile
 >>> filename = "path/to/data/2010/01/01/atha_nascam-iccd04/ut06/20100101_0600_atha_nascam-iccd04.png.tar"
 >>> img, meta, problematic_files = nascam_imager_readfile.read(filename)
 ```
```

