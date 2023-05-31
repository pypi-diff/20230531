# Comparing `tmp/simplicial-kuramoto-0.0.1.tar.gz` & `tmp/simplicial-kuramoto-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplicial-kuramoto-0.0.1.tar", last modified: Fri Jun 10 06:02:17 2022, max compression
+gzip compressed data, was "simplicial-kuramoto-0.0.2.tar", last modified: Wed May 31 04:59:53 2023, max compression
```

## Comparing `simplicial-kuramoto-0.0.1.tar` & `simplicial-kuramoto-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 06:02:17.977963 simplicial-kuramoto-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-06-10 06:02:17.973963 simplicial-kuramoto-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-06-10 06:02:08.000000 simplicial-kuramoto-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-10 06:02:17.977963 simplicial-kuramoto-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-06-10 06:02:08.000000 simplicial-kuramoto-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 06:02:17.973963 simplicial-kuramoto-0.0.1/simplicial_kuramoto/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-06-10 06:02:08.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-06-10 06:02:08.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto/chimera_measures.py
--rw-r--r--   0 runner    (1001) docker     (121)    16892 2022-06-10 06:02:08.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto/frustration_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     5466 2022-06-10 06:02:08.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto/graph_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-06-10 06:02:08.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto/integrators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2670 2022-06-10 06:02:08.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     7928 2022-06-10 06:02:08.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto/simplicial_complex.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 06:02:17.973963 simplicial-kuramoto-0.0.1/simplicial_kuramoto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-06-10 06:02:17.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-06-10 06:02:17.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-10 06:02:17.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-10 06:02:17.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-10 06:02:17.000000 simplicial-kuramoto-0.0.1/simplicial_kuramoto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:59:53.500673 simplicial-kuramoto-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-31 04:59:53.500673 simplicial-kuramoto-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 04:59:53.500673 simplicial-kuramoto-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:59:53.500673 simplicial-kuramoto-0.0.2/simplicial_kuramoto/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto/chimera_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto/frustration_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto/graph_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto/simplicial_complex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:59:53.500673 simplicial-kuramoto-0.0.2/simplicial_kuramoto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-31 04:59:53.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-31 04:59:53.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:59:53.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 04:59:53.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 04:59:53.000000 simplicial-kuramoto-0.0.2/simplicial_kuramoto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:59:53.500673 simplicial-kuramoto-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-31 04:59:39.000000 simplicial-kuramoto-0.0.2/tests/test_xgi.py
```

### Comparing `simplicial-kuramoto-0.0.1/README.md` & `simplicial-kuramoto-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -7,23 +7,40 @@
 by: Alexis Arnaudon, Robert L. Peach, Giovanni Petri and Paul Expert
 at: https://arxiv.org/pdf/2111.11073.pdf
 ```
 
 It numerically solves the Kuramoto model on simplicial complexes of order 1 (a graph) and 2 (a graph with faces), with node/edge/face weights and frustration.
 A small suite of analysis tool is available to compute the Hodge decomposition of the solution, the simplicial order parameter or the largest Lyapunov exponent.
 
+It also contains the models introduced in
+```
+A unified framework for Simplicial Kuramoto models
+by: Marco Nurisso, Alexis Arnaudon, Maxime Lucas, Robert L. Peach, Paul Expert, Francesco Vaccarino, Giovanni Petri
+at: https://arxiv.org/abs/2305.17977
+```
+
+and the connectome example in `example/connectome_example`, based on  
+```
+M. Pope, M. Fukushima, R. F. Betzel, and O. Sporns,
+Modular origins of high-amplitude cofluctuations in fine-scale functional connectivity dynamics, Proc. Natl. Acad.
+Sci. U.S.A. 118, e2109380118 (2021).
+```
+
 # Installation
 
-To install, clone the repository, and run in the main folder
+To install, it is on pypi.org, hence just do:
 ```
 pip install simplicial-kuramoto
 ```
 
 # Usage
 
+The documentation will come soon, but meanwhile:
+
 - The module `simplicial_complex.py` extends networkx graph to include faces and computed cached values of various graph theoretical operators such as boundary operators, or Hodge Laplacians.
+- The module `meausures.py` contains some measurements functions of the dynamics such as order parameters.
 - The module `graph_generator.py` contains a few functions to build simplicial complexes.
 - The module `integrators.py` solve the Kuramoto model on a given simplicial complex.
 - The module `plotting.py` has some plotting functions of the simplicial complex and the Kuramoto solution.
 - The module `frustration_scan.py` contains analysis tools to study frustration of simplicial Kuramoto.
 
-In the folder `examples` are present scripts to generate the figures of the paper. 
+In the folder `examples` are present scripts to generate the figures of the first paper as well as run some of the models of the second paper.
```

### Comparing `simplicial-kuramoto-0.0.1/simplicial_kuramoto/chimera_measures.py` & `simplicial-kuramoto-0.0.2/simplicial_kuramoto/chimera_measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
     """Shanahan metrics."""
     gms_matrix = pd.DataFrame()
     chi_matrix = pd.DataFrame()
     ce_matrix = pd.DataFrame()
     ceg_matrix = pd.DataFrame()
 
     for i, (a1, a2) in enumerate(product(alpha1, alpha2)):
-
         gms_ = []
         chi_ = []
         ce_ = []
         ceg_ = []
 
         for result in results[i]:
             op, _ = module_order_parameter(result.y, edge_community_assignment)
```

### Comparing `simplicial-kuramoto-0.0.1/simplicial_kuramoto/frustration_scan.py` & `simplicial-kuramoto-0.0.2/simplicial_kuramoto/frustration_scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import matplotlib.pyplot as plt
 import nolds
 import numpy as np
 import pandas as pd
 import scipy as sc
 from tqdm import tqdm
 
-from simplicial_kuramoto.integrators import integrate_edge_kuramoto
+from simplicial_kuramoto.integrators import compute_order_parameter, integrate_edge_kuramoto
+from simplicial_kuramoto.simplicial_complex import use_with_xgi
 
 L = logging.getLogger(__name__)
 
 
 def _integrate_several_kuramoto(
     parameters,
     simplicial_complex,
@@ -108,77 +109,35 @@
     if save:
         with open(folder + filename, "wb") as f:
             pickle.dump([simplicial_complex, results, alpha1, alpha2], f)
 
     return results
 
 
+@use_with_xgi
 def get_subspaces(Gsc):
     """ "Get grad, curl and harm subspaces from simplicial complex."""
     grad_subspace = sc.linalg.orth(Gsc.N0.todense())
     try:
         curl_subspace = sc.linalg.orth(Gsc.N1s.todense())
     except (ValueError, AttributeError):
-        curl_subspace = np.zeros([len(Gsc.graph.edges), 0])
+        curl_subspace = np.zeros([Gsc.n_edges, 0])
 
-    harm_subspace = sc.linalg.null_space(Gsc.L1.todense())
+    harm_subspace = sc.linalg.null_space(Gsc.L1.todense(), rcond=1e-1)
     return grad_subspace, curl_subspace, harm_subspace
 
 
 def proj_subspace(vec, subspace):
     """Project a list of vecs to a given subspace (from get_subspaces)."""
     proj = np.zeros_like(vec)
     for direction in subspace.T:
         proj += np.outer(vec.dot(direction), direction)
     return np.linalg.norm(proj, axis=1)
 
 
-def compute_node_order_parameter(result, Gsc):
-    """Compute the node Kuramoto order parameter."""
-    w1_inv = 1.0 / np.diag(Gsc.W1.toarray())
-    return w1_inv.dot(np.cos(Gsc.N0.dot(result))) / w1_inv.sum()
-
-
-def compute_order_parameter(result, Gsc, subset=None):
-    """Evaluate the order parameter, or the partial one for subset edges.
-    Args:
-        result (array): result of simulation (edge lenght by timepoints)
-        Gsc (SimplicialComplex): simplicial complex
-        subset (array): bool or int array of edges in the subset to consider
-
-    Returns:
-        total order, node order, face order
-    """
-    w0_inv = 1.0 / np.diag(Gsc.W0.toarray())
-    if Gsc.W2 is not None:
-        w2_inv = 1.0 / np.diag(Gsc.W2.toarray())
-
-    if subset is not None:
-        # if we have at least an adjacent edge in subset
-        w0_inv = w0_inv * np.clip(abs(Gsc.B0.T).dot(subset), 0, 1)
-        # if we have all 3 edges in subset
-        w2_inv = w2_inv * (abs(Gsc.B1).dot(subset) == 3)
-
-    order_node = w0_inv.dot(np.cos(Gsc.N0s.dot(result)))
-    norm_node = w0_inv.sum()
-
-    if Gsc.W2 is not None:
-        order_face = w2_inv.dot(np.cos(Gsc.N1.dot(result)))
-        norm_face = w2_inv.sum()
-    else:
-        order_face = 0
-        norm_face = 0
-
-    return (
-        (order_node + order_face) / (norm_node + norm_face),
-        order_node / norm_node,
-        order_face / norm_face if norm_face > 0 else 0,
-    )
-
-
 def get_projection_fit(
     Gsc, res, grad_subspace=None, curl_subspace=None, harm_subspace=None, n_min=0
 ):
     """Project result on subspaces and compute linear fit."""
     if grad_subspace is None:
         grad_subspace, curl_subspace, harm_subspace = get_subspaces(Gsc)
     time = res.t[n_min:]
@@ -202,15 +161,15 @@
     _grad, _curl, _harm, grad_slope, curl_slope, harm_slope = get_projection_fit(
         Gsc, result[0], grad_subspace, curl_subspace, harm_subspace, n_min
     )
     grad_slope = grad_slope[0]
     curl_slope = curl_slope[0]
     harm_slope = harm_slope[0]
 
-    harm_order = np.mean(compute_order_parameter(res, Gsc)[0])
+    harm_order = np.mean(compute_order_parameter(Gsc, res)[0])
 
     grad = grad_slope if np.std(_grad) > eps or grad_slope > eps else np.nan
     curl = curl_slope if np.std(_curl) > eps or curl_slope > eps else np.nan
     harm = harm_slope if np.std(_harm) > eps or harm_slope > eps else np.nan
     return grad, curl, harm, harm_order
 
 
@@ -261,15 +220,15 @@
     _grad, _curl, _harm, grad_slope, curl_slope, harm_slope = get_projection_fit(
         Gsc, result, grad_subspace, curl_subspace, harm_subspace, n_min
     )
     grad_slope = grad_slope[0]
     curl_slope = curl_slope[0]
     harm_slope = harm_slope[0]
 
-    harm_order = compute_order_parameter(res, Gsc)[0]
+    harm_order = compute_order_parameter(Gsc, res)[0]
     mean_harm_order = np.mean(harm_order)
     std_harm_order = np.std(harm_order)
 
     grad = grad_slope if np.std(_grad) > eps or grad_slope > eps else np.nan
     curl = curl_slope if np.std(_curl) > eps or curl_slope > eps else np.nan
     harm = harm_slope if np.std(_harm) > eps or harm_slope > eps else np.nan
     return grad, curl, harm, mean_harm_order, std_harm_order
@@ -352,15 +311,15 @@
     plt.xlabel(r"$\alpha_2$")
     plt.twinx()
     harm_order_df = _mean(alphas, std_harm_order)
     if with_std:
         std_harm_df = _std(alphas, std_harm_order)
         plt.errorbar(harm_order_df.index, harm_order_df.data, yerr=std_harm_df.data, c="C4")
     plt.plot(harm_order_df.index, harm_order_df.data, "-", c="C4", label="std(order)")
-    plt.gca().set_ylim(-0.01, max(max(std_harm_order), 0.1))
+    plt.gca().set_ylim(-0.01, max(*std_harm_order, 0.1))
     axs[1].set_xlim(alphas[0], alphas[-1])
     plt.legend(loc="upper left")
     plt.ylabel("std(order)")
     plt.savefig(filename, bbox_inches="tight")
 
 
 def plot_order(path, filename, frac=0.5, eps=1e-5, n_workers=4, with_proj=False):
```

### Comparing `simplicial-kuramoto-0.0.1/simplicial_kuramoto/plotting.py` & `simplicial-kuramoto-0.0.2/simplicial_kuramoto/plotting.py`

 * *Files identical despite different names*

### Comparing `simplicial-kuramoto-0.0.1/simplicial_kuramoto/simplicial_complex.py` & `simplicial-kuramoto-0.0.2/simplicial_kuramoto/simplicial_complex.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 """Representation of simplicial complex"""
 import networkx as nx
 import numpy as np
 import scipy as sc
 
+try:
+    import xgi
+except ImportError:
+    pass
+
 
 def pos(matrix):
     """Return positive part of matrix."""
     _matrix = matrix.copy()
     _matrix[_matrix < 0] = 0
     return _matrix
 
@@ -44,21 +49,28 @@
         self._N1s = None
         self._W0 = None
         self._W1 = None
         self._W2 = None
         self._L0 = None
         self._L1 = None
 
+        self._V0 = None
         self._V1 = None
         self._V2 = None
 
         self._lifted_N0 = None
+        self._lifted_N0s = None
+        self._lifted_N0s_left = None
         self._lifted_N0sn = None
+        self._lifted_N0n = None
+        self._lifted_N0n_right = None
         self._lifted_N1 = None
+        self._lifted_N1n_right = None
         self._lifted_N1sn = None
+        self._lifted_N1s_left = None
 
         self.set_lexicographic()
         self.no_faces = no_faces
         self.set_faces(faces)
         if face_weights is None:
             self.face_weights = np.ones(self.n_faces)
         else:
@@ -209,16 +221,25 @@
             self._L1 = self.N0.dot(self.N0s)
 
             if self.W2 is not None:
                 self._L1 += self.N1s.dot(self.N1)
         return self._L1
 
     @property
+    def V0(self):
+        """Lift operator on nodes."""
+        if self._V0 is None:
+            self._V0 = sc.sparse.csr_matrix(
+                np.concatenate((np.eye(self.n_nodes), -np.eye(self.n_nodes)), axis=0)
+            )
+        return self._V0
+
+    @property
     def V1(self):
-        """Lift operator on faces."""
+        """Lift operator on edges."""
         if self._V1 is None:
             self._V1 = sc.sparse.csr_matrix(
                 np.concatenate((np.eye(self.n_edges), -np.eye(self.n_edges)), axis=0)
             )
         return self._V1
 
     @property
@@ -234,26 +255,98 @@
     def lifted_N0(self):
         """Create lifted version of incidence matrices."""
         if self._lifted_N0 is None:
             self._lifted_N0 = self.V1.dot(self.N0)
         return self._lifted_N0
 
     @property
+    def lifted_N0s(self):
+        """Create lifted version of incidence matrices."""
+        if self._lifted_N0s is None:
+            self._lifted_N0s = self.N0s.dot(self.V1.T)
+        return self._lifted_N0s
+
+    @property
+    def lifted_N0s_left(self):
+        """Create lifted version of incidence matrices."""
+        if self._lifted_N0s_left is None:
+            self._lifted_N0s_left = self.V0.dot(self.N0s)
+        return self._lifted_N0s_left
+
+    @property
+    def lifted_N0n(self):
+        """Create lifted version of incidence matrices."""
+        if self._lifted_N0n is None:
+            self._lifted_N0n = neg(self.lifted_N0)
+        return self._lifted_N0n
+
+    @property
+    def lifted_N0n_right(self):
+        """Create lifted version of incidence matrices."""
+        if self._lifted_N0n_right is None:
+            self._lifted_N0n_right = neg(self.N0.dot(self.V0.T))
+        return self._lifted_N0n_right
+
+    @property
     def lifted_N0sn(self):
         """Create lifted version of incidence matrices."""
         if self._lifted_N0sn is None:
             self._lifted_N0sn = neg(self.N0s.dot(self.V1.T))
         return self._lifted_N0sn
 
     @property
     def lifted_N1(self):
         """Create lifted version of incidence matrices."""
         if self._lifted_N1 is None:
             self._lifted_N1 = self.V2.dot(self.N1)
         return self._lifted_N1
 
     @property
+    def lifted_N1n_right(self):
+        """Create lifted version of incidence matrices."""
+        if self._lifted_N1n_right is None:
+            self._lifted_N1n_right = neg(self.N1.dot(self.V1.T))
+        return self._lifted_N1n_right
+
+    @property
+    def lifted_N1s_left(self):
+        """Create lifted version of incidence matrices."""
+        if self._lifted_N1s_left is None:
+            self._lifted_N1s_left = self.V1.dot(self.N1s)
+        return self._lifted_N1s_left
+
+    @property
     def lifted_N1sn(self):
         """Create lifted version of incidence matrices."""
         if self._lifted_N1sn is None:
             self._lifted_N1sn = neg(self.N1s.dot(self.V2.T))
         return self._lifted_N1sn
+
+
+def use_with_xgi(func):
+    """Use this as a decorator to convert xgi simplicial complex to internal structure.
+
+    First argument of the functiou should be a SimplicialComplex object (internal of xgi)
+    """
+
+    def _process(*args, **kwargs):
+        sc = xgi_to_internal(args[0])
+        return func(sc, *args[1:], **kwargs)
+
+    return _process
+
+
+def xgi_to_internal(simplicial_complex):
+    """Convert xgi simplicial complex into internal simplicial complex structure."""
+    if isinstance(simplicial_complex, xgi.SimplicialComplex):
+        # we convert with incidence matrix to keep control on node ordering
+        B0 = sc.sparse.csr_matrix(
+            xgi.linalg.hodge_matrix.boundary_matrix(simplicial_complex, 1, None, False).T
+        )
+        B0 = B0[:, simplicial_complex.nodes]
+        A = B0.T.dot(B0).toarray()
+        A = np.diag(np.diag(A)) - A
+        graph = nx.from_numpy_array(A)
+
+        faces = [list(e) for e in simplicial_complex.edges.members() if len(e) == 3]
+        return SimplicialComplex(graph=graph, faces=faces)
+    return simplicial_complex
```

