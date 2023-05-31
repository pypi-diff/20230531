# Comparing `tmp/ilib-0.1.tar.gz` & `tmp/ilib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilib-0.1.tar", last modified: Tue May 30 20:59:04 2023, max compression
+gzip compressed data, was "ilib-0.1.1.tar", last modified: Wed May 31 04:18:26 2023, max compression
```

## Comparing `ilib-0.1.tar` & `ilib-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-30 20:59:04.097305 ilib-0.1/
--rw-r--r--   0 devinthakker   (501) staff       (20)     1069 2023-05-30 17:52:43.000000 ilib-0.1/LICENSE
--rw-r--r--   0 devinthakker   (501) staff       (20)      598 2023-05-30 20:59:04.097416 ilib-0.1/PKG-INFO
--rw-r--r--   0 devinthakker   (501) staff       (20)     2098 2023-05-30 18:38:47.000000 ilib-0.1/README.md
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-30 20:59:04.096018 ilib-0.1/ilib/
--rw-r--r--   0 devinthakker   (501) staff       (20)     2014 2023-05-30 16:10:37.000000 ilib-0.1/ilib/BollingerBands.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2040 2023-05-30 16:09:57.000000 ilib-0.1/ilib/CCI.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1810 2023-05-29 23:50:04.000000 ilib-0.1/ilib/EMA.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     3184 2023-05-30 16:13:12.000000 ilib-0.1/ilib/MACD.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1923 2023-05-30 16:14:32.000000 ilib-0.1/ilib/RSI.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1159 2023-05-30 16:16:06.000000 ilib-0.1/ilib/SMA.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      149 2023-05-30 20:29:37.000000 ilib-0.1/ilib/__init__.py
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-30 20:59:04.096975 ilib-0.1/ilib.egg-info/
--rw-r--r--   0 devinthakker   (501) staff       (20)      598 2023-05-30 20:59:04.000000 ilib-0.1/ilib.egg-info/PKG-INFO
--rw-r--r--   0 devinthakker   (501) staff       (20)      276 2023-05-30 20:59:04.000000 ilib-0.1/ilib.egg-info/SOURCES.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)        1 2023-05-30 20:59:04.000000 ilib-0.1/ilib.egg-info/dependency_links.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)       13 2023-05-30 20:59:04.000000 ilib-0.1/ilib.egg-info/requires.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)        5 2023-05-30 20:59:04.000000 ilib-0.1/ilib.egg-info/top_level.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)       79 2023-05-30 20:59:04.097985 ilib-0.1/setup.cfg
--rw-r--r--   0 devinthakker   (501) staff       (20)      905 2023-05-30 20:58:34.000000 ilib-0.1/setup.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 04:18:26.184277 ilib-0.1.1/
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1069 2023-05-30 17:52:43.000000 ilib-0.1.1/LICENSE
+-rw-r--r--   0 devinthakker   (501) staff       (20)      602 2023-05-31 04:18:26.184406 ilib-0.1.1/PKG-INFO
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2366 2023-05-31 03:59:09.000000 ilib-0.1.1/README.md
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 04:18:26.182912 ilib-0.1.1/ilib/
+-rw-r--r--   0 devinthakker   (501) staff       (20)     4476 2023-05-31 04:15:02.000000 ilib-0.1.1/ilib/ADX.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2296 2023-05-31 03:54:59.000000 ilib-0.1.1/ilib/ATR.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2014 2023-05-30 16:10:37.000000 ilib-0.1.1/ilib/BOLLINGERBANDS.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2431 2023-05-30 22:30:49.000000 ilib-0.1.1/ilib/CCI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1810 2023-05-29 23:50:04.000000 ilib-0.1.1/ilib/EMA.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3194 2023-05-31 03:55:36.000000 ilib-0.1.1/ilib/MACD.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1937 2023-05-31 03:55:51.000000 ilib-0.1.1/ilib/RSI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1159 2023-05-30 16:16:06.000000 ilib-0.1.1/ilib/SMA.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2723 2023-05-31 04:07:30.000000 ilib-0.1.1/ilib/STOCHOSCILLATOR.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2738 2023-05-31 04:10:04.000000 ilib-0.1.1/ilib/VWAP.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      260 2023-05-31 04:00:43.000000 ilib-0.1.1/ilib/__init__.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 04:18:26.184116 ilib-0.1.1/ilib.egg-info/
+-rw-r--r--   0 devinthakker   (501) staff       (20)      602 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/PKG-INFO
+-rw-r--r--   0 devinthakker   (501) staff       (20)      360 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/SOURCES.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)        1 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/dependency_links.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)       13 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/requires.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)        5 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/top_level.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)       79 2023-05-31 04:18:26.184960 ilib-0.1.1/setup.cfg
+-rw-r--r--   0 devinthakker   (501) staff       (20)      909 2023-05-31 04:17:43.000000 ilib-0.1.1/setup.py
```

### Comparing `ilib-0.1/LICENSE` & `ilib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ilib-0.1/PKG-INFO` & `ilib-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ilib
-Version: 0.1
+Version: 0.1.1
 Summary: A package for various technical indicators
 Home-page: https://github.com/devthakker/ilib
-Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.1.1.tar.gz
 Author: Devin Thakker
 Author-email: devin.thakker@outlook.com
 License: MIT
 Keywords: ilib,technical indicators,finance,trading,stocks,crypto
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
```

### Comparing `ilib-0.1/README.md` & `ilib-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 ![preview](preview.jpg)
 
 ILIB is a library of technical indicators that can be used to build trading strategies. It is written in Python and uses the [Pandas](https://pandas.pydata.org/docs/) and [Numpy](https://numpy.org/doc/stable/) library for data manipulation and [Matplotlib](https://matplotlib.org/) for charting.
 
 [![Python](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/downloads/release/python-370/)
 [![PyPI](https://img.shields.io/pypi/v/ilib)](https://pypi.org/project/ilib/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/ilib)](https://pypi.org/project/ilib/)
-![GitHub](https://img.shields.io/github/license/rohitgupta-iitm/ilib)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ilib)](https://img.shields.io/github/downloads/devthakker/ilib/total.svg)
+![GitHub](https://img.shields.io/github/license/devthakker/ilib)
 
 ## Features
 
 - Implements various popular technical indicators for financial analysis.
 - Simple and intuitive API for easy integration into your trading systems.
 - Supports Python 3.7 and above.
 - Well-documented codebase and example usage for each indicator.
@@ -21,21 +21,24 @@
 
 ```bash
 pip install ilib
 ```
 
 ## Available Indicators
 
+- [x] [Average True Range](https://www.investopedia.com/terms/a/atr.asp)
+- [x] [Average Directional Index](https://www.investopedia.com/terms/a/adx.asp)
 - [x] [Bollinger Bands](https://www.investopedia.com/terms/b/bollingerbands.asp)
 - [x] [Commodity Channel Index](https://www.investopedia.com/terms/c/commoditychannelindex.asp)
 - [x] [Exponential Moving Average](https://www.investopedia.com/terms/e/ema.asp)
 - [x] [Moving Average Convergence Divergence](https://www.investopedia.com/terms/m/macd.asp)
 - [x] [Relative Strength Index](https://www.investopedia.com/terms/r/rsi.asp)
 - [x] [Simple Moving Average](https://www.investopedia.com/terms/s/sma.asp)
 - [x] [Stochastic Oscillator](https://www.investopedia.com/terms/s/stochasticoscillator.asp)
+- [x] [Volume Weighted Average Price](https://www.investopedia.com/terms/v/vwap.asp)
 
 ## Usage
 
 ```python
 import ilib as ti
 
 #data
```

### Comparing `ilib-0.1/ilib/BollingerBands.py` & `ilib-0.1.1/ilib/BOLLINGERBANDS.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1/ilib/CCI.py` & `ilib-0.1.1/ilib/CCI.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,27 @@
         typical_prices = [(high + low + close) / 3 for high, low, close in zip(self.data, self.data, self.data)]
         sma = sum(typical_prices[:self.period]) / self.period
         mean_deviations = [abs(typical_price - sma) for typical_price in typical_prices]
         mda = sum(mean_deviations[:self.period]) / self.period
 
         self.cci = [(typical_price - sma) / (0.015 * mda) for typical_price in typical_prices]
         
+    def add_data_point(self, price):
+        """
+        Add a new price to the data list and recalculate the CCI.
+        
+        Parameters:
+            price (float): The latest price.
+        Returns:
+            null: The CCI is stored in the cci attribute.
+        """
+        self.data.append(price)
+        if len(self.data) > self.period:
+            self.calculate_cci()
+        
     def get_cci(self):
         """Return the current CCI value.
 
         Returns:
             float: The current CCI value.
         """
         return self.cci[-1]
```

### Comparing `ilib-0.1/ilib/EMA.py` & `ilib-0.1.1/ilib/EMA.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1/ilib/MACD.py` & `ilib-0.1.1/ilib/MACD.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,25 +63,27 @@
         alpha = 2 / (period + 1)
 
         for i in range(1, len(prices)):
             ema[i] = alpha * prices[i] + (1 - alpha) * ema[i - 1]
 
         return ema
     
-    def get_lines(self):
-        """
-        Returns:
-            tuple: The calculated MACD line, signal line, and MACD histogram.
-        """
-        return self.macd_line[-1], self.signal_line[-1], self.macd_histogram[-1]
-    
     def add_data_point(self, data_point):
         """
         Add a new data point to the existing data and recalculate the MACD line, signal line, and MACD histogram.
         
         Parameters:
             data_point (float or int): The new data point to be added.
         """
         np.append(self.data, data_point)
         if len(self.data) > self.long_period:
-            self.calculate_macd()        
+            self.calculate_macd()    
+    
+    def get_lines(self):
+        """
+        Returns:
+            tuple: The calculated MACD line, signal line, and MACD histogram.
+        """
+        return self.macd_line[-1], self.signal_line[-1], self.macd_histogram[-1]
+    
+
```

### Comparing `ilib-0.1/ilib/RSI.py` & `ilib-0.1.1/ilib/RSI.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,22 +18,14 @@
         if data is None:
             self.data = []
         else:
             self.data = data
             if len(self.data) > self.period:
                 self.calculate_rsi()
 
-    def add_data(self, value):
-        """
-        Add a new price to the data list and calculate the new RSI.
-        """
-        self.data.append(value)
-        if(len(self.data) > self.period):
-            self.calculate_rsi()
-
     def calculate_rsi(self):
         """
         Calculate the RSI of the stock based on its historical price data.
         """
         if len(self.data) <= self.period:
             raise ValueError("Insufficient data to calculate RSI.")
 
@@ -58,13 +50,21 @@
         if avg_loss == 0:
             return 100
 
         rs = avg_gain / avg_loss
         rsi = 100 - (100 / (1 + rs))
         self.rsi = rsi
         
+    def add_data_point(self, value):
+        """
+        Add a new price to the data list and calculate the new RSI.
+        """
+        self.data.append(value)
+        if(len(self.data) > self.period):
+            self.calculate_rsi()
+        
     def get_rsi(self):
         """
         Return the current RSI value."""
         return self.rsi
```

### Comparing `ilib-0.1/ilib/SMA.py` & `ilib-0.1.1/ilib/SMA.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1/ilib.egg-info/PKG-INFO` & `ilib-0.1.1/ilib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ilib
-Version: 0.1
+Version: 0.1.1
 Summary: A package for various technical indicators
 Home-page: https://github.com/devthakker/ilib
-Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.1.1.tar.gz
 Author: Devin Thakker
 Author-email: devin.thakker@outlook.com
 License: MIT
 Keywords: ilib,technical indicators,finance,trading,stocks,crypto
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
```

### Comparing `ilib-0.1/setup.py` & `ilib-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup( 
         name='ilib',
-        version='0.1',
+        version='0.1.1',
         # packages=find_packages(exclude=['tests*']),
         packages=find_packages(),
         license='MIT',
         description='A package for various technical indicators',
         install_requires=['numpy', 'pandas'],
         author='Devin Thakker',
         author_email='devin.thakker@outlook.com',
         url='https://github.com/devthakker/ilib',
-        download_url='https://github.com/devthakker/ilib/archive/refs/tags/v0.1.tar.gz',
+        download_url='https://github.com/devthakker/ilib/archive/refs/tags/v0.1.1.tar.gz',
         keywords=['ilib', 'technical indicators', 'finance', 'trading', 'stocks', 'crypto'],
         classifiers=[
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python :: 3.7',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: MIT License',
             ],
```

