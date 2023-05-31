# Comparing `tmp/sgw_tools-1.94.tar.gz` & `tmp/sgw_tools-1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgw_tools-1.94.tar", last modified: Mon Apr 24 20:49:09 2023, max compression
+gzip compressed data, was "sgw_tools-1.95.tar", last modified: Wed May 31 21:13:47 2023, max compression
```

## Comparing `sgw_tools-1.94.tar` & `sgw_tools-1.95.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:49:09.693380 sgw_tools-1.94/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-24 20:48:38.000000 sgw_tools-1.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-24 20:49:09.693380 sgw_tools-1.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-24 20:48:38.000000 sgw_tools-1.94/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:49:09.693380 sgw_tools-1.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 20:48:38.000000 sgw_tools-1.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:49:09.693380 sgw_tools-1.94/sgw_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:49:09.693380 sgw_tools-1.94/sgw_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-24 20:49:09.000000 sgw_tools-1.94/sgw_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-24 20:49:09.000000 sgw_tools-1.94/sgw_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:49:09.000000 sgw_tools-1.94/sgw_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 20:49:09.000000 sgw_tools-1.94/sgw_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:49:09.693380 sgw_tools-1.94/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:48:38.000000 sgw_tools-1.94/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-04-24 20:48:38.000000 sgw_tools-1.94/tests/test_biggraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:47.831453 sgw_tools-1.95/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-31 21:13:08.000000 sgw_tools-1.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-31 21:13:47.831453 sgw_tools-1.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-31 21:13:08.000000 sgw_tools-1.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:13:47.831453 sgw_tools-1.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-31 21:13:08.000000 sgw_tools-1.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:47.831453 sgw_tools-1.95/sgw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:47.831453 sgw_tools-1.95/sgw_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-31 21:13:47.000000 sgw_tools-1.95/sgw_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-31 21:13:47.000000 sgw_tools-1.95/sgw_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:13:47.000000 sgw_tools-1.95/sgw_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 21:13:47.000000 sgw_tools-1.95/sgw_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:47.831453 sgw_tools-1.95/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:08.000000 sgw_tools-1.95/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-05-31 21:13:08.000000 sgw_tools-1.95/tests/test_biggraph.py
```

### Comparing `sgw_tools-1.94/LICENSE` & `sgw_tools-1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.94/PKG-INFO` & `sgw_tools-1.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw_tools
-Version: 1.94
+Version: 1.95
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.94/setup.py` & `sgw_tools-1.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sgw_tools",
-    version="1.94",
+    version="1.95",
     author="Mark Hale",
     license="MIT",
     description="Spectral graph wavelet tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pulquero/sgw",
     packages=find_packages(),
```

### Comparing `sgw_tools-1.94/sgw_tools/__init__.py` & `sgw_tools-1.95/sgw_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.94/sgw_tools/filters.py` & `sgw_tools-1.95/sgw_tools/filters.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.94/sgw_tools/graph.py` & `sgw_tools-1.95/sgw_tools/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,16 @@
             Phi_sqrt, disconnected = util.power_diagonal(self.phi, 0.5)
             Phi_neg_sqrt, _ = util.power_diagonal(self.phi, -0.5)
             Phi_P_Phi = Phi_sqrt @ self.P @ Phi_neg_sqrt
             self.L = sparse.identity(self.N) - (Phi_P_Phi + Phi_P_Phi.T.conj())/2
             self.L[disconnected, disconnected] = 0
             self.L.eliminate_zeros()
         elif lap_type == 'adjacency':
-            self.L = sparse.identity(self.N) - self.Wq/sparse.linalg.norm(self.Wq.asfptype(), 2)
+            self.Wq_norm = util.operator_norm(self.Wq)
+            self.L = sparse.identity(self.N) - self.Wq/self.Wq_norm
         else:
             raise ValueError('Unknown Laplacian type {}'.format(lap_type))
 
     def get_edge_list(self):
         if self.is_directed():
             W = self.W.tocoo()
         else:
```

### Comparing `sgw_tools-1.94/sgw_tools/graphs.py` & `sgw_tools-1.95/sgw_tools/graphs.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.94/sgw_tools/util.py` & `sgw_tools-1.95/sgw_tools/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,7 +133,12 @@
 
 
 def perron_vector(P):
     _evals, evecs = sparse.linalg.eigs(P.T, k=1, v0=np.ones(P.shape[0]))
     p = evecs[:,0]
     assert np.allclose(p.imag, 0)
     return p.real/p.real.sum()
+
+
+def operator_norm(W, maxiter=1000):
+    svals = sparse.linalg.svds(W.asfptype(), k=1, return_singular_vectors=False, solver="lobpcg", maxiter=maxiter)
+    return svals[0]
```

### Comparing `sgw_tools-1.94/sgw_tools.egg-info/PKG-INFO` & `sgw_tools-1.95/sgw_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw-tools
-Version: 1.94
+Version: 1.95
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.94/tests/test_biggraph.py` & `sgw_tools-1.95/tests/test_biggraph.py`

 * *Files identical despite different names*

