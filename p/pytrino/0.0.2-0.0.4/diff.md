# Comparing `tmp/pytrino-0.0.2.tar.gz` & `tmp/pytrino-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrino-0.0.2.tar", last modified: Wed May 31 07:32:31 2023, max compression
+gzip compressed data, was "pytrino-0.0.4.tar", last modified: Wed May 31 09:38:18 2023, max compression
```

## Comparing `pytrino-0.0.2.tar` & `pytrino-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:32:31.437487 pytrino-0.0.2/
--rw-rw-rw-   0        0        0     2015 2023-05-31 07:32:31.436472 pytrino-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1442 2023-05-31 07:31:44.000000 pytrino-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 07:32:31.418478 pytrino-0.0.2/pytrino/
--rw-rw-rw-   0        0        0      147 2023-05-31 06:48:09.000000 pytrino-0.0.2/pytrino/__init__.py
--rw-rw-rw-   0        0        0    11382 2023-05-31 07:31:47.000000 pytrino-0.0.2/pytrino/oscprobs.py
--rw-rw-rw-   0        0        0      701 2023-05-16 05:03:51.000000 pytrino-0.0.2/pytrino/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:32:31.434490 pytrino-0.0.2/pytrino.egg-info/
--rw-rw-rw-   0        0        0     2015 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 07:32:31.000000 pytrino-0.0.2/pytrino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 07:32:31.437487 pytrino-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-05-31 07:32:22.000000 pytrino-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:38:18.081068 pytrino-0.0.4/
+-rw-rw-rw-   0        0        0     2015 2023-05-31 09:38:18.080082 pytrino-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1442 2023-05-31 07:31:44.000000 pytrino-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 09:38:18.053095 pytrino-0.0.4/pytrino/
+-rw-rw-rw-   0        0        0      147 2023-05-31 06:48:09.000000 pytrino-0.0.4/pytrino/__init__.py
+-rw-rw-rw-   0        0        0     8097 2023-05-31 09:36:02.000000 pytrino-0.0.4/pytrino/oscprobs.py
+-rw-rw-rw-   0        0        0      701 2023-05-16 05:03:51.000000 pytrino-0.0.4/pytrino/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:38:18.078086 pytrino-0.0.4/pytrino.egg-info/
+-rw-rw-rw-   0        0        0     2015 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 09:38:17.000000 pytrino-0.0.4/pytrino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 09:38:18.082068 pytrino-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-05-31 09:37:04.000000 pytrino-0.0.4/setup.py
```

### Comparing `pytrino-0.0.2/PKG-INFO` & `pytrino-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrino
-Version: 0.0.2
+Version: 0.0.4
 Summary: Pytrino: A new way to numerically compute neutrino oscillations
 Author: Baalateja Kataru
 Author-email: <kavesbteja@gmail.com>
 Keywords: probability,neutrino,oscillations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pytrino-0.0.2/README.md` & `pytrino-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pytrino-0.0.2/pytrino/oscprobs.py` & `pytrino-0.0.4/pytrino/oscprobs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from numpy import sin, cos
 from numpy.linalg import eigvals, eig
 
 from .utils import kroneckerdelta, product, crct, submatrix, adjugate
 
-class Eigen:
+class MatSolver:
     def __init__(self, baseline, energy, V, delmsq21, delmsq31, deltacp, theta12, theta13, theta23):
         self.baseline = baseline
         self.energy = energy
         self.deltacp = deltacp
         self.theta12 = theta12
         self.theta13 = theta13
         self.theta23 = theta23
@@ -27,14 +27,38 @@
 
         self.M = M = O13 @ O12 @ np.diag([0, alpha, 1]) @ O12.T @ O13.T + np.diag([a, 0, 0])
         self.H = H = O23 @ Udelta @ M @ Udelta.H @ O23.T
 
     def Hevals(self):
         H = self.H
         return eigvals(H)
+    
+    def probabilities(self):
+        labelmatrix = np.matrix([["Pee", "Pemu", "Petau"], ["Pmue", "Pmumu", "Pmutau"], ["Ptaue", "Ptaumu", "Ptautau"]])
+
+        probmatrix = np.zeros((3, 3))
+
+        for i in range(1, 4):
+            for j in range(1, 4):
+                label = labelmatrix[i - 1, j - 1]
+
+                if i == j:
+                    prob = self.disappearance(i)
+                else:
+                    prob = self.appearance(i, j)
+
+                # print(f"{label}: {prob}")
+                
+                probmatrix[i - 1, j - 1] = prob
+
+        return probmatrix
+
+class Eigen(MatSolver):
+    def __init__(self, *args):
+        super().__init__(*args)
 
     def Hevecs(self):
         H = self.H
         return eig(H)[1]
     
     def evolution_matrix(self):
         lda1, lda2, lda3 = self.Hevals()
@@ -53,67 +77,23 @@
     def probability(self, i, j):
         i, j = crct(i, j)
 
         S = self.evolution_matrix()
 
         return np.abs(S[j, i])**2
     
-    def prob_disappearance(self, i):
+    def disappearance(self, i):
         return self.probability(i, i)
 
-    def prob_appearance(self, i, j):
+    def appearance(self, i, j):
         return self.probability(i, j)
     
-    def probabilities(self):
-        labelmatrix = np.matrix([["Pee", "Pemu", "Petau"], ["Pmue", "Pmumu", "Pmutau"], ["Ptaue", "Ptaumu", "Ptautau"]])
-
-        probmatrix = np.zeros((3, 3))
-
-        for i in range(1, 4):
-            for j in range(1, 4):
-                label = labelmatrix[i - 1, j - 1]
-
-                if i == j:
-                    prob = self.prob_disappearance(i)
-                else:
-                    prob = self.prob_appearance(i, j)
-
-                # print(f"{label}: {prob}")
-                
-                probmatrix[i - 1, j - 1] = prob
-
-        return probmatrix
-    
-class CayleyHamilton:
-    def __init__(self, baseline, energy, V, delmsq21, delmsq31, deltacp, theta12, theta13, theta23):
-        self.baseline = baseline
-        self.energy = energy
-        self.deltacp = deltacp
-        self.theta12 = theta12
-        self.theta13 = theta13
-        self.theta23 = theta23
-        self.V = V
-
-        self.delmsq21 = delmsq21
-        self.delmsq31 = delmsq31
-
-        alpha = delmsq21 / delmsq31
-        a = (2 * energy * V)/delmsq31
-
-        self.O12 = O12 = np.matrix([[cos(theta12), sin(theta12), 0], [-sin(theta12), cos(theta12), 0], [0, 0, 1]])
-        self.O13 = O13 = np.matrix([[cos(theta13), 0, sin(theta13)], [0, 1, 0], [-sin(theta13), 0, cos(theta13)]])
-        self.O23 = O23 = np.matrix([[1, 0, 0], [0, cos(theta23), sin(theta23)], [0, -sin(theta23), cos(theta23)]])
-        self.Udelta = Udelta = np.matrix(np.diag([1, 1, np.exp(1j * deltacp)]))
-
-        self.M = M = O13 @ O12 @ np.diag([0, alpha, 1]) @ O12.T @ O13.T + np.diag([a, 0, 0])
-        self.H = H = O23 @ Udelta @ M @ Udelta.H @ O23.T
-
-    def Hevals(self):
-        H = self.H
-        return eigvals(H)
+class CayleyHamilton(MatSolver):
+    def __init__(self, *args):
+        super().__init__(*args)
     
     def evolution_matrix(self):
         H = self.H
         lda1, lda2, lda3 = self.Hevals()
 
         L = self.baseline
         En = self.energy
@@ -129,67 +109,23 @@
     def probability(self, i, j):
         i, j = crct(i, j)
 
         S = self.evolution_matrix()
 
         return np.abs(S[j, i])**2
     
-    def prob_disappearance(self, i):
+    def disappearance(self, i):
         return self.probability(i, i)
 
-    def prob_appearance(self, i, j):
+    def appearance(self, i, j):
         return self.probability(i, j)
-    
-    def probabilities(self):
-        labelmatrix = np.matrix([["Pee", "Pemu", "Petau"], ["Pmue", "Pmumu", "Pmutau"], ["Ptaue", "Ptaumu", "Ptautau"]])
-
-        probmatrix = np.zeros((3, 3))
-
-        for i in range(1, 4):
-            for j in range(1, 4):
-                label = labelmatrix[i - 1, j - 1]
-
-                if i == j:
-                    prob = self.prob_disappearance(i)
-                else:
-                    prob = self.prob_appearance(i, j)
-
-                # print(f"{label}: {prob}")
-                
-                probmatrix[i - 1, j - 1] = prob
-
-        return probmatrix
-
-class Identities:
-    def __init__(self, baseline, energy, V, delmsq21, delmsq31, deltacp, theta12, theta13, theta23):
-        self.baseline = baseline
-        self.energy = energy
-        self.deltacp = deltacp
-        self.theta12 = theta12
-        self.theta13 = theta13
-        self.theta23 = theta23
-        self.V = V
-
-        self.delmsq21 = delmsq21
-        self.delmsq31 = delmsq31
-
-        alpha = delmsq21 / delmsq31
-        a = (2 * energy * V)/delmsq31
-
-        self.O12 = O12 = np.matrix([[cos(theta12), sin(theta12), 0], [-sin(theta12), cos(theta12), 0], [0, 0, 1]])
-        self.O13 = O13 = np.matrix([[cos(theta13), 0, sin(theta13)], [0, 1, 0], [-sin(theta13), 0, cos(theta13)]])
-        self.O23 = O23 = np.matrix([[1, 0, 0], [0, cos(theta23), sin(theta23)], [0, -sin(theta23), cos(theta23)]])
-        self.Udelta = Udelta = np.matrix(np.diag([1, 1, np.exp(1j * deltacp)]))
-
-        self.M = M = O13 @ O12 @ np.diag([0, alpha, 1]) @ O12.T @ O13.T + np.diag([a, 0, 0])
-        self.H = H = O23 @ Udelta @ M @ Udelta.H @ O23.T
 
-    def Hevals(self):
-        H = self.H
-        return eigvals(H)
+class Identities(MatSolver):
+    def __init__(self, *args):
+        super().__init__(*args)
 
     def submatrix_evals(self):
         H = self.H
 
         He = submatrix(H, 1)
         Hmu = submatrix(H, 2)
         Htau = submatrix(H, 3)
@@ -236,60 +172,39 @@
         L = self.baseline
         En = self.energy
         delmsq31 = self.delmsq31
         delta = (1.267 * delmsq31 * L)/En
 
         return sin(n * (lda[k] - lda[j]) * delta)
     
-    def prob_disappearance(self, i):
+    def disappearance(self, i):
         sum_terms = []
         for j in range(1, 4):
             for k in range(j + 1, 4):
                 term = self.PMNSmattermodsq(i, k) * self.PMNSmattermodsq(i, j) * self.deltamatsq(k, j)**2
                 sum_terms.append(term)
 
         return (1 - 4 * sum(sum_terms)).real
     
-    def prob_appearance(self, a, b):
+    def appearance(self, a, b):
         firstsum = []
         for j in range(1, 4):
             for k in range(j + 1, 4):
                 term = (self.quartic_product(k, b, a) * self.quartic_product(j, a, b)).real * self.deltamatsq(k, j)**2
                 firstsum.append(term)
         firstsum = sum(firstsum)
 
         secondsum = []
         for j in range(1, 4):
             for k in range(j + 1, 4):
                 term = (self.quartic_product(k, b, a) * self.quartic_product(j, a, b)).imag * self.deltamatsq(k, j, 2)
                 secondsum.append(term)
         secondsum = sum(secondsum)
 
-        return (kroneckerdelta(a, b) - 4 * firstsum + 2 * secondsum).real
-    
-    def probabilities(self):
-        labelmatrix = np.matrix([["Pee", "Pemu", "Petau"], ["Pmue", "Pmumu", "Pmutau"], ["Ptaue", "Ptaumu", "Ptautau"]])
-
-        probmatrix = np.zeros((3, 3))
-
-        for i in range(1, 4):
-            for j in range(1, 4):
-                label = labelmatrix[i - 1, j - 1]
-
-                if i == j:
-                    prob = self.prob_disappearance(i)
-                else:
-                    prob = self.prob_appearance(i, j)
-
-                # print(f"{label}: {prob}")
-                
-                probmatrix[i - 1, j - 1] = prob
-
-        return probmatrix
-            
+        return (kroneckerdelta(a, b) - 4 * firstsum + 2 * secondsum).real       
     
     def mat_mixing_angles(self):
         s13matsq = self.PMNSmattermodsq(1, 3).real
         c13matsq = 1 - s13matsq
 
         s12matsq = self.PMNSmattermodsq(1, 2).real / c13matsq
         s23matsq = self.PMNSmattermodsq(2, 3).real / c13matsq
```

### Comparing `pytrino-0.0.2/pytrino/utils.py` & `pytrino-0.0.4/pytrino/utils.py`

 * *Files identical despite different names*

### Comparing `pytrino-0.0.2/pytrino.egg-info/PKG-INFO` & `pytrino-0.0.4/pytrino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrino
-Version: 0.0.2
+Version: 0.0.4
 Summary: Pytrino: A new way to numerically compute neutrino oscillations
 Author: Baalateja Kataru
 Author-email: <kavesbteja@gmail.com>
 Keywords: probability,neutrino,oscillations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pytrino-0.0.2/setup.py` & `pytrino-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 
-VERSION = '0.0.2' 
+VERSION = '0.0.4'
 DESCRIPTION = 'Pytrino: A new way to numerically compute neutrino oscillations'
 
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
         name="pytrino",
```

