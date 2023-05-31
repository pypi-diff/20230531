# Comparing `tmp/commonMethods_zhaozl_green-2.0.tar.gz` & `tmp/commonMethods_zhaozl_green-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/commonMethods_zhaozl_green-2.0.tar", last modified: Wed May 31 01:31:05 2023, max compression
+gzip compressed data, was "commonMethods_zhaozl_green-2.1.tar", last modified: Wed May 31 05:15:49 2023, max compression
```

## Comparing `commonMethods_zhaozl_green-2.0.tar` & `commonMethods_zhaozl_green-2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      963 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/PKG-INFO
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      291 2023-05-29 15:46:27.000000 commonMethods_zhaozl_green-2.0/README.md
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2217 2023-05-31 01:24:26.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/__init__.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/__version__.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8095 2023-05-30 08:17:36.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/core.py
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4700 2023-05-31 01:17:06.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_processBar.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1821 2023-05-31 01:17:47.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1749 2023-05-31 01:22:22.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/__init__.py
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      963 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/PKG-INFO
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      841 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/SOURCES.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)        1 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/dependency_links.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       90 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/requires.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       27 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/top_level.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       38 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/setup.cfg
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4059 2023-05-31 01:28:03.000000 commonMethods_zhaozl_green-2.0/setup.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 05:15:49.987176 commonMethods_zhaozl_green-2.1/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      963 2023-05-31 05:15:49.987063 commonMethods_zhaozl_green-2.1/PKG-INFO
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      291 2023-05-29 15:46:27.000000 commonMethods_zhaozl_green-2.1/README.md
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 05:15:49.984117 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2217 2023-05-31 01:24:26.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/__init__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/__version__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8095 2023-05-30 08:17:36.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/core.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 05:15:49.986777 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4700 2023-05-31 01:17:06.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_processBar.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1821 2023-05-31 01:17:47.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1749 2023-05-31 01:22:22.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/__init__.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 05:15:49.984942 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      963 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/PKG-INFO
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      841 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)        1 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       97 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/requires.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       27 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/top_level.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       38 2023-05-31 05:15:49.987217 commonMethods_zhaozl_green-2.1/setup.cfg
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4066 2023-05-31 05:14:50.000000 commonMethods_zhaozl_green-2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `commonMethods_zhaozl_green-2.0/PKG-INFO` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: commonMethods_zhaozl_green
-Version: 2.0
+Name: commonMethods-zhaozl-green
+Version: 2.1
 Summary: timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……
 Home-page: 
 Author: zhaozl1123
 Author-email: 545362989@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/__init__.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/__init__.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/core.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/core.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_processBar.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_processBar.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/__init__.py` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/PKG-INFO` & `commonMethods_zhaozl_green-2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: commonMethods-zhaozl-green
-Version: 2.0
+Name: commonMethods_zhaozl_green
+Version: 2.1
 Summary: timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……
 Home-page: 
 Author: zhaozl1123
 Author-email: 545362989@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/SOURCES.txt` & `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.0/setup.py` & `commonMethods_zhaozl_green-2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # Package meta-data.
 NAME = 'commonMethods_zhaozl_green'
 DESCRIPTION = 'timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……'
 URL = ''
 EMAIL = '545362989@qq.com'
 AUTHOR = 'zhaozl1123'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '2.0'
+VERSION = '2.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'numpy==1.24.3', 'joblib>=0.16.0', 'pandas==1.5.3', 'matplotlib>=3.3.0', 'sklearn>=0.0', 'PyMySQL>=0.10.0'
+    'numpy==1.24.3', 'joblib>=0.16.0', 'pandas==1.5.3', 'matplotlib>=3.3.0', 'scikit-learn>=1.2.2', 'PyMySQL>=0.10.0'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

