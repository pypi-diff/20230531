# Comparing `tmp/commonMethods_zhaozl_green-1.2.tar.gz` & `tmp/commonMethods_zhaozl_green-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonMethods_zhaozl_green-1.2.tar", last modified: Sun Sep 12 12:26:08 2021, max compression
+gzip compressed data, was "dist/commonMethods_zhaozl_green-2.0.tar", last modified: Wed May 31 01:31:05 2023, max compression
```

## Comparing `commonMethods_zhaozl_green-1.2.tar` & `commonMethods_zhaozl_green-2.0.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxrwx   0        0        0        0 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/
--rw-rw-rw-   0        0        0     1067 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-1.2/LICENSE
--rw-rw-rw-   0        0        0       27 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1040 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      240 2021-09-12 12:25:20.000000 commonMethods_zhaozl_green-1.2/README.md
-drwxrwxrwx   0        0        0        0 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/
--rw-rw-rw-   0        0        0     2265 2021-08-09 03:48:20.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/__init__.py
--rw-rw-rw-   0        0        0      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/__version__.py
--rw-rw-rw-   0        0        0    10716 2021-08-09 03:47:52.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/core.py
-drwxrwxrwx   0        0        0        0 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/
--rw-rw-rw-   0        0        0     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
--rw-rw-rw-   0        0        0    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
--rw-rw-rw-   0        0        0     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
--rw-rw-rw-   0        0        0     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
--rw-rw-rw-   0        0        0     3233 2021-05-19 03:58:28.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_processBar.py
--rw-rw-rw-   0        0        0     1815 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
--rw-rw-rw-   0        0        0    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
--rw-rw-rw-   0        0        0     1544 2021-08-09 02:56:53.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green.egg-info/
--rw-rw-rw-   0        0        0     1040 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-09-12 12:26:08.000000 commonMethods_zhaozl_green-1.2/setup.cfg
--rw-rw-rw-   0        0        0     4067 2021-09-12 12:24:48.000000 commonMethods_zhaozl_green-1.2/setup.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      963 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/PKG-INFO
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      291 2023-05-29 15:46:27.000000 commonMethods_zhaozl_green-2.0/README.md
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2217 2023-05-31 01:24:26.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/__init__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/__version__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8095 2023-05-30 08:17:36.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/core.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4700 2023-05-31 01:17:06.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_processBar.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1821 2023-05-31 01:17:47.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1749 2023-05-31 01:22:22.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/__init__.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      963 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/PKG-INFO
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      841 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)        1 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       90 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/requires.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       27 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/top_level.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       38 2023-05-31 01:31:05.000000 commonMethods_zhaozl_green-2.0/setup.cfg
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4059 2023-05-31 01:28:03.000000 commonMethods_zhaozl_green-2.0/setup.py
```

### Comparing `commonMethods_zhaozl_green-1.2/PKG-INFO` & `commonMethods_zhaozl_green-2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 2.1
-Name: commonMethods_zhaozl_green
-Version: 1.2
-Summary: timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine... by zhaozl.
-Home-page: UNKNOWN
-Author: zhaozl1123
-Author-email: 545362989@qq.com
-License: MIT
-Description: 
-        ## 版本记录
-        
-        v1.0 从commonMethods_zhaozl==v3.13版本中，删除bpNetWork的内容
-        
-        v1.1 从commonMethods_zhaozl==v3.14版本中，删除bpNetWork的内容，相比v1.0增加proportionalGrouping函数
-        
-        v1.2 修正了冗余代码
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: commonMethods_zhaozl_green
+Version: 2.0
+Summary: timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……
+Home-page: 
+Author: zhaozl1123
+Author-email: 545362989@qq.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+
+
+## 版本记录
+
+v1.0 从commonMethods_zhaozl==v3.13版本中，删除bpNetWork的内容
+
+v1.1 从commonMethods_zhaozl==v3.14版本中，删除bpNetWork的内容，相比v1.0增加proportionalGrouping函数
+
+v1.2 修正了冗余代码
+
+v2.0 简化并优化了脚本，适应Python3.8
```

### Comparing `commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/__init__.py` & `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """
-Core
-----------
-* code2Name: 通过输入词典对传入code进行转译同时使用_verbose控制是否显示对字典的预检验
-* printWithColor: 打印具有颜色和特定格式的字符串
-* mapminmax: 数据进行标准化[0，1]
-* moduleOfDataframe: 计算一个dataframe所表达的多个向量的模
-* cosineThetaOfVectors: 计算向量1（或多个向量1）与向量2的夹角余弦
-* randomGrouping: 根据比例随机取得一数据表中的样本
-* proportionalGrouping: 根据比例间隔取得一数据表中的样本，样本不重复，严格按照截取比例间隔抽样选取
-
-Toolbox
-----------
-* timeTrans: 通过输入list(int)或者int形式的时间戳unixTimestamp，与形如'%Y/%m/%d %H:%M:%S'的formation，对时间戳进行计算并输出string
-* mysqlOperator: mysql数据库操作， 包括创建table、添加列、新增数据、更新数据、查询数据
-* bpNetworkTrain: BP神经网络训练，默认三层，包括输出层
-* bpNetworkRun: BP神经网络计算
-* comtradeParser: 通过输入符合comtrade规范的文件名，对数据内容进行输出
-* processBar: 在打印的循环体中输出进度条
-* trendAnalyzer:
-	** trendAnalyzer: 使用三阶滑动平均与一阶导对输入数据的快速/缓慢的上升/下降状态进行判断
-
-	** trendPredict: 通过不断输入一时间序列的数值，顺序地对所定义窗口1内的数值进行三阶滑动平均处理，并计算所定义窗口2内的时序数据一阶导，通过
-	对所定义窗口3内一阶导数据均值进行判断，以确定原始数据的上升/下降情况，包括：是否处理上升/下降状态，是否处于快速/慢速    变化状态
-* bounceAnalyzer: 对新传入的数据进行缓存记录，通过平均值计算等方法对跳变状态与持续跳变状态进行判断
-* evennessDetermine: 包括两种方法
-    ** compareWithOthersAverage, 同类测点温度值稳定，单一测点温度测量在正常范围内，但明显高于除本测点外的同类平均值
+Notes:
+    - core中：
+        - formatTime:获取符合需求格式的时间
+        - printWithColor:打印所定义格式的字符串
+        - moduleOfDataframe:计算DF中所指多个向量样本的模
+        - cosineThetaOfVectors:计算向量组和单个向量间的夹角与余弦值
+        - RandomGrouping:根据所需样本数量不重复地随机进行抽样
 
-    ** circleSimilarity, 全体测点与均值圆的相似度, 使用向量间的相似度进行衡量
+Notes:
+    - toolbox中：
+        * timeTrans: 通过输入list(int)或者int形式的时间戳unixTimestamp，与形如'%Y/%m/%d %H:%M:%S'的formation，对时间戳进行计算并输出string
 
-	** modulo， 向量的模计算
+        * mysqlOperator: mysql数据库操作， 包括创建table、添加列、新增数据、更新数据、查询数据
 
-	** angleCal， 向量间夹角余弦值计算
+        * comtradeParser: 通过输入符合comtrade规范的文件名，对数据内容进行输出
 
-"""
+        * processBar: 包括以下几个不同样式的进度条：
+
+            ** Wave, 波浪形进度条
+
+            ** Rectangle, 方框形进度条
+
+            ** SelfDefine, 自定义符号样式的进度条
+
+        * trendAnalyzer:
+
+            ** trendAnalyzer: 使用三阶滑动平均与一阶导对输入数据的快速/缓慢的上升/下降状态进行判断
+
+            ** trendPredict: 通过不断输入一时间序列的数值，顺序地对所定义窗口1内的数值进行三阶滑动平均处理，并计算所定义窗口2内的时序数据一阶导，通过对所定义窗口3内一阶导数据均值进行判断，以确定原始数据的上升/下降情况，包括：是否处理上升/下降状态，是否处于快速/慢速变化状态
 
+        * bounceAnalyzer: 对新传入的数据进行缓存记录，通过平均值计算等方法对跳变状态与持续跳变状态进行判断
+
+        * evennessDetermine: 包括两种方法
+
+            ** compareWithOthersAverage, 同类测点温度值稳定，单一测点温度测量在正常范围内，但明显高于除本测点外的同类平均值
+
+            ** circleSimilarity, 全体测点与均值圆的相似度, 使用向量间的相似度进行衡量
+
+            ** modulo， 向量的模计算
+
+            ** angleCal， 向量间夹角余弦值计算
+"""
 from .core import *
```

### Comparing `commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py` & `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py` & `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py` & `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py` & `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py` & `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Classes
 ----------
 timeTrans: 通过输入list(int)或者int形式的时间戳unixTimestamp，与形如'%Y/%m/%d %H:%M:%S'的formation，对时间戳进行计算并输出string
 
 Example
 ----------
->>> from commonMethods_zhaozl.toolbox.Method_timeTrans import timeTrans
+>>> from commonMethods_zhaozl_green.toolbox.Method_timeTrans import timeTrans
 
 """
 
 import time
 
 
 class timeTrans:
```

### Comparing `commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py` & `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green/toolbox/__init__.py` & `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green/toolbox/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """
-Classes
-----------
-* timeTrans: 通过输入list(int)或者int形式的时间戳unixTimestamp，与形如'%Y/%m/%d %H:%M:%S'的formation，对时间戳进行计算并输出string
+Notes:
+    * timeTrans: 通过输入list(int)或者int形式的时间戳unixTimestamp，与形如'%Y/%m/%d %H:%M:%S'的formation，对时间戳进行计算并输出string
 
-* mysqlOperator: mysql数据库操作， 包括创建table、添加列、新增数据、更新数据、查询数据
+    * mysqlOperator: mysql数据库操作， 包括创建table、添加列、新增数据、更新数据、查询数据
 
-* comtradeParser: 通过输入符合comtrade规范的文件名，对数据内容进行输出
+    * comtradeParser: 通过输入符合comtrade规范的文件名，对数据内容进行输出
 
-* processBar: 在打印的循环体中输出进度条
+    * processBar: 包括以下几个不同样式的进度条：
 
-* trendAnalyzer:
+        ** Wave, 波浪形进度条
 
-	** trendAnalyzer: 使用三阶滑动平均与一阶导对输入数据的快速/缓慢的上升/下降状态进行判断
+        ** Rectangle, 方框形进度条
 
-	** trendPredict: 通过不断输入一时间序列的数值，顺序地对所定义窗口1内的数值进行三阶滑动平均处理，并计算所定义窗口2内的时序数据一阶导，通过对所定义窗口3内一阶导数据均值进行判断，以确定原始数据的上升/下降情况，包括：是否处理上升/下降状态，是否处于快速/慢速变化状态
-	
-* bounceAnalyzer: 对新传入的数据进行缓存记录，通过平均值计算等方法对跳变状态与持续跳变状态进行判断
+        ** SelfDefine, 自定义符号样式的进度条
 
-* evennessDetermine: 包括两种方法
+    * trendAnalyzer:
 
-	** compareWithOthersAverage, 同类测点温度值稳定，单一测点温度测量在正常范围内，但明显高于除本测点外的同类平均值
+        ** trendAnalyzer: 使用三阶滑动平均与一阶导对输入数据的快速/缓慢的上升/下降状态进行判断
 
-	** circleSimilarity, 全体测点与均值圆的相似度, 使用向量间的相似度进行衡量
+        ** trendPredict: 通过不断输入一时间序列的数值，顺序地对所定义窗口1内的数值进行三阶滑动平均处理，并计算所定义窗口2内的时序数据一阶导，通过对所定义窗口3内一阶导数据均值进行判断，以确定原始数据的上升/下降情况，包括：是否处理上升/下降状态，是否处于快速/慢速变化状态
 
-	** modulo， 向量的模计算
+    * bounceAnalyzer: 对新传入的数据进行缓存记录，通过平均值计算等方法对跳变状态与持续跳变状态进行判断
 
-	** angleCal， 向量间夹角余弦值计算
+    * evennessDetermine: 包括两种方法
 
+        ** compareWithOthersAverage, 同类测点温度值稳定，单一测点温度测量在正常范围内，但明显高于除本测点外的同类平均值
+
+        ** circleSimilarity, 全体测点与均值圆的相似度, 使用向量间的相似度进行衡量
+
+        ** modulo， 向量的模计算
+
+        ** angleCal， 向量间夹角余弦值计算
 """
 
-from . import *
+from . import *
```

### Comparing `commonMethods_zhaozl_green-1.2/commonMethods_zhaozl_green.egg-info/SOURCES.txt` & `commonMethods_zhaozl_green-2.0/commonMethods_zhaozl_green.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-LICENSE
-MANIFEST.in
 README.md
 setup.py
 commonMethods_zhaozl_green/__init__.py
 commonMethods_zhaozl_green/__version__.py
 commonMethods_zhaozl_green/core.py
 commonMethods_zhaozl_green.egg-info/PKG-INFO
 commonMethods_zhaozl_green.egg-info/SOURCES.txt
```

### Comparing `commonMethods_zhaozl_green-1.2/setup.py` & `commonMethods_zhaozl_green-2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'commonMethods_zhaozl_green'
-DESCRIPTION = 'timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine... by zhaozl.'
+DESCRIPTION = 'timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……'
 URL = ''
 EMAIL = '545362989@qq.com'
 AUTHOR = 'zhaozl1123'
-REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.2'
+REQUIRES_PYTHON = '>=3.8.0'
+VERSION = '2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'numpy==1.18.5', 'joblib==0.16.0', 'pandas==1.1.0', 'matplotlib==3.3.0', 'sklearn==0.0', 'PyMySQL==0.10.0'
+    'numpy==1.24.3', 'joblib>=0.16.0', 'pandas==1.5.3', 'matplotlib>=3.3.0', 'sklearn>=0.0', 'PyMySQL>=0.10.0'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

