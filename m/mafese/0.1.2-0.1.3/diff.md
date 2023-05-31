# Comparing `tmp/mafese-0.1.2.tar.gz` & `tmp/mafese-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafese-0.1.2.tar", last modified: Mon May 29 09:38:05 2023, max compression
+gzip compressed data, was "mafese-0.1.3.tar", last modified: Wed May 31 10:58:54 2023, max compression
```

## Comparing `mafese-0.1.2.tar` & `mafese-0.1.3.tar`

### file list

```diff
@@ -1,68 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.337797 mafese-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-29 09:37:18.000000 mafese-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 09:37:18.000000 mafese-0.1.2/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 09:37:18.000000 mafese-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 09:37:18.000000 mafese-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-05-29 09:38:05.333797 mafese-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-05-29 09:37:18.000000 mafese-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.309796 mafese-0.1.2/mafese/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.329797 mafese-0.1.2/mafese/data/
--rw-r--r--   0 runner    (1001) docker     (123)   369879 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Arrhythmia.csv
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/BreastCancer.csv
--rw-r--r--   0 runner    (1001) docker     (123)   119681 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/BreastEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/CongressEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498322 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Digits.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Exactly.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Exactly2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Glass.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/HeartEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)   438254 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Hill-valley.csv
--rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Horse.csv
--rw-r--r--   0 runner    (1001) docker     (123)    75329 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Ionosphere.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)   236504 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/KrVsKpEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Lymphography.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/M-of-n.csv
--rw-r--r--   0 runner    (1001) docker     (123)  5205194 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Madelon.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Monk1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Monk2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Monk3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/PenglungEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    85876 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Sonar.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Soybean-small.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/SpectEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Tic-tac-toe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Vote.csv
--rw-r--r--   0 runner    (1001) docker     (123)    65346 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Vowel.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1053755 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/WaveformEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Wine.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Zoo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.333797 mafese-0.1.2/mafese/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/mealpy_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.333797 mafese-0.1.2/mafese/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/wrapper/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/wrapper/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/wrapper/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.309796 mafese-0.1.2/mafese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:38:05.337797 mafese-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-29 09:37:18.000000 mafese-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.333797 mafese-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-29 09:37:18.000000 mafese-0.1.2/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-29 09:37:18.000000 mafese-0.1.2/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.615399 mafese-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-31 10:57:59.000000 mafese-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-31 10:57:59.000000 mafese-0.1.3/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 10:57:59.000000 mafese-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 10:57:59.000000 mafese-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-05-31 10:58:54.615399 mafese-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-05-31 10:57:59.000000 mafese-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.611399 mafese-0.1.3/mafese/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.611399 mafese-0.1.3/mafese/embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/embedded/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/embedded/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.615399 mafese-0.1.3/mafese/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/mealpy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.615399 mafese-0.1.3/mafese/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/wrapper/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/wrapper/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/wrapper/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.611399 mafese-0.1.3/mafese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 10:58:54.615399 mafese-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-31 10:57:59.000000 mafese-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.615399 mafese-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-31 10:57:59.000000 mafese-0.1.3/tests/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-31 10:57:59.000000 mafese-0.1.3/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-31 10:57:59.000000 mafese-0.1.3/tests/test_wrapper.py
```

### Comparing `mafese-0.1.2/CODE_OF_CONDUCT.md` & `mafese-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mafese-0.1.2/ChangeLog.md` & `mafese-0.1.3/ChangeLog.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# Version 0.1.3
+
++ Relocate regression and classification datasets
++ Add Embedded Feature Selection:
+  + Regularization methods (lasso-based)
+  + Tree-based methods
++ Update documents, examples, test
+
+---------------------------------------------------------------------
+
 
 # Version 0.1.2
 
 + Add transfer utility
 + Add mealpy_util wrapper
 + Add MhaSelector class that holds all Metaheuristic Algorithm for Feature Selector
 + Add examples, tests, docs for MhaSelector class
```

### Comparing `mafese-0.1.2/LICENSE` & `mafese-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mafese-0.1.2/PKG-INFO` & `mafese-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,14 @@
-Metadata-Version: 2.1
-Name: mafese
-Version: 0.1.2
-Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
-Home-page: https://github.com/thieu1995/mafese
-Author: Thieu
-Author-email: nguyenthieu2102@gmail.com
-License: GPLv3
-Project-URL: Documentation, https://mafese.readthedocs.io/
-Project-URL: Source Code, https://github.com/thieu1995/mafese
-Project-URL: Bug Tracker, https://github.com/thieu1995/mafese/issues
-Project-URL: Change Log, https://github.com/thieu1995/mafese/blob/master/ChangeLog.md
-Project-URL: Forum, https://t.me/+fRVCJGuGJg1mNDg1
-Keywords: engineering optimization problems,mathematical optimization,feature selection,classification problem,feature selector,dimensionality reduction,subset selection,wrapper methods,embedded methods,mutual information,correlation-based feature selection,recursive feature selection,principal component analysis,PCA,lasso regularization,ridge regularization,Genetic algorithm (GA),Particle swarm optimization (PSO),Ant colony optimization (ACO),Differential evolution (DE),Simulated annealing,Grey wolf optimizer (GWO),Whale Optimization Algorithm (WOA),confusion matrix,recall,precision,accuracy,K-Nearest Neighbors,random forest,support vector machine,pearson correlation coefficient (PCC),spearman correlation coefficient (SCC),relief,multi-objectives optimization problems,Stochastic optimization,Global optimization,Convergence analysis,Search space exploration,Local search,Computational intelligence,Robust optimization,Performance analysis,Intelligent optimization,Simulations
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: System :: Benchmark
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.2-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.3-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -66,32 +23,32 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library focused on feature selection 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total Wrapper-based (Metaheuristic Algorithms)**: > 170 methods 
-* **Total FilterSelector-based (Statistical-based)**: > 6 methods
-* **Total classification dataset**: > 20 datasets
-* **Total estimator methods**: > 3 methods
-* **Total performance metrics (as fitness)**: > 10 metrics
+* **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
+* **Total Filter-based (Statistical-based)**: > 12 methods
+* **Total Embedded-based (Tree and Lasso)**: > 10 methods
+* **Total classification dataset**: >= 30 datasets
+* **Total regression dataset**: >= 3 datasets
+* **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, matplotlib, mealpy, permetrics
 
 
-
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.2
+$ pip install mafese==0.1.3
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -108,14 +65,17 @@
         Arrhythmia.csv
         BreastCancer.csv
         ...
     wrapper/
         mha.py
         recursive.py
         sequential.py
+    embedded/
+        lasso.py
+        tree.py
     filter.py
     utils/
         correlation.py
         data_loader.py
         encoder.py
         estimator.py
         mealpy_util.py
@@ -285,23 +245,97 @@
 # Evaluate final dataset with different estimator with multiple performance metrics
 results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
 print(results)
 # {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
 ```
 
 
+Or, use Lasso-based feature selection with different estimator:
+
+```python
+from mafese.embedded.lasso import LassoSelector
+from mafese import get_dataset
+from mafese import evaluator
+from sklearn.svm import SVC
+
+
+data = get_dataset("Arrhythmia")
+data.split_train_test(test_size=0.2)
+print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
+
+# define mafese feature selection method
+feat_selector = LassoSelector(problem="classification", estimator="lasso", estimator_paras={"alpha": 0.1})
+# find all relevant features
+feat_selector.fit(data.X_train, data.y_train)
+
+# check selected features - True (or 1) is selected, False (or 0) is not selected
+print(feat_selector.selected_feature_masks)
+print(feat_selector.selected_feature_solution)
+
+# check the index of selected features
+print(feat_selector.selected_feature_indexes)
+
+# call transform() on X to filter it down to selected features
+X_train_selected = feat_selector.transform(data.X_train)
+X_test_selected = feat_selector.transform(data.X_test)
+
+# Evaluate final dataset with different estimator with multiple performance metrics
+results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
+print(results)
+# {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
+```
+
+
+Or, use Tree-based feature selection with different estimator:
+
+```python
+from mafese.embedded.tree import TreeSelector
+from mafese import get_dataset
+from mafese import evaluator
+from sklearn.svm import SVC
+
+
+data = get_dataset("Arrhythmia")
+data.split_train_test(test_size=0.2)
+print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
+
+# define mafese feature selection method
+feat_selector = TreeSelector(problem="classification", estimator="tree")
+# find all relevant features
+feat_selector.fit(data.X_train, data.y_train)
+
+# check selected features - True (or 1) is selected, False (or 0) is not selected
+print(feat_selector.selected_feature_masks)
+print(feat_selector.selected_feature_solution)
+
+# check the index of selected features
+print(feat_selector.selected_feature_indexes)
+
+# call transform() on X to filter it down to selected features
+X_train_selected = feat_selector.transform(data.X_train)
+X_test_selected = feat_selector.transform(data.X_test)
+
+# Evaluate final dataset with different estimator with multiple performance metrics
+results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
+print(results)
+# {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
+```
+
+
 
 For more usage examples please look at [examples](/examples) folder.
 
 ### Shortcut 
 To call the class
 
 ```code 
 from mafese import Data, get_dataset
-from mafese import SequentialSelector, RecursiveSelector, FilterSelector, MhaSelector
+from mafese import FilterSelector
+from mafese import SequentialSelector, RecursiveSelector, MhaSelector
+from mafese import LassoSelector, TreeSelector
 ```
 
 
 # Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/mafese
 * Official document: https://mafese.readthedocs.io/
```

### Comparing `mafese-0.1.2/README.md` & `mafese-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,57 @@
+Metadata-Version: 2.1
+Name: mafese
+Version: 0.1.3
+Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
+Home-page: https://github.com/thieu1995/mafese
+Author: Thieu
+Author-email: nguyenthieu2102@gmail.com
+License: GPLv3
+Project-URL: Documentation, https://mafese.readthedocs.io/
+Project-URL: Source Code, https://github.com/thieu1995/mafese
+Project-URL: Bug Tracker, https://github.com/thieu1995/mafese/issues
+Project-URL: Change Log, https://github.com/thieu1995/mafese/blob/master/ChangeLog.md
+Project-URL: Forum, https://t.me/+fRVCJGuGJg1mNDg1
+Keywords: engineering optimization problems,mathematical optimization,feature selection,classification problem,feature selector,dimensionality reduction,subset selection,wrapper methods,embedded methods,mutual information,correlation-based feature selection,recursive feature selection,principal component analysis,PCA,lasso regularization,ridge regularization,Genetic algorithm (GA),Particle swarm optimization (PSO),Ant colony optimization (ACO),Differential evolution (DE),Simulated annealing,Grey wolf optimizer (GWO),Whale Optimization Algorithm (WOA),confusion matrix,recall,precision,accuracy,K-Nearest Neighbors,random forest,support vector machine,pearson correlation coefficient (PCC),spearman correlation coefficient (SCC),relief,multi-objectives optimization problems,Stochastic optimization,Global optimization,Convergence analysis,Search space exploration,Local search,Computational intelligence,Robust optimization,Performance analysis,Intelligent optimization,Simulations
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Benchmark
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.2-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.3-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -23,32 +66,32 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library focused on feature selection 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total Wrapper-based (Metaheuristic Algorithms)**: > 170 methods 
-* **Total FilterSelector-based (Statistical-based)**: > 6 methods
-* **Total classification dataset**: > 20 datasets
-* **Total estimator methods**: > 3 methods
-* **Total performance metrics (as fitness)**: > 10 metrics
+* **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
+* **Total Filter-based (Statistical-based)**: > 12 methods
+* **Total Embedded-based (Tree and Lasso)**: > 10 methods
+* **Total classification dataset**: >= 30 datasets
+* **Total regression dataset**: >= 3 datasets
+* **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, matplotlib, mealpy, permetrics
 
 
-
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.2
+$ pip install mafese==0.1.3
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -65,14 +108,17 @@
         Arrhythmia.csv
         BreastCancer.csv
         ...
     wrapper/
         mha.py
         recursive.py
         sequential.py
+    embedded/
+        lasso.py
+        tree.py
     filter.py
     utils/
         correlation.py
         data_loader.py
         encoder.py
         estimator.py
         mealpy_util.py
@@ -242,23 +288,97 @@
 # Evaluate final dataset with different estimator with multiple performance metrics
 results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
 print(results)
 # {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
 ```
 
 
+Or, use Lasso-based feature selection with different estimator:
+
+```python
+from mafese.embedded.lasso import LassoSelector
+from mafese import get_dataset
+from mafese import evaluator
+from sklearn.svm import SVC
+
+
+data = get_dataset("Arrhythmia")
+data.split_train_test(test_size=0.2)
+print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
+
+# define mafese feature selection method
+feat_selector = LassoSelector(problem="classification", estimator="lasso", estimator_paras={"alpha": 0.1})
+# find all relevant features
+feat_selector.fit(data.X_train, data.y_train)
+
+# check selected features - True (or 1) is selected, False (or 0) is not selected
+print(feat_selector.selected_feature_masks)
+print(feat_selector.selected_feature_solution)
+
+# check the index of selected features
+print(feat_selector.selected_feature_indexes)
+
+# call transform() on X to filter it down to selected features
+X_train_selected = feat_selector.transform(data.X_train)
+X_test_selected = feat_selector.transform(data.X_test)
+
+# Evaluate final dataset with different estimator with multiple performance metrics
+results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
+print(results)
+# {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
+```
+
+
+Or, use Tree-based feature selection with different estimator:
+
+```python
+from mafese.embedded.tree import TreeSelector
+from mafese import get_dataset
+from mafese import evaluator
+from sklearn.svm import SVC
+
+
+data = get_dataset("Arrhythmia")
+data.split_train_test(test_size=0.2)
+print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
+
+# define mafese feature selection method
+feat_selector = TreeSelector(problem="classification", estimator="tree")
+# find all relevant features
+feat_selector.fit(data.X_train, data.y_train)
+
+# check selected features - True (or 1) is selected, False (or 0) is not selected
+print(feat_selector.selected_feature_masks)
+print(feat_selector.selected_feature_solution)
+
+# check the index of selected features
+print(feat_selector.selected_feature_indexes)
+
+# call transform() on X to filter it down to selected features
+X_train_selected = feat_selector.transform(data.X_train)
+X_test_selected = feat_selector.transform(data.X_test)
+
+# Evaluate final dataset with different estimator with multiple performance metrics
+results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
+print(results)
+# {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
+```
+
+
 
 For more usage examples please look at [examples](/examples) folder.
 
 ### Shortcut 
 To call the class
 
 ```code 
 from mafese import Data, get_dataset
-from mafese import SequentialSelector, RecursiveSelector, FilterSelector, MhaSelector
+from mafese import FilterSelector
+from mafese import SequentialSelector, RecursiveSelector, MhaSelector
+from mafese import LassoSelector, TreeSelector
 ```
 
 
 # Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/mafese
 * Official document: https://mafese.readthedocs.io/
```

### Comparing `mafese-0.1.2/mafese/evaluator.py` & `mafese-0.1.3/mafese/evaluator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.2/mafese/filter.py` & `mafese-0.1.3/mafese/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,24 +50,24 @@
 
     supported_methods: dict
         Key: is the support method name
         Value: is the support method function
 
     Examples
     --------
-    The following example shows how to retrieve the 5 most informative features in the FilterSelector FS method
+    The following example shows how to retrieve the most informative features in the FilterSelector FS method
 
     >>> import pandas as pd
     >>> from mafese.filter import FilterSelector
     >>> # load dataset
     >>> dataset = pd.read_csv('your_path/dataset.csv', index_col=0).values
     >>> X, y = dataset[:, 0:-1], dataset[:, -1]     # Assumption that the last column is label column
     >>> # define mafese feature selection method
     >>> feat_selector = FilterSelector(problem='classification', method='SPEARMAN', n_features=5)
-    >>> # find all relevant features - 5 features should be selected
+    >>> # find all relevant features
     >>> feat_selector.fit(X, y)
     >>> # check selected features - True (or 1) is selected, False (or 0) is not selected
     >>> print(feat_selector.selected_feature_masks)
     array([ True, True, True, False, False, True, False, False, False, True])
     >>> print(feat_selector.selected_feature_solution)
     array([ 1, 1, 1, 0, 0, 1, 0, 0, 0, 1])
     >>> # check the index of selected features
```

### Comparing `mafese-0.1.2/mafese/selector.py` & `mafese-0.1.3/mafese/selector.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.2/mafese/utils/correlation.py` & `mafese-0.1.3/mafese/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.2/mafese/utils/data_loader.py` & `mafese-0.1.3/mafese/utils/data_loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,44 +7,91 @@
 import pandas as pd
 import numpy as np
 from pathlib import Path
 from sklearn.model_selection import train_test_split
 
 
 class Data:
-    #  structure for the data (not dataset)
+    """
+    The structure of our supported Data class
+
+    Parameters
+    ----------
+    X : np.ndarray
+        The features of your data
+
+    y : np.ndarray
+        The labels of your data
+    """
     def __init__(self, X, y):
         self.X = X
         self.y = y
         self.X_train, self.y_train, self.X_test, self.y_test = None, None, None, None
 
     def split_train_test(self, test_size=0.2, train_size=None,
                          random_state=41, shuffle=True, stratify=None, inplace=True):
+        """
+        The wrapper of the split_train_test function in scikit-learn library.
+        """
         self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self.X, self.y, test_size=test_size,
                         train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=stratify)
         if not inplace:
             return self.X_train, self.X_test, self.y_train, self.y_test
 
     def set_train_test(self, X_train=None, y_train=None, X_test=None, y_test=None):
+        """
+        Function use to set your own X_train, y_train, X_test, y_test in case you don't want to use our split function
+
+        Parameters
+        ----------
+        X_train : np.ndarray
+        y_train : np.ndarray
+        X_test : np.ndarray
+        y_test : np.ndarray
+        """
         self.X_train = X_train
         self.y_train = y_train
         self.X_test = X_test
         self.y_test = y_test
 
 
 def get_dataset(dataset_name):
-    # function to retrieve the data
+    """
+    Helper function to retrieve the data
+
+    Parameters
+    ----------
+    dataset_name : str
+        Name of the dataset
+
+    Returns
+    -------
+    data: Data
+        The instance of Data class, that hold X and y variables.
+    """
     dir_root = f"{Path(__file__).parent.parent.__str__()}/data"
-    list_paths = Path(dir_root).glob("*.csv")
-    list_datasets = [pathfile.name[:-4] for pathfile in list_paths]
+    list_path_reg = Path(f"{dir_root}/reg").glob("*.csv")
+    list_path_cls = Path(f"{dir_root}/cls").glob("*.csv")
+    reg_list = [pf.name[:-4] for pf in list_path_reg]
+    cls_list = [pf.name[:-4] for pf in list_path_cls]
+    list_datasets = reg_list + cls_list
 
     if dataset_name not in list_datasets:
         print(f"MAFESE currently does not have '{dataset_name}' data in its database....")
         display = input("Enter 1 to see the available datasets: ") or 0
         if display:
-            for idx, dataset in enumerate(list_datasets):
-                print(f"{idx + 1}: {dataset}")
+            print("+ For classification problem. We support datasets:")
+            for idx, dataset in enumerate(cls_list):
+                print(f"\t{idx + 1}: {dataset}")
+            print("+ For regression problem. We support datasets:")
+            for idx, dataset in enumerate(reg_list):
+                print(f"\t{idx + 1}: {dataset}")
     else:
-        df = pd.read_csv(f"{dir_root}/{dataset_name}.csv", header=None)
+        if dataset_name in reg_list:
+            df = pd.read_csv(f"{dir_root}/reg/{dataset_name}.csv", header=None)
+            data_type = "REGRESSION"
+        else:
+            df = pd.read_csv(f"{dir_root}/cls/{dataset_name}.csv", header=None)
+            data_type = "CLASSIFICATION"
         data = Data(np.array(df.iloc[:, 0:-1]), np.array(df.iloc[:, -1]))
-        print(f"Requested dataset: {dataset_name} found and loaded...")
+        print(f"Requested {data_type} dataset: {dataset_name} found and loaded!")
         return data
```

### Comparing `mafese-0.1.2/mafese/utils/encoder.py` & `mafese-0.1.3/mafese/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.2/mafese/utils/estimator.py` & `mafese-0.1.3/mafese/utils/estimator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:43, 24/05/2023 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-from sklearn.svm import SVC, SVR
+from sklearn.svm import SVC, SVR, LinearSVC
 from sklearn.neighbors import KNeighborsClassifier, KNeighborsRegressor
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
+from sklearn.linear_model import Lasso, LogisticRegression, LinearRegression
 
 
 def get_classifier(name):
     name = name.lower()
     if name == 'knn':
         return KNeighborsClassifier()
     elif name == 'rf':
@@ -47,7 +48,60 @@
     name = name.lower()
     if name == "rf":
         return RandomForestRegressor()
     elif name == "svm":
         return SVR(kernel="linear")
     else:
         raise ValueError(f"Currently, we don't support: {name} regressor. You can define your own scikit-learn model.")
+
+
+def get_lasso_based_estimator(problem, name, paras=None):
+    if paras is None:
+        paras = {}
+    name = name.lower()
+    if problem == "regression":
+        if name == "lasso":
+            return Lasso(**paras)
+        else:
+            raise ValueError(f"For Regression problem, lasso-based method only supports 'lasso' estimator.")
+    else:
+        if name == "lasso":
+            return Lasso(**paras)
+        elif name == "lr":
+            est = LogisticRegression(**paras)
+            est.set_params(**{"penalty": "l1", "solver": "liblinear"})
+            return est
+        elif name == "svm":
+            return LinearSVC(**paras)
+        else:
+            raise ValueError(f"For Classification problem, lasso-based method supports: 'lasso', 'lr', and 'svm' estimator.")
+
+
+def get_tree_based_estimator(problem, name, paras=None):
+    from sklearn.ensemble import ExtraTreesRegressor, RandomForestRegressor, AdaBoostRegressor, GradientBoostingRegressor
+    from sklearn.ensemble import ExtraTreesClassifier, RandomForestClassifier, AdaBoostClassifier, GradientBoostingClassifier
+
+    if paras is None:
+        paras = {}
+    name = name.lower()
+    if problem == "regression":
+        if name == "rf":
+            return RandomForestRegressor(**paras)
+        elif name == "adaboost":
+            return AdaBoostRegressor(**paras)
+        elif name == "xgb":
+            return GradientBoostingRegressor(**paras)
+        elif name == "tree":
+            return ExtraTreesRegressor(**paras)
+        else:
+            raise ValueError(f"For Regression problem, we don't support {name} estimator.")
+    else:
+        if name == "rf":
+            return RandomForestClassifier(**paras)
+        elif name == "adaboost":
+            return AdaBoostClassifier(**paras)
+        elif name == "xgb":
+            return GradientBoostingClassifier(**paras)
+        elif name == "tree":
+            return ExtraTreesClassifier(**paras)
+        else:
+            raise ValueError(f"For Classification problem, we don't support {name} estimator.")
```

### Comparing `mafese-0.1.2/mafese/utils/mealpy_util.py` & `mafese-0.1.3/mafese/utils/mealpy_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.name = name
         super().__init__(lb, ub, minmax, **kwargs)
 
     def amend_position(self, position=None, lb=None, ub=None):
         position = self.transfer_func(position)
         cons = np.random.uniform(0, 1, len(position))
         x = np.where(cons < position, 1, 0)
-        if np.all((x == 0)):
+        if np.sum(x) == 0:
             x[np.random.randint(0, len(x))] = 1
         return x
 
     def fit_func(self, solution):
         cols = np.flatnonzero(solution)
         self.estimator.fit(self.data.X_train[:, cols], self.data.y_train)
         y_valid_pred = self.estimator.predict(self.data.X_test[:, cols])
```

### Comparing `mafese-0.1.2/mafese/utils/transfer.py` & `mafese-0.1.3/mafese/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.2/mafese/utils/validator.py` & `mafese-0.1.3/mafese/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.2/mafese/wrapper/mha.py` & `mafese-0.1.3/mafese/wrapper/mha.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         The name of objective for the problem, also depend on the problem is classification and regression.
 
         - If problem is classification, `None` will be replaced by AS (Accuracy score).
         - If problem is regression, `None` will be replaced by MSE (Mean squared error).
 
     Examples
     --------
-    The following example shows how to retrieve the 5 most informative features in the MhaSelector FS method
+    The following example shows how to retrieve the most informative features in the MhaSelector FS method
 
     >>> import pandas as pd
     >>> from mafese.wrapper.mha import MhaSelector
     >>> # load dataset
     >>> dataset = pd.read_csv('your_path/dataset.csv', index_col=0).values
     >>> X, y = dataset[:, 0:-1], dataset[:, -1]     # Assumption that the last column is label column
     >>> # define mafese feature selection method
```

### Comparing `mafese-0.1.2/mafese/wrapper/recursive.py` & `mafese-0.1.3/mafese/wrapper/recursive.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,24 +48,24 @@
         `named_steps.clf.feature_importances_` in case of class:`~sklearn.pipeline.Pipeline` with its last step named `clf`.
 
         If `callable`, overrides the default feature importance getter.
         The callable is passed with the fitted estimator and it should return importance for each feature.
 
     Examples
     --------
-    The following example shows how to retrieve the 5 most informative features in the RecursiveSelector FS method
+    The following example shows how to retrieve the most informative features in the RecursiveSelector FS method
 
     >>> import pandas as pd
     >>> from mafese.wrapper.recursive import RecursiveSelector
     >>> # load dataset
     >>> dataset = pd.read_csv('your_path/dataset.csv', index_col=0).values
     >>> X, y = dataset[:, 0:-1], dataset[:, -1]     # Assumption that the last column is label column
     >>> # define mafese feature selection method
     >>> feat_selector = RecursiveSelector(problem="classification", estimator="rf", n_features=5)
-    >>> # find all relevant features - 5 features should be selected
+    >>> # find all relevant features
     >>> feat_selector.fit(X, y)
     >>> # check selected features - True (or 1) is selected, False (or 0) is not selected
     >>> print(feat_selector.selected_feature_masks)
     array([ True, True, True, False, False, True, False, False, False, True])
     >>> print(feat_selector.selected_feature_solution)
     array([ 1, 1, 1, 0, 0, 1, 0, 0, 0, 1])
     >>> # check the index of selected features
```

### Comparing `mafese-0.1.2/mafese/wrapper/sequential.py` & `mafese-0.1.3/mafese/wrapper/sequential.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,24 +62,24 @@
     n_jobs : int, default=None
         Number of jobs to run in parallel. When evaluating a new feature to add or remove, the cross-validation
         procedure is parallel over the folds.
         ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context. ``-1`` means using all processors.
 
     Examples
     --------
-    The following example shows how to retrieve the 5 most informative features in the Forward FS method
+    The following example shows how to retrieve the most informative features in the Sequential-based (forward, backward) FS method
 
     >>> import pandas as pd
     >>> from mafese.wrapper.sequential import SequentialSelector
     >>> # load dataset
     >>> dataset = pd.read_csv('your_path/dataset.csv', index_col=0).values
     >>> X, y = dataset[:, 0:-1], dataset[:, -1]     # Assumption that the last column is label column
     >>> # define mafese feature selection method
     >>> feat_selector = SequentialSelector(problem="classification", estimator="knn", n_features=5, direction="forward")
-    >>> # find all relevant features - 5 features should be selected
+    >>> # find all relevant features
     >>> feat_selector.fit(X, y)
     >>> # check selected features - True (or 1) is selected, False (or 0) is not selected
     >>> print(feat_selector.selected_feature_masks)
     array([ True, True, True, False, False, True, False, False, False, True])
     >>> print(feat_selector.selected_feature_solution)
     array([ 1, 1, 1, 0, 0, 1, 0, 0, 0, 1])
     >>> # check the index of selected features
```

### Comparing `mafese-0.1.2/mafese.egg-info/PKG-INFO` & `mafese-0.1.3/mafese.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.2
+Version: 0.1.3
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -43,15 +43,15 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.2-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.3-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -66,32 +66,32 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library focused on feature selection 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total Wrapper-based (Metaheuristic Algorithms)**: > 170 methods 
-* **Total FilterSelector-based (Statistical-based)**: > 6 methods
-* **Total classification dataset**: > 20 datasets
-* **Total estimator methods**: > 3 methods
-* **Total performance metrics (as fitness)**: > 10 metrics
+* **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
+* **Total Filter-based (Statistical-based)**: > 12 methods
+* **Total Embedded-based (Tree and Lasso)**: > 10 methods
+* **Total classification dataset**: >= 30 datasets
+* **Total regression dataset**: >= 3 datasets
+* **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, matplotlib, mealpy, permetrics
 
 
-
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.2
+$ pip install mafese==0.1.3
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -108,14 +108,17 @@
         Arrhythmia.csv
         BreastCancer.csv
         ...
     wrapper/
         mha.py
         recursive.py
         sequential.py
+    embedded/
+        lasso.py
+        tree.py
     filter.py
     utils/
         correlation.py
         data_loader.py
         encoder.py
         estimator.py
         mealpy_util.py
@@ -285,23 +288,97 @@
 # Evaluate final dataset with different estimator with multiple performance metrics
 results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
 print(results)
 # {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
 ```
 
 
+Or, use Lasso-based feature selection with different estimator:
+
+```python
+from mafese.embedded.lasso import LassoSelector
+from mafese import get_dataset
+from mafese import evaluator
+from sklearn.svm import SVC
+
+
+data = get_dataset("Arrhythmia")
+data.split_train_test(test_size=0.2)
+print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
+
+# define mafese feature selection method
+feat_selector = LassoSelector(problem="classification", estimator="lasso", estimator_paras={"alpha": 0.1})
+# find all relevant features
+feat_selector.fit(data.X_train, data.y_train)
+
+# check selected features - True (or 1) is selected, False (or 0) is not selected
+print(feat_selector.selected_feature_masks)
+print(feat_selector.selected_feature_solution)
+
+# check the index of selected features
+print(feat_selector.selected_feature_indexes)
+
+# call transform() on X to filter it down to selected features
+X_train_selected = feat_selector.transform(data.X_train)
+X_test_selected = feat_selector.transform(data.X_test)
+
+# Evaluate final dataset with different estimator with multiple performance metrics
+results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
+print(results)
+# {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
+```
+
+
+Or, use Tree-based feature selection with different estimator:
+
+```python
+from mafese.embedded.tree import TreeSelector
+from mafese import get_dataset
+from mafese import evaluator
+from sklearn.svm import SVC
+
+
+data = get_dataset("Arrhythmia")
+data.split_train_test(test_size=0.2)
+print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
+
+# define mafese feature selection method
+feat_selector = TreeSelector(problem="classification", estimator="tree")
+# find all relevant features
+feat_selector.fit(data.X_train, data.y_train)
+
+# check selected features - True (or 1) is selected, False (or 0) is not selected
+print(feat_selector.selected_feature_masks)
+print(feat_selector.selected_feature_solution)
+
+# check the index of selected features
+print(feat_selector.selected_feature_indexes)
+
+# call transform() on X to filter it down to selected features
+X_train_selected = feat_selector.transform(data.X_train)
+X_test_selected = feat_selector.transform(data.X_test)
+
+# Evaluate final dataset with different estimator with multiple performance metrics
+results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
+print(results)
+# {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
+```
+
+
 
 For more usage examples please look at [examples](/examples) folder.
 
 ### Shortcut 
 To call the class
 
 ```code 
 from mafese import Data, get_dataset
-from mafese import SequentialSelector, RecursiveSelector, FilterSelector, MhaSelector
+from mafese import FilterSelector
+from mafese import SequentialSelector, RecursiveSelector, MhaSelector
+from mafese import LassoSelector, TreeSelector
 ```
 
 
 # Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/mafese
 * Official document: https://mafese.readthedocs.io/
```

### Comparing `mafese-0.1.2/setup.py` & `mafese-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mafese",
-    version="0.1.2",
+    version="0.1.3",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["engineering optimization problems", "mathematical optimization",
               "feature selection", "classification problem",
```

### Comparing `mafese-0.1.2/tests/test_filter.py` & `mafese-0.1.3/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.2/tests/test_wrapper.py` & `mafese-0.1.3/tests/test_embedded.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 14:15, 25/05/2023 ----------%                                                                               
+# Created by "Thieu" at 17:18, 31/05/2023 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
-from mafese.wrapper.sequential import SequentialSelector
-from mafese.wrapper.recursive import RecursiveSelector
+from mafese.embedded.lasso import LassoSelector
+from mafese.embedded.tree import TreeSelector
 
 np.random.seed(42)
 
 
-def test_Sequential_class():
+def test_LassoSelector_class():
     X = np.random.rand(10, 6)
     y = np.random.randint(0, 2, size=10)
-    n_features = 3
-    feat_selector = SequentialSelector(problem="regression", estimator="knn", n_features=n_features, direction="forward")
+    feat_selector = LassoSelector(problem="classification", estimator="lasso", estimator_paras={"alpha": 0.1})
     feat_selector.fit(X, y)
     X_selected = feat_selector.transform(X)
-    assert X_selected.shape[1] == n_features
-    assert len(feat_selector.selected_feature_indexes) == n_features
+    assert X_selected.shape[1] == len(feat_selector.selected_feature_indexes)
 
 
-def test_Recursive_class():
+def test_TreeSelector_class():
     X = np.random.rand(10, 6)
     y = np.random.randint(0, 2, size=10)
-    n_features = 3
-    feat_selector = RecursiveSelector(problem="classification", estimator="rf", n_features=3)
+    feat_selector = TreeSelector(problem="classification", estimator="tree")
     feat_selector.fit(X, y)
     X_selected = feat_selector.transform(X)
-    assert X_selected.shape[1] == n_features
-    assert len(feat_selector.selected_feature_indexes) == n_features
+    assert X_selected.shape[1] == len(feat_selector.selected_feature_indexes)
```

