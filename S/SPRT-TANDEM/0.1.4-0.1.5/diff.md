# Comparing `tmp/SPRT-TANDEM-0.1.4.tar.gz` & `tmp/SPRT-TANDEM-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPRT-TANDEM-0.1.4.tar", last modified: Wed May 31 20:34:35 2023, max compression
+gzip compressed data, was "SPRT-TANDEM-0.1.5.tar", last modified: Wed May 31 20:45:26 2023, max compression
```

## Comparing `SPRT-TANDEM-0.1.4.tar` & `SPRT-TANDEM-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/
--rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.4/LICENSE
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/PKG-INFO
--rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 12:20:47.000000 SPRT-TANDEM-0.1.4/README.md
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.621424 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/PKG-INFO
--rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/SOURCES.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/dependency_links.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       30 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/requires.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/top_level.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/setup.cfg
--rw-r--r--   0 afe       (1000) afe       (1000)     1167 2023-05-31 20:34:28.000000 SPRT-TANDEM-0.1.4/setup.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.621424 SPRT-TANDEM-0.1.4/tandem/
--rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 05:14:48.000000 SPRT-TANDEM-0.1.4/tandem/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.621424 SPRT-TANDEM-0.1.4/tandem/config/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.4/tandem/config/__init__.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    11204 2023-05-31 20:04:18.000000 SPRT-TANDEM-0.1.4/tandem/config/config_definition.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.621424 SPRT-TANDEM-0.1.4/tandem/data/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.4/tandem/data/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/tandem/models/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.4/tandem/models/__init__.py
--rw-r--r--   0 afe       (1000) afe       (1000)    14111 2023-05-31 05:13:13.000000 SPRT-TANDEM-0.1.4/tandem/models/losses.py
--rwxr--r--   0 afe       (1000) afe       (1000)     1417 2023-05-31 05:14:34.000000 SPRT-TANDEM-0.1.4/tandem/models/optimizers.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 05:17:50.000000 SPRT-TANDEM-0.1.4/tandem/models/temporal_integrators.py
--rwxr--r--   0 afe       (1000) afe       (1000)     2822 2023-05-31 05:19:38.000000 SPRT-TANDEM-0.1.4/tandem/sprt_tandem_main.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/tandem/utils/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.4/tandem/utils/__init__.py
--rwxr--r--   0 afe       (1000) afe       (1000)     6340 2023-05-31 05:18:03.000000 SPRT-TANDEM-0.1.4/tandem/utils/checkpoint.py
--rw-r--r--   0 afe       (1000) afe       (1000)    22645 2023-05-31 05:22:17.000000 SPRT-TANDEM-0.1.4/tandem/utils/data_processing.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 05:18:23.000000 SPRT-TANDEM-0.1.4/tandem/utils/hyperparameter_tuning.py
--rwxr--r--   0 afe       (1000) afe       (1000)    24962 2023-05-31 05:18:36.000000 SPRT-TANDEM-0.1.4/tandem/utils/logging.py
--rwxr--r--   0 afe       (1000) afe       (1000)    20082 2023-05-31 20:23:06.000000 SPRT-TANDEM-0.1.4/tandem/utils/misc.py
--rw-r--r--   0 afe       (1000) afe       (1000)    49570 2023-05-31 05:18:56.000000 SPRT-TANDEM-0.1.4/tandem/utils/performance_metrics.py
--rw-r--r--   0 afe       (1000) afe       (1000)    10223 2023-05-31 20:06:33.000000 SPRT-TANDEM-0.1.4/tandem/utils/training.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/
+-rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.5/LICENSE
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/PKG-INFO
+-rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 12:20:47.000000 SPRT-TANDEM-0.1.5/README.md
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/PKG-INFO
+-rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       30 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/requires.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/top_level.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/setup.cfg
+-rw-r--r--   0 afe       (1000) afe       (1000)     1167 2023-05-31 20:45:20.000000 SPRT-TANDEM-0.1.5/setup.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/
+-rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 05:14:48.000000 SPRT-TANDEM-0.1.5/tandem/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/config/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.5/tandem/config/__init__.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    11204 2023-05-31 20:04:18.000000 SPRT-TANDEM-0.1.5/tandem/config/config_definition.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/data/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.5/tandem/data/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/models/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.5/tandem/models/__init__.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    14111 2023-05-31 05:13:13.000000 SPRT-TANDEM-0.1.5/tandem/models/losses.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     1417 2023-05-31 05:14:34.000000 SPRT-TANDEM-0.1.5/tandem/models/optimizers.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 05:17:50.000000 SPRT-TANDEM-0.1.5/tandem/models/temporal_integrators.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     2822 2023-05-31 05:19:38.000000 SPRT-TANDEM-0.1.5/tandem/sprt_tandem_main.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/utils/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.5/tandem/utils/__init__.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     6340 2023-05-31 05:18:03.000000 SPRT-TANDEM-0.1.5/tandem/utils/checkpoint.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    22645 2023-05-31 05:22:17.000000 SPRT-TANDEM-0.1.5/tandem/utils/data_processing.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 05:18:23.000000 SPRT-TANDEM-0.1.5/tandem/utils/hyperparameter_tuning.py
+-rwxr--r--   0 afe       (1000) afe       (1000)    24962 2023-05-31 05:18:36.000000 SPRT-TANDEM-0.1.5/tandem/utils/logging.py
+-rwxr--r--   0 afe       (1000) afe       (1000)    20082 2023-05-31 20:23:06.000000 SPRT-TANDEM-0.1.5/tandem/utils/misc.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    49570 2023-05-31 05:18:56.000000 SPRT-TANDEM-0.1.5/tandem/utils/performance_metrics.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    10223 2023-05-31 20:06:33.000000 SPRT-TANDEM-0.1.5/tandem/utils/training.py
```

### Comparing `SPRT-TANDEM-0.1.4/LICENSE` & `SPRT-TANDEM-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/PKG-INFO` & `SPRT-TANDEM-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.4
+Version: 0.1.5
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.4/README.md` & `SPRT-TANDEM-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/PKG-INFO` & `SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.4
+Version: 0.1.5
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/SOURCES.txt` & `SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/setup.py` & `SPRT-TANDEM-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(
     path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
 ) as f:
     long_description = f.read()
 
 setup(
     name="SPRT-TANDEM",
-    version="0.1.4",
+    version="0.1.5",
     license="MIT",
     description="SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.",
     author="Akinori F. Ebihara",
     author_email="aebihara@nec.com",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `SPRT-TANDEM-0.1.4/tandem/config/config_definition.py` & `SPRT-TANDEM-0.1.5/tandem/config/config_definition.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/models/losses.py` & `SPRT-TANDEM-0.1.5/tandem/models/losses.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/models/optimizers.py` & `SPRT-TANDEM-0.1.5/tandem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/models/temporal_integrators.py` & `SPRT-TANDEM-0.1.5/tandem/models/temporal_integrators.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/sprt_tandem_main.py` & `SPRT-TANDEM-0.1.5/tandem/sprt_tandem_main.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/utils/checkpoint.py` & `SPRT-TANDEM-0.1.5/tandem/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/utils/data_processing.py` & `SPRT-TANDEM-0.1.5/tandem/utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/utils/hyperparameter_tuning.py` & `SPRT-TANDEM-0.1.5/tandem/utils/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/utils/logging.py` & `SPRT-TANDEM-0.1.5/tandem/utils/logging.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/utils/misc.py` & `SPRT-TANDEM-0.1.5/tandem/utils/misc.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/utils/performance_metrics.py` & `SPRT-TANDEM-0.1.5/tandem/utils/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.4/tandem/utils/training.py` & `SPRT-TANDEM-0.1.5/tandem/utils/training.py`

 * *Files identical despite different names*

