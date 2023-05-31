# Comparing `tmp/rainbow_imager_readfile-1.1.1.tar.gz` & `tmp/rainbow_imager_readfile-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rainbow_imager_readfile-1.1.1.tar", max compression
+gzip compressed data, was "rainbow_imager_readfile-1.2.0.tar", max compression
```

## Comparing `rainbow_imager_readfile-1.1.1.tar` & `rainbow_imager_readfile-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-06-16 15:28:11.000000 rainbow_imager_readfile-1.1.1/LICENSE
--rw-r--r--   0        0        0     2384 2023-05-04 21:39:27.812884 rainbow_imager_readfile-1.1.1/README.md
--rw-r--r--   0        0        0      671 2023-05-05 13:27:50.346960 rainbow_imager_readfile-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       50 2023-05-05 13:27:50.381960 rainbow_imager_readfile-1.1.1/rainbow_imager_readfile/__init__.py
--rw-r--r--   0        0        0     7868 2021-11-17 16:50:19.000000 rainbow_imager_readfile-1.1.1/rainbow_imager_readfile/_rainbow.py
--rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 rainbow_imager_readfile-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-06-16 15:28:11.000000 rainbow_imager_readfile-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2672 2023-05-31 17:20:46.890601 rainbow_imager_readfile-1.2.0/README.md
+-rw-r--r--   0        0        0      671 2023-05-31 17:20:46.899601 rainbow_imager_readfile-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-31 17:20:46.899601 rainbow_imager_readfile-1.2.0/rainbow_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8356 2023-05-31 17:20:46.899601 rainbow_imager_readfile-1.2.0/rainbow_imager_readfile/_rainbow.py
+-rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 rainbow_imager_readfile-1.2.0/PKG-INFO
```

### Comparing `rainbow_imager_readfile-1.1.1/LICENSE` & `rainbow_imager_readfile-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rainbow_imager_readfile-1.1.1/README.md` & `rainbow_imager_readfile-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import rainbow_imager_readfile`
 
+**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
+
 ### Read a single file
 
 ```python
 >>> import rainbow_imager_readfile
 >>> filename = "path/to/data/2015/01/01/fsmi_rainbow-11/ut06/20150101_0600_fsmi_rainbow-11_full.pgm.gz"
 >>> img, meta, problematic_files = rainbow_imager_readfile.read(filename)
 ```
```

### Comparing `rainbow_imager_readfile-1.1.1/pyproject.toml` & `rainbow_imager_readfile-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rainbow-imager-readfile"
-version = "1.1.1"
+version = "1.2.0"
 description = "Read functions for Rainbow ASI PNM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rainbow-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rainbow-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `rainbow_imager_readfile-1.1.1/rainbow_imager_readfile/_rainbow.py` & `rainbow_imager_readfile-1.2.0/rainbow_imager_readfile/_rainbow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-# Author: Lukas Vollmerhaus
-# Date: 2020-10-16
-
-import gzip as gzip
+import gzip
 import bz2
+import signal
 import numpy as np
-import signal as signal
-from multiprocessing import Pool as Pool
+from multiprocessing import Pool
 
 # globals
 RAINBOW_IMAGE_SIZE_BYTES = 256 * 512 * 2
 RAINBOW_DT = np.dtype("uint16")
 RAINBOW_DT = RAINBOW_DT.newbyteorder('>')  # force big endian byte ordering
 
 
@@ -27,33 +24,45 @@
     """
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 10
     images = np.empty([256, 512, predicted_num_frames], dtype=RAINBOW_DT)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
-    # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    pool = Pool(processes=workers)
-    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
-
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
-    # call readfile function, run each iteration with a single input file from file_list
-    # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
-    data = []
-    try:
-        data = pool.map(__rainbow_readfile_worker, file_list)
-    except KeyboardInterrupt:
-        pool.terminate()  # gracefully kill children
-        return np.empty((0, 0, 0), dtype=RAINBOW_DT), [], []
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
+            data = pool.map(__rainbow_readfile_worker, file_list)
+        except KeyboardInterrupt:
+            pool.terminate()  # gracefully kill children
+            return np.empty((0, 0, 0), dtype=RAINBOW_DT), [], []
+        else:
+            pool.close()
     else:
-        pool.close()
+        # don't bother using multiprocessing with one worker, just call the worker function directly
+        data = []
+        for f in file_list:
+            data.append(__rainbow_readfile_worker(f))
 
     # reorganize data
     list_position = 0
     for i in range(0, len(data)):
         # check if file was problematic
         if (data[i][2] is True):
             problematic_file_list.append({
```

### Comparing `rainbow_imager_readfile-1.1.1/PKG-INFO` & `rainbow_imager_readfile-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rainbow-imager-readfile
-Version: 1.1.1
+Version: 1.2.0
 Summary: Read functions for Rainbow ASI PNM raw files
 Home-page: https://github.com/ucalgary-aurora/rainbow-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,16 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import rainbow_imager_readfile`
 
+**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
+
 ### Read a single file
 
 ```python
 >>> import rainbow_imager_readfile
 >>> filename = "path/to/data/2015/01/01/fsmi_rainbow-11/ut06/20150101_0600_fsmi_rainbow-11_full.pgm.gz"
 >>> img, meta, problematic_files = rainbow_imager_readfile.read(filename)
 ```
```

