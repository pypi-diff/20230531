# Comparing `tmp/bacalhau_airflow-1.0.1.tar.gz` & `tmp/bacalhau_airflow-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacalhau_airflow-1.0.1.tar", last modified: Wed May 31 18:47:39 2023, max compression
+gzip compressed data, was "bacalhau_airflow-1.0.2.tar", last modified: Wed May 31 20:18:21 2023, max compression
```

## Comparing `bacalhau_airflow-1.0.1.tar` & `bacalhau_airflow-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 18:47:39.620402 bacalhau_airflow-1.0.1/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10247 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/LICENSE
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      242 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7815 2023-05-31 18:47:39.620402 bacalhau_airflow-1.0.1/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7092 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 18:47:39.620402 bacalhau_airflow-1.0.1/bacalhau_airflow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      137 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/bacalhau_airflow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2246 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/bacalhau_airflow/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6574 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/bacalhau_airflow/operators.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 18:47:39.620402 bacalhau_airflow-1.0.1/bacalhau_airflow.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7815 2023-05-31 18:47:39.000000 bacalhau_airflow-1.0.1/bacalhau_airflow.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-05-31 18:47:39.000000 bacalhau_airflow-1.0.1/bacalhau_airflow.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-31 18:47:39.000000 bacalhau_airflow-1.0.1/bacalhau_airflow.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-31 18:47:39.000000 bacalhau_airflow-1.0.1/bacalhau_airflow.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       35 2023-05-31 18:47:39.000000 bacalhau_airflow-1.0.1/bacalhau_airflow.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       17 2023-05-31 18:47:39.000000 bacalhau_airflow-1.0.1/bacalhau_airflow.egg-info/top_level.txt
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 18:47:39.620402 bacalhau_airflow-1.0.1/docs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/Makefile
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 18:47:39.620402 bacalhau_airflow-1.0.1/docs/_static/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   658378 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/_static/airflow_01.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   661811 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/_static/airflow_02.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   803839 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/_static/airflow_03.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   682446 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/_static/airflow_04.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      522 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/bacalhau_airflow.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5087 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/conf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/index.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       85 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/modules.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       27 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/docs/readme.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      394 2023-05-31 18:47:39.624402 bacalhau_airflow-1.0.1/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1338 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 18:47:39.620402 bacalhau_airflow-1.0.1/tests/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/tests/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1622 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/tests/test_hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2583 2023-05-31 18:46:24.000000 bacalhau_airflow-1.0.1/tests/test_operators.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 20:18:21.194138 bacalhau_airflow-1.0.2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10247 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/LICENSE
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      242 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7815 2023-05-31 20:18:21.194138 bacalhau_airflow-1.0.2/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7092 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 20:18:21.190138 bacalhau_airflow-1.0.2/bacalhau_airflow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      137 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/bacalhau_airflow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2246 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/bacalhau_airflow/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6574 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/bacalhau_airflow/operators.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 20:18:21.190138 bacalhau_airflow-1.0.2/bacalhau_airflow.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7815 2023-05-31 20:18:21.000000 bacalhau_airflow-1.0.2/bacalhau_airflow.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-05-31 20:18:21.000000 bacalhau_airflow-1.0.2/bacalhau_airflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-31 20:18:21.000000 bacalhau_airflow-1.0.2/bacalhau_airflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-31 20:18:21.000000 bacalhau_airflow-1.0.2/bacalhau_airflow.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       35 2023-05-31 20:18:21.000000 bacalhau_airflow-1.0.2/bacalhau_airflow.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       17 2023-05-31 20:18:21.000000 bacalhau_airflow-1.0.2/bacalhau_airflow.egg-info/top_level.txt
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 20:18:21.190138 bacalhau_airflow-1.0.2/docs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/Makefile
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 20:18:21.190138 bacalhau_airflow-1.0.2/docs/_static/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   658378 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/_static/airflow_01.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   661811 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/_static/airflow_02.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   803839 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/_static/airflow_03.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   682446 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/_static/airflow_04.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      522 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/bacalhau_airflow.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5087 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/conf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/index.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       85 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/modules.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       27 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/docs/readme.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      394 2023-05-31 20:18:21.194138 bacalhau_airflow-1.0.2/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1338 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 20:18:21.194138 bacalhau_airflow-1.0.2/tests/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/tests/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1622 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/tests/test_hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2583 2023-05-31 20:17:08.000000 bacalhau_airflow-1.0.2/tests/test_operators.py
```

### Comparing `bacalhau_airflow-1.0.1/LICENSE` & `bacalhau_airflow-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/PKG-INFO` & `bacalhau_airflow-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau_airflow
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Apache Airflow provider for Bacalhau.
 Home-page: https://github.com/filecoin-project/bacalhau/tree/main/integration/airflow
 Author: Enrico Rotundo
 Author-email: team@bacalhau.org
 License: Apache Software License 2.0
 Keywords: bacalhau,airflow,provider
 Platform: UNKNOWN
```

### Comparing `bacalhau_airflow-1.0.1/README.md` & `bacalhau_airflow-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/bacalhau_airflow/hooks.py` & `bacalhau_airflow-1.0.2/bacalhau_airflow/hooks.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/bacalhau_airflow/operators.py` & `bacalhau_airflow-1.0.2/bacalhau_airflow/operators.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/bacalhau_airflow.egg-info/PKG-INFO` & `bacalhau_airflow-1.0.2/bacalhau_airflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau-airflow
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Apache Airflow provider for Bacalhau.
 Home-page: https://github.com/filecoin-project/bacalhau/tree/main/integration/airflow
 Author: Enrico Rotundo
 Author-email: team@bacalhau.org
 License: Apache Software License 2.0
 Keywords: bacalhau,airflow,provider
 Platform: UNKNOWN
```

### Comparing `bacalhau_airflow-1.0.1/bacalhau_airflow.egg-info/SOURCES.txt` & `bacalhau_airflow-1.0.2/bacalhau_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/docs/Makefile` & `bacalhau_airflow-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/docs/_static/airflow_01.png` & `bacalhau_airflow-1.0.2/docs/_static/airflow_01.png`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/docs/_static/airflow_02.png` & `bacalhau_airflow-1.0.2/docs/_static/airflow_02.png`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/docs/_static/airflow_03.png` & `bacalhau_airflow-1.0.2/docs/_static/airflow_03.png`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/docs/_static/airflow_04.png` & `bacalhau_airflow-1.0.2/docs/_static/airflow_04.png`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/docs/bacalhau_airflow.rst` & `bacalhau_airflow-1.0.2/docs/bacalhau_airflow.rst`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/docs/conf.py` & `bacalhau_airflow-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/docs/index.rst` & `bacalhau_airflow-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/setup.py` & `bacalhau_airflow-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/tests/test_hooks.py` & `bacalhau_airflow-1.0.2/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-1.0.1/tests/test_operators.py` & `bacalhau_airflow-1.0.2/tests/test_operators.py`

 * *Files identical despite different names*

