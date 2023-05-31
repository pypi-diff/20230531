# Comparing `tmp/ilib-0.1.1.tar.gz` & `tmp/ilib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilib-0.1.1.tar", last modified: Wed May 31 04:18:26 2023, max compression
+gzip compressed data, was "ilib-0.2.tar", last modified: Wed May 31 16:02:06 2023, max compression
```

## Comparing `ilib-0.1.1.tar` & `ilib-0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 04:18:26.184277 ilib-0.1.1/
--rw-r--r--   0 devinthakker   (501) staff       (20)     1069 2023-05-30 17:52:43.000000 ilib-0.1.1/LICENSE
--rw-r--r--   0 devinthakker   (501) staff       (20)      602 2023-05-31 04:18:26.184406 ilib-0.1.1/PKG-INFO
--rw-r--r--   0 devinthakker   (501) staff       (20)     2366 2023-05-31 03:59:09.000000 ilib-0.1.1/README.md
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 04:18:26.182912 ilib-0.1.1/ilib/
--rw-r--r--   0 devinthakker   (501) staff       (20)     4476 2023-05-31 04:15:02.000000 ilib-0.1.1/ilib/ADX.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2296 2023-05-31 03:54:59.000000 ilib-0.1.1/ilib/ATR.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2014 2023-05-30 16:10:37.000000 ilib-0.1.1/ilib/BOLLINGERBANDS.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2431 2023-05-30 22:30:49.000000 ilib-0.1.1/ilib/CCI.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1810 2023-05-29 23:50:04.000000 ilib-0.1.1/ilib/EMA.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     3194 2023-05-31 03:55:36.000000 ilib-0.1.1/ilib/MACD.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1937 2023-05-31 03:55:51.000000 ilib-0.1.1/ilib/RSI.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1159 2023-05-30 16:16:06.000000 ilib-0.1.1/ilib/SMA.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2723 2023-05-31 04:07:30.000000 ilib-0.1.1/ilib/STOCHOSCILLATOR.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2738 2023-05-31 04:10:04.000000 ilib-0.1.1/ilib/VWAP.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      260 2023-05-31 04:00:43.000000 ilib-0.1.1/ilib/__init__.py
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 04:18:26.184116 ilib-0.1.1/ilib.egg-info/
--rw-r--r--   0 devinthakker   (501) staff       (20)      602 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/PKG-INFO
--rw-r--r--   0 devinthakker   (501) staff       (20)      360 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/SOURCES.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)        1 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/dependency_links.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)       13 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/requires.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)        5 2023-05-31 04:18:26.000000 ilib-0.1.1/ilib.egg-info/top_level.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)       79 2023-05-31 04:18:26.184960 ilib-0.1.1/setup.cfg
--rw-r--r--   0 devinthakker   (501) staff       (20)      909 2023-05-31 04:17:43.000000 ilib-0.1.1/setup.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 16:02:06.193215 ilib-0.2/
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1069 2023-05-30 17:52:43.000000 ilib-0.2/LICENSE
+-rw-r--r--   0 devinthakker   (501) staff       (20)      598 2023-05-31 16:02:06.193326 ilib-0.2/PKG-INFO
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2366 2023-05-31 03:59:09.000000 ilib-0.2/README.md
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 16:02:06.192074 ilib-0.2/ilib/
+-rw-r--r--   0 devinthakker   (501) staff       (20)     4476 2023-05-31 04:15:02.000000 ilib-0.2/ilib/ADX.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2296 2023-05-31 03:54:59.000000 ilib-0.2/ilib/ATR.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2014 2023-05-30 16:10:37.000000 ilib-0.2/ilib/BOLLINGERBANDS.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2431 2023-05-30 22:30:49.000000 ilib-0.2/ilib/CCI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1810 2023-05-29 23:50:04.000000 ilib-0.2/ilib/EMA.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3194 2023-05-31 03:55:36.000000 ilib-0.2/ilib/MACD.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1937 2023-05-31 03:55:51.000000 ilib-0.2/ilib/RSI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1159 2023-05-30 16:16:06.000000 ilib-0.2/ilib/SMA.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2723 2023-05-31 04:07:30.000000 ilib-0.2/ilib/STOCHOSCILLATOR.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2738 2023-05-31 04:10:04.000000 ilib-0.2/ilib/VWAP.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      260 2023-05-31 04:00:43.000000 ilib-0.2/ilib/__init__.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 16:02:06.193067 ilib-0.2/ilib.egg-info/
+-rw-r--r--   0 devinthakker   (501) staff       (20)      598 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/PKG-INFO
+-rw-r--r--   0 devinthakker   (501) staff       (20)      360 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/SOURCES.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)        1 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/dependency_links.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)       13 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/requires.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)        5 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/top_level.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)       79 2023-05-31 16:02:06.193841 ilib-0.2/setup.cfg
+-rw-r--r--   0 devinthakker   (501) staff       (20)      905 2023-05-31 16:00:21.000000 ilib-0.2/setup.py
```

### Comparing `ilib-0.1.1/LICENSE` & `ilib-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/PKG-INFO` & `ilib-0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ilib
-Version: 0.1.1
+Version: 0.2
 Summary: A package for various technical indicators
 Home-page: https://github.com/devthakker/ilib
-Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.2.tar.gz
 Author: Devin Thakker
 Author-email: devin.thakker@outlook.com
 License: MIT
 Keywords: ilib,technical indicators,finance,trading,stocks,crypto
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
```

### Comparing `ilib-0.1.1/README.md` & `ilib-0.2/README.md`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/ADX.py` & `ilib-0.2/ilib/ADX.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/ATR.py` & `ilib-0.2/ilib/ATR.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/BOLLINGERBANDS.py` & `ilib-0.2/ilib/BOLLINGERBANDS.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/CCI.py` & `ilib-0.2/ilib/CCI.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/EMA.py` & `ilib-0.2/ilib/EMA.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/MACD.py` & `ilib-0.2/ilib/MACD.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/RSI.py` & `ilib-0.2/ilib/RSI.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/SMA.py` & `ilib-0.2/ilib/SMA.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/STOCHOSCILLATOR.py` & `ilib-0.2/ilib/STOCHOSCILLATOR.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib/VWAP.py` & `ilib-0.2/ilib/VWAP.py`

 * *Files identical despite different names*

### Comparing `ilib-0.1.1/ilib.egg-info/PKG-INFO` & `ilib-0.2/ilib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ilib
-Version: 0.1.1
+Version: 0.2
 Summary: A package for various technical indicators
 Home-page: https://github.com/devthakker/ilib
-Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.2.tar.gz
 Author: Devin Thakker
 Author-email: devin.thakker@outlook.com
 License: MIT
 Keywords: ilib,technical indicators,finance,trading,stocks,crypto
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
```

### Comparing `ilib-0.1.1/setup.py` & `ilib-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup( 
         name='ilib',
-        version='0.1.1',
+        version='0.2',
         # packages=find_packages(exclude=['tests*']),
         packages=find_packages(),
         license='MIT',
         description='A package for various technical indicators',
         install_requires=['numpy', 'pandas'],
         author='Devin Thakker',
         author_email='devin.thakker@outlook.com',
         url='https://github.com/devthakker/ilib',
-        download_url='https://github.com/devthakker/ilib/archive/refs/tags/v0.1.1.tar.gz',
+        download_url='https://github.com/devthakker/ilib/archive/refs/tags/v0.2.tar.gz',
         keywords=['ilib', 'technical indicators', 'finance', 'trading', 'stocks', 'crypto'],
         classifiers=[
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python :: 3.7',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: MIT License',
             ],
```

