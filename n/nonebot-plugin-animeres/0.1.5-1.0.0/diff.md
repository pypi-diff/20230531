# Comparing `tmp/nonebot_plugin_animeres-0.1.5.tar.gz` & `tmp/nonebot_plugin_animeres-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_animeres-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_animeres-1.0.0.tar", max compression
```

## Comparing `nonebot_plugin_animeres-0.1.5.tar` & `nonebot_plugin_animeres-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    18431 2022-11-07 07:15:06.930293 nonebot_plugin_animeres-0.1.5/LICENSE
--rw-r--r--   0        0        0     2910 2022-11-15 09:05:49.385495 nonebot_plugin_animeres-0.1.5/nonebot_plugin_animeres/__init__.py
--rw-r--r--   0        0        0     5360 2022-11-15 09:06:39.182795 nonebot_plugin_animeres-0.1.5/nonebot_plugin_animeres/cartoon.py
--rw-r--r--   0        0        0      370 2022-11-15 09:02:23.741245 nonebot_plugin_animeres-0.1.5/nonebot_plugin_animeres/config.py
--rw-r--r--   0        0        0      921 2022-11-11 01:49:10.633983 nonebot_plugin_animeres-0.1.5/nonebot_plugin_animeres/functions.py
--rw-r--r--   0        0        0      521 2022-11-15 09:22:31.707147 nonebot_plugin_animeres-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1553 2022-11-15 09:00:55.600480 nonebot_plugin_animeres-0.1.5/README.md
--rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 nonebot_plugin_animeres-0.1.5/setup.py
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 nonebot_plugin_animeres-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-05-27 11:30:14.108178 nonebot_plugin_animeres-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2947 2023-05-30 11:50:40.494073 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/__init__.py
+-rw-r--r--   0        0        0      447 2023-05-30 11:50:00.391161 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/config.py
+-rw-r--r--   0        0        0     2172 2023-05-30 07:25:43.874767 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/internal.py
+-rw-r--r--   0        0        0     1820 2023-05-30 12:08:11.397488 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/resources/__init__.py
+-rw-r--r--   0        0        0     1557 2023-05-30 11:50:29.754653 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/resources/myheartsite.py
+-rw-r--r--   0        0        0     1036 2023-05-30 12:07:42.320956 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/schemas.py
+-rw-r--r--   0        0        0     1558 2023-05-30 08:09:48.266513 nonebot_plugin_animeres-1.0.0/nonebot_plugin_animeres/utils.py
+-rw-r--r--   0        0        0      919 2023-05-31 02:00:42.970686 nonebot_plugin_animeres-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1553 2023-05-27 11:30:14.109179 nonebot_plugin_animeres-1.0.0/README.md
+-rw-r--r--   0        0        0     2297 1970-01-01 00:00:00.000000 nonebot_plugin_animeres-1.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_animeres-0.1.5/LICENSE` & `nonebot_plugin_animeres-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-0.1.5/README.md` & `nonebot_plugin_animeres-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-0.1.5/PKG-INFO` & `nonebot_plugin_animeres-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-animeres
-Version: 0.1.5
+Version: 1.0.0
 Summary: 动漫资源获取插件
+License: GPL-2.0
 Keywords: nonebot,nonebot2,animeres,anime
 Author: MelodyKnit
 Author-email: 2711402357@qq.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: lxml (>=4.9.1,<5.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0rc1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 动漫资源获取插件
 
 这个插件主要是网站爬取过来的数据，在使用命令进行搜索时候采用关键字的方式，比如`天气之子`这时搜索的是`天气之子`相关资源，如果获取的资源并不理想或者你只需要生肉（无字幕）资源时，你就需要用`天气之子 raw`或`天气之子 mkv`这种多个关键字空格方式进行获取，这种方式准确度会比直接用`天气之子`精准且效果好，建议采用多关键字的方式进行搜索。
 
 ## 安装
```

