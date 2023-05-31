# Comparing `tmp/mpbn-3.1.1.tar.gz` & `tmp/mpbn-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpbn-3.1.1.tar", last modified: Wed May 31 08:30:48 2023, max compression
+gzip compressed data, was "mpbn-3.2.tar", last modified: Wed May 31 14:14:22 2023, max compression
```

## Comparing `mpbn-3.1.1.tar` & `mpbn-3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 08:30:35.000000 mpbn-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-31 08:30:48.399645 mpbn-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 08:30:35.000000 mpbn-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/mpbn/
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/mpbn/asplib/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/asplib/mp_attractor.asp
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/asplib/mp_eval.asp
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/asplib/mp_positivereach-np.asp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/mpbn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/cli/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-31 08:30:35.000000 mpbn-3.1.1/mpbn/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:48.399645 mpbn-3.1.1/mpbn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 08:30:48.000000 mpbn-3.1.1/mpbn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:30:48.399645 mpbn-3.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-05-31 08:30:35.000000 mpbn-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:14:22.897334 mpbn-3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 14:14:07.000000 mpbn-3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-31 14:14:22.897334 mpbn-3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 14:14:07.000000 mpbn-3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:14:22.893334 mpbn-3.2/mpbn/
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-05-31 14:14:07.000000 mpbn-3.2/mpbn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:14:22.897334 mpbn-3.2/mpbn/asplib/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-31 14:14:07.000000 mpbn-3.2/mpbn/asplib/mp_attractor.asp
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 14:14:07.000000 mpbn-3.2/mpbn/asplib/mp_eval.asp
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-31 14:14:07.000000 mpbn-3.2/mpbn/asplib/mp_positivereach-np.asp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:14:22.897334 mpbn-3.2/mpbn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 14:14:07.000000 mpbn-3.2/mpbn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-31 14:14:07.000000 mpbn-3.2/mpbn/cli/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-31 14:14:07.000000 mpbn-3.2/mpbn/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:14:22.897334 mpbn-3.2/mpbn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-31 14:14:22.000000 mpbn-3.2/mpbn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-31 14:14:22.000000 mpbn-3.2/mpbn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:14:22.000000 mpbn-3.2/mpbn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 14:14:22.000000 mpbn-3.2/mpbn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 14:14:22.000000 mpbn-3.2/mpbn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 14:14:22.000000 mpbn-3.2/mpbn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:14:22.897334 mpbn-3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-31 14:14:07.000000 mpbn-3.2/setup.py
```

### Comparing `mpbn-3.1.1/PKG-INFO` & `mpbn-3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbn
-Version: 3.1.1
+Version: 3.2
 Summary: Simple implementation of Most Permissive Boolean networks
 Home-page: https://github.com/bnediction/mpbn
 Author: Loïc Paulevé
 Author-email: loic.pauleve@labri.fr
 License: CeCILL
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mpbn-3.1.1/README.md` & `mpbn-3.2/README.md`

 * *Files identical despite different names*

### Comparing `mpbn-3.1.1/mpbn/__init__.py` & `mpbn-3.2/mpbn/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import sys
 from colomoto import minibn
 
 from boolean import boolean
 import clingo
 
 from pyeda.boolalg import bdd
+import pyeda.boolalg.expr
 from pyeda.boolalg.expr import expr
 sys.setrecursionlimit(max(100000, sys.getrecursionlimit()))
 
 __asplibdir__ = os.path.realpath(os.path.join(os.path.dirname(__file__), "asplib"))
 
 clingo_options = ["-W", "no-atom-undefined"]
 if hasattr(clingo, "version") and clingo.version() >= (5,5,0):
@@ -133,14 +134,34 @@
 
 def bddasp_of_boolfunc(f, i):
     e = expr(str(f).replace("!","~"))
     b = bdd.expr2bdd(e)
     atoms = asp_of_bdd(i, b)
     return "\n".join((f"{a}." for a in atoms))
 
+def expr2bpy(ex, ba):
+    """
+    converts a pyeda Boolean expression into a boolean.py one
+    """
+    if isinstance(ex, pyeda.boolalg.expr.Variable):
+        return ba.Symbol(str(ex))
+    elif isinstance(ex, pyeda.boolalg.expr._One):
+        return ba.TRUE
+    elif isinstance(ex, pyeda.boolalg.expr._Zero):
+        return ba.FALSE
+    elif isinstance(ex, pyeda.boolalg.expr.Complement):
+        return ba.NOT(ba.Symbol(str(ex.__invert__())))
+    elif isinstance(ex, pyeda.boolalg.expr.NotOp):
+        return ba.NOT(expr2bpy(ex.x, ba))
+    elif isinstance(ex, pyeda.boolalg.expr.OrOp):
+        return ba.OR(*(expr2bpy(x, ba) for x in ex.xs))
+    elif isinstance(ex, pyeda.boolalg.expr.AndOp):
+        return ba.AND(*(expr2bpy(x, ba) for x in ex.xs))
+    raise NotImplementedError(str(ex), type(ex))
+
 class MPBooleanNetwork(minibn.BooleanNetwork):
     """
     Most Permissive Boolean Network
 
     Extends ``colomoto.minibn.BooleanNetwork`` class by adding methods for
     computing reachable and attractor properties with the Most Permissive
     semantics.
@@ -148,15 +169,15 @@
 
     Ensures that the Boolean functions are monotonic and in disjunctive normal
     form (DNF).
     The local-monotonic checking requires that a literal never appears
     with both signs in a same Boolean function.
     """
     def __init__(self, bn=minibn.BooleanNetwork(), auto_dnf=True,
-                        try_unate_hard=True,
+                        try_unate_hard=False,
                         encoding="auto"):
         """
         Constructor for :py:class:`.MPBoooleanNetwork`.
 
         :param bn: Boolean network to copy from
         :type bn: :py:class:`colomoto.minibn.BooleanNetwork` or any type accepted by
             :py:class:`colomoto.minibn.BooleanNetwork` constructor
@@ -183,15 +204,18 @@
         Unless :py:attr:`.auto_dnf` is ``False``, ``f`` is converted into DNF
         form first.
         """
         if isinstance(f, str):
             f = self.ba.parse(f)
         f = self._autobool(f)
         if self.auto_dnf:
-            f = self.ba.dnf(f).simplify()
+            e = expr(str(f).replace("!","~"))
+            e = e.to_dnf()
+            e = e.simplify()
+            f = expr2bpy(e, self.ba)
             if self.try_unate_hard:
                 f = minibn.simplify_dnf(self.ba, f)
         a = self._autokey(a)
         if self.encoding != "bdd":
             self._is_unate[a] = is_unate(self.ba, f)
             if self.encoding == "unate-dnf":
                 assert self._is_unate[a], f"'{f}' seems not unate. Try simplify()?"
```

### Comparing `mpbn-3.1.1/mpbn/asplib/mp_eval.asp` & `mpbn-3.2/mpbn/asplib/mp_eval.asp`

 * *Files identical despite different names*

### Comparing `mpbn-3.1.1/mpbn/cli/__init__.py` & `mpbn-3.2/mpbn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.1.1/mpbn/cli/sim.py` & `mpbn-3.2/mpbn/cli/sim.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.1.1/mpbn/simulation.py` & `mpbn-3.2/mpbn/simulation.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.1.1/mpbn.egg-info/PKG-INFO` & `mpbn-3.2/mpbn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbn
-Version: 3.1.1
+Version: 3.2
 Summary: Simple implementation of Most Permissive Boolean networks
 Home-page: https://github.com/bnediction/mpbn
 Author: Loïc Paulevé
 Author-email: loic.pauleve@labri.fr
 License: CeCILL
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mpbn-3.1.1/setup.py` & `mpbn-3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8
 
 from setuptools import setup, find_packages
 
 NAME = "mpbn"
-VERSION = "3.1.1"
+VERSION = "3.2"
 
 setup(name=NAME,
     version=VERSION,
     author="Loïc Paulevé",
     author_email="loic.pauleve@labri.fr",
     url="https://github.com/bnediction/mpbn",
     license="CeCILL",
```

