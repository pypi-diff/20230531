# Comparing `tmp/exma-0.5.8.tar.gz` & `tmp/exma-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exma-0.5.8.tar", last modified: Fri Nov  4 18:58:43 2022, max compression
+gzip compressed data, was "exma-0.5.9.tar", last modified: Tue Jan 24 12:47:37 2023, max compression
```

## Comparing `exma-0.5.8.tar` & `exma-0.5.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:58:43.785877 exma-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-11-04 18:58:30.000000 exma-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-04 18:58:30.000000 exma-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-11-04 18:58:43.785877 exma-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-11-04 18:58:30.000000 exma-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:58:43.781877 exma-0.5.8/exma/
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-11-04 18:58:30.000000 exma-0.5.8/exma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8973 2022-11-04 18:58:30.000000 exma-0.5.8/exma/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-11-04 18:58:30.000000 exma-0.5.8/exma/cn.py
--rw-r--r--   0 runner    (1001) docker     (121)     8580 2022-11-04 18:58:30.000000 exma-0.5.8/exma/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3967 2022-11-04 18:58:30.000000 exma-0.5.8/exma/distances.py
--rw-r--r--   0 runner    (1001) docker     (121)     7870 2022-11-04 18:58:30.000000 exma-0.5.8/exma/electrochemistry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:58:43.781877 exma-0.5.8/exma/io/
--rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-11-04 18:58:30.000000 exma-0.5.8/exma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10902 2022-11-04 18:58:30.000000 exma-0.5.8/exma/io/positions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8671 2022-11-04 18:58:30.000000 exma-0.5.8/exma/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     7675 2022-11-04 18:58:30.000000 exma-0.5.8/exma/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:58:43.785877 exma-0.5.8/exma/lib/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-11-04 18:58:30.000000 exma-0.5.8/exma/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-11-04 18:58:30.000000 exma-0.5.8/exma/lib/cn.c
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-11-04 18:58:30.000000 exma-0.5.8/exma/lib/cn.h
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-11-04 18:58:30.000000 exma-0.5.8/exma/lib/pbc_distances.c
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-11-04 18:58:30.000000 exma-0.5.8/exma/lib/pbc_distances.h
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2022-11-04 18:58:30.000000 exma-0.5.8/exma/lib/rdf.c
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-11-04 18:58:30.000000 exma-0.5.8/exma/lib/rdf.h
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-11-04 18:58:30.000000 exma-0.5.8/exma/msd.py
--rw-r--r--   0 runner    (1001) docker     (121)     8997 2022-11-04 18:58:30.000000 exma-0.5.8/exma/rdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-11-04 18:58:30.000000 exma-0.5.8/exma/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:58:43.781877 exma-0.5.8/exma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-11-04 18:58:43.000000 exma-0.5.8/exma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-11-04 18:58:43.000000 exma-0.5.8/exma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 18:58:43.000000 exma-0.5.8/exma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-04 18:58:43.000000 exma-0.5.8/exma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-04 18:58:43.000000 exma-0.5.8/exma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 18:58:43.785877 exma-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2854 2022-11-04 18:58:30.000000 exma-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.082202 exma-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-24 12:47:24.000000 exma-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-24 12:47:24.000000 exma-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-01-24 12:47:37.082202 exma-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-01-24 12:47:24.000000 exma-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.078202 exma-0.5.9/exma/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-01-24 12:47:24.000000 exma-0.5.9/exma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-01-24 12:47:24.000000 exma-0.5.9/exma/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-01-24 12:47:24.000000 exma-0.5.9/exma/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-01-24 12:47:24.000000 exma-0.5.9/exma/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-01-24 12:47:24.000000 exma-0.5.9/exma/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-01-24 12:47:24.000000 exma-0.5.9/exma/electrochemistry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.082202 exma-0.5.9/exma/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-01-24 12:47:24.000000 exma-0.5.9/exma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-01-24 12:47:24.000000 exma-0.5.9/exma/io/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-01-24 12:47:24.000000 exma-0.5.9/exma/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-01-24 12:47:24.000000 exma-0.5.9/exma/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.082202 exma-0.5.9/exma/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/cn.c
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/cn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/pbc_distances.c
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/pbc_distances.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/rdf.c
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/rdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-01-24 12:47:24.000000 exma-0.5.9/exma/msd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-01-24 12:47:24.000000 exma-0.5.9/exma/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-01-24 12:47:24.000000 exma-0.5.9/exma/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.078202 exma-0.5.9/exma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-01-24 12:47:36.000000 exma-0.5.9/exma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-24 12:47:37.000000 exma-0.5.9/exma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 12:47:36.000000 exma-0.5.9/exma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-24 12:47:36.000000 exma-0.5.9/exma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-24 12:47:36.000000 exma-0.5.9/exma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 12:47:37.082202 exma-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-01-24 12:47:24.000000 exma-0.5.9/setup.py
```

### Comparing `exma-0.5.8/LICENSE` & `exma-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/PKG-INFO` & `exma-0.5.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exma
-Version: 0.5.8
+Version: 0.5.9
 Summary: extendable molecular dynamics analyzer
 Home-page: https://github.com/fernandezfran/exma
 Author: Francisco Fernandez
 Author-email: fernandezfrancisco2195@gmail.com
 License: MIT
 Keywords: exma,molecular-dynamics,data-analysis
 Classifier: Development Status :: 4 - Beta
@@ -16,17 +16,20 @@
 Classifier: Programming Language :: C
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # exma
 
-[![Github Actions CI](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml/badge.svg)](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml)
+[![exma CI](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml/badge.svg)](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/exma/badge/?version=latest)](https://exma.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/exma)](https://pypi.org/project/exma/)
+[![python version](https://img.shields.io/badge/python-3.8%2B-77b7fe)](https://www.python.org/)
+[![mit license](https://img.shields.io/badge/License-MIT-fcf695)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/exma?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/exma)
 
 **exma** is a Python library with C extensions to analyze and manipulate 
 molecular dynamics trajectories and electrochemical data.
 
 
 ## Main Features
```

### Comparing `exma-0.5.8/README.md` & `exma-0.5.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # exma
 
-[![Github Actions CI](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml/badge.svg)](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml)
+[![exma CI](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml/badge.svg)](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/exma/badge/?version=latest)](https://exma.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/exma)](https://pypi.org/project/exma/)
+[![python version](https://img.shields.io/badge/python-3.8%2B-77b7fe)](https://www.python.org/)
+[![mit license](https://img.shields.io/badge/License-MIT-fcf695)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/exma?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/exma)
 
 **exma** is a Python library with C extensions to analyze and manipulate 
 molecular dynamics trajectories and electrochemical data.
 
 
 ## Main Features
```

### Comparing `exma-0.5.8/exma/__init__.py` & `exma-0.5.9/exma/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # ============================================================================
 # CONSTANTS
 # ============================================================================
 
 __author__ = """Francisco Fernandez"""
 __email__ = "fernandezfrancisco2195@gmail.com"
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 
 
 # ============================================================================
 # IMPORTS
 # ============================================================================
 
 # core
```

### Comparing `exma-0.5.8/exma/cluster.py` & `exma-0.5.9/exma/cluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -98,17 +98,17 @@
         # calculate the weigth of the ith neighbor of the interact atom
         bondmin = np.min(distrix)
         matrix_a = np.exp(1.0 - np.power(distrix / bondmin, 6))
         bondavg = np.sum(distrix * matrix_a) / np.sum(matrix_a)
 
         weitrix = np.exp(1.0 - np.power(distrix / bondavg, 6))
 
-        # reshape the weight matrix and transpose it to obtain an interact
-        # atom in every row and normalize their weights
-        weitrix = np.reshape(weitrix, (self.natoms_c_, self.natoms_i_)).T
+        # transpose the weight matrix to obtain an interact atom in every row
+        # and normalize their weights
+        weitrix = weitrix.T
         weitrix = [
             weitrix[i] / np.sum(weitrix[i]) for i in range(self.natoms_i_)
         ]
 
         # the matrix is transpose again so now we have central atoms in each
         # row an each fraction of every interact neighbor is added to obtain
         # the effective (interact) neighbor
@@ -194,15 +194,14 @@
             isolated.
         """
         self.natoms_c_ = frame._natoms_type(frame._mask_type(self.type_c))
         self.natoms_i_ = frame._natoms_type(frame._mask_type(self.type_i))
 
         distrix = pbc_distances(frame, frame, self.type_c, self.type_i)
 
-        distrix = distrix.reshape((self.natoms_c_, self.natoms_i_))
         db = sklearn.cluster.DBSCAN(
             eps=self.eps,
             min_samples=self.min_samples,
             metric="precomputed",
             **kwargs,
         ).fit(distrix)
```

### Comparing `exma-0.5.8/exma/cn.py` & `exma-0.5.9/exma/cn.py`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/core.py` & `exma-0.5.9/exma/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 # ============================================================================
 # IMPORTS
 # ============================================================================
 
 import numpy as np
 
-
 # ============================================================================
 # CLASSES
 # ============================================================================
 
 
 class AtomicSystem:
     """Define the configurations of the atomic system.
@@ -101,16 +100,20 @@
         return self.types == atom_type
 
     def _natoms_type(self, mask_type):
         """Count the number of atoms of an specific type."""
         return np.count_nonzero(mask_type)
 
     def _sorted(self):
-        """Tells if the array x is sorted (-> True) or not (-> False)."""
-        return (np.diff(self.idx) >= 0).all()
+        """Tells if the array x is sorted (-> True) or not (-> False).
+
+        Note that for xyz files self.idx is None and the frame is sorted by
+        definition.
+        """
+        return (np.diff(self.idx) >= 0).all() if self.idx is not None else True
 
     def _sort(self, dontsort=("natoms", "box")):
         """Sort the Atomic System from the sortening of the atoms id."""
         id_argsort = np.argsort(self.idx)
 
         for key in self.__dict__.keys():
             if (
@@ -201,16 +204,15 @@
 
         for i, frame in enumerate(self.frames):
             # add the box if not in frame
             frame.box = box if box is not None else frame.box
 
             # sort the frames if is not sorted, this might not be necessary
             # for all observables and all trajectories
-            if frame.idx is not None:
-                frame = frame._sort() if not frame._sorted() else frame
+            frame = frame._sort() if not frame._sorted() else frame
 
             if i == 0:
                 self._local_configure(frame)
 
             self._accumulate(frame)
 
     def calculate(self):
```

### Comparing `exma-0.5.8/exma/distances.py` & `exma-0.5.9/exma/distances.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,17 +59,16 @@
     type_i : int or str, default="all"
         type of interacting atoms, by default it computes the distances for all
         the atoms
 
     Returns
     -------
     np.array
-        array with a vector where the first natoms_i components are the
-        distances of the interacting atoms to the first central one, then the
-        second natoms_i to the second central atom, etc.
+        array with the distance matrix where the rows are the central atoms
+        and the columns the interacting ones.
     """
     lib_pbc_distances = ct.CDLL(
         str(PATH / "lib" / "lib_pbc_distances")
         + sysconfig.get_config_var("EXT_SUFFIX")
     )
     distance_matrix_c = lib_pbc_distances.distance_matrix
     distance_matrix_c.argtypes = [
@@ -114,8 +113,8 @@
     distrix_c = distrix.ctypes.data_as(ct.POINTER(ct.c_void_p))
 
     # calculates the distance matrix between interact and central atoms
     distance_matrix_c(
         natoms_c, natoms_i, box_c, xcentral_c, xinteract_c, distrix_c
     )
 
-    return distrix
+    return distrix.reshape((natoms_c, natoms_i))
```

### Comparing `exma-0.5.8/exma/electrochemistry.py` & `exma-0.5.9/exma/electrochemistry.py`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/io/__init__.py` & `exma-0.5.9/exma/io/__init__.py`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/io/positions.py` & `exma-0.5.9/exma/io/positions.py`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/io/reader.py` & `exma-0.5.9/exma/io/reader.py`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/io/writer.py` & `exma-0.5.9/exma/io/writer.py`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/lib/cn.c` & `exma-0.5.9/exma/lib/cn.c`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/lib/pbc_distances.c` & `exma-0.5.9/exma/lib/pbc_distances.c`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/lib/rdf.c` & `exma-0.5.9/exma/lib/rdf.c`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/msd.py` & `exma-0.5.9/exma/msd.py`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/rdf.py` & `exma-0.5.9/exma/rdf.py`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma/statistics.py` & `exma-0.5.9/exma/statistics.py`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/exma.egg-info/PKG-INFO` & `exma-0.5.9/exma.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exma
-Version: 0.5.8
+Version: 0.5.9
 Summary: extendable molecular dynamics analyzer
 Home-page: https://github.com/fernandezfran/exma
 Author: Francisco Fernandez
 Author-email: fernandezfrancisco2195@gmail.com
 License: MIT
 Keywords: exma,molecular-dynamics,data-analysis
 Classifier: Development Status :: 4 - Beta
@@ -16,17 +16,20 @@
 Classifier: Programming Language :: C
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # exma
 
-[![Github Actions CI](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml/badge.svg)](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml)
+[![exma CI](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml/badge.svg)](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/exma/badge/?version=latest)](https://exma.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/exma)](https://pypi.org/project/exma/)
+[![python version](https://img.shields.io/badge/python-3.8%2B-77b7fe)](https://www.python.org/)
+[![mit license](https://img.shields.io/badge/License-MIT-fcf695)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/exma?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/exma)
 
 **exma** is a Python library with C extensions to analyze and manipulate 
 molecular dynamics trajectories and electrochemical data.
 
 
 ## Main Features
```

### Comparing `exma-0.5.8/exma.egg-info/SOURCES.txt` & `exma-0.5.9/exma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exma-0.5.8/setup.py` & `exma-0.5.9/setup.py`

 * *Files identical despite different names*

