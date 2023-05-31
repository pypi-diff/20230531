# Comparing `tmp/commonMethods_zhaozl_green-2.1.tar.gz` & `tmp/commonMethods_zhaozl_green-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonMethods_zhaozl_green-2.1.tar", last modified: Wed May 31 05:15:49 2023, max compression
+gzip compressed data, was "commonMethods_zhaozl_green-2.2.tar", last modified: Wed May 31 12:13:20 2023, max compression
```

## Comparing `commonMethods_zhaozl_green-2.1.tar` & `commonMethods_zhaozl_green-2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 05:15:49.987176 commonMethods_zhaozl_green-2.1/
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      963 2023-05-31 05:15:49.987063 commonMethods_zhaozl_green-2.1/PKG-INFO
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      291 2023-05-29 15:46:27.000000 commonMethods_zhaozl_green-2.1/README.md
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 05:15:49.984117 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2217 2023-05-31 01:24:26.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/__init__.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/__version__.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8095 2023-05-30 08:17:36.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/core.py
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 05:15:49.986777 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4700 2023-05-31 01:17:06.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_processBar.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1821 2023-05-31 01:17:47.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1749 2023-05-31 01:22:22.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/__init__.py
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 05:15:49.984942 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      963 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/PKG-INFO
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      841 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/SOURCES.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)        1 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/dependency_links.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       97 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/requires.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       27 2023-05-31 05:15:49.000000 commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/top_level.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       38 2023-05-31 05:15:49.987217 commonMethods_zhaozl_green-2.1/setup.cfg
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4066 2023-05-31 05:14:50.000000 commonMethods_zhaozl_green-2.1/setup.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 12:13:20.372518 commonMethods_zhaozl_green-2.2/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      994 2023-05-31 12:13:20.372398 commonMethods_zhaozl_green-2.2/PKG-INFO
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      324 2023-05-31 12:11:38.000000 commonMethods_zhaozl_green-2.2/README.md
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 12:13:20.369574 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2378 2023-05-31 12:09:13.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/__init__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/__version__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8061 2023-05-31 12:11:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/core.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 12:13:20.372108 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8260 2023-05-31 12:08:15.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_processBar.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1821 2023-05-31 01:17:47.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1902 2023-05-31 12:08:58.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/__init__.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 12:13:20.370340 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      994 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/PKG-INFO
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      841 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)        1 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       97 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/requires.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       27 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/top_level.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       38 2023-05-31 12:13:20.372563 commonMethods_zhaozl_green-2.2/setup.cfg
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4066 2023-05-31 12:10:23.000000 commonMethods_zhaozl_green-2.2/setup.py
```

### Comparing `commonMethods_zhaozl_green-2.1/PKG-INFO` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: commonMethods_zhaozl_green
-Version: 2.1
+Name: commonMethods-zhaozl-green
+Version: 2.2
 Summary: timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……
 Home-page: 
 Author: zhaozl1123
 Author-email: 545362989@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -21,7 +21,9 @@
 v1.0 从commonMethods_zhaozl==v3.13版本中，删除bpNetWork的内容
 
 v1.1 从commonMethods_zhaozl==v3.14版本中，删除bpNetWork的内容，相比v1.0增加proportionalGrouping函数
 
 v1.2 修正了冗余代码
 
 v2.0 简化并优化了脚本，适应Python3.8
+
+v2.2 增加了几种进度条
```

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/__init__.py` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 
             ** Wave, 波浪形进度条
 
             ** Rectangle, 方框形进度条
 
             ** SelfDefine, 自定义符号样式的进度条
 
+            ** FocusedLine, 可自定义符号样式的具有当前正在执行进度位置的进度条
+
+            ** OceanWave, 波浪型动态指示条
+
         * trendAnalyzer:
 
             ** trendAnalyzer: 使用三阶滑动平均与一阶导对输入数据的快速/缓慢的上升/下降状态进行判断
 
             ** trendPredict: 通过不断输入一时间序列的数值，顺序地对所定义窗口1内的数值进行三阶滑动平均处理，并计算所定义窗口2内的时序数据一阶导，通过对所定义窗口3内一阶导数据均值进行判断，以确定原始数据的上升/下降情况，包括：是否处理上升/下降状态，是否处于快速/慢速变化状态
 
         * bounceAnalyzer: 对新传入的数据进行缓存记录，通过平均值计算等方法对跳变状态与持续跳变状态进行判断
```

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/core.py` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 Examples:
     >>> from commonMethods_zhaozl_green.core import {
     >>>     formatTime, printWithColor, moduleOfDataframe, cosineThetaOfVectors, RandomGrouping
     >>> }
 """
 import time
-import numpy as np  # numpy==1.18.5
-import pandas as pd  # pandas==1.1.0
+import numpy as np
+import pandas as pd
 
 
 pd.set_option(
     'display.max_columns', 10000, 'display.width', 10000,
     'display.max_rows', 50, 'display.min_rows', 20,
     'display.unicode.east_asian_width', True
 )
```

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green/toolbox/__init__.py` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
         ** Wave, 波浪形进度条
 
         ** Rectangle, 方框形进度条
 
         ** SelfDefine, 自定义符号样式的进度条
 
+        ** FocusedLine, 可自定义符号样式的具有当前正在执行进度位置的进度条
+
+        ** OceanWave, 波浪型动态指示条
+
     * trendAnalyzer:
 
         ** trendAnalyzer: 使用三阶滑动平均与一阶导对输入数据的快速/缓慢的上升/下降状态进行判断
 
         ** trendPredict: 通过不断输入一时间序列的数值，顺序地对所定义窗口1内的数值进行三阶滑动平均处理，并计算所定义窗口2内的时序数据一阶导，通过对所定义窗口3内一阶导数据均值进行判断，以确定原始数据的上升/下降情况，包括：是否处理上升/下降状态，是否处于快速/慢速变化状态
 
     * bounceAnalyzer: 对新传入的数据进行缓存记录，通过平均值计算等方法对跳变状态与持续跳变状态进行判断
```

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/PKG-INFO` & `commonMethods_zhaozl_green-2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: commonMethods-zhaozl-green
-Version: 2.1
+Name: commonMethods_zhaozl_green
+Version: 2.2
 Summary: timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……
 Home-page: 
 Author: zhaozl1123
 Author-email: 545362989@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -21,7 +21,9 @@
 v1.0 从commonMethods_zhaozl==v3.13版本中，删除bpNetWork的内容
 
 v1.1 从commonMethods_zhaozl==v3.14版本中，删除bpNetWork的内容，相比v1.0增加proportionalGrouping函数
 
 v1.2 修正了冗余代码
 
 v2.0 简化并优化了脚本，适应Python3.8
+
+v2.2 增加了几种进度条
```

### Comparing `commonMethods_zhaozl_green-2.1/commonMethods_zhaozl_green.egg-info/SOURCES.txt` & `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.1/setup.py` & `commonMethods_zhaozl_green-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'commonMethods_zhaozl_green'
 DESCRIPTION = 'timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……'
 URL = ''
 EMAIL = '545362989@qq.com'
 AUTHOR = 'zhaozl1123'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '2.1'
+VERSION = '2.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy==1.24.3', 'joblib>=0.16.0', 'pandas==1.5.3', 'matplotlib>=3.3.0', 'scikit-learn>=1.2.2', 'PyMySQL>=0.10.0'
 ]
 
 # What packages are optional?
```

