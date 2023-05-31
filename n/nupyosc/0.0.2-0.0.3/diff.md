# Comparing `tmp/nupyosc-0.0.2.tar.gz` & `tmp/nupyosc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nupyosc-0.0.2.tar", last modified: Mon May 22 03:24:03 2023, max compression
+gzip compressed data, was "nupyosc-0.0.3.tar", last modified: Wed May 31 06:38:10 2023, max compression
```

## Comparing `nupyosc-0.0.2.tar` & `nupyosc-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 03:24:03.568925 nupyosc-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-22 03:24:03.555238 nupyosc-0.0.2/NuPy/
--rw-rw-rw-   0        0        0      147 2023-05-16 07:44:59.000000 nupyosc-0.0.2/NuPy/__init__.py
--rw-rw-rw-   0        0        0    10475 2023-05-17 01:58:51.000000 nupyosc-0.0.2/NuPy/oscprobs.py
--rw-rw-rw-   0        0        0      701 2023-05-16 05:03:51.000000 nupyosc-0.0.2/NuPy/utils.py
--rw-rw-rw-   0        0        0     2012 2023-05-22 03:24:03.568925 nupyosc-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-05-22 03:19:24.000000 nupyosc-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 03:24:03.567926 nupyosc-0.0.2/nupyosc.egg-info/
--rw-rw-rw-   0        0        0     2012 2023-05-22 03:24:03.000000 nupyosc-0.0.2/nupyosc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-05-22 03:24:03.000000 nupyosc-0.0.2/nupyosc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 03:24:03.000000 nupyosc-0.0.2/nupyosc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 03:24:03.000000 nupyosc-0.0.2/nupyosc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-22 03:24:03.000000 nupyosc-0.0.2/nupyosc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 03:24:03.569919 nupyosc-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-05-22 03:23:51.000000 nupyosc-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:38:10.817892 nupyosc-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-31 06:38:10.793899 nupyosc-0.0.3/NuPy/
+-rw-rw-rw-   0        0        0      147 2023-05-16 07:44:59.000000 nupyosc-0.0.3/NuPy/__init__.py
+-rw-rw-rw-   0        0        0    11402 2023-05-31 05:36:06.000000 nupyosc-0.0.3/NuPy/oscprobs.py
+-rw-rw-rw-   0        0        0      701 2023-05-16 05:03:51.000000 nupyosc-0.0.3/NuPy/utils.py
+-rw-rw-rw-   0        0        0     2002 2023-05-31 06:38:10.817892 nupyosc-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-05-22 03:19:24.000000 nupyosc-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 06:38:10.814910 nupyosc-0.0.3/nupyosc.egg-info/
+-rw-rw-rw-   0        0        0     2002 2023-05-31 06:38:10.000000 nupyosc-0.0.3/nupyosc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-05-31 06:38:10.000000 nupyosc-0.0.3/nupyosc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 06:38:10.000000 nupyosc-0.0.3/nupyosc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 06:38:10.000000 nupyosc-0.0.3/nupyosc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-31 06:38:10.000000 nupyosc-0.0.3/nupyosc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 06:38:10.818892 nupyosc-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-05-31 06:19:12.000000 nupyosc-0.0.3/setup.py
```

### Comparing `nupyosc-0.0.2/NuPy/oscprobs.py` & `nupyosc-0.0.3/NuPy/oscprobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import numpy as np
 from numpy import sin, cos
 from numpy.linalg import eigvals, eig
 
 from .utils import kroneckerdelta, product, crct, submatrix, adjugate
 
 class OscProbStandard:
-    def __init__(self, alpha, a, delta, deltacp, theta12, theta13, theta23):
-        self.alpha = alpha
-        self.a = a
-        self.delta = delta
+    def __init__(self, baseline, energy, V, delmsq21, delmsq31, deltacp, theta12, theta13, theta23):
+        self.baseline = baseline
+        self.energy = energy
         self.deltacp = deltacp
         self.theta12 = theta12
         self.theta13 = theta13
         self.theta23 = theta23
+        self.V = V
+
+        self.delmsq21 = delmsq21
+        self.delmsq31 = delmsq31
+
+        alpha = delmsq21 / delmsq31
+        a = (2 * energy * V)/delmsq31
 
         self.O12 = O12 = np.matrix([[cos(theta12), sin(theta12), 0], [-sin(theta12), cos(theta12), 0], [0, 0, 1]])
         self.O13 = O13 = np.matrix([[cos(theta13), 0, sin(theta13)], [0, 1, 0], [-sin(theta13), 0, cos(theta13)]])
         self.O23 = O23 = np.matrix([[1, 0, 0], [0, cos(theta23), sin(theta23)], [0, -sin(theta23), cos(theta23)]])
         self.Udelta = Udelta = np.matrix(np.diag([1, 1, np.exp(1j * deltacp)]))
 
         self.M = M = O13 @ O12 @ np.diag([0, alpha, 1]) @ O12.T @ O13.T + np.diag([a, 0, 0])
@@ -27,21 +33,25 @@
         return eigvals(H)
 
     def Hevecs(self):
         H = self.H
         return eig(H)[1]
     
     def evolution_matrix(self):
-        E1, E2, E3 = self.Hevals()
+        lda1, lda2, lda3 = self.Hevals()
         evecs = self.Hevecs()
-        delta = self.delta
+
+        L = self.baseline
+        En = self.energy
+        delmsq31 = self.delmsq31
+        delta = (1.267 * delmsq31 * L)/En
 
         eigmat = np.matrix(evecs)
 
-        S = eigmat @ np.diag([np.exp(-1j * E1 * 2 * delta), np.exp(-1j * E2 * 2 * delta), np.exp(-1j * E3 * 2 * delta)]) @ eigmat.H
+        S = eigmat @ np.diag([np.exp(-1j * lda1 * 2 * delta), np.exp(-1j * lda2 * 2 * delta), np.exp(-1j * lda3 * 2 * delta)]) @ eigmat.H
         return S
     
     def probability(self, i, j):
         i, j = crct(i, j)
 
         S = self.evolution_matrix()
 
@@ -70,22 +80,28 @@
                 print(f"{label}: {prob}")
                 
                 probmatrix[i - 1, j - 1] = prob
 
         return probmatrix
     
 class OscProbCayleyHamilton:
-    def __init__(self, alpha, a, delta, deltacp, theta12, theta13, theta23):
-        self.alpha = alpha
-        self.a = a
-        self.delta = delta
+    def __init__(self, baseline, energy, V, delmsq21, delmsq31, deltacp, theta12, theta13, theta23):
+        self.baseline = baseline
+        self.energy = energy
         self.deltacp = deltacp
         self.theta12 = theta12
         self.theta13 = theta13
         self.theta23 = theta23
+        self.V = V
+
+        self.delmsq21 = delmsq21
+        self.delmsq31 = delmsq31
+
+        alpha = delmsq21 / delmsq31
+        a = (2 * energy * V)/delmsq31
 
         self.O12 = O12 = np.matrix([[cos(theta12), sin(theta12), 0], [-sin(theta12), cos(theta12), 0], [0, 0, 1]])
         self.O13 = O13 = np.matrix([[cos(theta13), 0, sin(theta13)], [0, 1, 0], [-sin(theta13), 0, cos(theta13)]])
         self.O23 = O23 = np.matrix([[1, 0, 0], [0, cos(theta23), sin(theta23)], [0, -sin(theta23), cos(theta23)]])
         self.Udelta = Udelta = np.matrix(np.diag([1, 1, np.exp(1j * deltacp)]))
 
         self.M = M = O13 @ O12 @ np.diag([0, alpha, 1]) @ O12.T @ O13.T + np.diag([a, 0, 0])
@@ -93,20 +109,24 @@
 
     def Hevals(self):
         H = self.H
         return eigvals(H)
     
     def evolution_matrix(self):
         H = self.H
-        E1, E2, E3 = self.Hevals()
-        delta = self.delta
+        lda1, lda2, lda3 = self.Hevals()
 
-        S = (np.exp(-1j * E1 * 2 * delta)/((E1 - E2) * (E1 - E3))) * (E2 * E3 * np.identity(3) - (E2 + E3) * H + H @ H) +\
-        (np.exp(-1j * E2 * 2 * delta)/((E2 - E1) * (E2 - E3))) * (E1 * E3 * np.identity(3) - (E1 + E3) * H + H @ H) +\
-        (np.exp(-1j * E3 * 2 * delta)/((E3 - E1) * (E3 - E2))) * (E1 * E2 * np.identity(3) - (E1 + E2) * H + H @ H)
+        L = self.baseline
+        En = self.energy
+        delmsq31 = self.delmsq31
+        delta = (1.267 * delmsq31 * L)/En
+
+        S = (np.exp(-1j * lda1 * 2 * delta)/((lda1 - lda2) * (lda1 - lda3))) * (lda2 * lda3 * np.identity(3) - (lda2 + lda3) * H + H @ H) +\
+        (np.exp(-1j * lda2 * 2 * delta)/((lda2 - lda1) * (lda2 - lda3))) * (lda1 * lda3 * np.identity(3) - (lda1 + lda3) * H + H @ H) +\
+        (np.exp(-1j * lda3 * 2 * delta)/((lda3 - lda1) * (lda3 - lda2))) * (lda1 * lda2 * np.identity(3) - (lda1 + lda2) * H + H @ H)
 
         return S
     
     def probability(self, i, j):
         i, j = crct(i, j)
 
         S = self.evolution_matrix()
@@ -136,22 +156,28 @@
                 print(f"{label}: {prob}")
                 
                 probmatrix[i - 1, j - 1] = prob
 
         return probmatrix
 
 class OscProbIdentities:
-    def __init__(self, alpha, a, delta, deltacp, theta12, theta13, theta23):
-        self.alpha = alpha
-        self.a = a
-        self.delta = delta
+    def __init__(self, baseline, energy, V, delmsq21, delmsq31, deltacp, theta12, theta13, theta23):
+        self.baseline = baseline
+        self.energy = energy
         self.deltacp = deltacp
         self.theta12 = theta12
         self.theta13 = theta13
         self.theta23 = theta23
+        self.V = V
+
+        self.delmsq21 = delmsq21
+        self.delmsq31 = delmsq31
+
+        alpha = delmsq21 / delmsq31
+        a = (2 * energy * V)/delmsq31
 
         self.O12 = O12 = np.matrix([[cos(theta12), sin(theta12), 0], [-sin(theta12), cos(theta12), 0], [0, 0, 1]])
         self.O13 = O13 = np.matrix([[cos(theta13), 0, sin(theta13)], [0, 1, 0], [-sin(theta13), 0, cos(theta13)]])
         self.O23 = O23 = np.matrix([[1, 0, 0], [0, cos(theta23), sin(theta23)], [0, -sin(theta23), cos(theta23)]])
         self.Udelta = Udelta = np.matrix(np.diag([1, 1, np.exp(1j * deltacp)]))
 
         self.M = M = O13 @ O12 @ np.diag([0, alpha, 1]) @ O12.T @ O13.T + np.diag([a, 0, 0])
@@ -202,15 +228,19 @@
 
         return modsq
     
     def deltamatsq(self, k, j, n=1):
         k, j = crct(k, j)
 
         lda = self.Hevals()
-        delta = self.delta
+
+        L = self.baseline
+        En = self.energy
+        delmsq31 = self.delmsq31
+        delta = (1.267 * delmsq31 * L)/En
 
         return sin(n * (lda[k] - lda[j]) * delta)
     
     def prob_disappearance(self, i):
         sum_terms = []
         for j in range(1, 4):
             for k in range(j + 1, 4):
@@ -289,15 +319,15 @@
 
     def mat_angles_phase(self):
         theta12mat, theta13mat, theta23mat = self.mat_mixing_angles()
         matdeltacp = self.toshev_identity()
 
         return matdeltacp, theta12mat, theta13mat, theta23mat
     
-    def PMNS(self):
+    def PMNSmat(self):
         deltacp, theta12, theta13, theta23 = self.mat_angles_phase()
 
         O12 = np.matrix([[cos(theta12), sin(theta12), 0], [-sin(theta12), cos(theta12), 0], [0, 0, 1]])
         O13 = np.matrix([[cos(theta13), 0, sin(theta13)], [0, 1, 0], [-sin(theta13), 0, cos(theta13)]])
         O23 = np.matrix([[1, 0, 0], [0, cos(theta23), sin(theta23)], [0, -sin(theta23), cos(theta23)]])
         Udelta = np.matrix(np.diag([1, 1, np.exp(1j * deltacp)]))
```

### Comparing `nupyosc-0.0.2/NuPy/utils.py` & `nupyosc-0.0.3/NuPy/utils.py`

 * *Files identical despite different names*

### Comparing `nupyosc-0.0.2/PKG-INFO` & `nupyosc-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nupyosc
-Version: 0.0.2
-Summary: NuPy: A new way to numerically compute neutrino oscillations in matter
+Version: 0.0.3
+Summary: NuPy: A new way to numerically compute neutrino oscillations
 Author: Baalateja Kataru
 Author-email: <kavesbteja@gmail.com>
 Keywords: probability,neutrino,oscillations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nupyosc-0.0.2/README.md` & `nupyosc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nupyosc-0.0.2/nupyosc.egg-info/PKG-INFO` & `nupyosc-0.0.3/nupyosc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nupyosc
-Version: 0.0.2
-Summary: NuPy: A new way to numerically compute neutrino oscillations in matter
+Version: 0.0.3
+Summary: NuPy: A new way to numerically compute neutrino oscillations
 Author: Baalateja Kataru
 Author-email: <kavesbteja@gmail.com>
 Keywords: probability,neutrino,oscillations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nupyosc-0.0.2/setup.py` & `nupyosc-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 
-VERSION = '0.0.2' 
-DESCRIPTION = 'NuPy: A new way to numerically compute neutrino oscillations in matter'
+VERSION = '0.0.3' 
+DESCRIPTION = 'NuPy: A new way to numerically compute neutrino oscillations'
 
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="nupyosc",
```

