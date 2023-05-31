# Comparing `tmp/mlflow-watsonml-0.6.3.tar.gz` & `tmp/mlflow-watsonml-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-watsonml-0.6.3.tar", last modified: Fri May 12 13:50:30 2023, max compression
+gzip compressed data, was "mlflow-watsonml-0.7.3.tar", last modified: Wed May 31 16:40:19 2023, max compression
```

## Comparing `mlflow-watsonml-0.6.3.tar` & `mlflow-watsonml-0.7.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:50:30.392009 mlflow-watsonml-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-12 13:50:30.392009 mlflow-watsonml-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:50:30.388009 mlflow-watsonml-0.6.3/mlflow_watsonml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/wml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:50:30.388009 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:50:30.392009 mlflow-watsonml-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:40:19.935496 mlflow-watsonml-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-31 16:40:19.935496 mlflow-watsonml-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-31 16:40:06.000000 mlflow-watsonml-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:40:19.935496 mlflow-watsonml-0.7.3/mlflow_watsonml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 16:40:06.000000 mlflow-watsonml-0.7.3/mlflow_watsonml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-31 16:40:06.000000 mlflow-watsonml-0.7.3/mlflow_watsonml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-05-31 16:40:06.000000 mlflow-watsonml-0.7.3/mlflow_watsonml/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-31 16:40:06.000000 mlflow-watsonml-0.7.3/mlflow_watsonml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-31 16:40:06.000000 mlflow-watsonml-0.7.3/mlflow_watsonml/wml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:40:19.935496 mlflow-watsonml-0.7.3/mlflow_watsonml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-31 16:40:19.000000 mlflow-watsonml-0.7.3/mlflow_watsonml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-31 16:40:19.000000 mlflow-watsonml-0.7.3/mlflow_watsonml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:40:19.000000 mlflow-watsonml-0.7.3/mlflow_watsonml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 16:40:19.000000 mlflow-watsonml-0.7.3/mlflow_watsonml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 16:40:19.000000 mlflow-watsonml-0.7.3/mlflow_watsonml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 16:40:19.000000 mlflow-watsonml-0.7.3/mlflow_watsonml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 16:40:19.935496 mlflow-watsonml-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-31 16:40:06.000000 mlflow-watsonml-0.7.3/setup.py
```

### Comparing `mlflow-watsonml-0.6.3/PKG-INFO` & `mlflow-watsonml-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.6.3
+Version: 0.7.3
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Mlflow-WatsonML
 
 A plugin that integrates [WatsonML](http://ibm-wml-api-pyclient.mybluemix.net) with MLflow pipeline.
 ``mlflow_watsonml`` enables mlflow users to deploy mlflow pipeline models into WatsonML.
```

### Comparing `mlflow-watsonml-0.6.3/README.md` & `mlflow-watsonml-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.3/mlflow_watsonml/config.py` & `mlflow-watsonml-0.7.3/mlflow_watsonml/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.3/mlflow_watsonml/deploy.py` & `mlflow-watsonml-0.7.3/mlflow_watsonml/deploy.py`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.3/mlflow_watsonml/utils.py` & `mlflow-watsonml-0.7.3/mlflow_watsonml/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.3/mlflow_watsonml/wml.py` & `mlflow-watsonml-0.7.3/mlflow_watsonml/wml.py`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/PKG-INFO` & `mlflow-watsonml-0.7.3/mlflow_watsonml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.6.3
+Version: 0.7.3
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Mlflow-WatsonML
 
 A plugin that integrates [WatsonML](http://ibm-wml-api-pyclient.mybluemix.net) with MLflow pipeline.
 ``mlflow_watsonml`` enables mlflow users to deploy mlflow pipeline models into WatsonML.
```

### Comparing `mlflow-watsonml-0.6.3/setup.py` & `mlflow-watsonml-0.7.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,9 +18,9 @@
     url="https://github.com/IBM/mlflow-watsonml",
     packages=["mlflow_watsonml"],
     author="IBM AI Model Factory team",
     author_email="dhruv.shah@ibm.com",
     install_requires=install_requires,
     extras_require={"dev": ["ipython", "black", "pytest", "build", "wheel", "twine"]},
     entry_points={"mlflow.deployments": "watsonml=mlflow_watsonml.deploy"},
-    python_requires=">=3.9",
+    python_requires=">=3.8",
 )
```

