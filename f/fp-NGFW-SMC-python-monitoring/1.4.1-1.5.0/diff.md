# Comparing `tmp/fp-NGFW-SMC-python-monitoring-1.4.1.tar.gz` & `tmp/fp-NGFW-SMC-python-monitoring-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fp-NGFW-SMC-python-monitoring-1.4.1.tar", last modified: Fri May 26 09:34:53 2023, max compression
+gzip compressed data, was "fp-NGFW-SMC-python-monitoring-1.5.0.tar", last modified: Wed May 31 08:32:27 2023, max compression
```

## Comparing `fp-NGFW-SMC-python-monitoring-1.4.1.tar` & `fp-NGFW-SMC-python-monitoring-1.5.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       40 2023-05-25 13:16:11.000000 fp-NGFW-SMC-python-monitoring-1.4.1/MANIFEST.in
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9361 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/PKG-INFO
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7334 2022-10-19 07:17:48.000000 fp-NGFW-SMC-python-monitoring-1.4.1/README.rst
-drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.523753 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9361 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/PKG-INFO
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     1238 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)        1 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/dependency_links.txt
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)        1 2023-05-26 09:31:55.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/not-zip-safe
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       51 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/requires.txt
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       21 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/top_level.txt
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       67 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/setup.cfg
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     2065 2023-05-25 13:34:06.000000 fp-NGFW-SMC-python-monitoring-1.4.1/setup.py
-drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.523753 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      678 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/__init__.py
-drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      756 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/__init__.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6416 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/calendar.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    23470 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/constants.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    11993 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/filters.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7444 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/formats.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     8355 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/formatters.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    14473 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/query.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6974 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/values.py
-drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      814 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/__init__.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6055 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/alerts.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9936 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/blacklist.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9653 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/block_list.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6303 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/connections.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     8723 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/logs.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5976 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/neighbors.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5938 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/routes.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     4899 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/sslvpn.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5306 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/users.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7588 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/vpns.py
-drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/pubsub/
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      554 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/pubsub/__init__.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5355 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/pubsub/subscribers.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    10017 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/wsocket.py
-drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/tests/
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      554 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/tests/__init__.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9625 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/tests/docker_smc_bootstrap.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    16709 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/tests/test_filters.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7079 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/tests/test_queries.py
--rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       18 2023-05-26 09:31:29.000000 fp-NGFW-SMC-python-monitoring-1.4.1/version.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-31 08:32:27.047122 fp-NGFW-SMC-python-monitoring-1.5.0/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     1064 2023-02-07 09:01:38.000000 fp-NGFW-SMC-python-monitoring-1.5.0/HISTORY.rst
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       42 2023-02-07 09:01:38.000000 fp-NGFW-SMC-python-monitoring-1.5.0/MANIFEST.in
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     8976 2023-05-31 08:32:27.047122 fp-NGFW-SMC-python-monitoring-1.5.0/PKG-INFO
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7334 2023-02-07 09:01:38.000000 fp-NGFW-SMC-python-monitoring-1.5.0/README.rst
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-31 08:32:27.043122 fp-NGFW-SMC-python-monitoring-1.5.0/fp_NGFW_SMC_python_monitoring.egg-info/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     8976 2023-05-31 08:32:26.000000 fp-NGFW-SMC-python-monitoring-1.5.0/fp_NGFW_SMC_python_monitoring.egg-info/PKG-INFO
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     1250 2023-05-31 08:32:27.000000 fp-NGFW-SMC-python-monitoring-1.5.0/fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)        1 2023-05-31 08:32:26.000000 fp-NGFW-SMC-python-monitoring-1.5.0/fp_NGFW_SMC_python_monitoring.egg-info/dependency_links.txt
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)        1 2023-05-31 08:32:21.000000 fp-NGFW-SMC-python-monitoring-1.5.0/fp_NGFW_SMC_python_monitoring.egg-info/not-zip-safe
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       51 2023-05-31 08:32:26.000000 fp-NGFW-SMC-python-monitoring-1.5.0/fp_NGFW_SMC_python_monitoring.egg-info/requires.txt
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       21 2023-05-31 08:32:26.000000 fp-NGFW-SMC-python-monitoring-1.5.0/fp_NGFW_SMC_python_monitoring.egg-info/top_level.txt
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       67 2023-05-31 08:32:27.047122 fp-NGFW-SMC-python-monitoring-1.5.0/setup.cfg
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     2016 2023-05-31 08:19:15.000000 fp-NGFW-SMC-python-monitoring-1.5.0/setup.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-31 08:32:27.043122 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      678 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/__init__.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-31 08:32:27.047122 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      756 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/__init__.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6416 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/calendar.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    23470 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/constants.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    11993 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/filters.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7444 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/formats.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     8458 2023-05-31 08:19:15.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/formatters.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    14625 2023-05-31 08:19:15.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/query.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6974 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/values.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-31 08:32:27.047122 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      814 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/__init__.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6055 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/alerts.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9936 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/blacklist.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9653 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/block_list.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6303 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/connections.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     8853 2023-05-31 08:19:15.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/logs.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5976 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/neighbors.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6014 2023-05-31 08:19:15.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/routes.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     4899 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/sslvpn.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5306 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/users.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7588 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/vpns.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-31 08:32:27.047122 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/pubsub/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      554 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/pubsub/__init__.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5355 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/pubsub/subscribers.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    15735 2023-05-31 08:19:15.000000 fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/wsocket.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-31 08:32:27.047122 fp-NGFW-SMC-python-monitoring-1.5.0/tests/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      554 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/tests/__init__.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9625 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/tests/docker_smc_bootstrap.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    16709 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/tests/test_filters.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7079 2023-02-07 16:22:32.000000 fp-NGFW-SMC-python-monitoring-1.5.0/tests/test_queries.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       18 2023-05-31 08:19:15.000000 fp-NGFW-SMC-python-monitoring-1.5.0/version.py
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/PKG-INFO` & `fp-NGFW-SMC-python-monitoring-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: fp-NGFW-SMC-python-monitoring
-Version: 1.4.1
+Version: 1.5.0
 Summary: Forcepoint NGFW Management Center Monitoring
 Home-page: https://github.com/Forcepoint/fp-NGFW-SMC-python
 Author: Forcepoint
 Author-email: PSIRT@forcepoint.com
 License: Apache License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 
 |PyPI version|
 
@@ -289,17 +288,8 @@
 - Fixed fetch_batch to only return a single payload, previous versions were unlimited
 
 1.4.0
 +++++
 
 - Update requirements to fp_NGFW_SMC_python >= 1.0.0
 
-1.4.1
-+++++
 
--fixed blacklist entry issue
--added first_fetch support
--added support to NumberValue and TranslatedValue in QueryFilter
--blacklist -> block_list renaming
--support "use ssl for session id" (Fix session lost issue)
--Adding asynchronious callback support (@see SMCSocketAsyncProtocol)
--support certificate options in wsocket
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/README.rst` & `fp-NGFW-SMC-python-monitoring-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/PKG-INFO` & `fp-NGFW-SMC-python-monitoring-1.5.0/fp_NGFW_SMC_python_monitoring.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: fp-NGFW-SMC-python-monitoring
-Version: 1.4.1
+Version: 1.5.0
 Summary: Forcepoint NGFW Management Center Monitoring
 Home-page: https://github.com/Forcepoint/fp-NGFW-SMC-python
 Author: Forcepoint
 Author-email: PSIRT@forcepoint.com
 License: Apache License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 
 |PyPI version|
 
@@ -289,17 +288,8 @@
 - Fixed fetch_batch to only return a single payload, previous versions were unlimited
 
 1.4.0
 +++++
 
 - Update requirements to fp_NGFW_SMC_python >= 1.0.0
 
-1.4.1
-+++++
 
--fixed blacklist entry issue
--added first_fetch support
--added support to NumberValue and TranslatedValue in QueryFilter
--blacklist -> block_list renaming
--support "use ssl for session id" (Fix session lost issue)
--Adding asynchronious callback support (@see SMCSocketAsyncProtocol)
--support certificate options in wsocket
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt` & `fp-NGFW-SMC-python-monitoring-1.5.0/fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+HISTORY.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 version.py
 fp_NGFW_SMC_python_monitoring.egg-info/PKG-INFO
 fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/setup.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,15 @@
     url="https://github.com/Forcepoint/fp-NGFW-SMC-python",
     # packages=['smc_monitoring'],
     packages=find_packages(),
     # namespace_packages=['smc_monitoring'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
     ],
     zip_safe=False,
-    install_requires=["fp_NGFW_SMC_python >=1.0.0", "websocket-client >=0.48.0"],
+    install_requires=["fp_NGFW_SMC_python >=1.0.19", "websocket-client >=1.5.0"],
 )
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/__init__.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/__init__.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/calendar.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/calendar.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/constants.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/constants.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/filters.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/filters.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/formats.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/formats.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/formatters.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,7 +218,13 @@
     """
 
     def __init__(self, query):
         pass
 
     def formatted(self, alist):
         return alist
+
+
+class ElementFormat(RawDictFormat):
+    """
+    Return the data as a list in Element format.
+    """
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/query.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,14 +282,18 @@
         :return: raw dict returned from query
         :rtype: dict(list)
         """
         with SMCSocketProtocol(self, **self.sockopt) as protocol:
             for result in protocol.receive():
                 yield result
 
+    def get_record(self, results):
+        if "records" in results and results["records"].get("added"):
+            return results["records"]["added"]
+
     def fetch_raw(self, **kw):
         """
         Fetch the records for this query. This fetch type will return the
         results in raw dict format. It is possible to limit the number of
         receives on the socket that return results before exiting by providing
         max_recv.
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/values.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/models/values.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/__init__.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/__init__.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/alerts.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/alerts.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/blacklist.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/blacklist.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/block_list.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/block_list.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/connections.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/connections.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/logs.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,18 @@
 
         :return: configured fetch size for this query
         :rtype: int
         """
         if "quantity" in self.request["fetch"]:
             return self.request["fetch"]["quantity"]
 
+    def get_record(self, results):
+        if "records" in results and results["records"]:
+            return results["records"]
+
     def fetch_raw(self):
         """
         Execute the query and return by batches.
         Optional keyword arguments are passed to Query.execute(). Whether
         this is real-time or stored logs is dependent on the value of
         ``fetch_type``.
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/neighbors.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/neighbors.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/routes.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,12 +203,16 @@
 
         :return: route metric
         :rtype: int
         """
         return int(self.rt.get(str(LogField.ROUTEMETRIC)), 0)
 
     def __str__(self):
-        return "{}(dest_if={},network={},type={})".format(
-            self.__class__.__name__, self.dest_if, self.route_network, self.route_type)
+        return "{}(dest_if={}, gateway={}, network={},type={})".format(
+            self.__class__.__name__,
+            self.dest_if,
+            self.route_gw,
+            self.route_network,
+            self.route_type)
 
     def __repr__(self):
         return str(self)
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/sslvpn.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/sslvpn.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/users.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/users.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/vpns.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/monitors/vpns.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/pubsub/__init__.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/pubsub/__init__.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/pubsub/subscribers.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/pubsub/subscribers.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/wsocket.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/smc_monitoring/wsocket.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 import select
 import logging
 import threading
 import time
 from pprint import pformat
 from smc import session
 from smc.compat import PYTHON_v3_9
+from smc_monitoring.models.formatters import TableFormat, ElementFormat
 
 import websocket
-
+from websocket import WebSocketApp
 
 logger = logging.getLogger(__name__)
 
 
 def websocket_debug():
     websocket.enableTrace(True)
 
@@ -53,14 +54,190 @@
         import certifi
 
         return certifi.where()
     except ImportError:
         pass
 
 
+def get_ssl_opt(**kw):
+    sslopt = {}
+    if session.is_ssl:
+        # SSL verification is based on the session settings since the
+        # session must be made before calling this class. If verify=True,
+        # try to get the CA bundle from certifi if the package exists
+        # Set check_hostname to False because python ssl doesn't appear
+        # to validate the subjectAltName properly, however requests does
+        # and would have already validated this when the session was set
+        # up. This can still be overridden by setting check_hostname=True.
+        sslopt.update(cert_reqs=ssl.CERT_NONE, check_hostname=False)
+
+        certfile = session.session.verify
+        if certfile:
+            if isinstance(certfile, bool):  # verify=True
+                certfile = _get_ca_bundle()
+                if certfile is None:
+                    certfile = ""
+
+            sslopt.update(
+                cert_reqs=kw.pop("cert_reqs", ssl.CERT_REQUIRED),
+                check_hostname=kw.pop("check_hostname", False),
+            )
+
+            if sslopt.get("cert_reqs") != ssl.CERT_NONE:
+                os.environ["WEBSOCKET_CLIENT_CA_BUNDLE"] = certfile
+
+    return sslopt
+
+
+def get_sock_from_session():
+    sock = None
+    if session.session_id is None:
+        sock = session.sock
+        if sock is None:
+            # Need to refresh the session
+            session.refresh()
+            sock = session.sock
+            logger.debug("WS: socket from new session:{} id:{}".format(sock,
+                                                                       sock.session.id))
+        else:
+            logger.debug("WS: session still available socket:{} id:{}".format(sock,
+                                                                              sock.session.id))
+    return sock
+
+
+class SMCSocketAsyncProtocol:
+    """
+    SMCSocketAsyncProtocol manages the web socket connection between this
+    client and the SMC. It provides the interface to monitor the query
+    results and call the callback_method provided on the fly when there is new data.
+    It is possible to provide formatter like TableFormat, ElementFormat and the element name you
+    want to retrieve
+
+    Example of subscribing to log notifications using callback method::
+
+        >>>     def callback_log_table_fct(wso, data):
+        ...         print(data)
+
+        >>>     query = LogQuery()
+        >>>     query.add_or_filter([
+        ...               InFilter(FieldValue(LogField.DPORT), [NumberValue(80)]),
+        ...               InFilter(FieldValue(LogField.SERVICE), [ServiceValue('TCP/80')])])
+
+        >>>    async_ws = SMCSocketAsyncProtocol(query=query,
+        ...                              on_message_fct=callback_log_table_fct,
+        ...                              formatter=TableFormat)
+        >>>     async_ws.run(background=True)
+
+
+    """
+
+    def __init__(self, query, on_message_fct, formatter=TableFormat, element_name=None, **kw):
+        """
+        Initialize the web socket.
+
+        :param Query query: Query type from `smc_monitoring.monitors`
+        :param formatter: Custom formats used to return data in different formats.
+        :param element_name: if formatter is ElementFormat give the name of the element to retrieve
+            e.g. Neighbor, RoutingView, Alert..
+        """
+
+        self.query = query
+        self.on_message_fct = on_message_fct
+        self.formatter = formatter
+        self.element_name = element_name
+        self.thread = None
+        self.fetch_id = None
+
+        if formatter is ElementFormat:
+            query.format.field_format("id")
+            for custom_field in ["field_ids", "field_names"]:
+                query.format.data.pop(custom_field, None)
+
+        if not session.session:
+            raise SessionNotFound(
+                "No SMC session found. You must first "
+                "obtain an SMC session through session.login before making "
+                "a web socket connection."
+            )
+
+        # Case use ssl for session_id
+        self.sock = get_sock_from_session()
+
+        self.sslopt = get_ssl_opt(**kw)
+
+        self.ws = WebSocketApp(session.web_socket_url + query.location,
+                               on_open=self._on_open_ws,
+                               on_message=self._on_message_ws,
+                               on_close=self._on_close,
+                               on_error=self._on_error,
+                               cookie=session.session_id,
+                               socket=self.sock)
+
+    def run(self, background=False):
+        """
+        Start listening from the websocket on the callback method
+        """
+        if background:
+            logger.debug("WS run in new thread...")
+            self.thread = threading.Thread(target=self.ws.run_forever,
+                                           kwargs={"sslopt": self.sslopt})
+            self.thread.start()
+        else:
+            logger.debug("WS run in main thread...")
+            self.ws.run_forever(sslopt=self.sslopt)
+
+    def _on_open_ws(self, ws):
+        logger.debug("WS:{} open".format(ws))
+        ws.send(json.dumps(self.query.request))
+
+    def _on_message_ws(self, ws, message):
+        data = json.loads(message)
+        self.fetch_id = data.get("fetch")
+        records = self.query.get_record(results=data)
+        if records:
+            if self.formatter is ElementFormat:
+                for message in records:
+                    self.on_message_fct(ws, self.element_name(**message))
+            else:
+                fmt = self.formatter(self.query)
+                self.on_message_fct(ws, fmt.formatted(records))
+
+    def _on_error(self, ws, err):
+        ws.close()
+        logger.error("WS:{} error: {}".format(ws, err))
+
+    def _on_close(self, ws, close_status_code, close_msg):
+        logger.debug("WS:{} closed status={} message={} ! ".format(ws,
+                                                                   close_status_code,
+                                                                   close_msg))
+
+    def abort(self):
+        """
+        Abort
+        End listening for new messages and let server close the websocket
+        :return: True ws connection aborted
+        """
+        if self.fetch_id is None:
+            logger.warning("WS fetch_id is None: can't abort !")
+            return False
+        if session.session_id is None and self.sock is None:
+            self.sock = get_sock_from_session()
+
+        self.ws.send("{{'abort': {}}}".format(self.fetch_id))
+        logger.debug("WS connection aborted !")
+        return True
+
+    def close(self):
+        """
+        Close the websocket
+        """
+        logger.info("Close WS:{}".format(self))
+        self.ws.close()
+
+
 class SMCSocketProtocol(websocket.WebSocket):
     """
     SMCSocketProtocol manages the web socket connection between this
     client and the SMC. It provides the interface to monitor the query
     results and yield them back to the caller as a context manager.
     """
 
@@ -90,39 +267,15 @@
         if not session.session:
             raise SessionNotFound(
                 "No SMC session found. You must first "
                 "obtain an SMC session through session.login before making "
                 "a web socket connection."
             )
 
-        sslopt = {}
-        if session.is_ssl:
-            # SSL verification is based on the session settings since the
-            # session must be made before calling this class. If verify=True,
-            # try to get the CA bundle from certifi if the package exists
-            # Set check_hostname to False because python ssl doesn't appear
-            # to validate the subjectAltName properly, however requests does
-            # and would have already validated this when the session was set
-            # up. This can still be overridden by setting check_hostname=True.
-            sslopt.update(cert_reqs=ssl.CERT_NONE, check_hostname=False)
-
-            certfile = session.session.verify
-            if certfile:
-                if isinstance(certfile, bool):  # verify=True
-                    certfile = _get_ca_bundle()
-                    if certfile is None:
-                        certfile = ""
-
-                sslopt.update(
-                    cert_reqs=kw.pop("cert_reqs", ssl.CERT_REQUIRED),
-                    check_hostname=kw.pop("check_hostname", False),
-                )
-
-                if sslopt.get("cert_reqs") != ssl.CERT_NONE:
-                    os.environ["WEBSOCKET_CLIENT_CA_BUNDLE"] = certfile
+        sslopt = get_ssl_opt(**kw)
 
         # Enable multithread locking
         if "enable_multithread" not in kw:
             kw.update(enable_multithread=True)
 
         # Max number of receives, configurable for batching
         self.max_recv = kw.pop("max_recv", 0)
@@ -138,14 +291,15 @@
         self.sock_timeout = sock_timeout
 
     def __enter__(self):
         if session.session_id is None:
             sock = session.sock
             if sock is None:
                 # Need to obtain new socket
+                logger.debug("Refresh the login session..")
                 session.refresh()
             self.connect(
                 url=session.web_socket_url + self.query.location,
                 socket=session.sock)
         else:
             self.connect(
                 url=session.web_socket_url + self.query.location,
@@ -274,8 +428,8 @@
 
             if self.thread:
                 self.event.set()
                 while (not PYTHON_v3_9 and self.thread.isAlive()) or \
                       (PYTHON_v3_9 and self.thread.is_alive()):
                     self.event.wait(1)
 
-            logger.info("Closed web socket connection normally.")
+            logger.info("Closed web socket connection normally:{}.".format(self))
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/tests/__init__.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/tests/docker_smc_bootstrap.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/tests/docker_smc_bootstrap.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/tests/test_filters.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.1/tests/test_queries.py` & `fp-NGFW-SMC-python-monitoring-1.5.0/tests/test_queries.py`

 * *Files identical despite different names*

