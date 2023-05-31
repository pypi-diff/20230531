# Comparing `tmp/hyponic-0.0.3.tar.gz` & `tmp/hyponic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyponic-0.0.3.tar", last modified: Sun May  7 20:23:52 2023, max compression
+gzip compressed data, was "hyponic-0.1.0.tar", last modified: Wed May 31 07:45:00 2023, max compression
```

## Comparing `hyponic-0.0.3.tar` & `hyponic-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 20:23:33.000000 hyponic-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-07 20:23:52.021546 hyponic-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-07 20:23:33.000000 hyponic-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/hyponic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/metrics/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/metrics/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/base_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/optimizers/genetic_based/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/genetic_based/GA.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/genetic_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/optimizers/physics_based/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/physics_based/SA.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/physics_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/optimizers/swarm_based/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/swarm_based/ABC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/swarm_based/ACO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/swarm_based/PSO.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/swarm_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:23:52.021546 hyponic-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 20:23:33.000000 hyponic-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.124993 hyponic-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-31 07:44:46.000000 hyponic-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-31 07:45:00.120993 hyponic-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-31 07:44:46.000000 hyponic-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/hyponic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/metrics/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/metrics/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/base_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/optimizers/genetic_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/genetic_based/GA.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/genetic_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/optimizers/physics_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/physics_based/SA.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/physics_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/optimizers/swarm_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/ABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/ACO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/CS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/GWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/PSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/optimizers/swarm_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/utils/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/utils/problem_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-31 07:44:46.000000 hyponic-0.1.0/hyponic/utils/symtable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:45:00.120993 hyponic-0.1.0/hyponic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 07:45:00.000000 hyponic-0.1.0/hyponic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:45:00.124993 hyponic-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-31 07:44:46.000000 hyponic-0.1.0/setup.py
```

### Comparing `hyponic-0.0.3/LICENSE` & `hyponic-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyponic-0.0.3/PKG-INFO` & `hyponic-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,14 @@
-Metadata-Version: 2.1
-Name: hyponic
-Version: 0.0.3
-Summary: Hyperparameter Optimization with Nature-Inspired Computing
-Home-page: https://github.com/slewie/HypONIC
-Author: Vladislav Kulikov, Daniel Satarov, Ivan Chernakov
-Author-email: v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
+[![Documentation Status](https://readthedocs.org/projects/hyponic/badge/?version=latest)](https://hyponic.readthedocs.io/en/latest/?badge=latest)
 # HypONIC -- Hyperparameter Optimization with Nature Inspired Computing
 
 *HypONIC* is a hyperparameter optimization library that uses various nature inspired computing algorithms to optimize
-the hyperparameters of machine learning models. The library provides a simple interface for sklearn and keras models.
+the hyperparameters of machine learning models. The library provides a simple interface for sklearn models.
 
+*Documentation*: https://hyponic.readthedocs.io/en/latest/
 ## Library Structure
 ```
 |-- hyponic/
 |   |-- hyponic.py
 |   |-- space.py
 |   |
 |   |-- metrics/
@@ -43,18 +31,73 @@
 |   |       |-- GA.py
 |   |
 |   |-- space/
 |   |   |-- encoders.py (planned)
 |   |   |-- mappers.py  (planned)
 |   |
 |   |-- utils/
-|
+|       |-- history.py
+|       |-- problem_identifier.py
 |-- examples/
     |-- datasets/
 ```
+## Installation
+### Install from PyPI
+```bash
+pip install hyponic
+```
+## Minimal Example
+This is a minimal example for tuning hyperparameters of the `SVC` from `sklearn`.
+The default optimization is *Inertia Weight Particle Swarm Optimization* (IWPSO),
+as it has high applicability and has shown fast convergence.
+
+```python
+# 1. Import of the model, dataset, metric and optimizer
+#    with the algorithm of choice
+from sklearn.svm import SVC
+from sklearn.datasets import load_wine
+
+from hyponic.hyponic import HypONIC
+
+#    ...in this case, log_loss and Inertia Weight PSO
+from hyponic.metrics.classification import log_loss
+from hyponic.optimizers.swarm_based.PSO import IWPSO
+
+# 2. Creating the model and loading the dataset
+model = SVC()
+X, y = load_wine(return_X_y=True)
+
+# 3. Defining our problem
+hyperparams = {
+    "C": (0.01, 1),
+    "kernel": ["linear", "poly", "rbf", "sigmoid"],
+    "degree": [2, 3, 4, 5],
+}
+
+# 4. Parameterizing the optimizer
+optimizer_kwargs = {
+    "epoch": 10,
+    "population_size": 10,
+}
+
+# 5. Passing all to the optimizer
+hyponic = HypONIC(
+    model,
+    X, y,
+    log_loss,
+    optimizer=IWPSO,
+    **optimizer_kwargs
+)
+
+# 6. Solving for the given problem
+hyponic.optimize(hyperparams, verbose=True)
+print(hyponic.get_optimized_parameters())
+print(hyponic.get_optimized_metric())
+print(hyponic.get_optimized_model())
+```
 
 ## Implementation details
 *HypONIC* library follows a common high-level approach by providing a unified interface for applying an optimization algorithm
 of choice to the parameters of a machine learning model (based on the `BaseEstimator` from the `sklearn`). Evaluation of the
 optimization process is done by a metric of choice.
 
 ### Metrics
@@ -173,66 +216,30 @@
 The following algorithms are currently implemented or are planned to be implemented:
 
 **Swarm-based:**
 - - [x] Particle Swarm Optimization (PSO)
 - - [x] Inertia Weight PSO (IWPSO)
 - - [x] Ant Colony Optimization (ACO)
 - - [x] Artificial Bee Colony (ABC)
-- - [ ] Grey Wolf Optimizer (GWO)
-- - [ ] Cuckoo Search (CS)
+- - [x] Grey Wolf Optimizer (GWO)
+- - [x] Cuckoo Search (CS)
 - - [ ] Firefly Algorithm (FA)
 
 **Physics-based:**
 - - [x] Simulated Annealing (SA)
 
 **Genetic-based:**
 - - [x] Genetic Algorithm (GA)
 
-## Minimal Example
-This is a minimal example for tuning hyperparameters of the `RandomForestRegressor` from `sklearn`.
-The default optimization is *Inertia Weight Particle Swarm Optimization* (IWPSO),
-as it has high applicability and has shown fast convergence.
-
-```python
-# 1. Import of the model, dataset, metric and optimizer
-#    with the algorithm of choice
-from sklearn.svm import SVR
-from sklearn.datasets import load_wine
-
-from hyponic.hyponic import HypONIC
 
-#    ...in this case, log_loss and Inertia Weight PSO
-from hyponic.metrics.classification import log_loss
-from hyponic.optimizers.swarm_based.PSO import IWPSO
+The following features are currently implemented or are planned to be implemented:
+- - [x] Early stopping based on the number of epoch without improvement
+- - [x] History of optimization
+- - [x] Parallelization
+- - [x] Visualization of the history
+- - [ ] Visualization of the optimization process
+- - [ ] Customizable stopping criteria
+- - [ ] Partial fit
+- - [ ] Different population initializations
+- - [x] Identifying the problem type (regression, classification)
+- - [ ] Support for pytorch or keras models
 
-# 2. Creating the model and loading the dataset
-model = SVR()
-X, y = load_wine(return_X_y=True)
-
-# 3. Defining our problem
-hyperparams = {
-    "C":       (0.01, 1),
-    "epsilon": (0.01, 0.9),
-    "kernel": ["linear", "poly", "rbf", "sigmoid"],
-}
-
-# 4. Parameterizing the optimizer
-optimizer_kwargs = {
-    "epoch": 10,
-    "pop_size": 10,
-}
-
-# 5. Passing all to the optimizer
-hyponic = HypONIC(
-    model,
-    X, y,
-    log_loss,
-    optimizer=IWPSO,
-    **optimizer_kwargs
-)
-
-# 6. Solving for the given problem
-hyponic.optimize(hyperparams, verbose=True)
-print(hyponic.get_optimized_parameters())
-print(hyponic.get_optimized_metric())
-print(hyponic.get_optimized_model())
-```
```

### Comparing `hyponic-0.0.3/README.md` & `hyponic-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,28 @@
+Metadata-Version: 2.1
+Name: hyponic
+Version: 0.1.0
+Summary: Hyperparameter Optimization with Nature-Inspired Computing
+Home-page: https://github.com/slewie/HypONIC
+Author: Vladislav Kulikov, Daniel Satarov, Ivan Chernakov
+Author-email: v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Documentation Status](https://readthedocs.org/projects/hyponic/badge/?version=latest)](https://hyponic.readthedocs.io/en/latest/?badge=latest)
 # HypONIC -- Hyperparameter Optimization with Nature Inspired Computing
 
 *HypONIC* is a hyperparameter optimization library that uses various nature inspired computing algorithms to optimize
-the hyperparameters of machine learning models. The library provides a simple interface for sklearn and keras models.
+the hyperparameters of machine learning models. The library provides a simple interface for sklearn models.
 
+*Documentation*: https://hyponic.readthedocs.io/en/latest/
 ## Library Structure
 ```
 |-- hyponic/
 |   |-- hyponic.py
 |   |-- space.py
 |   |
 |   |-- metrics/
@@ -29,18 +45,73 @@
 |   |       |-- GA.py
 |   |
 |   |-- space/
 |   |   |-- encoders.py (planned)
 |   |   |-- mappers.py  (planned)
 |   |
 |   |-- utils/
-|
+|       |-- history.py
+|       |-- problem_identifier.py
 |-- examples/
     |-- datasets/
 ```
+## Installation
+### Install from PyPI
+```bash
+pip install hyponic
+```
+## Minimal Example
+This is a minimal example for tuning hyperparameters of the `SVC` from `sklearn`.
+The default optimization is *Inertia Weight Particle Swarm Optimization* (IWPSO),
+as it has high applicability and has shown fast convergence.
+
+```python
+# 1. Import of the model, dataset, metric and optimizer
+#    with the algorithm of choice
+from sklearn.svm import SVC
+from sklearn.datasets import load_wine
+
+from hyponic.hyponic import HypONIC
+
+#    ...in this case, log_loss and Inertia Weight PSO
+from hyponic.metrics.classification import log_loss
+from hyponic.optimizers.swarm_based.PSO import IWPSO
+
+# 2. Creating the model and loading the dataset
+model = SVC()
+X, y = load_wine(return_X_y=True)
+
+# 3. Defining our problem
+hyperparams = {
+    "C": (0.01, 1),
+    "kernel": ["linear", "poly", "rbf", "sigmoid"],
+    "degree": [2, 3, 4, 5],
+}
+
+# 4. Parameterizing the optimizer
+optimizer_kwargs = {
+    "epoch": 10,
+    "population_size": 10,
+}
+
+# 5. Passing all to the optimizer
+hyponic = HypONIC(
+    model,
+    X, y,
+    log_loss,
+    optimizer=IWPSO,
+    **optimizer_kwargs
+)
+
+# 6. Solving for the given problem
+hyponic.optimize(hyperparams, verbose=True)
+print(hyponic.get_optimized_parameters())
+print(hyponic.get_optimized_metric())
+print(hyponic.get_optimized_model())
+```
 
 ## Implementation details
 *HypONIC* library follows a common high-level approach by providing a unified interface for applying an optimization algorithm
 of choice to the parameters of a machine learning model (based on the `BaseEstimator` from the `sklearn`). Evaluation of the
 optimization process is done by a metric of choice.
 
 ### Metrics
@@ -159,66 +230,30 @@
 The following algorithms are currently implemented or are planned to be implemented:
 
 **Swarm-based:**
 - - [x] Particle Swarm Optimization (PSO)
 - - [x] Inertia Weight PSO (IWPSO)
 - - [x] Ant Colony Optimization (ACO)
 - - [x] Artificial Bee Colony (ABC)
-- - [ ] Grey Wolf Optimizer (GWO)
-- - [ ] Cuckoo Search (CS)
+- - [x] Grey Wolf Optimizer (GWO)
+- - [x] Cuckoo Search (CS)
 - - [ ] Firefly Algorithm (FA)
 
 **Physics-based:**
 - - [x] Simulated Annealing (SA)
 
 **Genetic-based:**
 - - [x] Genetic Algorithm (GA)
 
-## Minimal Example
-This is a minimal example for tuning hyperparameters of the `RandomForestRegressor` from `sklearn`.
-The default optimization is *Inertia Weight Particle Swarm Optimization* (IWPSO),
-as it has high applicability and has shown fast convergence.
-
-```python
-# 1. Import of the model, dataset, metric and optimizer
-#    with the algorithm of choice
-from sklearn.svm import SVR
-from sklearn.datasets import load_wine
-
-from hyponic.hyponic import HypONIC
 
-#    ...in this case, log_loss and Inertia Weight PSO
-from hyponic.metrics.classification import log_loss
-from hyponic.optimizers.swarm_based.PSO import IWPSO
+The following features are currently implemented or are planned to be implemented:
+- - [x] Early stopping based on the number of epoch without improvement
+- - [x] History of optimization
+- - [x] Parallelization
+- - [x] Visualization of the history
+- - [ ] Visualization of the optimization process
+- - [ ] Customizable stopping criteria
+- - [ ] Partial fit
+- - [ ] Different population initializations
+- - [x] Identifying the problem type (regression, classification)
+- - [ ] Support for pytorch or keras models
 
-# 2. Creating the model and loading the dataset
-model = SVR()
-X, y = load_wine(return_X_y=True)
-
-# 3. Defining our problem
-hyperparams = {
-    "C":       (0.01, 1),
-    "epsilon": (0.01, 0.9),
-    "kernel": ["linear", "poly", "rbf", "sigmoid"],
-}
-
-# 4. Parameterizing the optimizer
-optimizer_kwargs = {
-    "epoch": 10,
-    "pop_size": 10,
-}
-
-# 5. Passing all to the optimizer
-hyponic = HypONIC(
-    model,
-    X, y,
-    log_loss,
-    optimizer=IWPSO,
-    **optimizer_kwargs
-)
-
-# 6. Solving for the given problem
-hyponic.optimize(hyperparams, verbose=True)
-print(hyponic.get_optimized_parameters())
-print(hyponic.get_optimized_metric())
-print(hyponic.get_optimized_model())
-```
```

### Comparing `hyponic-0.0.3/hyponic/__init__.py` & `hyponic-0.1.0/hyponic/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.1-alpha-0'
+__version__ = '0.1.0'
 
 from .hyponic import HypONIC
 
 from .metrics.decorators import add_metric_to_dict, add_metric_info,\
     add_metric_aliases, minimize_metric, maximize_metric
 
 from .metrics.classification import accuracy, precision, recall, f1_score,\
@@ -11,10 +11,15 @@
 from .metrics.regression import mae, mse, rmse, rmsle, r2, adjusted_r2, huber_loss
 
 from .optimizers.genetic_based.GA import GA
 from .optimizers.physics_based.SA import SA
 from .optimizers.swarm_based.ABC import ABC
 from .optimizers.swarm_based.ACO import ACO
 from .optimizers.swarm_based.PSO import PSO, IWPSO
+from .optimizers.swarm_based.GWO import GWO
+from .optimizers.swarm_based.CS import CS
 from .optimizers.base_optimizer import BaseOptimizer
 
 from .space import Space, Dimension, Continuous, Discrete
+
+from .utils.history import History
+from .utils.problem_identifier import ProblemIdentifier, ProblemType
```

### Comparing `hyponic-0.0.3/hyponic/hyponic.py` & `hyponic-0.1.0/hyponic/hyponic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 from warnings import warn
 
 from hyponic.optimizers.swarm_based.PSO import IWPSO
 from hyponic.metrics.decorators import METRICS_DICT
+from hyponic.utils.problem_identifier import ProblemIdentifier, ProblemType
 
 from typing import Callable
 
 from hyponic.space import Space
 from functools import partial
 
 
 class HypONIC:
     """
     HypONIC (Hyperparameter Optimization using Nature-Inspired Computing)
 
     Main class for hyperparameter optimization.
     """
-    def __init__(self, model, X, y, metric: Callable | str, optimizer=None, **kwargs):
+
+    def __init__(self, model, X, y, metric: Callable | str | None = None, optimizer=None, **kwargs):
         self.model = model
         self.X = X
         self.y = y
 
         if isinstance(metric, str):
             # Try to get metric from the METRICS_DICT
             self.metric = METRICS_DICT.get(metric, None)
 
             if self.metric is None:
                 raise Exception(f"Metric {metric} is not found.")
         elif isinstance(metric, Callable):
             self.metric = metric
+        elif metric is None:
+            # If metric is None, then try to get metric from the problem type
+            problem_type = ProblemIdentifier(self.y).get_problem_type()
+
+            match problem_type:
+                case ProblemType.REGRESSION:
+                    self.metric = METRICS_DICT["mse"]
+                case ProblemType.BINARY_CLASSIFICATION:
+                    self.metric = METRICS_DICT["binary_crossentropy"]
+                case ProblemType.MULTICLASS_CLASSIFICATION:
+                    self.metric = METRICS_DICT["log_loss"]
+        else:
+            raise Exception(f"Metric {metric} is not found.")
 
         try:
             self.minmax = self.metric.__getattribute__("minmax")
         except AttributeError:
             # If a metric does not have minmax attribute,
             # then it is assumed to be a custom metric and will be minimized by default
             warn(f"Metric {metric.__name__} does not have minmax attribute. Minimize by default.")
@@ -126,7 +141,15 @@
     @warn_not_optimized
     def get_optimized_parameters(self) -> dict:
         return self.hyperparams_optimized
 
     @warn_not_optimized
     def get_optimized_metric(self) -> float:
         return self.metric_optimized
+
+    @warn_not_optimized
+    def visualize_history_fitness(self):
+        self.optimizer.visualize_history_fitness()
+
+    @warn_not_optimized
+    def visualize_history_time(self):
+        self.optimizer.visualize_history_time()
```

### Comparing `hyponic-0.0.3/hyponic/metrics/decorators.py` & `hyponic-0.1.0/hyponic/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.0.3/hyponic/space.py` & `hyponic-0.1.0/hyponic/space.py`

 * *Files identical despite different names*

### Comparing `hyponic-0.0.3/hyponic.egg-info/PKG-INFO` & `hyponic-0.1.0/hyponic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: hyponic
-Version: 0.0.3
+Version: 0.1.0
 Summary: Hyperparameter Optimization with Nature-Inspired Computing
 Home-page: https://github.com/slewie/HypONIC
 Author: Vladislav Kulikov, Daniel Satarov, Ivan Chernakov
 Author-email: v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Documentation Status](https://readthedocs.org/projects/hyponic/badge/?version=latest)](https://hyponic.readthedocs.io/en/latest/?badge=latest)
 # HypONIC -- Hyperparameter Optimization with Nature Inspired Computing
 
 *HypONIC* is a hyperparameter optimization library that uses various nature inspired computing algorithms to optimize
-the hyperparameters of machine learning models. The library provides a simple interface for sklearn and keras models.
+the hyperparameters of machine learning models. The library provides a simple interface for sklearn models.
 
+*Documentation*: https://hyponic.readthedocs.io/en/latest/
 ## Library Structure
 ```
 |-- hyponic/
 |   |-- hyponic.py
 |   |-- space.py
 |   |
 |   |-- metrics/
@@ -43,18 +45,73 @@
 |   |       |-- GA.py
 |   |
 |   |-- space/
 |   |   |-- encoders.py (planned)
 |   |   |-- mappers.py  (planned)
 |   |
 |   |-- utils/
-|
+|       |-- history.py
+|       |-- problem_identifier.py
 |-- examples/
     |-- datasets/
 ```
+## Installation
+### Install from PyPI
+```bash
+pip install hyponic
+```
+## Minimal Example
+This is a minimal example for tuning hyperparameters of the `SVC` from `sklearn`.
+The default optimization is *Inertia Weight Particle Swarm Optimization* (IWPSO),
+as it has high applicability and has shown fast convergence.
+
+```python
+# 1. Import of the model, dataset, metric and optimizer
+#    with the algorithm of choice
+from sklearn.svm import SVC
+from sklearn.datasets import load_wine
+
+from hyponic.hyponic import HypONIC
+
+#    ...in this case, log_loss and Inertia Weight PSO
+from hyponic.metrics.classification import log_loss
+from hyponic.optimizers.swarm_based.PSO import IWPSO
+
+# 2. Creating the model and loading the dataset
+model = SVC()
+X, y = load_wine(return_X_y=True)
+
+# 3. Defining our problem
+hyperparams = {
+    "C": (0.01, 1),
+    "kernel": ["linear", "poly", "rbf", "sigmoid"],
+    "degree": [2, 3, 4, 5],
+}
+
+# 4. Parameterizing the optimizer
+optimizer_kwargs = {
+    "epoch": 10,
+    "population_size": 10,
+}
+
+# 5. Passing all to the optimizer
+hyponic = HypONIC(
+    model,
+    X, y,
+    log_loss,
+    optimizer=IWPSO,
+    **optimizer_kwargs
+)
+
+# 6. Solving for the given problem
+hyponic.optimize(hyperparams, verbose=True)
+print(hyponic.get_optimized_parameters())
+print(hyponic.get_optimized_metric())
+print(hyponic.get_optimized_model())
+```
 
 ## Implementation details
 *HypONIC* library follows a common high-level approach by providing a unified interface for applying an optimization algorithm
 of choice to the parameters of a machine learning model (based on the `BaseEstimator` from the `sklearn`). Evaluation of the
 optimization process is done by a metric of choice.
 
 ### Metrics
@@ -173,66 +230,30 @@
 The following algorithms are currently implemented or are planned to be implemented:
 
 **Swarm-based:**
 - - [x] Particle Swarm Optimization (PSO)
 - - [x] Inertia Weight PSO (IWPSO)
 - - [x] Ant Colony Optimization (ACO)
 - - [x] Artificial Bee Colony (ABC)
-- - [ ] Grey Wolf Optimizer (GWO)
-- - [ ] Cuckoo Search (CS)
+- - [x] Grey Wolf Optimizer (GWO)
+- - [x] Cuckoo Search (CS)
 - - [ ] Firefly Algorithm (FA)
 
 **Physics-based:**
 - - [x] Simulated Annealing (SA)
 
 **Genetic-based:**
 - - [x] Genetic Algorithm (GA)
 
-## Minimal Example
-This is a minimal example for tuning hyperparameters of the `RandomForestRegressor` from `sklearn`.
-The default optimization is *Inertia Weight Particle Swarm Optimization* (IWPSO),
-as it has high applicability and has shown fast convergence.
-
-```python
-# 1. Import of the model, dataset, metric and optimizer
-#    with the algorithm of choice
-from sklearn.svm import SVR
-from sklearn.datasets import load_wine
-
-from hyponic.hyponic import HypONIC
-
-#    ...in this case, log_loss and Inertia Weight PSO
-from hyponic.metrics.classification import log_loss
-from hyponic.optimizers.swarm_based.PSO import IWPSO
-
-# 2. Creating the model and loading the dataset
-model = SVR()
-X, y = load_wine(return_X_y=True)
-
-# 3. Defining our problem
-hyperparams = {
-    "C":       (0.01, 1),
-    "epsilon": (0.01, 0.9),
-    "kernel": ["linear", "poly", "rbf", "sigmoid"],
-}
-
-# 4. Parameterizing the optimizer
-optimizer_kwargs = {
-    "epoch": 10,
-    "pop_size": 10,
-}
 
-# 5. Passing all to the optimizer
-hyponic = HypONIC(
-    model,
-    X, y,
-    log_loss,
-    optimizer=IWPSO,
-    **optimizer_kwargs
-)
+The following features are currently implemented or are planned to be implemented:
+- - [x] Early stopping based on the number of epoch without improvement
+- - [x] History of optimization
+- - [x] Parallelization
+- - [x] Visualization of the history
+- - [ ] Visualization of the optimization process
+- - [ ] Customizable stopping criteria
+- - [ ] Partial fit
+- - [ ] Different population initializations
+- - [x] Identifying the problem type (regression, classification)
+- - [ ] Support for pytorch or keras models
 
-# 6. Solving for the given problem
-hyponic.optimize(hyperparams, verbose=True)
-print(hyponic.get_optimized_parameters())
-print(hyponic.get_optimized_metric())
-print(hyponic.get_optimized_model())
-```
```

### Comparing `hyponic-0.0.3/hyponic.egg-info/SOURCES.txt` & `hyponic-0.1.0/hyponic.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,9 +17,15 @@
 hyponic/optimizers/base_optimizer.py
 hyponic/optimizers/genetic_based/GA.py
 hyponic/optimizers/genetic_based/__init__.py
 hyponic/optimizers/physics_based/SA.py
 hyponic/optimizers/physics_based/__init__.py
 hyponic/optimizers/swarm_based/ABC.py
 hyponic/optimizers/swarm_based/ACO.py
+hyponic/optimizers/swarm_based/CS.py
+hyponic/optimizers/swarm_based/GWO.py
 hyponic/optimizers/swarm_based/PSO.py
-hyponic/optimizers/swarm_based/__init__.py
+hyponic/optimizers/swarm_based/__init__.py
+hyponic/utils/__init__.py
+hyponic/utils/history.py
+hyponic/utils/problem_identifier.py
+hyponic/utils/symtable.py
```

### Comparing `hyponic-0.0.3/setup.py` & `hyponic-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setuptools.setup(
     name='hyponic',
-    version='0.0.3',
+    version='0.1.0',
     author='Vladislav Kulikov, Daniel Satarov, Ivan Chernakov',
     author_email='v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university',
     description='Hyperparameter Optimization with Nature-Inspired Computing',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/slewie/HypONIC',
     packages=setuptools.find_packages(),
     install_requires=[
-        'numpy>=1.19.2',
+        'numpy>=1.24.2',
+        'numexpr>=2.8.4',
+        'numba>=0.57.0',
+        'matplotlib>=3.7.1',
     ],
     classifiers=[
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```

