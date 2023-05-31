# Comparing `tmp/pyrothc-0.0.2.tar.gz` & `tmp/pyRothC-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pyRothC-0.0.3.tar", last modified: Wed May 31 20:26:20 2023, max compression
```

## Comparing `pyrothc-0.0.2.tar` & `pyRothC-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,30 @@
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pyrothc-0.0.2/setup.py
--rw-r--r--   0        0        0    19832 2020-02-02 00:00:00.000000 pyrothc-0.0.2/notebooks/pyRothC.ipynb
--rw-r--r--   0        0        0    16308 2020-02-02 00:00:00.000000 pyrothc-0.0.2/plots/Logo.svg
--rw-r--r--   0        0        0    50344 2020-02-02 00:00:00.000000 pyrothc-0.0.2/plots/moisture_factor.png
--rw-r--r--   0        0        0    45995 2020-02-02 00:00:00.000000 pyrothc-0.0.2/plots/soil_clay_factor.png
--rw-r--r--   0        0        0    68569 2020-02-02 00:00:00.000000 pyrothc-0.0.2/plots/temp_factor.png
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 pyrothc-0.0.2/pyRothC/RothC.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrothc-0.0.2/pyRothC/__init__.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 pyrothc-0.0.2/.gitignore
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 pyrothc-0.0.2/LICENSE
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 pyrothc-0.0.2/README.md
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 pyrothc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 pyrothc-0.0.2/PKG-INFO
+drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.857877 pyRothC-0.0.3/
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)     1834 2023-05-31 20:17:09.000000 pyRothC-0.0.3/.gitignore
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)     7048 2022-10-29 10:17:12.000000 pyRothC-0.0.3/LICENSE
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)    12953 2023-05-31 20:26:20.856849 pyRothC-0.0.3/PKG-INFO
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)     3816 2023-05-31 20:17:09.000000 pyRothC-0.0.3/README.md
+drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.843214 pyRothC-0.0.3/notebooks/
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)    73445 2023-03-05 20:21:46.000000 pyRothC-0.0.3/notebooks/pyRothC.ipynb
+drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.846913 pyRothC-0.0.3/plots/
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)    16308 2023-03-04 11:17:28.000000 pyRothC-0.0.3/plots/Logo.svg
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)    50344 2023-03-02 11:58:47.000000 pyRothC-0.0.3/plots/moisture_factor.png
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)    45995 2023-03-02 11:59:35.000000 pyRothC-0.0.3/plots/soil_clay_factor.png
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)    68569 2023-03-02 11:58:17.000000 pyRothC-0.0.3/plots/temp_factor.png
+drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.848395 pyRothC-0.0.3/pyRothC/
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)    10905 2023-05-31 20:17:09.000000 pyRothC-0.0.3/pyRothC/RothC.py
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)        0 2023-03-04 12:14:32.000000 pyRothC-0.0.3/pyRothC/__init__.py
+drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.851878 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)    12953 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/PKG-INFO
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)      483 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)        1 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)       56 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/requires.txt
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)        1 2023-05-31 20:26:20.000000 pyRothC-0.0.3/pyRothC/pyRothC.egg-info/top_level.txt
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)     1356 2023-05-31 20:24:07.000000 pyRothC-0.0.3/pyproject.toml
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)       38 2023-05-31 20:26:20.858074 pyRothC-0.0.3/setup.cfg
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)       38 2023-03-04 10:37:19.000000 pyRothC-0.0.3/setup.py
+drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.854342 pyRothC-0.0.3/tests/
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:17:09.000000 pyRothC-0.0.3/tests/__init__.py
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)      261 2023-05-31 20:17:09.000000 pyRothC-0.0.3/tests/conftest.py
+drwxr-xr-x   0 mikhailgasanov   (501) staff       (20)        0 2023-05-31 20:26:20.855374 pyRothC-0.0.3/tests/data/
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)     2269 2023-05-31 20:17:09.000000 pyRothC-0.0.3/tests/data/2years_results.csv
+-rw-r--r--   0 mikhailgasanov   (501) staff       (20)      919 2023-05-31 20:17:09.000000 pyRothC-0.0.3/tests/test_rothc.py
```

### Comparing `pyrothc-0.0.2/plots/Logo.svg` & `pyRothC-0.0.3/plots/Logo.svg`

 * *Files identical despite different names*

### Comparing `pyrothc-0.0.2/plots/moisture_factor.png` & `pyRothC-0.0.3/plots/moisture_factor.png`

 * *Files identical despite different names*

### Comparing `pyrothc-0.0.2/plots/soil_clay_factor.png` & `pyRothC-0.0.3/plots/soil_clay_factor.png`

 * *Files identical despite different names*

### Comparing `pyrothc-0.0.2/plots/temp_factor.png` & `pyRothC-0.0.3/plots/temp_factor.png`

 * *Files identical despite different names*

### Comparing `pyrothc-0.0.2/pyRothC/RothC.py` & `pyRothC-0.0.3/pyRothC/RothC.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     Author: Misha Grol - grol81@mail.ru
     """
 from typing import Union, Tuple
 import numpy as np
 import pandas as pd
 from scipy.integrate import odeint
 from scipy.interpolate import interp1d
-import matplotlib.pyplot as plt
 
 
 class RothC:
     """Class for Python version of The Rothamsted carbon model (RothC) 26.3."""
 
     def __init__(
         self,
@@ -31,19 +30,19 @@
         pE: float = 0.75,
         bare: bool = False,
         solver: str = "euler",
     ):
         """Python version of The Rothamsted carbon model (RothC) 26.3.
 
         Args:
-            temperature (Union[list, np.ndarray]): Values of montly temperature
+            temperature (Union[list, np.ndarray]): Values of monthly temperature
                                                 for which the effects on decomposition rates are calculated (°C).
-            precip (Union[list, np.ndarray]): Values of montly precipitaion
+            precip (Union[list, np.ndarray]): Values of monthly precipitaion
                                                 for which the effects on decomposition rates are calculated (mm).
-            evaporation (Union[list, np.ndarray]): Values of montly open pan evaporation or evapotranspiration (mm).
+            evaporation (Union[list, np.ndarray]): Values of monthly open pan evaporation or evapotranspiration (mm).
             years (int, optional): Number of years to run RothC model. Defaults to 500.
             ks (np.ndarray, optional): A vector of length 5 containing the values of the
                                     decomposition rates for the different pools.
                                     Defaults to np.array([10, 0.3, 0.66, 0.02, 0]).
             C0 (np.ndarray, optional): A numpy of length 5 containing the initial amount
                                         of carbon for the 5 pools. Defaults to np.array([0, 0, 0, 0, 2.7]).
             input_carbon (Union[float, np.ndarray], optional): A scalar or np.array
@@ -96,21 +95,21 @@
 
     def _get_stress_parameters(
         self, temperature: np.ndarray, precip: np.ndarray, evaporation: np.ndarray
     ) -> np.ndarray:
         """Compute decomposition impact of Temperature and Moisture (fT * fW)
 
         Args:
-            temperature (np.ndarray): Values of montly temperature
+            temperature (np.ndarray): Values of monthly temperature
                                     for which the effects on decomposition
                                     rates are calculated (°C).
-            precip (np.ndarray): Values of montly precipitaion
+            precip (np.ndarray): Values of monthly precipitaion
                                 for which the effects on
                                 decomposition rates are calculated (mm).
-            evaporation (np.ndarray): Values of montly open pan evaporation or evapotranspiration (mm).
+            evaporation (np.ndarray): Values of monthly open pan evaporation or evapotranspiration (mm).
 
         Returns:
             np.ndarray: Effects of moisture and temperature
                         on decomposition rates according to the RothC model.
         """
 
         stress_temp = self.fT(temperature=temperature)
@@ -128,18 +127,18 @@
         xi = np.tile(xi, self.years)
         return xi
 
     def fT(self, temperature: np.ndarray) -> list:
         """Compute Temperature factor
 
         Args:
-            temperature (np.ndarray): montly mean temperature
+            temperature (np.ndarray): monthly mean temperature
 
         Returns:
-            list: montly temperature factor
+            list: monthly temperature factor
         """
         stress_coef = []
         for x in temperature:
             if x < -18.3:
                 stress_coef.append(np.nan)
             else:
                 stress_coef.append(47.9 / (1 + np.exp(106 / (x + 18.3))))
@@ -153,18 +152,18 @@
         pE: float = 0.75,
         clay: float = 20.0,
         bare: bool = False,
     ) -> Tuple[np.ndarray, np.ndarray]:
         """Compute Soil moisture factor
 
         Args:
-            precip (np.ndarray): Values of montly precipitaion
+            precip (np.ndarray): Values of monthly precipitaion
                                 for which the effects on 
                                 decomposition rates are calculated (mm).
-            evaporation (np.ndarray): Values of montly open pan evaporation or evapotranspiration (mm).
+            evaporation (np.ndarray): Values of monthly open pan evaporation or evapotranspiration (mm).
             soil_thickness (float): Soil thickness in cm. Default for Rothamsted is 23 cm.
             pE (float, optional): Evaporation coefficient.
                                 If open pan evaporation is used pE=0.75.
                                 If Potential evaporation is used, pE=1.0.. Defaults to 0.75.
             clay (float, optional): Percent clay in mineral soil. Defaults to 23.4.
                                  Defaults to 20.0.
             bare (bool, optional): Logical. Under bare soil conditions, bare=True.
@@ -172,16 +171,16 @@
                                 Defaults to False.
 
         Raises:
             ValueError: Precip and evaporation have different shape
 
         Returns:
             Tuple[np.ndarray, np.ndarray]: _description_
-        """ """"""
-        # compute maximum soil moisture defficit
+        """
+        # compute maximum soil moisture deficit
         if precip.shape != evaporation.shape:
             raise ValueError("Precip and evaporation have different shape")
         #     max_smd = -(20.0 + 1.3 * clay - 0.01 * clay**2)
         max_smd = -(20.0 + 1.3 * clay - 0.01 * clay**2) * (
             soil_thickness / 23
         )  # TO-DO Verify this soil_thik / 23
         if bare:
@@ -247,54 +246,8 @@
         xi_f = self.xi_func(t)
         self._current_XI.append(xi_f)
         C_next = in_flux + (A * xi_f).dot(C)
         return C_next
 
     def compute(self):
         y1 = odeint(self.dCdt, self.C0, t=self.t, rtol=0.01, atol=0.01)
-        self.df = pd.DataFrame(y1, columns=self.ks_pulls)
-        return self.df
-
-    def plot(self):
-        fig, ax = plt.subplots(1, 1, figsize=(12, 8))
-        self.df.plot(ax=ax)
-        ax.set_ylabel("C stocks (Mg/ha)")
-        plt.show()
-
-
-def test():
-    """Test pyRothC model"""
-
-    Temp = np.array([-0.4, 0.3, 4.2, 8.3, 13.0, 15.9, 18.0, 17.5, 13.4, 8.7, 3.9, 0.6])
-    Precip = np.array([49, 39, 44, 41, 61, 58, 71, 58, 51, 48, 50, 58])
-    Evp = np.array([12, 18, 35, 58, 82, 90, 97, 84, 54, 31, 14, 10])
-
-    soil_thick = 25  # Soil thickness (organic layer topsoil), in cm
-    SOC = 69.7  # Soil organic carbon in Mg/ha
-    clay = 48  # Percent clay
-    Cinputs = 2.7  # Annual C inputs to soil in Mg/ha/yr
-
-    rothC = RothC(
-        temperature=Temp,
-        precip=Precip,
-        evaporation=Evp,
-        clay=48,
-        input_carbon=Cinputs,
-        pE=1.0,
-        C0=np.array([0, 0, 0, 0, 2.7]),
-    )
-
-    y1 = odeint(rothC.dCdt, rothC.C0, t=rothC.t, rtol=0.01, atol=0.01)
-    df = pd.DataFrame(y1, columns=rothC.ks_pulls)
-    print("test passed - ✅")
-    fig, ax = plt.subplots(1, 1, figsize=(12, 8))
-    df.plot(ax=ax)
-    ax.set_ylabel("C stocks (Mg/ha)")
-    plt.show()
-
-
-if __name__ == "__main__":
-    try:
-        test()
-    except Exception as e:
-        print(e)
-        print("test not passed - ❌")
+        return pd.DataFrame(y1, columns=self.ks_pulls)
```

### Comparing `pyrothc-0.0.2/.gitignore` & `pyRothC-0.0.3/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -123,7 +123,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# Jetbrains PyCharm
+.idea/
```

### Comparing `pyrothc-0.0.2/LICENSE` & `pyRothC-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrothc-0.0.2/README.md` & `pyRothC-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,35 @@
+## pyRothC
 <p align="center">
-<!-- <a href="https://github.com/tiangolo/fastapi/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
-    <img src="https://github.com/tiangolo/fastapi/workflows/Test/badge.svg?event=push&branch=master" alt="Test">
-</a>
-<a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/fastapi" target="_blank">
-    <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/fastapi.svg" alt="Coverage">
-</a> -->
-<!-- <a href="https://pypi.org/project/fastapi" target="_blank">
-    <img src="https://img.shields.io/pypi/v/fastapi?color=%2334D058&label=pypi%20package" alt="Package version"> -->
-<!-- </a>
-<a href="https://pypi.org/project/fastapi" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/fastapi.svg?color=%2334D058" alt="Supported Python versions">
-</a> -->
-
 <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/mishagrol/pyRothC?style=social">
 
 <a href="https://github.com/mishagrol/pyRothC/issues" target="_blank">
     <img src="https://img.shields.io/github/issues/mishagrol/pyRothC" alt="Issues">
 </a>
 
 
-
 <a href="https://github.com/mishagrol/pyRothC/blob/main/LICENSE" target="_blank">
     <img src="https://img.shields.io/github/license/mishagrol/pyRothC" alt="License">
 </a>
 </p>
 
-## pyRothC
 
 <p align="left">
     <em>Python version of The Rothamsted carbon model (RothC) 26.3.</em>
 </p>
 
 ________
 **Documentation**: <a href="https://www.rothamsted.ac.uk/sites/default/files/RothC_guide_DOS.pdf" target="_blank">Rothamsted RothC Model</a>
 
 **Source Code**: <a href="https://github.com/mishagrol/pyRothC" target="_blank">https://github.com/mishagrol/pyRothC</a>
 
 ---
 
 pyRothc is a Python version of The Rothamsted carbon model (RothC) 26.3.
 
-
 RothC is a model for the turnover of organic carbon in non-waterlogged topsoil that allows for the effects of soil type, temperature, soil moisture and plant cover on the turnover process.
 
 Inspired by SoilR version <a href="https://www.bgc-jena.mpg.de/TEE/basics/2015/11/19/RothC/" target="_blank">SoilR RothC</a>
 
 ## Requirements
 
 Python 3.7+
@@ -63,57 +48,81 @@
 $ pip install pyRothC
 ```
 
 </div>
 
 ## Example
 
+Below is an example of how the `RothC` class should be used. It needs 
+[matplotlib](https://matplotlib.org/stable/users/installing/index.html) library to be installed in
+order to draw the graphs.
+
 
 ```Python
+import numpy as np
+import matplotlib.pyplot as plt
 
-Temp=np.array([-0.4, 0.3, 4.2, 8.3, 13.0, 15.9,18.
-                0, 17.5, 13.4, 8.7, 3.9,  0.6])
-Precip=np.array([49, 39, 44, 41, 61, 58, 71, 58, 
-                51,48, 50, 58])
-Evp=np.array([12, 18, 35, 58, 82, 90, 97, 84, 54,
-                31,14, 10])
+from pyRothC.RothC import RothC
 
-soil_thick=25  #Soil thickness (organic layer 
-                #topsoil), in cm
+
+Temp=np.array([-0.4, 0.3, 4.2, 8.3, 13.0, 15.9,18.0, 
+                17.5, 13.4, 8.7, 3.9,  0.6])
+Precip=np.array([49, 39, 44, 41, 61, 58,
+                71, 58, 51,48, 50, 58])
+Evp=np.array([12, 18, 35, 58, 82, 90,
+            97, 84, 54, 31,14, 10])
+
+soil_thick=25  #Soil thickness (organic layer topsoil), in cm
 SOC=69.7       #Soil organic carbon in Mg/ha 
 clay=48        #Percent clay
-Cinputs=2.7   #Annual C inputs to soil in Mg/ha/yr
+input_carbon=2.7   #Annual C inputs to soil in Mg/ha/yr
 
+IOM=0.049*SOC**(1.139) # Falloon et al. (1998)
 
 rothC = RothC(temperature=Temp, 
              precip=Precip, 
              evaporation=Evp,
              clay = 48,
-             input_carbon=Cinputs,
+             input_carbon=input_carbon,
              pE=1.0,
-             C0=np.array([0, 0, 0, 0, 2.7]))
+             C0=np.array([0, 0, 0, 0, IOM]))
 
 df = rothC.compute()
-
+df.index = rothC.t
 fig, ax = plt.subplots(1,1,figsize=(6,4))
 df.plot(ax=ax)
 ax.set_ylabel('C stocks (Mg/ha)')
+ax.set_ylabel('Years')
 plt.show()
+```
 
+## Testing
 
+If you need to run the test suite, first install the package in "editable" mode with the `test`
+optional dependencies:
+
+```bash
+git clone git@github.com:mishagrol/pyRothC.git
+cd pyRothC
+pip install -e ".[test]"
 ```
 
+Now you can run the tests by simply running this command:
+
+```bash
+pytest tests
+```
 
 ## Structure of the RothC model
 
 **Credits**: <a href="https://www.bgc-jena.mpg.de/TEE/software/bgc-md/soil/Jenkinson1977SoilScience-S0003/Report.html" target="_blank">Theoretical Ecosystem Ecology group of the Max Planck Institute for Biogeochemistry</a>
 
 
 <p align="center">
-  <a href="RothC"><img src="./plots/Logo.svg" alt="FastAPI"></a>
+  <a href="RothC"><img src="./plots/Logo.svg" alt="RothC"></a>
 </p>
 
 ### Equations
 
 $$
 \begin{aligned}
 & \frac{d \boldsymbol{C}}{\mathrm{d} t}=I\left(\begin{array}{c}
```

#### html2text {}

```diff
@@ -1,30 +1,39 @@
-                      [GitHub Repo stars] [Issues] [License]
 ## pyRothC
+                    [GitHub Repo stars] [Issues] [License]
 Python version of The Rothamsted carbon model (RothC) 26.3.
 ________ **Documentation**: Rothamsted_RothC_Model **Source Code**: https://
 github.com/mishagrol/pyRothC --- pyRothc is a Python version of The Rothamsted
 carbon model (RothC) 26.3. RothC is a model for the turnover of organic carbon
 in non-waterlogged topsoil that allows for the effects of soil type,
 temperature, soil moisture and plant cover on the turnover process. Inspired by
 SoilR version SoilR_RothC ## Requirements Python 3.7+ SciPy NumPy Pandas ##
 Installation
 ```console $ pip install pyRothC ```
-## Example ```Python Temp=np.array([-0.4, 0.3, 4.2, 8.3, 13.0, 15.9,18. 0,
-17.5, 13.4, 8.7, 3.9, 0.6]) Precip=np.array([49, 39, 44, 41, 61, 58, 71, 58,
-51,48, 50, 58]) Evp=np.array([12, 18, 35, 58, 82, 90, 97, 84, 54, 31,14, 10])
-soil_thick=25 #Soil thickness (organic layer #topsoil), in cm SOC=69.7 #Soil
-organic carbon in Mg/ha clay=48 #Percent clay Cinputs=2.7 #Annual C inputs to
-soil in Mg/ha/yr rothC = RothC(temperature=Temp, precip=Precip,
-evaporation=Evp, clay = 48, input_carbon=Cinputs, pE=1.0, C0=np.array([0, 0, 0,
-0, 2.7])) df = rothC.compute() fig, ax = plt.subplots(1,1,figsize=(6,4))
-df.plot(ax=ax) ax.set_ylabel('C stocks (Mg/ha)') plt.show() ``` ## Structure of
-the RothC model **Credits**: Theoretical_Ecosystem_Ecology_group_of_the_Max
-Planck_Institute_for_Biogeochemistry
-                                   [FastAPI]
+## Example Below is an example of how the `RothC` class should be used. It
+needs [matplotlib](https://matplotlib.org/stable/users/installing/index.html)
+library to be installed in order to draw the graphs. ```Python import numpy as
+np import matplotlib.pyplot as plt from pyRothC.RothC import RothC
+Temp=np.array([-0.4, 0.3, 4.2, 8.3, 13.0, 15.9,18.0, 17.5, 13.4, 8.7, 3.9,
+0.6]) Precip=np.array([49, 39, 44, 41, 61, 58, 71, 58, 51,48, 50, 58])
+Evp=np.array([12, 18, 35, 58, 82, 90, 97, 84, 54, 31,14, 10]) soil_thick=25
+#Soil thickness (organic layer topsoil), in cm SOC=69.7 #Soil organic carbon in
+Mg/ha clay=48 #Percent clay input_carbon=2.7 #Annual C inputs to soil in Mg/ha/
+yr IOM=0.049*SOC**(1.139) # Falloon et al. (1998) rothC = RothC
+(temperature=Temp, precip=Precip, evaporation=Evp, clay = 48,
+input_carbon=input_carbon, pE=1.0, C0=np.array([0, 0, 0, 0, IOM])) df =
+rothC.compute() df.index = rothC.t fig, ax = plt.subplots(1,1,figsize=(6,4))
+df.plot(ax=ax) ax.set_ylabel('C stocks (Mg/ha)') ax.set_ylabel('Years')
+plt.show() ``` ## Testing If you need to run the test suite, first install the
+package in "editable" mode with the `test` optional dependencies: ```bash git
+clone git@github.com:mishagrol/pyRothC.git cd pyRothC pip install -e ".[test]"
+``` Now you can run the tests by simply running this command: ```bash pytest
+tests ``` ## Structure of the RothC model **Credits**: Theoretical_Ecosystem
+Ecology_group_of_the_Max_Planck_Institute_for_Biogeochemistry
+                                    [RothC]
 ### Equations $$ \begin{aligned} & \frac{d \boldsymbol{C}}{\mathrm{d} t}=I\left
 (\begin{array}{c} \gamma \\ 1-\gamma \\ 0 \\ 0 \\ 0 \end{array}\right) +\left
 (\begin{array}{ccccc} -k_1 & 0 & 0 & 0 & 0 \\ 0 & -k_2 & 0 & 0 & 0 \\ a_{3,1} &
 a_{3,2} & -k_3+a_{3,3} & a_{3,4} & 0 \\ a_{4,1} & a_{4,2} & a_{4,3} & -k_4+a_
 {4,4} & 0 \\ 0 & 0 & 0 & 0 & 0 \end{array}\right)\left(\begin{array}{l} C_1 \\
 C_2 \\ C_3 \\ C_4 \\ C_5 \end{array}\right) \\ & \end{aligned} $$ ## Optional
 Dependencies Matplotlib ## License This project is licensed under the terms of
```

### Comparing `pyrothc-0.0.2/pyproject.toml` & `pyRothC-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.8.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyRothC"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python version of The Rothamsted carbon model (RothC) 26.3. RothC is a model for the turnover of organic carbon in non-waterlogged topsoil that allows for the effects of soil type, temperature, soil moisture and plant cover on the turnover process."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   { name = "Misha Grol", email = "grol81@mail.ru" }
 ]
@@ -29,14 +29,18 @@
 ]
 
 dependencies = [
   "numpy>=1.20.3",
   "pandas>=1.3.4",
   "scipy>=1.7.3"
 ]
+[project.optional-dependencies]
+test = [
+    "pytest"
+]
 
 [tool.setuptools.packages.find]
 
 where = ["pyRothC"]
 include = ["*"]
```

### Comparing `pyrothc-0.0.2/PKG-INFO` & `pyRothC-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: pyRothC
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python version of The Rothamsted carbon model (RothC) 26.3. RothC is a model for the turnover of organic carbon in non-waterlogged topsoil that allows for the effects of soil type, temperature, soil moisture and plant cover on the turnover process.
-Project-URL: Documentation, https://mishagrol.github.io
-Project-URL: Source code, https://github.com/mishagrol/pyRothC
 Author-email: Misha Grol <grol81@mail.ru>
 Maintainer: misha grol
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -123,74 +121,60 @@
             limitation any person's Copyright and Related Rights in the Work.
             Further, Affirmer disclaims responsibility for obtaining any necessary
             consents, permissions or other rights required for any use of the
             Work.
          d. Affirmer understands and acknowledges that Creative Commons is not a
             party to this document and has no duty or obligation with respect to
             this CC0 or use of the Work.
-License-File: LICENSE
+        
+Project-URL: Documentation, https://mishagrol.github.io
+Project-URL: Source code, https://github.com/mishagrol/pyRothC
 Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Requires-Dist: numpy>=1.20.3
-Requires-Dist: pandas>=1.3.4
-Requires-Dist: scipy>=1.7.3
 Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
 
+## pyRothC
 <p align="center">
-<!-- <a href="https://github.com/tiangolo/fastapi/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
-    <img src="https://github.com/tiangolo/fastapi/workflows/Test/badge.svg?event=push&branch=master" alt="Test">
-</a>
-<a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/fastapi" target="_blank">
-    <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/fastapi.svg" alt="Coverage">
-</a> -->
-<!-- <a href="https://pypi.org/project/fastapi" target="_blank">
-    <img src="https://img.shields.io/pypi/v/fastapi?color=%2334D058&label=pypi%20package" alt="Package version"> -->
-<!-- </a>
-<a href="https://pypi.org/project/fastapi" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/fastapi.svg?color=%2334D058" alt="Supported Python versions">
-</a> -->
-
 <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/mishagrol/pyRothC?style=social">
 
 <a href="https://github.com/mishagrol/pyRothC/issues" target="_blank">
     <img src="https://img.shields.io/github/issues/mishagrol/pyRothC" alt="Issues">
 </a>
 
 
-
 <a href="https://github.com/mishagrol/pyRothC/blob/main/LICENSE" target="_blank">
     <img src="https://img.shields.io/github/license/mishagrol/pyRothC" alt="License">
 </a>
 </p>
 
-## pyRothC
 
 <p align="left">
     <em>Python version of The Rothamsted carbon model (RothC) 26.3.</em>
 </p>
 
 ________
 **Documentation**: <a href="https://www.rothamsted.ac.uk/sites/default/files/RothC_guide_DOS.pdf" target="_blank">Rothamsted RothC Model</a>
 
 **Source Code**: <a href="https://github.com/mishagrol/pyRothC" target="_blank">https://github.com/mishagrol/pyRothC</a>
 
 ---
 
 pyRothc is a Python version of The Rothamsted carbon model (RothC) 26.3.
 
-
 RothC is a model for the turnover of organic carbon in non-waterlogged topsoil that allows for the effects of soil type, temperature, soil moisture and plant cover on the turnover process.
 
 Inspired by SoilR version <a href="https://www.bgc-jena.mpg.de/TEE/basics/2015/11/19/RothC/" target="_blank">SoilR RothC</a>
 
 ## Requirements
 
 Python 3.7+
@@ -209,57 +193,81 @@
 $ pip install pyRothC
 ```
 
 </div>
 
 ## Example
 
+Below is an example of how the `RothC` class should be used. It needs 
+[matplotlib](https://matplotlib.org/stable/users/installing/index.html) library to be installed in
+order to draw the graphs.
+
 
 ```Python
+import numpy as np
+import matplotlib.pyplot as plt
 
-Temp=np.array([-0.4, 0.3, 4.2, 8.3, 13.0, 15.9,18.
-                0, 17.5, 13.4, 8.7, 3.9,  0.6])
-Precip=np.array([49, 39, 44, 41, 61, 58, 71, 58, 
-                51,48, 50, 58])
-Evp=np.array([12, 18, 35, 58, 82, 90, 97, 84, 54,
-                31,14, 10])
+from pyRothC.RothC import RothC
 
-soil_thick=25  #Soil thickness (organic layer 
-                #topsoil), in cm
+
+Temp=np.array([-0.4, 0.3, 4.2, 8.3, 13.0, 15.9,18.0, 
+                17.5, 13.4, 8.7, 3.9,  0.6])
+Precip=np.array([49, 39, 44, 41, 61, 58,
+                71, 58, 51,48, 50, 58])
+Evp=np.array([12, 18, 35, 58, 82, 90,
+            97, 84, 54, 31,14, 10])
+
+soil_thick=25  #Soil thickness (organic layer topsoil), in cm
 SOC=69.7       #Soil organic carbon in Mg/ha 
 clay=48        #Percent clay
-Cinputs=2.7   #Annual C inputs to soil in Mg/ha/yr
+input_carbon=2.7   #Annual C inputs to soil in Mg/ha/yr
 
+IOM=0.049*SOC**(1.139) # Falloon et al. (1998)
 
 rothC = RothC(temperature=Temp, 
              precip=Precip, 
              evaporation=Evp,
              clay = 48,
-             input_carbon=Cinputs,
+             input_carbon=input_carbon,
              pE=1.0,
-             C0=np.array([0, 0, 0, 0, 2.7]))
+             C0=np.array([0, 0, 0, 0, IOM]))
 
 df = rothC.compute()
-
+df.index = rothC.t
 fig, ax = plt.subplots(1,1,figsize=(6,4))
 df.plot(ax=ax)
 ax.set_ylabel('C stocks (Mg/ha)')
+ax.set_ylabel('Years')
 plt.show()
+```
 
+## Testing
 
+If you need to run the test suite, first install the package in "editable" mode with the `test`
+optional dependencies:
+
+```bash
+git clone git@github.com:mishagrol/pyRothC.git
+cd pyRothC
+pip install -e ".[test]"
 ```
 
+Now you can run the tests by simply running this command:
+
+```bash
+pytest tests
+```
 
 ## Structure of the RothC model
 
 **Credits**: <a href="https://www.bgc-jena.mpg.de/TEE/software/bgc-md/soil/Jenkinson1977SoilScience-S0003/Report.html" target="_blank">Theoretical Ecosystem Ecology group of the Max Planck Institute for Biogeochemistry</a>
 
 
 <p align="center">
-  <a href="RothC"><img src="./plots/Logo.svg" alt="FastAPI"></a>
+  <a href="RothC"><img src="./plots/Logo.svg" alt="RothC"></a>
 </p>
 
 ### Equations
 
 $$
 \begin{aligned}
 & \frac{d \boldsymbol{C}}{\mathrm{d} t}=I\left(\begin{array}{c}
@@ -287,8 +295,8 @@
 $$
 ## Optional Dependencies
 
 Matplotlib
 
 ## License
 
-This project is licensed under the terms of the CC0 1.0 Universal license.
+This project is licensed under the terms of the CC0 1.0 Universal license.
```

