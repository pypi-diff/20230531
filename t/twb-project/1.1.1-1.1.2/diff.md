# Comparing `tmp/twb_project-1.1.1.tar.gz` & `tmp/twb_project-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-1.1.1.tar", max compression
+gzip compressed data, was "twb_project-1.1.2.tar", max compression
```

## Comparing `twb_project-1.1.1.tar` & `twb_project-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-1.1.1/LICENSE
--rw-r--r--   0        0        0     1547 2023-05-21 20:04:40.510524 twb_project-1.1.1/README.md
--rw-r--r--   0        0        0      789 2023-05-24 01:45:19.534352 twb_project-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      143 2023-05-07 20:45:45.325589 twb_project-1.1.1/twb/__init__.py
--rw-r--r--   0        0        0    17371 2023-05-24 01:44:19.877508 twb_project-1.1.1/twb/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-1.1.1/twb/builder_helpers.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-1.1.1/twb/decompressor.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-1.1.1/twb/logger.py
--rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-1.1.1/twb/logger_init.py
--rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-1.1.1/twb/modifier.py
--rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-1.1.1/twb/parallelization.py
--rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-1.1.1/twb/reader.py
--rw-r--r--   0        0        0     6171 2023-05-07 20:45:49.998705 twb_project-1.1.1/twb/utils.py
--rw-r--r--   0        0        0     3727 2023-05-22 12:48:38.539400 twb_project-1.1.1/twb/warehouse.py
--rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 twb_project-1.1.1/setup.py
--rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 twb_project-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-28 03:07:12.633514 twb_project-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1547 2023-05-30 07:08:14.558669 twb_project-1.1.2/README.md
+-rw-r--r--   0        0        0      789 2023-05-30 07:30:59.971888 twb_project-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-05-30 07:08:14.560735 twb_project-1.1.2/twb/__init__.py
+-rw-r--r--   0        0        0    17495 2023-05-30 07:19:35.445062 twb_project-1.1.2/twb/builder.py
+-rw-r--r--   0        0        0      227 2023-05-11 18:08:24.857609 twb_project-1.1.2/twb/builder_helpers.py
+-rw-r--r--   0        0        0     4614 2023-04-06 18:50:03.439320 twb_project-1.1.2/twb/decompressor.py
+-rw-r--r--   0        0        0     3794 2023-05-02 18:22:48.993196 twb_project-1.1.2/twb/logger.py
+-rw-r--r--   0        0        0     1817 2023-05-11 18:08:24.856968 twb_project-1.1.2/twb/logger_init.py
+-rw-r--r--   0        0        0    10603 2023-05-02 19:31:59.045022 twb_project-1.1.2/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-05-02 18:22:48.993375 twb_project-1.1.2/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 18:23:52.860733 twb_project-1.1.2/twb/reader.py
+-rw-r--r--   0        0        0     6171 2023-05-30 07:08:14.561011 twb_project-1.1.2/twb/utils.py
+-rw-r--r--   0        0        0     3727 2023-05-30 07:08:14.560833 twb_project-1.1.2/twb/warehouse.py
+-rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 twb_project-1.1.2/PKG-INFO
```

### Comparing `twb_project-1.1.1/LICENSE` & `twb_project-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/README.md` & `twb_project-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/pyproject.toml` & `twb_project-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "1.1.1"
+version = "1.1.2"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-1.1.1/twb/builder.py` & `twb_project-1.1.2/twb/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,23 +83,27 @@
         archive_filename = os.path.basename(file_path)
         random_id = uuid.uuid4().hex
         decompressed_dir_path = os.path.join(temp_dir, random_id)
         os.makedirs(decompressed_dir_path, exist_ok=True)
 
         logging.debug(f'Decompressing [{archive_filename}]...')
 
-        with py7zr.SevenZipFile(file_path, mode='r', mp=False) as z:
-            start_time = time.time()
-            z.extractall(path=decompressed_dir_path)
-            end_time = time.time()
-            execution_duration = (end_time - start_time) / 60
-            logging.debug(f'Decompression took {execution_duration:.2f} min. ({archive_filename})')
-        decompressed_files = get_file_list(decompressed_dir_path)
+        try:
+            with py7zr.SevenZipFile(file_path, mode='r', mp=False) as z:
+                start_time = time.time()
+                z.extractall(path=decompressed_dir_path)
+                end_time = time.time()
+                execution_duration = (end_time - start_time) / 60
+                logging.debug(f'Decompression took {execution_duration:.2f} min. ({archive_filename})')
+            decompressed_files = get_file_list(decompressed_dir_path)
+            return decompressed_files
 
-        return decompressed_files
+        except Exception as e:
+            logging.critical(f'Failed to decompress [{archive_filename}] for this reason: {e}')
+            return []
 
     def _process_executor(self, xml_path: str, warehouse: Warehouse) -> List[str]:
         """
         Process the file.
         :param xml_path: the path of the file to be processed.
         :return: the number of URLs processed
         """
@@ -303,60 +307,55 @@
             initializer=self._worker_initializer,
             initargs=(q,),
         )
 
         processed_count = 0
 
         def _decompress_callback(decompressed_files: List[str]):
-            nonlocal available_process_count
-
             if not decompressed_files:
                 logging.debug(f'Decompressed (EMPTY): {decompressed_files}')
                 return
 
             decompressed_dir = os.path.dirname(decompressed_files[0])
             logging.debug(f'Decompressed (OK): {decompressed_dir} ({len(decompressed_files)})')
 
             for decompressed_file in decompressed_files:
                 next_task_type = 'process'
                 next_args = (decompressed_file,)
                 tasks.insert(0, (next_task_type, next_args))
 
-            available_process_count += 1
-
         def _process_callback(full_warehouse_paths: List[Tuple[str, str]]):
-            nonlocal available_process_count, processed_count
+            nonlocal processed_count
             processed_count += 1
 
             logging.info(f'({processed_count / total_count * 100:.2f}% = {processed_count} / {total_count}) | '
                          f'Full warehouses: {len(full_warehouse_paths)}')
 
             for full_warehouse_path in full_warehouse_paths:
                 next_task_type = 'cleanup'
                 next_args = (full_warehouse_path,)
                 tasks.insert(0, (next_task_type, next_args))
 
-            available_process_count += 1
-
         def _cleanup_callback(cleanup_path):
-            nonlocal available_process_count
             logging.info(f'Warehouse packed: {cleanup_path}')
 
-            available_process_count += 1
-
         def _success_callback(task_type, file_path):
+            nonlocal available_process_count
             if task_type == 'decompress':
                 _decompress_callback(file_path)
             elif task_type == 'process':
                 _process_callback(file_path)
             elif task_type == 'cleanup':
                 _cleanup_callback(file_path)
+            available_process_count += 1
 
         def _error_callback(e):
+            nonlocal available_process_count
             logging.critical(f'Process terminated-level error: {e}')
+            available_process_count += 1
 
         # Built-up initial tasks.
         for curr_file_path in self.files:
             tasks.append(('decompress', (curr_file_path,)))
 
         # Main semaphore loop.
         while tasks or available_process_count < self.num_proc:
```

### Comparing `twb_project-1.1.1/twb/decompressor.py` & `twb_project-1.1.2/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/twb/logger.py` & `twb_project-1.1.2/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/twb/logger_init.py` & `twb_project-1.1.2/twb/logger_init.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/twb/modifier.py` & `twb_project-1.1.2/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/twb/parallelization.py` & `twb_project-1.1.2/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/twb/reader.py` & `twb_project-1.1.2/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/twb/utils.py` & `twb_project-1.1.2/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/twb/warehouse.py` & `twb_project-1.1.2/twb/warehouse.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.1/PKG-INFO` & `twb_project-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 1.1.1
+Version: 1.1.2
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

