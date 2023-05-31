# Comparing `tmp/csle_system_identification-0.2.3.tar.gz` & `tmp/csle_system_identification-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_system_identification-0.2.3.tar", last modified: Wed May 31 12:13:56 2023, max compression
+gzip compressed data, was "csle_system_identification-0.2.4.tar", last modified: Wed May 31 13:43:41 2023, max compression
```

## Comparing `csle_system_identification-0.2.3.tar` & `csle_system_identification-0.2.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.191142 csle_system_identification-0.2.3/
--rw-r--r--   0 kimham     (501) staff       (20)      671 2023-05-31 12:13:56.191262 csle_system_identification-0.2.3/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     4235 2023-01-11 18:45:47.000000 csle_system_identification-0.2.3/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      686 2023-02-12 08:59:32.000000 csle_system_identification-0.2.3/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1340 2023-05-31 12:13:56.191882 csle_system_identification-0.2.3/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.178554 csle_system_identification-0.2.3/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.181907 csle_system_identification-0.2.3/src/csle_system_identification/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 12:12:15.000000 csle_system_identification-0.2.3/src/csle_system_identification/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.185193 csle_system_identification-0.2.3/src/csle_system_identification/base/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/base/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2074 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/base/base_system_identification_algorithm.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.186036 csle_system_identification-0.2.3/src/csle_system_identification/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      688 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.187044 csle_system_identification-0.2.3/src/csle_system_identification/empirical/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/empirical/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     7249 2023-03-31 11:14:06.000000 csle_system_identification-0.2.3/src/csle_system_identification/empirical/empirical_algorithm.py
--rw-r--r--   0 kimham     (501) staff       (20)    17108 2023-04-19 06:25:48.000000 csle_system_identification-0.2.3/src/csle_system_identification/emulator.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.187898 csle_system_identification-0.2.3/src/csle_system_identification/expectation_maximization/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/expectation_maximization/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     7494 2023-03-31 11:14:06.000000 csle_system_identification-0.2.3/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.189431 csle_system_identification-0.2.3/src/csle_system_identification/gp/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/gp/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     9801 2023-03-31 11:14:06.000000 csle_system_identification-0.2.3/src/csle_system_identification/gp/gp_regression_algorithm.py
--rw-r--r--   0 kimham     (501) staff       (20)      555 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.190839 csle_system_identification-0.2.3/src/csle_system_identification/job_controllers/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/job_controllers/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2159 2022-12-07 07:23:42.000000 csle_system_identification-0.2.3/src/csle_system_identification/job_controllers/data_collection_job_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     2212 2022-11-28 13:00:49.000000 csle_system_identification-0.2.3/src/csle_system_identification/job_controllers/system_identification_job_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:13:56.184733 csle_system_identification-0.2.3/src/csle_system_identification.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      671 2023-05-31 12:13:55.000000 csle_system_identification-0.2.3/src/csle_system_identification.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     1412 2023-05-31 12:13:56.000000 csle_system_identification-0.2.3/src/csle_system_identification.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 12:13:55.000000 csle_system_identification-0.2.3/src/csle_system_identification.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:48.000000 csle_system_identification-0.2.3/src/csle_system_identification.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      257 2023-05-31 12:13:56.000000 csle_system_identification-0.2.3/src/csle_system_identification.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       27 2023-05-31 12:13:56.000000 csle_system_identification-0.2.3/src/csle_system_identification.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.391920 csle_system_identification-0.2.4/
+-rw-r--r--   0 kimham     (501) staff       (20)      671 2023-05-31 13:43:41.392129 csle_system_identification-0.2.4/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     4235 2023-01-11 18:45:47.000000 csle_system_identification-0.2.4/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      686 2023-02-12 08:59:32.000000 csle_system_identification-0.2.4/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1340 2023-05-31 13:43:41.393101 csle_system_identification-0.2.4/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.375199 csle_system_identification-0.2.4/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.378273 csle_system_identification-0.2.4/src/csle_system_identification/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 csle_system_identification-0.2.4/src/csle_system_identification/__version__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.382676 csle_system_identification-0.2.4/src/csle_system_identification/base/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/base/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2074 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/base/base_system_identification_algorithm.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.383976 csle_system_identification-0.2.4/src/csle_system_identification/constants/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/constants/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      688 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/constants/constants.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.385155 csle_system_identification-0.2.4/src/csle_system_identification/empirical/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/empirical/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7249 2023-03-31 11:14:06.000000 csle_system_identification-0.2.4/src/csle_system_identification/empirical/empirical_algorithm.py
+-rw-r--r--   0 kimham     (501) staff       (20)    17108 2023-04-19 06:25:48.000000 csle_system_identification-0.2.4/src/csle_system_identification/emulator.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.386325 csle_system_identification-0.2.4/src/csle_system_identification/expectation_maximization/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/expectation_maximization/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7494 2023-03-31 11:14:06.000000 csle_system_identification-0.2.4/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.388856 csle_system_identification-0.2.4/src/csle_system_identification/gp/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/gp/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     9801 2023-03-31 11:14:06.000000 csle_system_identification-0.2.4/src/csle_system_identification/gp/gp_regression_algorithm.py
+-rw-r--r--   0 kimham     (501) staff       (20)      555 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.391391 csle_system_identification-0.2.4/src/csle_system_identification/job_controllers/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/job_controllers/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2159 2022-12-07 07:23:42.000000 csle_system_identification-0.2.4/src/csle_system_identification/job_controllers/data_collection_job_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2212 2022-11-28 13:00:49.000000 csle_system_identification-0.2.4/src/csle_system_identification/job_controllers/system_identification_job_manager.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:41.381956 csle_system_identification-0.2.4/src/csle_system_identification.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      671 2023-05-31 13:43:40.000000 csle_system_identification-0.2.4/src/csle_system_identification.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     1412 2023-05-31 13:43:41.000000 csle_system_identification-0.2.4/src/csle_system_identification.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:43:40.000000 csle_system_identification-0.2.4/src/csle_system_identification.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:48.000000 csle_system_identification-0.2.4/src/csle_system_identification.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      257 2023-05-31 13:43:41.000000 csle_system_identification-0.2.4/src/csle_system_identification.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       27 2023-05-31 13:43:41.000000 csle_system_identification-0.2.4/src/csle_system_identification.egg-info/top_level.txt
```

### Comparing `csle_system_identification-0.2.3/PKG-INFO` & `csle_system_identification-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_system_identification
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.2.3/README.md` & `csle_system_identification-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/pyproject.toml` & `csle_system_identification-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/setup.cfg` & `csle_system_identification-0.2.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.2.3
-	csle-collector>=0.2.3
-	csle-attacker>=0.2.3
-	csle-defender>=0.2.3
+	csle-common>=0.2.4
+	csle-collector>=0.2.4
+	csle-attacker>=0.2.4
+	csle-defender>=0.2.4
 	gpytorch>=1.9.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
```

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification/base/base_system_identification_algorithm.py` & `csle_system_identification-0.2.4/src/csle_system_identification/base/base_system_identification_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification/constants/constants.py` & `csle_system_identification-0.2.4/src/csle_system_identification/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification/empirical/empirical_algorithm.py` & `csle_system_identification-0.2.4/src/csle_system_identification/empirical/empirical_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification/emulator.py` & `csle_system_identification-0.2.4/src/csle_system_identification/emulator.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py` & `csle_system_identification-0.2.4/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification/gp/gp_regression_algorithm.py` & `csle_system_identification-0.2.4/src/csle_system_identification/gp/gp_regression_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py` & `csle_system_identification-0.2.4/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification/job_controllers/data_collection_job_manager.py` & `csle_system_identification-0.2.4/src/csle_system_identification/job_controllers/data_collection_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification/job_controllers/system_identification_job_manager.py` & `csle_system_identification-0.2.4/src/csle_system_identification/job_controllers/system_identification_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification.egg-info/PKG-INFO` & `csle_system_identification-0.2.4/src/csle_system_identification.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-system-identification
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.2.3/src/csle_system_identification.egg-info/SOURCES.txt` & `csle_system_identification-0.2.4/src/csle_system_identification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

