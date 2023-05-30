# Comparing `tmp/quick_batch-0.1.6.tar.gz` & `tmp/quick_batch-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_batch-0.1.6.tar", max compression
+gzip compressed data, was "quick_batch-0.1.7.tar", max compression
```

## Comparing `quick_batch-0.1.6.tar` & `quick_batch-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     3734 2023-05-30 16:09:01.056282 quick_batch-0.1.6/README.md
--rw-r--r--   0        0        0      729 2023-05-30 16:09:01.056282 quick_batch-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      120 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/__init__.py
--rw-r--r--   0        0        0      906 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/main.py
--rw-r--r--   0        0        0     1037 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/manual_scaler.py
--rwxr-xr-x   0        0        0     1215 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/processor_app/__init__.py
--rwxr-xr-x   0        0        0     1747 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/processor_app/activate_process.py
--rwxr-xr-x   0        0        0     2234 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/processor_app/api_connects.py
--rwxr-xr-x   0        0        0      409 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/processor_app/run.py
--rwxr-xr-x   0        0        0     5224 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/wait-for-it.sh
--rw-r--r--   0        0        0      241 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/Dockerfile
--rw-r--r--   0        0        0     1220 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/queue_app/__init__.py
--rw-r--r--   0        0        0     2312 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/queue_app/apis.py
--rw-r--r--   0        0        0     3250 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/queue_app/queues_init.py
--rw-r--r--   0        0        0      424 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/queue_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/wait-for-it.sh
--rw-r--r--   0        0        0      551 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/utilities/__init__.py
--rw-r--r--   0        0        0      146 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/utilities/manage_client.py
--rw-r--r--   0        0        0     2088 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/utilities/manage_containers.py
--rw-r--r--   0        0        0     1244 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/utilities/manage_dockerfile.py
--rw-r--r--   0        0        0     4624 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_images.py
--rw-r--r--   0        0        0     1951 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_loggers.py
--rw-r--r--   0        0        0      551 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_networks.py
--rw-r--r--   0        0        0     2487 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_queue.py
--rw-r--r--   0        0        0     2033 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_requirements.py
--rw-r--r--   0        0        0     4722 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_services.py
--rw-r--r--   0        0        0     3115 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_setup.py
--rw-r--r--   0        0        0      229 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_swarm.py
--rw-r--r--   0        0        0     4429 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/param_checks.py
--rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 quick_batch-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4187 2023-05-30 23:18:23.808608 quick_batch-0.1.7/README.md
+-rw-r--r--   0        0        0      685 2023-05-30 23:18:23.808608 quick_batch-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/__init__.py
+-rw-r--r--   0        0        0      580 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/main.py
+-rw-r--r--   0        0        0      831 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/manual_scaler.py
+-rwxr-xr-x   0        0        0     1215 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/processor_app/__init__.py
+-rwxr-xr-x   0        0        0     1747 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/processor_app/activate_process.py
+-rwxr-xr-x   0        0        0     2234 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/processor_app/api_connects.py
+-rwxr-xr-x   0        0        0      409 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/processor_app/run.py
+-rwxr-xr-x   0        0        0     5224 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/processor_app/wait-for-it.sh
+-rw-r--r--   0        0        0      241 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/Dockerfile
+-rw-r--r--   0        0        0     1220 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/queue_app/__init__.py
+-rw-r--r--   0        0        0     2312 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/queue_app/apis.py
+-rw-r--r--   0        0        0     3250 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/queue_app/queues_init.py
+-rw-r--r--   0        0        0      424 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/queue_app/run.py
+-rwxr-xr-x   0        0        0       21 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/requirements.txt
+-rwxr-xr-x   0        0        0     5224 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/queue_app/wait-for-it.sh
+-rw-r--r--   0        0        0      721 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/runner.py
+-rw-r--r--   0        0        0      551 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/__init__.py
+-rw-r--r--   0        0        0      146 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_client.py
+-rw-r--r--   0        0        0     2088 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_containers.py
+-rw-r--r--   0        0        0     1244 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_dockerfile.py
+-rw-r--r--   0        0        0     4624 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_images.py
+-rw-r--r--   0        0        0     1951 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_loggers.py
+-rw-r--r--   0        0        0      551 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_networks.py
+-rw-r--r--   0        0        0     2487 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_queue.py
+-rw-r--r--   0        0        0     2033 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_requirements.py
+-rw-r--r--   0        0        0     4722 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_services.py
+-rw-r--r--   0        0        0     3207 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_setup.py
+-rw-r--r--   0        0        0      229 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/manage_swarm.py
+-rw-r--r--   0        0        0     4429 2023-05-30 23:18:23.808608 quick_batch-0.1.7/quick_batch/utilities/param_checks.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 quick_batch-0.1.7/PKG-INFO
```

### Comparing `quick_batch-0.1.6/README.md` & `quick_batch-0.1.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 `quick_batch` is an ultra-simple command-line tool for large batch python-driven processing and transformation.  It was designed to be fast to deploy, transparent, and portable.  This allows you to scale any `processor` function that needs to be run over a large set of input data, enabling batch/parallel processing of the input with minimal setup and teardown.
 
 
 - [quick\_batch](#quick_batch)
 - [Getting started](#getting-started)
   - [Usage](#usage)
+  - [Scaling](#scaling)
   - [Installation](#installation)
   - [The `processor.py` file](#the-processorpy-file)
 - [Why use quick\_batch](#why-use-quick_batch)
 
 # Getting started
 
 All you need to scale batch transformations with `quick_batch` is a
@@ -47,20 +48,32 @@
 Output will be written to the `output_path` specified in the configuration file.
 
 You can see `tests/config_files` for examples of valid configs.
 
 
 ## Usage
 
-With your `config.yaml` defined you can use `quick_batch` at the terminal by typing
+To start processing with your `config.yaml` use `quick_batch`'s `config` command at the terminal by typing
 
 ```bash
-quick_batch /path/to/your/config.yaml
+quick_batch config /path/to/your/config.yaml
 ```
 
+This will start the build and deploy process for processing your data as defined in your `config.yaml`.
+
+## Scaling
+
+Use the `scale` commoand to manually scale the number of processors / containers running your process
+
+```bash
+quick_batch scale <num_processors> 
+```
+
+Here `<num_processors>` is an integer >= 1.   For example, to scale to 3 parallel processors / containers: `quick_batch scale 3`
+
 ## Installation
 
 To install quick_batch, simply use `pip`:
 
 ```bash
 pip install quick-batch
 ```
```

### Comparing `quick_batch-0.1.6/pyproject.toml` & `quick_batch-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "quick_batch"
-version = "0.1.6"
+version = "0.1.7"
 description = "ultra simple command line tool for docker-scaling batch processing"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/quick_batch"
 license = "MIT"
 
 [tool.poetry.scripts]
 quick_batch = "quick_batch.main:main"
-qb_scale = "quick_batch.manual_scaler:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^6.1.2"
 fire = "^0.5.0"
 pyyaml = "<5.5"
 dockerfile-parse = "^2.0.0"
```

### Comparing `quick_batch-0.1.6/quick_batch/main.py` & `quick_batch-0.1.7/quick_batch/runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-import sys
-import fire
 from utilities.manage_setup import setup_client
 from utilities.manage_setup import reset_workspace
 from utilities.manage_setup import setup_workspace
 from utilities.manage_queue import monitor_queue
 from utilities.manage_services import scaleup_processor_service
 
 
-def main(config=None):
-    # check config - used as script fire will not be used
-    if not config:
-        config = sys.argv[1]
-
+def run(config):
     # setup
     client, input_path, output_path, processor, num_processors, \
         logger = setup_client(config)
 
     # reset workspace
     reset_workspace(client)
 
@@ -26,11 +20,7 @@
     scaleup_processor_service(client, num_processors)
 
     # monitor queue
     monitor_queue(client)
 
     # close log
     logger.close_log()
-
-
-if __name__ == '__main__':
-    fire.Fire(main)
```

### Comparing `quick_batch-0.1.6/quick_batch/manual_scaler.py` & `quick_batch-0.1.7/quick_batch/manual_scaler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,12 @@
-import sys
-import fire
 from utilities.manage_client import create_client
 from utilities.manage_services import scaleup_processor_service
 
 
-def main(num_processors=None):
-    # check num_processors - used as script fire will not be used
-    if not num_processors:
-        num_processors = int(sys.argv[1])
-
+def scaler(num_processors=None):
     # check num_processors is an integer
     try:
         num_processors = int(num_processors)
     except ValueError:
         raise ValueError("FAILURE: num_processors must be an integer")
 
     # check basic value of num_processors
@@ -27,11 +21,7 @@
           "scaling processor service to {num_processors} instances...")
 
     # scale up processor service
     scaleup_processor_service(client, num_processors)
 
     # print update
     print("INFO: ...complete")
-
-
-if __name__ == '__main__':
-    fire.Fire(main)
```

### Comparing `quick_batch-0.1.6/quick_batch/processor_app/processor_app/__init__.py` & `quick_batch-0.1.7/quick_batch/processor_app/processor_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/processor_app/processor_app/activate_process.py` & `quick_batch-0.1.7/quick_batch/processor_app/processor_app/activate_process.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/processor_app/processor_app/api_connects.py` & `quick_batch-0.1.7/quick_batch/processor_app/processor_app/api_connects.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/processor_app/wait-for-it.sh` & `quick_batch-0.1.7/quick_batch/processor_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/queue_app/queue_app/__init__.py` & `quick_batch-0.1.7/quick_batch/queue_app/queue_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/queue_app/queue_app/apis.py` & `quick_batch-0.1.7/quick_batch/queue_app/queue_app/apis.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/queue_app/queue_app/queues_init.py` & `quick_batch-0.1.7/quick_batch/queue_app/queue_app/queues_init.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/queue_app/wait-for-it.sh` & `quick_batch-0.1.7/quick_batch/queue_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/__init__.py` & `quick_batch-0.1.7/quick_batch/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/manage_containers.py` & `quick_batch-0.1.7/quick_batch/utilities/manage_containers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/manage_dockerfile.py` & `quick_batch-0.1.7/quick_batch/utilities/manage_dockerfile.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/manage_images.py` & `quick_batch-0.1.7/quick_batch/utilities/manage_images.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/manage_loggers.py` & `quick_batch-0.1.7/quick_batch/utilities/manage_loggers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/manage_networks.py` & `quick_batch-0.1.7/quick_batch/utilities/manage_networks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/manage_queue.py` & `quick_batch-0.1.7/quick_batch/utilities/manage_queue.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/manage_requirements.py` & `quick_batch-0.1.7/quick_batch/utilities/manage_requirements.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/manage_services.py` & `quick_batch-0.1.7/quick_batch/utilities/manage_services.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/quick_batch/utilities/manage_setup.py` & `quick_batch-0.1.7/quick_batch/utilities/manage_setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from utilities.manage_services import remove_all_services
 from utilities.manage_swarm import leave_swarm
 from utilities.manage_swarm import create_swarm
 from utilities.manage_networks import create_network
 from utilities.manage_services import create_queue_service
 from utilities.manage_services import create_processor_service
 from utilities.manage_queue import monitor_queue_app_containers
+from utilities.manage_images import pull_and_tag_image
 
 
 @log_exceptions
 def setup_client(config):
     # setup logger
     logger = setup_logger(config)
 
@@ -36,19 +37,19 @@
     # check dockerfile - seems to save a copy local to the project - not using for now
     # check_dockerfile(dockerfile_path)
 
     # create docker client
     client = create_client()
 
     # # try to pull and tag image
-    # pull_success = pull_and_tag_image(client, 'jermwatt/quick_batch_queue_app', 'quick_batch_queue_app')
+    # pull_success = pull_and_tag_image(client, 'jermwatt/quick_batch_queue_app',
+    #                                   'quick_batch_queue_app')
 
-    # # if not successful, build image
+    # if not successful, build image
     # if not pull_success:
-
     manage_images.build_queue_image(client)
 
     # # try to pull and tag image
     # pull_success = pull_and_tag_image(client, image_name, 'quick_batch_processor_app')
 
     # # if not successful, build image
     # if not pull_success:
```

### Comparing `quick_batch-0.1.6/quick_batch/utilities/param_checks.py` & `quick_batch-0.1.7/quick_batch/utilities/param_checks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.6/PKG-INFO` & `quick_batch-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-batch
-Version: 0.1.6
+Version: 0.1.7
 Summary: ultra simple command line tool for docker-scaling batch processing
 Home-page: https://github.com/jermwatt/quick_batch
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,15 @@
 
 `quick_batch` is an ultra-simple command-line tool for large batch python-driven processing and transformation.  It was designed to be fast to deploy, transparent, and portable.  This allows you to scale any `processor` function that needs to be run over a large set of input data, enabling batch/parallel processing of the input with minimal setup and teardown.
 
 
 - [quick\_batch](#quick_batch)
 - [Getting started](#getting-started)
   - [Usage](#usage)
+  - [Scaling](#scaling)
   - [Installation](#installation)
   - [The `processor.py` file](#the-processorpy-file)
 - [Why use quick\_batch](#why-use-quick_batch)
 
 # Getting started
 
 All you need to scale batch transformations with `quick_batch` is a
@@ -67,20 +68,32 @@
 Output will be written to the `output_path` specified in the configuration file.
 
 You can see `tests/config_files` for examples of valid configs.
 
 
 ## Usage
 
-With your `config.yaml` defined you can use `quick_batch` at the terminal by typing
+To start processing with your `config.yaml` use `quick_batch`'s `config` command at the terminal by typing
 
 ```bash
-quick_batch /path/to/your/config.yaml
+quick_batch config /path/to/your/config.yaml
 ```
 
+This will start the build and deploy process for processing your data as defined in your `config.yaml`.
+
+## Scaling
+
+Use the `scale` commoand to manually scale the number of processors / containers running your process
+
+```bash
+quick_batch scale <num_processors> 
+```
+
+Here `<num_processors>` is an integer >= 1.   For example, to scale to 3 parallel processors / containers: `quick_batch scale 3`
+
 ## Installation
 
 To install quick_batch, simply use `pip`:
 
 ```bash
 pip install quick-batch
 ```
```

