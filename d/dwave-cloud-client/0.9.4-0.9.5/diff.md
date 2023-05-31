# Comparing `tmp/dwave-cloud-client-0.9.4.tar.gz` & `tmp/dwave-cloud-client-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave-cloud-client-0.9.4.tar", last modified: Wed Apr  6 19:20:17 2022, max compression
+gzip compressed data, was "dwave-cloud-client-0.9.5.tar", last modified: Fri Apr 15 19:16:53 2022, max compression
```

## Comparing `dwave-cloud-client-0.9.4.tar` & `dwave-cloud-client-0.9.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-06 19:20:17.195132 dwave-cloud-client-0.9.4/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11386 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4491 2022-04-06 19:20:17.195132 dwave-cloud-client-0.9.4/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3670 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-06 19:20:17.191132 dwave-cloud-client-0.9.4/dwave/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      648 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-06 19:20:17.195132 dwave-cloud-client-0.9.4/dwave/cloud/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2761 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-06 19:20:17.195132 dwave-cloud-client-0.9.4/dwave/cloud/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1156 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12260 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/api/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1826 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/api/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/api/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3340 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/api/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9992 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/api/resources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33063 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/cli.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-06 19:20:17.195132 dwave-cloud-client-0.9.4/dwave/cloud/client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      767 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/client/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83400 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/client/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2416 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/client/hybrid.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2867 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/client/qpu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2501 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/client/sw.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13806 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/coders.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37994 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/computation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4020 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/concurrency.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34013 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3664 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/events.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2857 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      928 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/package_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    42411 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/solver.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-06 19:20:17.195132 dwave-cloud-client-0.9.4/dwave/cloud/testing/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4366 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/testing/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9478 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/testing/mocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12248 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/upload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22831 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/dwave/cloud/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-06 19:20:17.195132 dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4491 2022-04-06 19:20:17.000000 dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      999 2022-04-06 19:20:17.000000 dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-04-06 19:20:17.000000 dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2022-04-06 19:20:17.000000 dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-04-06 19:20:17.000000 dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      434 2022-04-06 19:20:17.000000 dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-04-06 19:20:17.000000 dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2022-04-06 19:20:17.199132 dwave-cloud-client-0.9.4/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2470 2022-04-06 19:19:49.000000 dwave-cloud-client-0.9.4/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 19:16:53.627171 dwave-cloud-client-0.9.5/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11386 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4491 2022-04-15 19:16:53.627171 dwave-cloud-client-0.9.5/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3670 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 19:16:53.623171 dwave-cloud-client-0.9.5/dwave/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      648 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 19:16:53.627171 dwave-cloud-client-0.9.5/dwave/cloud/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2761 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 19:16:53.627171 dwave-cloud-client-0.9.5/dwave/cloud/api/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1156 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/api/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12260 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/api/client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1826 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/api/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/api/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3340 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/api/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9992 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/api/resources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33066 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/cli.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 19:16:53.627171 dwave-cloud-client-0.9.5/dwave/cloud/client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      767 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/client/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83400 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/client/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2416 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/client/hybrid.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2867 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/client/qpu.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2501 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/client/sw.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13806 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/coders.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37994 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/computation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4020 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/concurrency.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34013 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3664 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/events.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2857 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      928 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/package_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    42411 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/solver.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 19:16:53.627171 dwave-cloud-client-0.9.5/dwave/cloud/testing/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4366 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/testing/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9478 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/testing/mocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12248 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/upload.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22831 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/dwave/cloud/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-04-15 19:16:53.627171 dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4491 2022-04-15 19:16:53.000000 dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      999 2022-04-15 19:16:53.000000 dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-04-15 19:16:53.000000 dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2022-04-15 19:16:53.000000 dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-04-15 19:16:53.000000 dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      434 2022-04-15 19:16:53.000000 dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-04-15 19:16:53.000000 dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2022-04-15 19:16:53.627171 dwave-cloud-client-0.9.5/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2470 2022-04-15 19:16:44.000000 dwave-cloud-client-0.9.5/setup.py
```

### Comparing `dwave-cloud-client-0.9.4/LICENSE` & `dwave-cloud-client-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/PKG-INFO` & `dwave-cloud-client-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-cloud-client
-Version: 0.9.4
+Version: 0.9.5
 Summary: A minimal client for interacting with D-Wave cloud resources.
 Home-page: https://github.com/dwavesystems/dwave-cloud-client
 Author: D-Wave Systems Inc.
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dwave-cloud-client-0.9.4/README.rst` & `dwave-cloud-client-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/__init__.py` & `dwave-cloud-client-0.9.5/dwave/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/__init__.py` & `dwave-cloud-client-0.9.5/dwave/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/api/__init__.py` & `dwave-cloud-client-0.9.5/dwave/cloud/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/api/client.py` & `dwave-cloud-client-0.9.5/dwave/cloud/api/client.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/api/constants.py` & `dwave-cloud-client-0.9.5/dwave/cloud/api/constants.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/api/exceptions.py` & `dwave-cloud-client-0.9.5/dwave/cloud/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/api/models.py` & `dwave-cloud-client-0.9.5/dwave/cloud/api/models.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/api/resources.py` & `dwave-cloud-client-0.9.5/dwave/cloud/api/resources.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/cli.py` & `dwave-cloud-client-0.9.5/dwave/cloud/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
 def _sample(solver, problem, params, output):
     """Blocking sample call with error handling and using custom printer."""
 
     try:
         response = solver.sample_ising(*problem, **params)
         problem_id = response.wait_id()
         output("Submitted problem ID: {problem_id}", problem_id=problem_id)
-        response.wait()
+        response.result()
     except RequestTimeout:
         raise CLIError("API connection timed out.", 8)
     except PollingTimeout:
         raise CLIError("Polling timeout exceeded.", 9)
     except Exception as e:
         raise CLIError("Sampling error: {!r}".format(e), 10)
 
@@ -420,15 +420,15 @@
 
         try:
             fn(*args, output=output, **kwargs)
         except CLIError as error:
             output("Error: {error} (code: {code})", error=str(error), code=error.code)
             sys.exit(error.code)
         except Exception as error:
-            output("Unhandled error: {error}", error=str(error))
+            output("Unhandled error: {error}", error=repr(error))
             sys.exit(127)
         finally:
             flush()
 
     return wrapped
```

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/client/__init__.py` & `dwave-cloud-client-0.9.5/dwave/cloud/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/client/base.py` & `dwave-cloud-client-0.9.5/dwave/cloud/client/base.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/client/hybrid.py` & `dwave-cloud-client-0.9.5/dwave/cloud/client/hybrid.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/client/qpu.py` & `dwave-cloud-client-0.9.5/dwave/cloud/client/qpu.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/client/sw.py` & `dwave-cloud-client-0.9.5/dwave/cloud/client/sw.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/coders.py` & `dwave-cloud-client-0.9.5/dwave/cloud/coders.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/computation.py` & `dwave-cloud-client-0.9.5/dwave/cloud/computation.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/concurrency.py` & `dwave-cloud-client-0.9.5/dwave/cloud/concurrency.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/config.py` & `dwave-cloud-client-0.9.5/dwave/cloud/config.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/events.py` & `dwave-cloud-client-0.9.5/dwave/cloud/events.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/exceptions.py` & `dwave-cloud-client-0.9.5/dwave/cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/package_info.py` & `dwave-cloud-client-0.9.5/dwave/cloud/package_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __packagename__ = 'dwave-cloud-client'
 __title__ = 'D-Wave Cloud Client'
-__version__ = '0.9.4'
+__version__ = '0.9.5'
 __author__ = 'D-Wave Systems Inc.'
 __description__ = 'A minimal client for interacting with D-Wave cloud resources.'
 __url__ = 'https://github.com/dwavesystems/dwave-cloud-client'
 __license__ = 'Apache 2.0'
 __copyright__ = '2017, D-Wave Systems Inc.'
```

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/solver.py` & `dwave-cloud-client-0.9.5/dwave/cloud/solver.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/testing/__init__.py` & `dwave-cloud-client-0.9.5/dwave/cloud/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/testing/mocks.py` & `dwave-cloud-client-0.9.5/dwave/cloud/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/upload.py` & `dwave-cloud-client-0.9.5/dwave/cloud/upload.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave/cloud/utils.py` & `dwave-cloud-client-0.9.5/dwave/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/PKG-INFO` & `dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-cloud-client
-Version: 0.9.4
+Version: 0.9.5
 Summary: A minimal client for interacting with D-Wave cloud resources.
 Home-page: https://github.com/dwavesystems/dwave-cloud-client
 Author: D-Wave Systems Inc.
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dwave-cloud-client-0.9.4/dwave_cloud_client.egg-info/SOURCES.txt` & `dwave-cloud-client-0.9.5/dwave_cloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dwave-cloud-client-0.9.4/setup.py` & `dwave-cloud-client-0.9.5/setup.py`

 * *Files identical despite different names*

