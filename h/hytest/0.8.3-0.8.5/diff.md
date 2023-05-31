# Comparing `tmp/hytest-0.8.3-py3-none-any.whl.zip` & `tmp/hytest-0.8.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26948 bytes, number of entries: 17
+Zip file size: 27165 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       69 b- defN 21-Jun-03 08:24 hytest/__init__.py
 -rw-rw-rw-  2.0 fat      705 b- defN 23-Jan-08 10:00 hytest/cfg.py
--rw-rw-rw-  2.0 fat     2510 b- defN 22-Sep-12 02:08 hytest/common.py
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jan-09 01:02 hytest/product.py
+-rw-rw-rw-  2.0 fat     2795 b- defN 23-May-29 09:38 hytest/common.py
+-rw-rw-rw-  2.0 fat       16 b- defN 23-May-31 01:06 hytest/product.py
 -rw-rw-rw-  2.0 fat     6536 b- defN 23-Jan-09 02:09 hytest/run.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-24 03:36 hytest/utils/__init__.py
--rw-rw-rw-  2.0 fat    30857 b- defN 23-Jan-08 13:47 hytest/utils/log.py
--rw-rw-rw-  2.0 fat     3466 b- defN 22-Sep-12 03:50 hytest/utils/report.css
+-rw-rw-rw-  2.0 fat    30996 b- defN 23-Apr-06 02:10 hytest/utils/log.py
+-rw-rw-rw-  2.0 fat     3471 b- defN 23-Feb-22 02:05 hytest/utils/report.css
 -rw-rw-rw-  2.0 fat     1891 b- defN 22-Sep-12 03:09 hytest/utils/report.js
 -rw-rw-rw-  2.0 fat    24796 b- defN 23-Jan-08 04:19 hytest/utils/runner.py
 -rw-rw-rw-  2.0 fat      571 b- defN 21-Jun-03 08:24 hytest/utils/signal.py
--rw-rw-rw-  2.0 fat    11535 b- defN 23-Jan-09 02:12 hytest-0.8.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1244 b- defN 23-Jan-09 02:12 hytest-0.8.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-09 02:12 hytest-0.8.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       42 b- defN 23-Jan-09 02:12 hytest-0.8.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jan-09 02:12 hytest-0.8.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1308 b- defN 23-Jan-09 02:12 hytest-0.8.3.dist-info/RECORD
-17 files, 85645 bytes uncompressed, 24822 bytes compressed:  71.0%
+-rw-rw-rw-  2.0 fat    11535 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1244 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       42 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1308 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/RECORD
+17 files, 86074 bytes uncompressed, 25039 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: hytest/utils/runner.py
 Comment: 
 
 Filename: hytest/utils/signal.py
 Comment: 
 
-Filename: hytest-0.8.3.dist-info/LICENSE.txt
+Filename: hytest-0.8.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hytest-0.8.3.dist-info/METADATA
+Filename: hytest-0.8.5.dist-info/METADATA
 Comment: 
 
-Filename: hytest-0.8.3.dist-info/WHEEL
+Filename: hytest-0.8.5.dist-info/WHEEL
 Comment: 
 
-Filename: hytest-0.8.3.dist-info/entry_points.txt
+Filename: hytest-0.8.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: hytest-0.8.3.dist-info/top_level.txt
+Filename: hytest-0.8.5.dist-info/top_level.txt
 Comment: 
 
-Filename: hytest-0.8.3.dist-info/RECORD
+Filename: hytest-0.8.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hytest/common.py

```diff
@@ -1,16 +1,24 @@
 from .utils.signal import signal
 from .utils.runner import Runner
 from datetime import datetime
 from .cfg import l
 
+class _GlobalStore:
+    def __getitem__(self, key, default=None):
+        if hasattr(self, key):
+            return getattr(self, key)
+        else:
+            return default
+    def __setitem__(self,key,value):
+        setattr(self, key, value )
 
-
+    get = __getitem__
 # 存储 全局共享 数据
-GSTORE = {}
+GSTORE = _GlobalStore()
 
 def INFO(info):
     """
     在日志和测试报告中打印 重要信息，
     使得 运行报告更加清晰
 
     参数：
@@ -26,33 +34,33 @@
     参数：
     @param stepNo : 指定 是第几步
     @param desc :   步骤描述
     """
     signal.step(stepNo,desc)
 
 
-def CHECK_POINT(desc:str, condition, failStop=True, LogSreenWebDriverIfFail = None):
+def CHECK_POINT(desc:str, condition, failStop=True, failLogScreenWebDriver = None):
     """
     检查点
 
     参数：
     @param desc :   检查点 文字描述
     @param condition : 检查点 表达式
     @param failStop : 检查点即使不通过也继续
-    @param LogSreenWebDriverIfFail ： 如果检查错误，需要截屏，提供的webdirver对象
+    @param failLogScreenWebDriver ： 如果检查错误，需要截屏，提供的webdirver对象
     """
 
     if condition:
         signal.checkpoint_pass(desc)
     else:
         signal.checkpoint_fail(desc)
 
         # 如果需要截屏
-        if LogSreenWebDriverIfFail is not None:
-            SELENIUM_LOG_SCREEN(LogSreenWebDriverIfFail)
+        if failLogScreenWebDriver is not None:
+            SELENIUM_LOG_SCREEN(failLogScreenWebDriver)
 
         # 记录下当前执行结果为失败
         Runner.curRunningCase.execRet='fail'
         Runner.curRunningCase.error=('检查点不通过','checkpoint failed')[l.n]
         Runner.curRunningCase.stacktrace="\n"*3+('具体错误看测试步骤检查点','see checkpoint of case for details')[l.n]
         # 如果失败停止，中止此测试用例
         if failStop:
```

## hytest/product.py

```diff
@@ -1 +1 @@
-version= '0.8.3'
+version= '0.8.5'
```

## hytest/utils/log.py

```diff
@@ -263,15 +263,15 @@
 
 
     def test_end(self, runner):
         endTime = time.strftime('%Y%m%d_%H%M%S',
                                   time.localtime(stats.end_time))
         logger.info(f'\n\n  ========= {("测试结束","Test End")[l.n]} : {endTime} =========\n')
 
-        logger.info(f"\n  {('耗时','Duration Of Testing')[l.n]}    : {(stats.end_time-stats.start_time):.3f} 秒\n")
+        logger.info(f"\n  {('耗时','Duration Of Testing ')[l.n]}    : {(stats.end_time-stats.start_time):.3f} 秒\n")
         ret = stats.result
 
         logger.info(f"\n  {('预备执行用例数量','number of cases to run')[l.n]} : {ret['case_count_toberun']}")
         logger.info(f"\n  {('实际执行用例数量','number of cases actually run')[l.n]} : {ret['case_count']}")
         logger.info(f"\n  {('通过','passed')[l.n]} : {ret['case_pass']}")
         logger.info(f"\n  {('失败','failed')[l.n]} : {ret['case_fail']}")
         logger.info(f"\n  {('异常','exception aborted')[l.n]} : {ret['case_abort']}")
@@ -461,15 +461,15 @@
 
         errorNum = 0
 
         trs = []
         trs.append(tr(td(('开始时间','Test Start Time')[l.n]), td(f'{execStartTime}')))
         trs.append(tr(td(('结束时间','Test End Time')[l.n]), td(f'{execEndTime}')))
 
-        trs.append(tr(td(('耗时','Duration Of Testing')[l.n]), td(f'{stats.test_duration:.3f}' + ('秒','Seconds')[l.n])))
+        trs.append(tr(td(('耗时','Duration Of Testing')[l.n]), td(f'{stats.test_duration:.3f}' + (' 秒',' Seconds')[l.n])))
 
         trs.append(tr(td(('预备执行用例数量','number of cases to run')[l.n]), td(f"{ret['case_count_toberun']}")))
         trs.append(tr(td(('实际执用例行数量','number of cases actually run')[l.n]), td(f"{ret['case_count']}")))
 
         trs.append(tr(td(('通过','passed')[l.n]), td(f"{ret['case_pass']}")))
 
 
@@ -530,15 +530,15 @@
                 percentStr = f'{percent}%'
 
             self.result_barchart.add(
                 div(
                     span(statName),
                     div(
                         div(
-                            percentStr ,
+                            "" , # 柱状里面不填写内容了，如果值为1.86%,背景色部分太短，由于颜色是白色，溢出到右边的空白背景，看不清
                             style=f'width: {barPercentStr}; background-color: {color};',
                             _class="barchart_bar",
                         ),
                         _class="barchart_barbox"
                     ),
                     _class="barchar_item"
                 )
@@ -547,15 +547,15 @@
         # add_barchar_item(
         #     f"用例总数 ： {ret['case_count']} 个",
         #     100,
         #     '#2196f3')
 
 
         def percentCalc(upper,lower):
-            percent = str(round(upper * 100 / lower, 2))
+            percent = str(round(upper * 100 / lower, 1))
             percent = percent[:-2] if percent.endswith('.0') else percent
             return percent
 
         percent = percentCalc(ret['case_pass'], case_count_toberun)
         add_barchar_item(
             f"{('用例通过','cases passed')[l.n]} {percent}% ： {ret['case_pass']} {('个','')[l.n]}",
             float(percent),
```

## hytest/utils/report.css

```diff
@@ -49,28 +49,28 @@
   
 .result_barchart{  
     width: 30em;
     margin: 0 5em 0 5em;
 }
   
 .barchar_item{
-    margin: 2em 0;
+    margin: 2.5rem 0;
 }
   
 .barchart_barbox {
     margin: 0.5em 0;
     width: 100%;
     background-color: #fff;
     border: 1px solid #86c2dd;
     border-radius: .2em;
 }
   
 .barchart_bar {
     text-align: right;
-    color: white;
+    height: 1.2rem;
 }
   
   
 
 
 
 .h3_button {
```

## Comparing `hytest-0.8.3.dist-info/LICENSE.txt` & `hytest-0.8.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hytest-0.8.3.dist-info/METADATA` & `hytest-0.8.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hytest
-Version: 0.8.3
+Version: 0.8.5
 Summary: 一款系统测试自动化框架 Generic automation framework for QA testing
 Home-page: http://www.byhy.net
 Download-URL: https://pypi.python.org/pypi/hytest
 Author: 白月黑羽 - Jiangchunyang
 Author-email: jcyrss@gmail.com
 License: Apache License 2.0
 Keywords: hytest automation testautomation
```

## Comparing `hytest-0.8.3.dist-info/RECORD` & `hytest-0.8.5.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 hytest/__init__.py,sha256=0rezOcKJbE44qmj74qlHlEQRzuO3sOO6tVcLkzaperY,69
 hytest/cfg.py,sha256=Sa03mxXfEDXG-MuOH3ASnz4CHMI-dup0V220p6JNEjo,705
-hytest/common.py,sha256=Eu04dnGZsusDZk67x8J7dyBkUT3zXWE0eKu940WoNwQ,2510
-hytest/product.py,sha256=vljw09kv_G5mBzpUnGjRgqIwiioa4VV1GbGMPijMG8I,16
+hytest/common.py,sha256=GwcoIo1HhWhRIkQt3y9pYioy0tpnHgqNw-EEfs3e8JM,2795
+hytest/product.py,sha256=SKZOWVqvOYqJmDjWBRM1QbKMwQl7PvzFS_6K1MPB4zc,16
 hytest/run.py,sha256=HLhYFREfmDJIIFLvrKnIRuurZvC2qU1TjLypgMBKQIc,6536
 hytest/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hytest/utils/log.py,sha256=8DxbLP2QuxWQuJGO0CjiuTT1T8X_sMb65RqmjUx4Yew,30857
-hytest/utils/report.css,sha256=2MCCFrZUtdvu0Sbwe4jtAQmXWkZ6bzJ_CcRrzaezj4Y,3466
+hytest/utils/log.py,sha256=Q_-S022bRbGGCWtx5m4Ir1KEkMSXSBDQV6zDCqOnx38,30996
+hytest/utils/report.css,sha256=Z5HA_BY7lNXHjJWu8ac7Z6_NlrO7jtARIsZqIrZcjAQ,3471
 hytest/utils/report.js,sha256=WN6rsPyK0smI-1gL2CC1mk2fo3rTRgoBHzK3N_yZRXY,1891
 hytest/utils/runner.py,sha256=qwHxowUUBDIaIUuEhuZlbCXweiKZRUSrFG2x5mIRq1I,24796
 hytest/utils/signal.py,sha256=J45d7BVO1e2oO0tfqWB26ozd0f1EDYT2kj56AtyP0OE,571
-hytest-0.8.3.dist-info/LICENSE.txt,sha256=KmdujD1z5SnrNIuBIyrwfCrwMpq0oMIfCVF_unj7hOA,11535
-hytest-0.8.3.dist-info/METADATA,sha256=MHQcXwTem-dYcPk5zkqZ-8EROthFL01kCjW4gmKBo9s,1244
-hytest-0.8.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hytest-0.8.3.dist-info/entry_points.txt,sha256=92p-5tIrvS1iq_ZMXOUEuhfjr3BDyfuWESt7FpeNP_k,42
-hytest-0.8.3.dist-info/top_level.txt,sha256=UQV_P0cF4XBYxd8wZW0nATrwbqWbWcMstjkj786kst0,7
-hytest-0.8.3.dist-info/RECORD,,
+hytest-0.8.5.dist-info/LICENSE.txt,sha256=KmdujD1z5SnrNIuBIyrwfCrwMpq0oMIfCVF_unj7hOA,11535
+hytest-0.8.5.dist-info/METADATA,sha256=DPzTFOkhZSQwpSbnBZpYgtRd-Q6KCWsZCyhlXVgWhFM,1244
+hytest-0.8.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hytest-0.8.5.dist-info/entry_points.txt,sha256=92p-5tIrvS1iq_ZMXOUEuhfjr3BDyfuWESt7FpeNP_k,42
+hytest-0.8.5.dist-info/top_level.txt,sha256=UQV_P0cF4XBYxd8wZW0nATrwbqWbWcMstjkj786kst0,7
+hytest-0.8.5.dist-info/RECORD,,
```

