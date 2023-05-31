# Comparing `tmp/aiobalaboba-3.0.0.tar.gz` & `tmp/aiobalaboba-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobalaboba-3.0.0.tar", max compression
+gzip compressed data, was "aiobalaboba-3.0.1.tar", max compression
```

## Comparing `aiobalaboba-3.0.0.tar` & `aiobalaboba-3.0.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1065 2022-11-21 19:58:08.836339 aiobalaboba-3.0.0/LICENSE
--rw-r--r--   0        0        0     1376 2022-11-26 18:15:51.713649 aiobalaboba-3.0.0/README.md
--rw-r--r--   0        0        0      141 2022-11-21 19:58:08.836339 aiobalaboba-3.0.0/aiobalaboba/__init__.py
--rw-r--r--   0        0        0     1642 2022-11-26 18:23:32.683468 aiobalaboba-3.0.0/aiobalaboba/_balaboba.py
--rw-r--r--   0        0        0     1270 2022-11-26 18:10:10.762895 aiobalaboba-3.0.0/aiobalaboba/_http.py
--rw-r--r--   0        0        0      147 2022-11-26 18:06:56.620360 aiobalaboba-3.0.0/aiobalaboba/_text_type.py
--rw-r--r--   0        0        0        0 2022-11-26 18:18:28.031945 aiobalaboba-3.0.0/aiobalaboba/py.typed
--rw-r--r--   0        0        0     1525 2022-11-26 18:19:42.666079 aiobalaboba-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 aiobalaboba-3.0.0/setup.py
--rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 aiobalaboba-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/LICENSE
+-rw-r--r--   0        0        0     1158 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/README.md
+-rw-r--r--   0        0        0      141 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/__init__.py
+-rw-r--r--   0        0        0     3022 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/_balaboba.py
+-rw-r--r--   0        0        0     1582 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/_http.py
+-rw-r--r--   0        0        0      147 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/_text_type.py
+-rw-r--r--   0        0        0        0 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/py.typed
+-rw-r--r--   0        0        0     2883 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 aiobalaboba-3.0.1/PKG-INFO
```

### Comparing `aiobalaboba-3.0.0/LICENSE` & `aiobalaboba-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobalaboba-3.0.0/README.md` & `aiobalaboba-3.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # aiobalaboba
 
-[![CI](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/aiobalaboba/main.svg)](https://results.pre-commit.ci/latest/github/monosans/aiobalaboba/main)
-[![codecov](https://codecov.io/gh/monosans/aiobalaboba/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/aiobalaboba)
+[![CI](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml/badge.svg)](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml)
+[![Downloads](https://static.pepy.tech/badge/aiobalaboba)](https://pepy.tech/project/aiobalaboba)
 
 Asynchronous wrapper for [Yandex Balaboba](https://yandex.com/lab/yalm-en) ([Яндекс Балабоба](https://yandex.ru/lab/yalm)).
 
 Synchronous version [here](https://github.com/monosans/balaboba).
 
 ## Disclaimer
 
 The neural network doesn’t really know what it’s saying, so it can say absolutely anything. Don’t get offended if it says something that hurts your feelings. When sharing the texts, make sure they’re not offensive or violate the law.
 
 ## Installation
 
 ```bash
-python -m pip install aiobalaboba
+python -m pip install -U aiobalaboba
 ```
 
 ## Usage example
 
 ```python
 import asyncio
 
 from aiobalaboba import Balaboba
 
 
 async def main():
     bb = Balaboba()
-    intros = await bb.get_text_types(language="en")
+    text_types = await bb.get_text_types(language="en")
     response = await bb.balaboba("Hello", text_type=text_types[0])
     print(response)
 
 asyncio.run(main())
 ```
 
 ## License
```

### Comparing `aiobalaboba-3.0.0/PKG-INFO` & `aiobalaboba-3.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,74 @@
 Metadata-Version: 2.1
 Name: aiobalaboba
-Version: 3.0.0
+Version: 3.0.1
 Summary: Asynchronous wrapper for Yandex Balaboba
 Home-page: https://github.com/monosans/aiobalaboba
 License: MIT
 Keywords: yalm
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>=3.8,<4.0)
-Requires-Dist: typing-extensions (>=3.7.4.3,<5); python_version < "3.8"
+Requires-Dist: typing-extensions (>=3.7.4.3,<5) ; python_version < "3.8"
 Project-URL: Repository, https://github.com/monosans/aiobalaboba
 Description-Content-Type: text/markdown
 
 # aiobalaboba
 
-[![CI](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/aiobalaboba/main.svg)](https://results.pre-commit.ci/latest/github/monosans/aiobalaboba/main)
-[![codecov](https://codecov.io/gh/monosans/aiobalaboba/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/aiobalaboba)
+[![CI](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml/badge.svg)](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml)
+[![Downloads](https://static.pepy.tech/badge/aiobalaboba)](https://pepy.tech/project/aiobalaboba)
 
 Asynchronous wrapper for [Yandex Balaboba](https://yandex.com/lab/yalm-en) ([Яндекс Балабоба](https://yandex.ru/lab/yalm)).
 
 Synchronous version [here](https://github.com/monosans/balaboba).
 
 ## Disclaimer
 
 The neural network doesn’t really know what it’s saying, so it can say absolutely anything. Don’t get offended if it says something that hurts your feelings. When sharing the texts, make sure they’re not offensive or violate the law.
 
 ## Installation
 
 ```bash
-python -m pip install aiobalaboba
+python -m pip install -U aiobalaboba
 ```
 
 ## Usage example
 
 ```python
 import asyncio
 
 from aiobalaboba import Balaboba
 
 
 async def main():
     bb = Balaboba()
-    intros = await bb.get_text_types(language="en")
+    text_types = await bb.get_text_types(language="en")
     response = await bb.balaboba("Hello", text_type=text_types[0])
     print(response)
 
 asyncio.run(main())
 ```
 
 ## License
```

