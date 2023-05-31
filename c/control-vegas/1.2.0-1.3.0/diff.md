# Comparing `tmp/control-vegas-1.2.0.tar.gz` & `tmp/control-vegas-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-vegas-1.2.0.tar", last modified: Thu May 25 16:31:08 2023, max compression
+gzip compressed data, was "control-vegas-1.3.0.tar", last modified: Wed May 31 06:27:11 2023, max compression
```

## Comparing `control-vegas-1.2.0.tar` & `control-vegas-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-25 16:31:08.809237 control-vegas-1.2.0/
--rw-r--r--   0 person    (1000) person    (1000)       66 2023-03-31 14:30:55.000000 control-vegas-1.2.0/.gitattributes
--rw-r--r--   0 person    (1000) person    (1000)      114 2023-03-31 14:30:55.000000 control-vegas-1.2.0/.gitignore
--rw-r--r--   0 person    (1000) person    (1000)      634 2023-05-25 16:27:17.000000 control-vegas-1.2.0/CITATION.cff
--rw-r--r--   0 person    (1000) person    (1000)    35149 2023-03-31 14:30:55.000000 control-vegas-1.2.0/LICENSE
--rw-r--r--   0 person    (1000) person    (1000)    49800 2023-05-25 16:31:08.805904 control-vegas-1.2.0/PKG-INFO
--rw-r--r--   0 person    (1000) person    (1000)     8318 2023-05-25 16:14:49.000000 control-vegas-1.2.0/README.md
--rw-r--r--   0 person    (1000) person    (1000)     1282 2023-05-25 16:29:32.000000 control-vegas-1.2.0/pyproject.toml
--rw-r--r--   0 person    (1000) person    (1000)       38 2023-05-25 16:31:08.809237 control-vegas-1.2.0/setup.cfg
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-25 16:31:08.805904 control-vegas-1.2.0/src/
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-25 16:31:08.805904 control-vegas-1.2.0/src/control_vegas/
--rw-r--r--   0 person    (1000) person    (1000)      264 2023-05-13 08:27:23.000000 control-vegas-1.2.0/src/control_vegas/__init__.py
--rw-r--r--   0 person    (1000) person    (1000)       76 2023-04-12 21:33:59.000000 control-vegas-1.2.0/src/control_vegas/_exceptions.py
--rw-r--r--   0 person    (1000) person    (1000)      340 2023-05-13 08:25:27.000000 control-vegas-1.2.0/src/control_vegas/_types.py
--rw-r--r--   0 person    (1000) person    (1000)    22721 2023-05-13 08:25:08.000000 control-vegas-1.2.0/src/control_vegas/cvintegrator.py
--rw-r--r--   0 person    (1000) person    (1000)    10282 2023-05-13 08:23:18.000000 control-vegas-1.2.0/src/control_vegas/functions.py
--rw-r--r--   0 person    (1000) person    (1000)     4789 2023-05-13 07:34:13.000000 control-vegas-1.2.0/src/control_vegas/utilities.py
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-25 16:31:08.805904 control-vegas-1.2.0/src/control_vegas.egg-info/
--rw-r--r--   0 person    (1000) person    (1000)    49800 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/PKG-INFO
--rw-r--r--   0 person    (1000) person    (1000)      462 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/SOURCES.txt
--rw-r--r--   0 person    (1000) person    (1000)        1 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/dependency_links.txt
--rw-r--r--   0 person    (1000) person    (1000)      111 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/requires.txt
--rw-r--r--   0 person    (1000) person    (1000)       14 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/top_level.txt
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 06:27:11.486844 control-vegas-1.3.0/
+-rw-r--r--   0 person    (1000) person    (1000)       66 2023-03-31 14:30:55.000000 control-vegas-1.3.0/.gitattributes
+-rw-r--r--   0 person    (1000) person    (1000)      114 2023-03-31 14:30:55.000000 control-vegas-1.3.0/.gitignore
+-rw-r--r--   0 person    (1000) person    (1000)      650 2023-05-25 16:37:14.000000 control-vegas-1.3.0/CITATION.cff
+-rw-r--r--   0 person    (1000) person    (1000)    35149 2023-03-31 14:30:55.000000 control-vegas-1.3.0/LICENSE
+-rw-r--r--   0 person    (1000) person    (1000)    49800 2023-05-31 06:27:11.486844 control-vegas-1.3.0/PKG-INFO
+-rw-r--r--   0 person    (1000) person    (1000)     8318 2023-05-25 16:14:49.000000 control-vegas-1.3.0/README.md
+-rw-r--r--   0 person    (1000) person    (1000)     1232 2023-05-31 06:24:50.000000 control-vegas-1.3.0/pyproject.toml
+-rw-r--r--   0 person    (1000) person    (1000)       38 2023-05-31 06:27:11.486844 control-vegas-1.3.0/setup.cfg
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 06:27:11.483511 control-vegas-1.3.0/src/
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 06:27:11.486844 control-vegas-1.3.0/src/control_vegas/
+-rw-r--r--   0 person    (1000) person    (1000)      228 2023-05-31 01:47:58.000000 control-vegas-1.3.0/src/control_vegas/__init__.py
+-rw-r--r--   0 person    (1000) person    (1000)       76 2023-04-12 21:33:59.000000 control-vegas-1.3.0/src/control_vegas/_exceptions.py
+-rw-r--r--   0 person    (1000) person    (1000)      340 2023-05-13 08:25:27.000000 control-vegas-1.3.0/src/control_vegas/_types.py
+-rw-r--r--   0 person    (1000) person    (1000)     1353 2023-05-31 01:48:31.000000 control-vegas-1.3.0/src/control_vegas/_wrappers.py
+-rw-r--r--   0 person    (1000) person    (1000)    22721 2023-05-31 05:51:32.000000 control-vegas-1.3.0/src/control_vegas/cvintegrator.py
+-rw-r--r--   0 person    (1000) person    (1000)    12676 2023-05-31 06:20:53.000000 control-vegas-1.3.0/src/control_vegas/functions.py
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-31 06:27:11.486844 control-vegas-1.3.0/src/control_vegas.egg-info/
+-rw-r--r--   0 person    (1000) person    (1000)    49800 2023-05-31 06:27:11.000000 control-vegas-1.3.0/src/control_vegas.egg-info/PKG-INFO
+-rw-r--r--   0 person    (1000) person    (1000)      462 2023-05-31 06:27:11.000000 control-vegas-1.3.0/src/control_vegas.egg-info/SOURCES.txt
+-rw-r--r--   0 person    (1000) person    (1000)        1 2023-05-31 06:27:11.000000 control-vegas-1.3.0/src/control_vegas.egg-info/dependency_links.txt
+-rw-r--r--   0 person    (1000) person    (1000)       74 2023-05-31 06:27:11.000000 control-vegas-1.3.0/src/control_vegas.egg-info/requires.txt
+-rw-r--r--   0 person    (1000) person    (1000)       14 2023-05-31 06:27:11.000000 control-vegas-1.3.0/src/control_vegas.egg-info/top_level.txt
```

### Comparing `control-vegas-1.2.0/CITATION.cff` & `control-vegas-1.3.0/CITATION.cff`

 * *Files 23% similar despite different names*

```diff
@@ -15,11 +15,12 @@
   reduction technique on top of the vegas algorithm for
   Monte Carlo integration.
 keywords:
   - Monte Carlo
   - variance reduction
   - vegas
   - python
+  - integration
 license: GPL-3.0+
-commit: 6b9660c
-version: 1.1.0
-date-released: '2023-04-19'
+commit: b1f2a2c
+version: 1.2.0
+date-released: '2023-05-25'
```

### Comparing `control-vegas-1.2.0/LICENSE` & `control-vegas-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `control-vegas-1.2.0/PKG-INFO` & `control-vegas-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-vegas
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Control Variate wrapper over the vegas python package.
 Author-email: Jacob Scott <jscott137@pm.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `control-vegas-1.2.0/README.md` & `control-vegas-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `control-vegas-1.2.0/pyproject.toml` & `control-vegas-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools.scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "control-vegas"
-version = "1.2.0"
+version = "1.3.0"
 description = "A Control Variate wrapper over the vegas python package."
 authors = [
     {name = "Jacob Scott", email = "jscott137@pm.me"}
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
@@ -33,13 +33,11 @@
 
 [project.optional-dependencies]
 dev = [
     "build",
     "twine",
     "black",
     "isort",
-    "jupyterlab",
-    "jupyterlab_code_formatter"
 ]
 
 [project.urls]
 Github = "https://github.com/crumpstrr33/control-vegas"
```

### Comparing `control-vegas-1.2.0/src/control_vegas/cvintegrator.py` & `control-vegas-1.3.0/src/control_vegas/cvintegrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 import numpy as np
 from nptyping import Float, NDArray, Shape
 from numpy.random import RandomState
 from vegas import Integrator
 
 from ._types import _ftype
+from ._wrappers import check_attrs, timing
 from .functions import Function, make_func
-from .utilities import check_attrs, timing
 
 
 def quick_integrate(
     function: _ftype,
     evals: int,
     tot_iters: int,
     bounds: Union[Sequence[tuple[float, float]], tuple[float, float]],
```

### Comparing `control-vegas-1.2.0/src/control_vegas/functions.py` & `control-vegas-1.3.0/src/control_vegas/functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -170,17 +170,17 @@
     mu: float = 0.5
     sigma: float = 0.2
     name: str = field(default="{}D Gaussian", init=False)
 
     def __post_init__(self):
         super().__post_init__()
         if self.mu > 1 or self.mu < 0:
-            raise """
-                Mean must be between the bounds [0, 1]. Currently set at {self.mu}.
-            """ from ParameterBoundError
+            raise ParameterBoundError(
+                f"Mean must be between the bounds [0, 1]. Currently set at {self.mu}."
+            ) from None
 
         self.true_value = (
             (erf((1 - self.mu) / self.sigma) + erf(self.mu / self.sigma)) / 2
         ) ** self.dim
         self.name = self.name.format(self.dim)
 
     @batchintegrand
@@ -206,21 +206,21 @@
     mu2: float = 2 / 3
     sigma: float = 0.2
     name: str = field(default="{}D Camel", init=False)
 
     def __post_init__(self):
         super().__post_init__()
         if self.mu1 > 1 or self.mu1 < 0:
-            raise f"""
-                First mean must be between [0, 1]. Currently set at {self.mu1}.
-            """ from ParameterBoundError
+            raise ParameterBoundError(
+                f"First mean must be between [0, 1]. Currently set at {self.mu1}."
+            ) from None
         if self.mu2 > 1 or self.mu2 < 0:
-            raise f"""
-                Second mean must be between [0, 1]. Currently set at {self.mu2}.
-            """ from ParameterBoundError
+            raise ParameterBoundError(
+                f"Second mean must be between [0, 1]. Currently set at {self.mu2}."
+            ) from None
 
         self.true_value = (
             (
                 erf((1 - self.mu1) / self.sigma)
                 + erf(self.mu1 / self.sigma)
                 + erf((1 - self.mu2) / self.sigma)
                 + erf(self.mu2 / self.sigma)
@@ -234,54 +234,109 @@
         norm_factor = 1 / (2 * (self.sigma * np.sqrt(np.pi)) ** (self.dim))
         exp1 = -np.sum((x - self.mu1) ** 2, axis=1) / self.sigma**2
         exp2 = -np.sum((x - self.mu2) ** 2, axis=1) / self.sigma**2
         return norm_factor * (np.exp(exp1) + np.exp(exp2))
 
 
 @dataclass(repr=False)
-class NPolynomial(Function):
+class EntangledCircles(Function):
     """
-    N-dimensional Polynomial of the form: sum of -x_i^2 + x_i.
+    A function of two shifted circles. True value depends on default values.
 
     Parameters:
-    dimension - Dimension of Polynomial
+    p1, p2 (defaults 0.4, 0.6) - Shifts of the two variables
+    r (default 0.25) - Radius
+    w, a (default 1/0.004, 3)
     """
 
-    name: str = field(default="{}D Polynomial", init=False)
+    p1: float = 0.4
+    p2: float = 0.6
+    r: float = 0.25
+    w: float = 1 / 0.004
+    a: float = 3
+    dimension: int = field(default=2, init=False)
+    name: str = field(default="Entangled Circles", init=False)
 
     def __post_init__(self):
         super().__post_init__()
-        self.true_value = self.dim / 6
-        self.name = self.name.format(self.dim)
+        self.true_value = 0.01368
 
-    @staticmethod
     @batchintegrand
-    def _function(x: _x) -> _f:
-        return np.sum(-(x**2) + x, axis=1)
+    def _function(self, x: _x) -> _f:
+        x1 = x[:, 0]
+        x2 = x[:, 1]
+        exp1 = np.exp(
+            -self.w * abs((x2 - self.p2) ** 2 + (x1 - self.p1) ** 2 - self.r**2)
+        )
+        exp2 = np.exp(
+            -self.w
+            * abs((x2 - 1 + self.p2) ** 2 + (x1 - 1 + self.p1) ** 2 - self.r**2)
+        )
+        return x2**self.a * exp1 + (1 - x2) ** self.a * exp2
+
+
+@dataclass(repr=False)
+class AnnulusWCuts(Function):
+    """
+    An annulus with hard cuts
+
+    Parameters:
+    rmin - Radius of inner circle
+    rmax - Radius of outer circle
+    """
+
+    rmin: float = 0.2
+    rmax: float = 0.45
+    dimension: int = field(default=2, init=False)
+    name: str = field(default="Annulus with Cuts", init=False)
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.rminsq = self.rmin**2
+        self.rmaxsq = self.rmax**2
+        if self.rmin < 0:
+            raise ParameterBoundError(
+                f"Minimum radius must be positive. Currently set at {self.rmin}."
+            ) from None
+        if self.rmax < 0:
+            raise ParameterBoundError(
+                f"Maximum radius must be positive. Currently set at {self.rmax}."
+            ) from None
+        if self.rmin > self.rmax:
+            raise ParameterBoundError(
+                "Minimum radius must be less than maximum radius but they are "
+                + f"{self.rmin} and {self.rmax} currently."
+            ) from None
+        self.true_value = np.pi / 4 * (self.rmax**2 - self.rmin**2)
+
+    @batchintegrand
+    def _function(self, x: _x) -> _f:
+        dist = x[:, 0] ** 2 + x[:, 1] ** 2
+        return np.logical_and(dist > self.rminsq, dist < self.rmaxsq).astype(float)
 
 
 @dataclass(repr=False)
 class ScalarTopLoop(Function):
     """
-    A one-loop scalar box integral.
+    A one-loop scalar box integral. True value depends on default values.
 
     Parameters:
     s12, s23, s1, s2, s3, s4 (defaults 130**2, -130**2, 0, 0, 0, 125**2) =
         Parameters of function
     mtsq (default 173.9**2) - Square of top quark mass
     """
 
     s12: float = 130**2
     s23: float = -(130**2) / 2
     s1: float = 0
     s2: float = 0
     s3: float = 0
     s4: float = 125**2
     mtsq: float = 173.9**2
-    dimension: int = 3
+    dimension: int = field(default=3, init=False)
     name: str = field(default="Scalar Top Loop", init=False)
 
     def __post_init__(self):
         super().__post_init__()
         self.true_value = 1.93741e-10
 
     def _Fbox(self, x, s12, s23, s1, s2, s3, s4):
@@ -304,7 +359,29 @@
     def _function(self, x: _x) -> _f:
         return (
             self._Sbox(x, self.s12, self.s23, self.s1, self.s2, self.s3, self.s4)
             + self._Sbox(x, self.s23, self.s12, self.s2, self.s3, self.s4, self.s1)
             + self._Sbox(x, self.s12, self.s23, self.s3, self.s4, self.s1, self.s2)
             + self._Sbox(x, self.s23, self.s12, self.s4, self.s1, self.s2, self.s3)
         )
+
+
+@dataclass(repr=False)
+class NPolynomial(Function):
+    """
+    N-dimensional Polynomial of the form: sum of -x_i^2 + x_i.
+
+    Parameters:
+    dimension - Dimension of Polynomial
+    """
+
+    name: str = field(default="{}D Polynomial", init=False)
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.true_value = self.dim / 6
+        self.name = self.name.format(self.dim)
+
+    @staticmethod
+    @batchintegrand
+    def _function(x: _x) -> _f:
+        return np.sum(-(x**2) + x, axis=1)
```

### Comparing `control-vegas-1.2.0/src/control_vegas.egg-info/PKG-INFO` & `control-vegas-1.3.0/src/control_vegas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-vegas
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Control Variate wrapper over the vegas python package.
 Author-email: Jacob Scott <jscott137@pm.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

