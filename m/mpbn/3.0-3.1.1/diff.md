# Comparing `tmp/mpbn-3.0.tar.gz` & `tmp/mpbn-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpbn-3.0.tar", last modified: Thu May 25 22:04:40 2023, max compression
+gzip compressed data, was "mpbn-3.1.1.tar", last modified: Wed May 31 08:30:48 2023, max compression
```

## Comparing `mpbn-3.0.tar` & `mpbn-3.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 22:04:29.000000 mpbn-3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-25 22:04:40.905704 mpbn-3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-25 22:04:29.000000 mpbn-3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/mpbn/
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/mpbn/asplib/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/asplib/mp_attractor.asp
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/asplib/mp_eval.asp
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/asplib/mp_positivereach-np.asp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/mpbn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/cli/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-25 22:04:29.000000 mpbn-3.0/mpbn/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:04:40.905704 mpbn-3.0/mpbn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 22:04:40.000000 mpbn-3.0/mpbn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 22:04:40.905704 mpbn-3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-25 22:04:29.000000 mpbn-3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 08:30:35.000000 mpbn-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-31 08:30:48.399645 mpbn-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 08:30:35.000000 mpbn-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/mpbn/
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/mpbn/asplib/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/asplib/mp_attractor.asp
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/asplib/mp_eval.asp
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/asplib/mp_positivereach-np.asp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/mpbn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/cli/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/mpbn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:30:48.399645 mpbn-3.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-05-31 08:30:35.000000 mpbn-3.1.1/setup.py
```

### Comparing `mpbn-3.0/PKG-INFO` & `mpbn-3.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbn
-Version: 3.0
+Version: 3.1.1
 Summary: Simple implementation of Most Permissive Boolean networks
 Home-page: https://github.com/bnediction/mpbn
 Author: Loïc Paulevé
 Author-email: loic.pauleve@labri.fr
 License: CeCILL
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mpbn-3.0/README.md` & `mpbn-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mpbn-3.0/mpbn/__init__.py` & `mpbn-3.1.1/mpbn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,23 @@
 >>> mbn.reachability({'a': 0, 'b': 0, 'c': 0}, {'a': 1, 'b': 1, 'c': 1})
 True
 >>> list(mbn.attractors(reachable_from={'a': 0, 'b': 1, 'c': 0}))
 [{'a': 0, 'b': 1, 'c': 1}]
 """
 
 import os
+import sys
 from colomoto import minibn
 
 from boolean import boolean
 import clingo
 
 from pyeda.boolalg import bdd
 from pyeda.boolalg.expr import expr
+sys.setrecursionlimit(max(100000, sys.getrecursionlimit()))
 
 __asplibdir__ = os.path.realpath(os.path.join(os.path.dirname(__file__), "asplib"))
 
 clingo_options = ["-W", "no-atom-undefined"]
 if hasattr(clingo, "version") and clingo.version() >= (5,5,0):
     clingo_options.append("--single-shot")
```

### Comparing `mpbn-3.0/mpbn/asplib/mp_eval.asp` & `mpbn-3.1.1/mpbn/asplib/mp_eval.asp`

 * *Files identical despite different names*

### Comparing `mpbn-3.0/mpbn/cli/__init__.py` & `mpbn-3.1.1/mpbn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.0/mpbn/cli/sim.py` & `mpbn-3.1.1/mpbn/cli/sim.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.0/mpbn/simulation.py` & `mpbn-3.1.1/mpbn/simulation.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.0/mpbn.egg-info/PKG-INFO` & `mpbn-3.1.1/mpbn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbn
-Version: 3.0
+Version: 3.1.1
 Summary: Simple implementation of Most Permissive Boolean networks
 Home-page: https://github.com/bnediction/mpbn
 Author: Loïc Paulevé
 Author-email: loic.pauleve@labri.fr
 License: CeCILL
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mpbn-3.0/setup.py` & `mpbn-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8
 
 from setuptools import setup, find_packages
 
 NAME = "mpbn"
-VERSION = "3.0"
+VERSION = "3.1.1"
 
 setup(name=NAME,
     version=VERSION,
     author="Loïc Paulevé",
     author_email="loic.pauleve@labri.fr",
     url="https://github.com/bnediction/mpbn",
     license="CeCILL",
```

