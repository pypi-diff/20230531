# Comparing `tmp/sb-arch-opt-1.0.0.tar.gz` & `tmp/sb-arch-opt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb-arch-opt-1.0.0.tar", last modified: Thu May 25 15:27:46 2023, max compression
+gzip compressed data, was "sb-arch-opt-1.1.0.tar", last modified: Wed May 31 14:04:46 2023, max compression
```

## Comparing `sb-arch-opt-1.0.0.tar` & `sb-arch-opt-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:27:46.102867 sb-arch-opt-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-25 15:27:31.000000 sb-arch-opt-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-25 15:27:46.102867 sb-arch-opt-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-25 15:27:31.000000 sb-arch-opt-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:27:31.000000 sb-arch-opt-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:27:46.102867 sb-arch-opt-1.0.0/sb_arch_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 15:27:31.000000 sb-arch-opt-1.0.0/sb_arch_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-05-25 15:27:31.000000 sb-arch-opt-1.0.0/sb_arch_opt/design_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-05-25 15:27:31.000000 sb-arch-opt-1.0.0/sb_arch_opt/design_space_explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-25 15:27:31.000000 sb-arch-opt-1.0.0/sb_arch_opt/pareto_front.py
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-05-25 15:27:31.000000 sb-arch-opt-1.0.0/sb_arch_opt/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22217 2023-05-25 15:27:32.000000 sb-arch-opt-1.0.0/sb_arch_opt/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-25 15:27:32.000000 sb-arch-opt-1.0.0/sb_arch_opt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:27:46.102867 sb-arch-opt-1.0.0/sb_arch_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-25 15:27:46.000000 sb-arch-opt-1.0.0/sb_arch_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-25 15:27:46.000000 sb-arch-opt-1.0.0/sb_arch_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:27:46.000000 sb-arch-opt-1.0.0/sb_arch_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 15:27:46.000000 sb-arch-opt-1.0.0/sb_arch_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 15:27:46.000000 sb-arch-opt-1.0.0/sb_arch_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:27:46.102867 sb-arch-opt-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-25 15:27:32.000000 sb-arch-opt-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/sb_arch_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/design_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/design_space_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22217 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/setup.py
```

### Comparing `sb-arch-opt-1.0.0/LICENSE` & `sb-arch-opt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.0.0/PKG-INFO` & `sb-arch-opt-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb-arch-opt
-Version: 1.0.0
+Version: 1.1.0
 Summary: SBArchOpt: Surrogate-Based Architecture Optimization
 Author: Jasper Bussemaker
 Author-email: jasper.bussemaker@dlr.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,18 @@
 Provides-Extra: botorch
 Provides-Extra: trieste
 Provides-Extra: tpe
 License-File: LICENSE
 
 # SBArchOpt: Surrogate-Based Architecture Optimization
 
+[![Tests](https://github.com/jbussemaker/SBArchOpt/workflows/Tests/badge.svg)](https://github.com/jbussemaker/SBArchOpt/actions/workflows/tests.yml?query=workflow%3ATests)
+[![PyPI](https://img.shields.io/pypi/v/sb-arch-opt.svg)](https://pypi.org/project/sb-arch-opt)
+[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
+
 SBArchOpt (es-bee-ARK-opt) provides a set of classes and interfaces for applying Surrogate-Based Optimization (SBO)
 for system architecture optimization problems:
 - Expensive black-box problems: evaluating one candidate architecture might be computationally expensive
 - Mixed-discrete design variables: categorical architectural decisions mixed with continuous sizing variables
 - Hierarchical design variables: decisions can deactivate/activate (parts of) downstream decisions
 - Multi-objective: stemming from conflicting stakeholder needs
 - Subject to hidden constraints: simulation tools might not converge for all design points
```

### Comparing `sb-arch-opt-1.0.0/README.md` & `sb-arch-opt-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # SBArchOpt: Surrogate-Based Architecture Optimization
 
+[![Tests](https://github.com/jbussemaker/SBArchOpt/workflows/Tests/badge.svg)](https://github.com/jbussemaker/SBArchOpt/actions/workflows/tests.yml?query=workflow%3ATests)
+[![PyPI](https://img.shields.io/pypi/v/sb-arch-opt.svg)](https://pypi.org/project/sb-arch-opt)
+[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
+
 SBArchOpt (es-bee-ARK-opt) provides a set of classes and interfaces for applying Surrogate-Based Optimization (SBO)
 for system architecture optimization problems:
 - Expensive black-box problems: evaluating one candidate architecture might be computationally expensive
 - Mixed-discrete design variables: categorical architectural decisions mixed with continuous sizing variables
 - Hierarchical design variables: decisions can deactivate/activate (parts of) downstream decisions
 - Multi-objective: stemming from conflicting stakeholder needs
 - Subject to hidden constraints: simulation tools might not converge for all design points
```

### Comparing `sb-arch-opt-1.0.0/sb_arch_opt/design_space.py` & `sb-arch-opt-1.1.0/sb_arch_opt/design_space.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.0.0/sb_arch_opt/design_space_explicit.py` & `sb-arch-opt-1.1.0/sb_arch_opt/design_space_explicit.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.0.0/sb_arch_opt/pareto_front.py` & `sb-arch-opt-1.1.0/sb_arch_opt/pareto_front.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.0.0/sb_arch_opt/problem.py` & `sb-arch-opt-1.1.0/sb_arch_opt/problem.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.0.0/sb_arch_opt/sampling.py` & `sb-arch-opt-1.1.0/sb_arch_opt/sampling.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.0.0/sb_arch_opt/util.py` & `sb-arch-opt-1.1.0/sb_arch_opt/util.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.0.0/sb_arch_opt.egg-info/PKG-INFO` & `sb-arch-opt-1.1.0/sb_arch_opt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb-arch-opt
-Version: 1.0.0
+Version: 1.1.0
 Summary: SBArchOpt: Surrogate-Based Architecture Optimization
 Author: Jasper Bussemaker
 Author-email: jasper.bussemaker@dlr.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,18 @@
 Provides-Extra: botorch
 Provides-Extra: trieste
 Provides-Extra: tpe
 License-File: LICENSE
 
 # SBArchOpt: Surrogate-Based Architecture Optimization
 
+[![Tests](https://github.com/jbussemaker/SBArchOpt/workflows/Tests/badge.svg)](https://github.com/jbussemaker/SBArchOpt/actions/workflows/tests.yml?query=workflow%3ATests)
+[![PyPI](https://img.shields.io/pypi/v/sb-arch-opt.svg)](https://pypi.org/project/sb-arch-opt)
+[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
+
 SBArchOpt (es-bee-ARK-opt) provides a set of classes and interfaces for applying Surrogate-Based Optimization (SBO)
 for system architecture optimization problems:
 - Expensive black-box problems: evaluating one candidate architecture might be computationally expensive
 - Mixed-discrete design variables: categorical architectural decisions mixed with continuous sizing variables
 - Hierarchical design variables: decisions can deactivate/activate (parts of) downstream decisions
 - Multi-objective: stemming from conflicting stakeholder needs
 - Subject to hidden constraints: simulation tools might not converge for all design points
```

### Comparing `sb-arch-opt-1.0.0/setup.py` & `sb-arch-opt-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             'cached-property~=1.5',
             'ConfigSpace~=0.6.1',
             'more-itertools~=9.1',
         ],
         extras_require={
             'arch_sbo': [
                 'smt~=2.0b3',
+                'scikit-learn',
             ],
             # 'ota': [  # pip install -r requirements-ota.txt
             #     'open_turb_arch @ git+https://github.com/jbussemaker/OpenTurbofanArchitecting@pymoo_optional#egg=open_turb_arch',
             # ],
             # 'assignment': [  # pip install -r requirements-assignment.txt
             #     'assign_enc @ git+https://github.com/jbussemaker/AssignmentEncoding#egg=assign_enc',
             # ],
```

