# Comparing `tmp/vdk-dag-0.1.872432630.tar.gz` & `tmp/vdk-dag-0.1.884801326.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-dag-0.1.872432630.tar", last modified: Fri May 19 09:16:37 2023, max compression
+gzip compressed data, was "vdk-dag-0.1.884801326.tar", last modified: Wed May 31 14:08:17 2023, max compression
```

## Comparing `vdk-dag-0.1.872432630.tar` & `vdk-dag-0.1.884801326.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/
--rw-r--r--   0 root         (0) root         (0)     8454 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7887 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-19 09:16:26.000000 vdk-dag-0.1.872432630/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/vdk/plugin/dag/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/vdk/plugin/dag/api/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/api/dag.py
--rw-rw-rw-   0 root         (0) root         (0)    10184 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     7481 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6480 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_plugin_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     7838 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2353 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dags.py
--rw-rw-rw-   0 root         (0) root         (0)     9385 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8454 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/tests/
--rw-rw-rw-   0 root         (0) root         (0)    19438 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/tests/test_dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/tests/test_dag_object.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:08:17.266251 vdk-dag-0.1.884801326/
+-rw-r--r--   0 root         (0) root         (0)     8466 2023-05-31 14:08:17.266251 vdk-dag-0.1.884801326/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7899 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 14:08:17.266251 vdk-dag-0.1.884801326/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-31 14:08:05.000000 vdk-dag-0.1.884801326/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:08:17.262251 vdk-dag-0.1.884801326/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:08:17.262251 vdk-dag-0.1.884801326/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:08:17.262251 vdk-dag-0.1.884801326/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:08:17.266251 vdk-dag-0.1.884801326/src/vdk/plugin/dag/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:08:17.266251 vdk-dag-0.1.884801326/src/vdk/plugin/dag/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/api/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)    10184 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7481 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6480 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag_plugin_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     7838 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2353 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/dags.py
+-rw-rw-rw-   0 root         (0) root         (0)     9385 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/src/vdk/plugin/dag/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:08:17.266251 vdk-dag-0.1.884801326/src/vdk_dag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8466 2023-05-31 14:08:17.000000 vdk-dag-0.1.884801326/src/vdk_dag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-31 14:08:17.000000 vdk-dag-0.1.884801326/src/vdk_dag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 14:08:17.000000 vdk-dag-0.1.884801326/src/vdk_dag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-31 14:08:17.000000 vdk-dag-0.1.884801326/src/vdk_dag.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-31 14:08:17.000000 vdk-dag-0.1.884801326/src/vdk_dag.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-31 14:08:17.000000 vdk-dag-0.1.884801326/src/vdk_dag.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:08:17.266251 vdk-dag-0.1.884801326/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    19438 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/tests/test_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/tests/test_dag_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-31 14:08:00.000000 vdk-dag-0.1.884801326/tests/test_tracking_job_executor.py
```

### Comparing `vdk-dag-0.1.872432630/PKG-INFO` & `vdk-dag-0.1.884801326/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-dag
-Version: 0.1.872432630
+Version: 0.1.884801326
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -61,15 +61,15 @@
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
 
 
-![img_2.png](img_2.png)
+![example_dag.png](example_dag.png)
 
 In this example what happens is:
 * Job 1 will execute.
 * After Job 1 is completed, jobs 2,3,4 will start executing in parallel.
 * Jobs 5 and 6 will start executing after job 3 completes, but will not wait for the completion of jobs 2 and 4.
```

### Comparing `vdk-dag-0.1.872432630/README.md` & `vdk-dag-0.1.884801326/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
 
 
-![img_2.png](img_2.png)
+![example_dag.png](example_dag.png)
 
 In this example what happens is:
 * Job 1 will execute.
 * After Job 1 is completed, jobs 2,3,4 will start executing in parallel.
 * Jobs 5 and 6 will start executing after job 3 completes, but will not wait for the completion of jobs 2 and 4.
```

### Comparing `vdk-dag-0.1.872432630/setup.py` & `vdk-dag-0.1.884801326/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.872432630"
+__version__ = "0.1.884801326"
 
 setuptools.setup(
     name="vdk-dag",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/api/dag.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/api/dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/cached_data_job_executor.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/cached_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_plugin.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_plugin_configuration.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_runner.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag_runner.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_validator.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/dag_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dags.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/dags.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/remote_data_job.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/remote_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/remote_data_job_executor.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/remote_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk/plugin/dag/time_based_queue.py` & `vdk-dag-0.1.884801326/src/vdk/plugin/dag/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/src/vdk_dag.egg-info/PKG-INFO` & `vdk-dag-0.1.884801326/src/vdk_dag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-dag
-Version: 0.1.872432630
+Version: 0.1.884801326
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -61,15 +61,15 @@
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
 
 
-![img_2.png](img_2.png)
+![example_dag.png](example_dag.png)
 
 In this example what happens is:
 * Job 1 will execute.
 * After Job 1 is completed, jobs 2,3,4 will start executing in parallel.
 * Jobs 5 and 6 will start executing after job 3 completes, but will not wait for the completion of jobs 2 and 4.
```

### Comparing `vdk-dag-0.1.872432630/src/vdk_dag.egg-info/SOURCES.txt` & `vdk-dag-0.1.884801326/src/vdk_dag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/tests/test_dag.py` & `vdk-dag-0.1.884801326/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/tests/test_dag_object.py` & `vdk-dag-0.1.884801326/tests/test_dag_object.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/tests/test_time_based_queue.py` & `vdk-dag-0.1.884801326/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.872432630/tests/test_tracking_job_executor.py` & `vdk-dag-0.1.884801326/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

