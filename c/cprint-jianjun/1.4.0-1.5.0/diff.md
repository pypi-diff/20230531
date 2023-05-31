# Comparing `tmp/cprint-jianjun-1.4.0.tar.gz` & `tmp/cprint-jianjun-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cprint-jianjun-1.4.0.tar", last modified: Wed Mar 15 02:46:09 2023, max compression
+gzip compressed data, was "cprint-jianjun-1.5.0.tar", last modified: Wed May 31 07:18:34 2023, max compression
```

## Comparing `cprint-jianjun-1.4.0.tar` & `cprint-jianjun-1.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 02:46:09.425266 cprint-jianjun-1.4.0/
--rw-rw-rw-   0        0        0    18431 2021-04-19 08:51:39.000000 cprint-jianjun-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     3355 2023-03-15 02:46:09.425266 cprint-jianjun-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3029 2023-03-15 02:45:01.000000 cprint-jianjun-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 02:46:09.420280 cprint-jianjun-1.4.0/cprint/
--rw-rw-rw-   0        0        0      373 2023-03-15 01:02:15.000000 cprint-jianjun-1.4.0/cprint/__init__.py
--rw-rw-rw-   0        0        0     1821 2022-11-16 06:51:11.000000 cprint-jianjun-1.4.0/cprint/config.py
--rw-rw-rw-   0        0        0     2506 2023-03-15 02:38:47.000000 cprint-jianjun-1.4.0/cprint/main.py
--rw-rw-rw-   0        0        0     6070 2023-02-23 02:37:14.000000 cprint-jianjun-1.4.0/cprint/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-15 02:46:09.424268 cprint-jianjun-1.4.0/cprint_jianjun.egg-info/
--rw-rw-rw-   0        0        0     3355 2023-03-15 02:46:09.000000 cprint-jianjun-1.4.0/cprint_jianjun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-03-15 02:46:09.000000 cprint-jianjun-1.4.0/cprint_jianjun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 02:46:09.000000 cprint-jianjun-1.4.0/cprint_jianjun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-03-15 02:46:09.000000 cprint-jianjun-1.4.0/cprint_jianjun.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-03-15 02:46:09.000000 cprint-jianjun-1.4.0/cprint_jianjun.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-15 02:46:09.000000 cprint-jianjun-1.4.0/cprint_jianjun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 02:46:09.426263 cprint-jianjun-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      871 2023-03-15 01:02:18.000000 cprint-jianjun-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:18:34.847221 cprint-jianjun-1.5.0/
+-rw-rw-rw-   0        0        0    18431 2021-04-19 08:51:39.000000 cprint-jianjun-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     3355 2023-05-31 07:18:34.846223 cprint-jianjun-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3029 2023-03-15 02:45:01.000000 cprint-jianjun-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 07:18:34.841236 cprint-jianjun-1.5.0/cprint/
+-rw-rw-rw-   0        0        0      373 2023-05-31 07:15:41.000000 cprint-jianjun-1.5.0/cprint/__init__.py
+-rw-rw-rw-   0        0        0     1821 2022-11-16 06:51:11.000000 cprint-jianjun-1.5.0/cprint/config.py
+-rw-rw-rw-   0        0        0     2506 2023-03-15 02:38:47.000000 cprint-jianjun-1.5.0/cprint/main.py
+-rw-rw-rw-   0        0        0     6649 2023-05-31 07:15:20.000000 cprint-jianjun-1.5.0/cprint/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:18:34.846223 cprint-jianjun-1.5.0/cprint_jianjun.egg-info/
+-rw-rw-rw-   0        0        0     3355 2023-05-31 07:18:34.000000 cprint-jianjun-1.5.0/cprint_jianjun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-31 07:18:34.000000 cprint-jianjun-1.5.0/cprint_jianjun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:18:34.000000 cprint-jianjun-1.5.0/cprint_jianjun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-31 07:18:34.000000 cprint-jianjun-1.5.0/cprint_jianjun.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2023-05-31 07:18:34.000000 cprint-jianjun-1.5.0/cprint_jianjun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 07:18:34.000000 cprint-jianjun-1.5.0/cprint_jianjun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:18:34.847221 cprint-jianjun-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      871 2023-05-31 07:16:57.000000 cprint-jianjun-1.5.0/setup.py
```

### Comparing `cprint-jianjun-1.4.0/LICENSE` & `cprint-jianjun-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cprint-jianjun-1.4.0/PKG-INFO` & `cprint-jianjun-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cprint-jianjun
-Version: 1.4.0
+Version: 1.5.0
 Summary: Colorful Print 彩色文本格式化, 彩色文本输出, 控制打印字符颜色样式!
 Home-page: https://github.com/EVA-JianJun/cprint
 Author: jianjun
 Author-email: 910667956@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cprint-jianjun-1.4.0/README.md` & `cprint-jianjun-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cprint-jianjun-1.4.0/cprint/config.py` & `cprint-jianjun-1.5.0/cprint/config.py`

 * *Files identical despite different names*

### Comparing `cprint-jianjun-1.4.0/cprint/main.py` & `cprint-jianjun-1.5.0/cprint/main.py`

 * *Files identical despite different names*

### Comparing `cprint-jianjun-1.4.0/cprint/tools.py` & `cprint-jianjun-1.5.0/cprint/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import math
+import traceback
 from cprint.config import COLOR32, COLOR256
 
 def getshow_config(mode: int=1) -> dict or None:
     """
     文档:
         获取 or 显示 32 colors 配置信息
     参数:
@@ -102,15 +103,27 @@
         for color_code_38 in COLOR256.COLOR_CODE:
             # use_print_1("\033[48;5;{0}m\033[38;5;{1}m CHERRY \033[0;0m".format(color_code_48, color_code_38))
             STYLE_ID_DICT[id_plus] = "\033[48;5;{0}m\033[38;5;{1}m".format(color_code_48, color_code_38)
             id_plus += 1
 
     """ 打印所有颜色样式列表 """
     print_n = 0
-    columns = os.get_terminal_size().columns
+    try:
+        columns = os.get_terminal_size().columns
+    except Exception as err:
+        # File "/usr/local/lib/python3.9/site-packages/cprint/main.py", line 7, in <module>
+        #     STYLE_CONFIG = getshow_config(1)
+        # File "/usr/local/lib/python3.9/site-packages/cprint/tools.py", line 109, in getshow_config
+        #     columns = os.get_terminal_size().columns
+        # OSError: [Errno 25] Inappropriate ioctl for device
+        columns = 100
+        print("WARNING: os.get_terminal_size Err, Get default columns = 100.")
+        traceback.print_exc()
+        print(err)
+
     for style_id, style_code in STYLE_ID_DICT.items():
         use_print_2('{0} {1:^5} \033[0;0m'.format(style_code, style_id), end="")
         print_n += 1
         if print_n % math.floor(columns / 7) == 0:
             use_print_2()
 
     # print("DEBUG Caclute 2!")
```

### Comparing `cprint-jianjun-1.4.0/cprint_jianjun.egg-info/PKG-INFO` & `cprint-jianjun-1.5.0/cprint_jianjun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cprint-jianjun
-Version: 1.4.0
+Version: 1.5.0
 Summary: Colorful Print 彩色文本格式化, 彩色文本输出, 控制打印字符颜色样式!
 Home-page: https://github.com/EVA-JianJun/cprint
 Author: jianjun
 Author-email: 910667956@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cprint-jianjun-1.4.0/setup.py` & `cprint-jianjun-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name = 'cprint-jianjun',
-    version = '1.4.0',
+    version = '1.5.0',
     author = 'jianjun',
     author_email = '910667956@qq.com',
     url = 'https://github.com/EVA-JianJun/cprint',
     description = u'Colorful Print 彩色文本格式化, 彩色文本输出, 控制打印字符颜色样式!',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = ["cprint"],
```

