# Comparing `tmp/hyponic-0.1.0.tar.gz` & `tmp/hyponic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyponic-0.1.0.tar", last modified: Wed May 31 07:45:00 2023, max compression
+gzip compressed data, was "hyponic-0.1.1.tar", last modified: Wed May 31 07:52:29 2023, max compression
```

## Comparing `hyponic-0.1.0.tar` & `hyponic-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.124993 hyponic-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-31 07:44:46.000000 hyponic-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-31 07:45:00.120993 hyponic-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-31 07:44:46.000000 hyponic-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/hyponic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/metrics/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/metrics/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/base_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/optimizers/genetic_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/genetic_based/GA.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/genetic_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/optimizers/physics_based/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/physics_based/SA.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/physics_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/optimizers/swarm_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/ABC.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/ACO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/CS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/GWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/PSO.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/utils/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/utils/problem_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/utils/symtable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:45:00.124993 hyponic-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-31 07:44:46.000000 hyponic-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:29.101872 hyponic-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-31 07:52:18.000000 hyponic-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-31 07:52:29.101872 hyponic-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-31 07:52:18.000000 hyponic-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:29.101872 hyponic-0.1.1/hyponic/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/hyponic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:29.101872 hyponic-0.1.1/hyponic/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/metrics/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/metrics/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:29.101872 hyponic-0.1.1/hyponic/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/base_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:29.101872 hyponic-0.1.1/hyponic/optimizers/genetic_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/genetic_based/GA.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/genetic_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:29.101872 hyponic-0.1.1/hyponic/optimizers/physics_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/physics_based/SA.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/physics_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:29.101872 hyponic-0.1.1/hyponic/optimizers/swarm_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/swarm_based/ABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/swarm_based/ACO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/swarm_based/CS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/swarm_based/GWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/swarm_based/PSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/optimizers/swarm_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:29.101872 hyponic-0.1.1/hyponic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/utils/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/utils/problem_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-31 07:52:18.000000 hyponic-0.1.1/hyponic/utils/symtable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:52:29.101872 hyponic-0.1.1/hyponic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-31 07:52:29.000000 hyponic-0.1.1/hyponic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-31 07:52:29.000000 hyponic-0.1.1/hyponic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:52:29.000000 hyponic-0.1.1/hyponic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 07:52:29.000000 hyponic-0.1.1/hyponic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 07:52:29.000000 hyponic-0.1.1/hyponic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:52:29.101872 hyponic-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-31 07:52:18.000000 hyponic-0.1.1/setup.py
```

### Comparing `hyponic-0.1.0/LICENSE` & `hyponic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/PKG-INFO` & `hyponic-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyponic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hyperparameter Optimization with Nature-Inspired Computing
 Home-page: https://github.com/slewie/HypONIC
 Author: Vladislav Kulikov, Daniel Satarov, Ivan Chernakov
 Author-email: v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hyponic-0.1.0/README.md` & `hyponic-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/__init__.py` & `hyponic-0.1.1/hyponic/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 from .hyponic import HypONIC
 
 from .metrics.decorators import add_metric_to_dict, add_metric_info,\
     add_metric_aliases, minimize_metric, maximize_metric
 
 from .metrics.classification import accuracy, precision, recall, f1_score,\
```

### Comparing `hyponic-0.1.0/hyponic/hyponic.py` & `hyponic-0.1.1/hyponic/hyponic.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/metrics/classification.py` & `hyponic-0.1.1/hyponic/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/metrics/decorators.py` & `hyponic-0.1.1/hyponic/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/metrics/regression.py` & `hyponic-0.1.1/hyponic/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/optimizers/base_optimizer.py` & `hyponic-0.1.1/hyponic/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/optimizers/genetic_based/GA.py` & `hyponic-0.1.1/hyponic/optimizers/genetic_based/GA.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/optimizers/physics_based/SA.py` & `hyponic-0.1.1/hyponic/optimizers/physics_based/SA.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/optimizers/swarm_based/ABC.py` & `hyponic-0.1.1/hyponic/optimizers/swarm_based/ABC.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/optimizers/swarm_based/ACO.py` & `hyponic-0.1.1/hyponic/optimizers/swarm_based/ACO.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/optimizers/swarm_based/CS.py` & `hyponic-0.1.1/hyponic/optimizers/swarm_based/CS.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/optimizers/swarm_based/GWO.py` & `hyponic-0.1.1/hyponic/optimizers/swarm_based/GWO.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/optimizers/swarm_based/PSO.py` & `hyponic-0.1.1/hyponic/optimizers/swarm_based/PSO.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/space.py` & `hyponic-0.1.1/hyponic/space.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/utils/history.py` & `hyponic-0.1.1/hyponic/utils/history.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/utils/problem_identifier.py` & `hyponic-0.1.1/hyponic/utils/problem_identifier.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic/utils/symtable.py` & `hyponic-0.1.1/hyponic/utils/symtable.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/hyponic.egg-info/PKG-INFO` & `hyponic-0.1.1/hyponic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyponic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hyperparameter Optimization with Nature-Inspired Computing
 Home-page: https://github.com/slewie/HypONIC
 Author: Vladislav Kulikov, Daniel Satarov, Ivan Chernakov
 Author-email: v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hyponic-0.1.0/hyponic.egg-info/SOURCES.txt` & `hyponic-0.1.1/hyponic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyponic-0.1.0/setup.py` & `hyponic-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setuptools.setup(
     name='hyponic',
-    version='0.1.0',
+    version='0.1.1',
     author='Vladislav Kulikov, Daniel Satarov, Ivan Chernakov',
     author_email='v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university',
     description='Hyperparameter Optimization with Nature-Inspired Computing',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/slewie/HypONIC',
     packages=setuptools.find_packages(),
     install_requires=[
-        'numpy>=1.24.2',
+        'numpy>=1.23.5',
         'numexpr>=2.8.4',
         'numba>=0.57.0',
-        'matplotlib>=3.7.1',
+        'matplotlib>=3.6.3',
     ],
     classifiers=[
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```

