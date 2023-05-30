# Comparing `tmp/quick_batch-0.1.7.tar.gz` & `tmp/quick_batch-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_batch-0.1.7.tar", max compression
+gzip compressed data, was "quick_batch-0.1.8.tar", max compression
```

## Comparing `quick_batch-0.1.7.tar` & `quick_batch-0.1.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     4187 2023-05-30 23:18:23.808608 quick_batch-0.1.7/README.md
--rw-r--r--   0        0        0      685 2023-05-30 23:18:23.808608 quick_batch-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      120 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/__init__.py
--rw-r--r--   0        0        0      580 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/main.py
--rw-r--r--   0        0        0      831 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/manual_scaler.py
--rwxr-xr-x   0        0        0     1215 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/processor_app/__init__.py
--rwxr-xr-x   0        0        0     1747 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/processor_app/activate_process.py
--rwxr-xr-x   0        0        0     2234 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/processor_app/api_connects.py
--rwxr-xr-x   0        0        0      409 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/processor_app/run.py
--rwxr-xr-x   0        0        0     5224 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/wait-for-it.sh
--rw-r--r--   0        0        0      241 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/Dockerfile
--rw-r--r--   0        0        0     1220 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/queue_app/__init__.py
--rw-r--r--   0        0        0     2312 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/queue_app/apis.py
--rw-r--r--   0        0        0     3250 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/queue_app/queues_init.py
--rw-r--r--   0        0        0      424 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/queue_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/wait-for-it.sh
--rw-r--r--   0        0        0      721 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/runner.py
--rw-r--r--   0        0        0      551 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/__init__.py
--rw-r--r--   0        0        0      146 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_client.py
--rw-r--r--   0        0        0     2088 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_containers.py
--rw-r--r--   0        0        0     1244 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_dockerfile.py
--rw-r--r--   0        0        0     4624 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_images.py
--rw-r--r--   0        0        0     1951 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_loggers.py
--rw-r--r--   0        0        0      551 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_networks.py
--rw-r--r--   0        0        0     2487 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_queue.py
--rw-r--r--   0        0        0     2033 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_requirements.py
--rw-r--r--   0        0        0     4722 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_services.py
--rw-r--r--   0        0        0     3207 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_setup.py
--rw-r--r--   0        0        0      229 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_swarm.py
--rw-r--r--   0        0        0     4429 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/param_checks.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 quick_batch-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4187 2023-05-30 23:49:42.799400 quick_batch-0.1.8/README.md
+-rw-r--r--   0        0        0      685 2023-05-30 23:49:42.799400 quick_batch-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/__init__.py
+-rw-r--r--   0        0        0      644 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/main.py
+-rw-r--r--   0        0        0      831 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/manual_scaler.py
+-rwxr-xr-x   0        0        0     1215 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/processor_app/__init__.py
+-rwxr-xr-x   0        0        0     1747 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/processor_app/activate_process.py
+-rwxr-xr-x   0        0        0     2234 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/processor_app/api_connects.py
+-rwxr-xr-x   0        0        0      409 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/processor_app/run.py
+-rwxr-xr-x   0        0        0     5224 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/processor_app/wait-for-it.sh
+-rw-r--r--   0        0        0      241 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/Dockerfile
+-rw-r--r--   0        0        0     1220 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/queue_app/__init__.py
+-rw-r--r--   0        0        0     2312 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/queue_app/apis.py
+-rw-r--r--   0        0        0     3252 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/queue_app/queues_init.py
+-rw-r--r--   0        0        0      424 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/queue_app/run.py
+-rwxr-xr-x   0        0        0       21 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/requirements.txt
+-rwxr-xr-x   0        0        0     5224 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/queue_app/wait-for-it.sh
+-rw-r--r--   0        0        0      721 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/runner.py
+-rw-r--r--   0        0        0      551 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/__init__.py
+-rw-r--r--   0        0        0      146 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_client.py
+-rw-r--r--   0        0        0     2088 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_containers.py
+-rw-r--r--   0        0        0     1244 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_dockerfile.py
+-rw-r--r--   0        0        0     4624 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_images.py
+-rw-r--r--   0        0        0     1951 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_loggers.py
+-rw-r--r--   0        0        0      551 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_networks.py
+-rw-r--r--   0        0        0     2487 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_queue.py
+-rw-r--r--   0        0        0     2033 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_requirements.py
+-rw-r--r--   0        0        0     4722 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_services.py
+-rw-r--r--   0        0        0     3207 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_setup.py
+-rw-r--r--   0        0        0      229 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/manage_swarm.py
+-rw-r--r--   0        0        0     4429 2023-05-30 23:49:42.799400 quick_batch-0.1.8/quick_batch/utilities/param_checks.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 quick_batch-0.1.8/PKG-INFO
```

### Comparing `quick_batch-0.1.7/README.md` & `quick_batch-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/pyproject.toml` & `quick_batch-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quick_batch"
-version = "0.1.7"
+version = "0.1.8"
 description = "ultra simple command line tool for docker-scaling batch processing"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/quick_batch"
 license = "MIT"
 
 [tool.poetry.scripts]
```

### Comparing `quick_batch-0.1.7/quick_batch/main.py` & `quick_batch-0.1.8/quick_batch/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 def main(config=None):
     # check config - used as script fire will not be used
     if not config:
         # check argument provided - config or num_processors
         if sys.argv[1] == 'config':
             config = sys.argv[2]
             runner.run(config)
+            return None
         elif sys.argv[1] == 'scale':
             num_processors = int(sys.argv[2])
             manual_scaler.scaler(num_processors)
+            return None
 
     # check config - used as script fire will be used
     runner.run(config)
+    return None
 
 
 if __name__ == '__main__':
     fire.Fire(main)
```

### Comparing `quick_batch-0.1.7/quick_batch/manual_scaler.py` & `quick_batch-0.1.8/quick_batch/manual_scaler.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/processor_app/processor_app/__init__.py` & `quick_batch-0.1.8/quick_batch/processor_app/processor_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/processor_app/processor_app/activate_process.py` & `quick_batch-0.1.8/quick_batch/processor_app/processor_app/activate_process.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/processor_app/processor_app/api_connects.py` & `quick_batch-0.1.8/quick_batch/processor_app/processor_app/api_connects.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/processor_app/wait-for-it.sh` & `quick_batch-0.1.8/quick_batch/processor_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/queue_app/queue_app/__init__.py` & `quick_batch-0.1.8/quick_batch/queue_app/queue_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/queue_app/queue_app/apis.py` & `quick_batch-0.1.8/quick_batch/queue_app/queue_app/apis.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/queue_app/queue_app/queues_init.py` & `quick_batch-0.1.8/quick_batch/queue_app/queue_app/queues_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,14 @@
     # load up queue with organized_paths
     feed_counter = 0
     for item in organized_datapaths:
         app.feeder_queue.append(item)
         feed_counter += 1
 
     print('done loading feeder queue!', flush=True)
-    print(app.feeder_queue, flush=True)
+    # print(app.feeder_queue, flush=True)
 
     # init queue counters
     app.feed_queue_length = feed_counter
     app.original_feed_queue_length = feed_counter
     app.wip_queue_length = 0
     app.done_queue_length = 0
```

### Comparing `quick_batch-0.1.7/quick_batch/queue_app/wait-for-it.sh` & `quick_batch-0.1.8/quick_batch/queue_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/runner.py` & `quick_batch-0.1.8/quick_batch/runner.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/__init__.py` & `quick_batch-0.1.8/quick_batch/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/manage_containers.py` & `quick_batch-0.1.8/quick_batch/utilities/manage_containers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/manage_dockerfile.py` & `quick_batch-0.1.8/quick_batch/utilities/manage_dockerfile.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/manage_images.py` & `quick_batch-0.1.8/quick_batch/utilities/manage_images.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/manage_loggers.py` & `quick_batch-0.1.8/quick_batch/utilities/manage_loggers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/manage_networks.py` & `quick_batch-0.1.8/quick_batch/utilities/manage_networks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/manage_queue.py` & `quick_batch-0.1.8/quick_batch/utilities/manage_queue.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/manage_requirements.py` & `quick_batch-0.1.8/quick_batch/utilities/manage_requirements.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/manage_services.py` & `quick_batch-0.1.8/quick_batch/utilities/manage_services.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/manage_setup.py` & `quick_batch-0.1.8/quick_batch/utilities/manage_setup.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/quick_batch/utilities/param_checks.py` & `quick_batch-0.1.8/quick_batch/utilities/param_checks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.7/PKG-INFO` & `quick_batch-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-batch
-Version: 0.1.7
+Version: 0.1.8
 Summary: ultra simple command line tool for docker-scaling batch processing
 Home-page: https://github.com/jermwatt/quick_batch
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

