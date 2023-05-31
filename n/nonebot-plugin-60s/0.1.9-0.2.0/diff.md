# Comparing `tmp/nonebot_plugin_60s-0.1.9.tar.gz` & `tmp/nonebot_plugin_60s-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_60s-0.1.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_60s-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_60s-0.1.9.tar` & `nonebot_plugin_60s-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1085 2023-02-25 14:18:39.512595 nonebot_plugin_60s-0.1.9/LICENSE
--rw-r--r--   0        0        0     4835 2023-03-08 15:16:01.747197 nonebot_plugin_60s-0.1.9/nonebot_plugin_60s/__init__.py
--rw-r--r--   0        0        0      476 2023-03-08 15:16:01.751196 nonebot_plugin_60s-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2361 2023-02-28 02:57:57.221310 nonebot_plugin_60s-0.1.9/README.md
--rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 nonebot_plugin_60s-0.1.9/setup.py
--rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 nonebot_plugin_60s-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-02-25 14:18:39.512595 nonebot_plugin_60s-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7245 2023-05-31 11:31:49.320217 nonebot_plugin_60s-0.2.0/nonebot_plugin_60s/__init__.py
+-rw-r--r--   0        0        0      246 2023-05-31 11:27:54.713255 nonebot_plugin_60s-0.2.0/nonebot_plugin_60s/config.py
+-rw-r--r--   0        0        0      476 2023-05-31 11:31:49.325222 nonebot_plugin_60s-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3245 2023-05-31 11:27:54.710251 nonebot_plugin_60s-0.2.0/README.md
+-rw-r--r--   0        0        0     3996 1970-01-01 00:00:00.000000 nonebot_plugin_60s-0.2.0/setup.py
+-rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 nonebot_plugin_60s-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_60s-0.1.9/LICENSE` & `nonebot_plugin_60s-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_60s-0.1.9/README.md` & `nonebot_plugin_60s-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,99 @@
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-60s
-
-_✨ 每天60秒读懂世界 ✨_
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/A-kirami/nonebot-plugin-moyu.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-60s">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-60s.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-## 📖 介绍
-
-<details>
-  <summary>效果图</summary>
-
-![example](https://raw.githubusercontent.com/techotaku39/nonebot-plugin-60s/master/readme/example.jpg)
-
-</details>
-
-## 💿 安装
-
-<details>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-60s
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-60s
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-60s
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-60s
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-60s
-</details>
-
-打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
-
-    nonebot.load_plugin('nonebot_plugin_60s')
-
-</details>
-
-## 🎉 使用
-### 指令表
-| 指令  | 说明 |
-|:-----:|:----:|
-| 60s/读懂世界 | 查看今天的60s日历 |
-| 60s/读懂世界+设置 | 以连续对话的形式设置60s日历的推送时间 |
-| 60s/读懂世界+设置 小时:分钟 | 设置60s日历的推送时间 |
-| 60s/读懂世界+状态 | 查看本群的60s日历状态 |
-| 60s/读懂世界+禁用 | 禁用本群的60s日历推送 |
-
-## 💡 鸣谢
-
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-60s
+
+_✨ 每天60秒读懂世界 ✨_
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/A-kirami/nonebot-plugin-moyu.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-60s">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-60s.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+## 📖 介绍
+
+<details>
+  <summary>效果图</summary>
+
+![example](https://raw.githubusercontent.com/techotaku39/nonebot-plugin-60s/master/readme/example.jpg)
+
+</details>
+
+## 💿 安装
+
+<details>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-60s
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+    pip install nonebot-plugin-60s
+</details>
+<details>
+<summary>pdm</summary>
+
+    pdm add nonebot-plugin-60s
+</details>
+<details>
+<summary>poetry</summary>
+
+    poetry add nonebot-plugin-60s
+</details>
+<details>
+<summary>conda</summary>
+
+    conda install nonebot-plugin-60s
+</details>
+
+打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
+
+    nonebot.load_plugin('nonebot_plugin_60s')
+
+</details>
+
+## 配置说明(可选)
+有时候api会失效，就改了下
+微信公众号地址：https://mp.weixin.qq.com/
+抓取的是公众号的内容，我也就找了一个直接分享图片的公众号：每日60s简报（dailybriefing60s），也是很稳定的每天都会在8点前就会推送当天简报
+
+先登陆你的公众号，因为我们要获取一些你的cookie以及token
+登陆后F12查看请求
+![](./images/123.png)
+红圆框是可以找到的地方（大概），红方框就是cookie以及token(cookies:后面的才是，你也可以右键复制值，token=后面的才是)(这也不懂就使用默认吧)
+| 配置项 | 说明 |
+|:-----:|:----:|
+| calendar_cookie: str = "" | 填写微信公众号的cookie |
+| calendar_token: str = "" | 填写微信公众号的token |
+
+## 🎉 使用
+### 指令表
+| 指令  | 说明 |
+|:-----:|:----:|
+| 60s/读懂世界 | 查看今天的60s日历 |
+| 60s/读懂世界+设置 | 以连续对话的形式设置60s日历的推送时间 |
+| 60s/读懂世界+设置 小时:分钟 | 设置60s日历的推送时间 |
+| 60s/读懂世界+状态 | 查看本群的60s日历状态 |
+| 60s/读懂世界+禁用 | 禁用本群的60s日历推送 |
+
+## 💡 鸣谢
+
 ### [A-kirami摸鱼日历](https://github.com/A-kirami/nonebot-plugin-moyu)：本项目就是用大佬的项目改了几行代码，连说明文档也是（）
```

#### html2text {}

```diff
@@ -7,15 +7,26 @@
 ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-60s
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-60s   pdm pdm add nonebot-plugin-60s   poetry
 poetry add nonebot-plugin-60s   conda conda install nonebot-plugin-60s  æå¼
 nonebot2 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
-('nonebot_plugin_60s')  ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | è¯´æ | |:----
--:|:----:| | 60s/è¯»æä¸ç | æ¥çä»å¤©ç60sæ¥å | | 60s/
-è¯»æä¸ç+è®¾ç½® | ä»¥è¿ç»­å¯¹è¯çå½¢å¼è®¾ç½®60sæ¥åçæ¨éæ¶é´ |
-| 60s/è¯»æä¸ç+è®¾ç½® å°æ¶:åé | è®¾ç½®60sæ¥åçæ¨éæ¶é´ | |
-60s/è¯»æä¸ç+ç¶æ | æ¥çæ¬ç¾¤ç60sæ¥åç¶æ | | 60s/
+('nonebot_plugin_60s')  ## éç½®è¯´æ(å¯é)
+ææ¶åapiä¼å¤±æï¼å°±æ¹äºä¸ å¾®ä¿¡å¬ä¼å·å°åï¼https://
+mp.weixin.qq.com/
+æåçæ¯å¬ä¼å·çåå®¹ï¼æä¹å°±æ¾äºä¸ä¸ªç´æ¥åäº«å¾ççå¬ä¼å·ï¼æ¯æ¥60sç®æ¥ï¼dailybriefing60sï¼ï¼ä¹æ¯å¾ç¨³å®çæ¯å¤©é½ä¼å¨8ç¹åå°±ä¼æ¨éå½å¤©ç®æ¥
+åç»éä½ çå¬ä¼å·ï¼å ä¸ºæä»¬è¦è·åä¸äºä½ çcookieä»¥åtoken
+ç»éåF12æ¥çè¯·æ± ![](./images/123.png)
+çº¢åæ¡æ¯å¯ä»¥æ¾å°çå°æ¹ï¼å¤§æ¦ï¼ï¼çº¢æ¹æ¡å°±æ¯cookieä»¥åtoken
+(cookies:åé¢çææ¯ï¼ä½ ä¹å¯ä»¥å³é®å¤å¶å¼ï¼token=åé¢çææ¯)
+(è¿ä¹ä¸æå°±ä½¿ç¨é»è®¤å§) | éç½®é¡¹ | è¯´æ | |:-----:|:----:| |
+calendar_cookie: str = "" | å¡«åå¾®ä¿¡å¬ä¼å·çcookie | | calendar_token:
+str = "" | å¡«åå¾®ä¿¡å¬ä¼å·çtoken | ## ð ä½¿ç¨ ### æä»¤è¡¨ |
+æä»¤ | è¯´æ | |:-----:|:----:| | 60s/è¯»æä¸ç |
+æ¥çä»å¤©ç60sæ¥å | | 60s/è¯»æä¸ç+è®¾ç½® |
+ä»¥è¿ç»­å¯¹è¯çå½¢å¼è®¾ç½®60sæ¥åçæ¨éæ¶é´ | | 60s/
+è¯»æä¸ç+è®¾ç½® å°æ¶:åé | è®¾ç½®60sæ¥åçæ¨éæ¶é´ | | 60s/
+è¯»æä¸ç+ç¶æ | æ¥çæ¬ç¾¤ç60sæ¥åç¶æ | | 60s/
 è¯»æä¸ç+ç¦ç¨ | ç¦ç¨æ¬ç¾¤ç60sæ¥åæ¨é | ## ð¡ é¸£è°¢ ### [A-
 kiramiæ¸é±¼æ¥å](https://github.com/A-kirami/nonebot-plugin-
 moyu)ï¼æ¬é¡¹ç®å°±æ¯ç¨å¤§ä½¬çé¡¹ç®æ¹äºå è¡ä»£ç ï¼è¿è¯´æææ¡£ä¹æ¯ï¼ï¼
```

### Comparing `nonebot_plugin_60s-0.1.9/setup.py` & `nonebot_plugin_60s-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['httpx>=0.23.0,<0.24.0',
  'nonebot-adapter-onebot>=2.0.0b1,<3.0.0',
  'nonebot-plugin-apscheduler>=0.2.0,<0.3.0',
  'nonebot2>=2.0.0b2,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-60s',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': '每天60秒读懂世界',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-60s\n\n_✨ 每天60秒读懂世界 ✨_\n\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/A-kirami/nonebot-plugin-moyu.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot-plugin-60s">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-60s.svg" alt="pypi">\n</a>\n<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n\n</div>\n\n## 📖 介绍\n\n<details>\n  <summary>效果图</summary>\n\n![example](https://raw.githubusercontent.com/techotaku39/nonebot-plugin-60s/master/readme/example.jpg)\n\n</details>\n\n## 💿 安装\n\n<details>\n<summary>使用 nb-cli 安装</summary>\n在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装\n\n    nb plugin install nonebot-plugin-60s\n\n</details>\n\n<details>\n<summary>使用包管理器安装</summary>\n在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令\n\n<details>\n<summary>pip</summary>\n\n    pip install nonebot-plugin-60s\n</details>\n<details>\n<summary>pdm</summary>\n\n    pdm add nonebot-plugin-60s\n</details>\n<details>\n<summary>poetry</summary>\n\n    poetry add nonebot-plugin-60s\n</details>\n<details>\n<summary>conda</summary>\n\n    conda install nonebot-plugin-60s\n</details>\n\n打开 nonebot2 项目的 `bot.py` 文件, 在其中写入\n\n    nonebot.load_plugin(\'nonebot_plugin_60s\')\n\n</details>\n\n## 🎉 使用\n### 指令表\n| 指令  | 说明 |\n|:-----:|:----:|\n| 60s/读懂世界 | 查看今天的60s日历 |\n| 60s/读懂世界+设置 | 以连续对话的形式设置60s日历的推送时间 |\n| 60s/读懂世界+设置 小时:分钟 | 设置60s日历的推送时间 |\n| 60s/读懂世界+状态 | 查看本群的60s日历状态 |\n| 60s/读懂世界+禁用 | 禁用本群的60s日历推送 |\n\n## 💡 鸣谢\n\n### [A-kirami摸鱼日历](https://github.com/A-kirami/nonebot-plugin-moyu)：本项目就是用大佬的项目改了几行代码，连说明文档也是（）',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-60s\n\n_✨ 每天60秒读懂世界 ✨_\n\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/A-kirami/nonebot-plugin-moyu.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot-plugin-60s">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-60s.svg" alt="pypi">\n</a>\n<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n\n</div>\n\n## 📖 介绍\n\n<details>\n  <summary>效果图</summary>\n\n![example](https://raw.githubusercontent.com/techotaku39/nonebot-plugin-60s/master/readme/example.jpg)\n\n</details>\n\n## 💿 安装\n\n<details>\n<summary>使用 nb-cli 安装</summary>\n在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装\n\n    nb plugin install nonebot-plugin-60s\n\n</details>\n\n<details>\n<summary>使用包管理器安装</summary>\n在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令\n\n<details>\n<summary>pip</summary>\n\n    pip install nonebot-plugin-60s\n</details>\n<details>\n<summary>pdm</summary>\n\n    pdm add nonebot-plugin-60s\n</details>\n<details>\n<summary>poetry</summary>\n\n    poetry add nonebot-plugin-60s\n</details>\n<details>\n<summary>conda</summary>\n\n    conda install nonebot-plugin-60s\n</details>\n\n打开 nonebot2 项目的 `bot.py` 文件, 在其中写入\n\n    nonebot.load_plugin(\'nonebot_plugin_60s\')\n\n</details>\n\n## 配置说明(可选)\n有时候api会失效，就改了下\n微信公众号地址：https://mp.weixin.qq.com/\n抓取的是公众号的内容，我也就找了一个直接分享图片的公众号：每日60s简报（dailybriefing60s），也是很稳定的每天都会在8点前就会推送当天简报\n\n先登陆你的公众号，因为我们要获取一些你的cookie以及token\n登陆后F12查看请求\n![](./images/123.png)\n红圆框是可以找到的地方（大概），红方框就是cookie以及token(cookies:后面的才是，你也可以右键复制值，token=后面的才是)(这也不懂就使用默认吧)\n| 配置项 | 说明 |\n|:-----:|:----:|\n| calendar_cookie: str = "" | 填写微信公众号的cookie |\n| calendar_token: str = "" | 填写微信公众号的token |\n\n## 🎉 使用\n### 指令表\n| 指令  | 说明 |\n|:-----:|:----:|\n| 60s/读懂世界 | 查看今天的60s日历 |\n| 60s/读懂世界+设置 | 以连续对话的形式设置60s日历的推送时间 |\n| 60s/读懂世界+设置 小时:分钟 | 设置60s日历的推送时间 |\n| 60s/读懂世界+状态 | 查看本群的60s日历状态 |\n| 60s/读懂世界+禁用 | 禁用本群的60s日历推送 |\n\n## 💡 鸣谢\n\n### [A-kirami摸鱼日历](https://github.com/A-kirami/nonebot-plugin-moyu)：本项目就是用大佬的项目改了几行代码，连说明文档也是（）',
     'author': 'Ananovo',
     'author_email': 'techotaku39@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_60s'] package_data = \ {'': ['*']} install_requires = \
 ['httpx>=0.23.0,<0.24.0', 'nonebot-adapter-onebot>=2.0.0b1,<3.0.0', 'nonebot-
 plugin-apscheduler>=0.2.0,<0.3.0', 'nonebot2>=2.0.0b2,<3.0.0'] setup_kwargs =
-{ 'name': 'nonebot-plugin-60s', 'version': '0.1.9', 'description':
+{ 'name': 'nonebot-plugin-60s', 'version': '0.2.0', 'description':
 'æ¯å¤©60ç§è¯»æä¸ç', 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
      \n\n# nonebot-plugin-60s\n\n_â¨ æ¯å¤©60ç§è¯»æä¸ç â¨_\n\n\n_
@@ -17,17 +17,27 @@
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£\n\n nb
 plugin install nonebot-plugin-60s\n\n\n\n\nä½¿ç¨åç®¡çå¨å®è£\nå¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤\n\n\npip\n\n pip
 install nonebot-plugin-60s\n\n\npdm\n\n pdm add nonebot-plugin-
 60s\n\n\npoetry\n\n poetry add nonebot-plugin-60s\n\n\nconda\n\n conda install
 nonebot-plugin-60s\n\n\næå¼ nonebot2 é¡¹ç®ç `bot.py` æä»¶,
-å¨å¶ä¸­åå¥\n\n nonebot.load_plugin(\'nonebot_plugin_60s\')\n\n\n\n## ð
-ä½¿ç¨\n### æä»¤è¡¨\n| æä»¤ | è¯´æ |\n|:-----:|:----:|\n| 60s/
-è¯»æä¸ç | æ¥çä»å¤©ç60sæ¥å |\n| 60s/è¯»æä¸ç+è®¾ç½® |
+å¨å¶ä¸­åå¥\n\n nonebot.load_plugin(\'nonebot_plugin_60s\')\n\n\n\n##
+éç½®è¯´æ
+(å¯é)\nææ¶åapiä¼å¤±æï¼å°±æ¹äºä¸\nå¾®ä¿¡å¬ä¼å·å°åï¼https:/
+/mp.weixin.qq.com/
+\næåçæ¯å¬ä¼å·çåå®¹ï¼æä¹å°±æ¾äºä¸ä¸ªç´æ¥åäº«å¾ççå¬ä¼å·ï¼æ¯æ¥60sç®æ¥ï¼dailybriefing60sï¼ï¼ä¹æ¯å¾ç¨³å®çæ¯å¤©é½ä¼å¨8ç¹åå°±ä¼æ¨éå½å¤©ç®æ¥\n\nåç»éä½ çå¬ä¼å·ï¼å ä¸ºæä»¬è¦è·åä¸äºä½ çcookieä»¥åtoken\nç»éåF12æ¥çè¯·æ±\n!
+[](./images/
+123.png)\nçº¢åæ¡æ¯å¯ä»¥æ¾å°çå°æ¹ï¼å¤§æ¦ï¼ï¼çº¢æ¹æ¡å°±æ¯cookieä»¥åtoken
+(cookies:åé¢çææ¯ï¼ä½ ä¹å¯ä»¥å³é®å¤å¶å¼ï¼token=åé¢çææ¯)
+(è¿ä¹ä¸æå°±ä½¿ç¨é»è®¤å§)\n| éç½®é¡¹ | è¯´æ |\n|:-----:|:----:|\n|
+calendar_cookie: str = "" | å¡«åå¾®ä¿¡å¬ä¼å·çcookie |\n| calendar_token:
+str = "" | å¡«åå¾®ä¿¡å¬ä¼å·çtoken |\n\n## ð ä½¿ç¨\n### æä»¤è¡¨\n|
+æä»¤ | è¯´æ |\n|:-----:|:----:|\n| 60s/è¯»æä¸ç |
+æ¥çä»å¤©ç60sæ¥å |\n| 60s/è¯»æä¸ç+è®¾ç½® |
 ä»¥è¿ç»­å¯¹è¯çå½¢å¼è®¾ç½®60sæ¥åçæ¨éæ¶é´ |\n| 60s/
 è¯»æä¸ç+è®¾ç½® å°æ¶:åé | è®¾ç½®60sæ¥åçæ¨éæ¶é´ |\n| 60s/
 è¯»æä¸ç+ç¶æ | æ¥çæ¬ç¾¤ç60sæ¥åç¶æ |\n| 60s/
 è¯»æä¸ç+ç¦ç¨ | ç¦ç¨æ¬ç¾¤ç60sæ¥åæ¨é |\n\n## ð¡ é¸£è°¢\n\n###
 [A-kiramiæ¸é±¼æ¥å](https://github.com/A-kirami/nonebot-plugin-
 moyu)ï¼æ¬é¡¹ç®å°±æ¯ç¨å¤§ä½¬çé¡¹ç®æ¹äºå è¡ä»£ç ï¼è¿è¯´æææ¡£ä¹æ¯ï¼ï¼',
 'author': 'Ananovo', 'author_email': 'techotaku39@outlook.com', 'maintainer':
```

