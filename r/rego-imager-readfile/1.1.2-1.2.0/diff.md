# Comparing `tmp/rego_imager_readfile-1.1.2.tar.gz` & `tmp/rego_imager_readfile-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rego_imager_readfile-1.1.2.tar", max compression
+gzip compressed data, was "rego_imager_readfile-1.2.0.tar", max compression
```

## Comparing `rego_imager_readfile-1.1.2.tar` & `rego_imager_readfile-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.1.2/LICENSE
--rw-r--r--   0        0        0     2688 2023-05-30 20:01:33.986595 rego_imager_readfile-1.1.2/README.md
--rw-r--r--   0        0        0      656 2023-05-30 19:42:44.551426 rego_imager_readfile-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-30 19:42:44.587427 rego_imager_readfile-1.1.2/rego_imager_readfile/__init__.py
--rw-r--r--   0        0        0     7886 2023-05-30 19:54:16.486928 rego_imager_readfile-1.1.2/rego_imager_readfile/_rego.py
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 rego_imager_readfile-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2688 2023-05-30 20:01:33.986595 rego_imager_readfile-1.2.0/README.md
+-rw-r--r--   0        0        0      656 2023-05-30 21:50:02.012379 rego_imager_readfile-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-05-30 21:50:02.056681 rego_imager_readfile-1.2.0/rego_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8216 2023-05-31 15:31:57.803617 rego_imager_readfile-1.2.0/rego_imager_readfile/_rego.py
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 rego_imager_readfile-1.2.0/PKG-INFO
```

### Comparing `rego_imager_readfile-1.1.2/LICENSE` & `rego_imager_readfile-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rego_imager_readfile-1.1.2/README.md` & `rego_imager_readfile-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rego_imager_readfile-1.1.2/pyproject.toml` & `rego_imager_readfile-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rego-imager-readfile"
-version = "1.1.2"
+version = "1.2.0"
 description = "Read functions for REGO ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `rego_imager_readfile-1.1.2/rego_imager_readfile/_rego.py` & `rego_imager_readfile-1.2.0/rego_imager_readfile/_rego.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,38 +23,45 @@
     """
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 20
     images = np.empty([512, 512, predicted_num_frames], dtype=REGO_DT)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
-    # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    try:
-        original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-        pool = Pool(processes=workers)
-        signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
-    except ValueError:
-        # likely the read call is being used within a context that doesn't support the usage
-        # of signals in this way, proceed without it
-        pool = Pool(processes=workers)
-
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
-    # call readfile function, run each iteration with a single input file from file_list
-    # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
-    data = []
-    try:
-        data = pool.map(__rego_readfile_worker, file_list)
-    except KeyboardInterrupt:
-        pool.terminate()  # gracefully kill children
-        return np.empty((0, 0, 0), dtype=REGO_DT), [], []
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
+            data = pool.map(__rego_readfile_worker, file_list)
+        except KeyboardInterrupt:
+            pool.terminate()  # gracefully kill children
+            return np.empty((0, 0, 0), dtype=REGO_DT), [], []
+        else:
+            pool.close()
     else:
-        pool.close()
+        # don't bother using multiprocessing with one worker, just call the worker function directly
+        data = []
+        for f in file_list:
+            data.append(__rego_readfile_worker(f))
 
     # reorganize data
     list_position = 0
     for i in range(0, len(data)):
         # check if file was problematic
         if (data[i][2] is True):
             problematic_file_list.append({
```

### Comparing `rego_imager_readfile-1.1.2/PKG-INFO` & `rego_imager_readfile-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rego-imager-readfile
-Version: 1.1.2
+Version: 1.2.0
 Summary: Read functions for REGO ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/rego-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

