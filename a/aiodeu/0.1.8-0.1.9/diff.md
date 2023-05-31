# Comparing `tmp/aiodeu-0.1.8.tar.gz` & `tmp/aiodeu-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodeu-0.1.8.tar", max compression
+gzip compressed data, was "aiodeu-0.1.9.tar", max compression
```

## Comparing `aiodeu-0.1.8.tar` & `aiodeu-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2021-02-02 16:12:52.942988 aiodeu-0.1.8/LICENSE
--rw-r--r--   0        0        0       22 2021-04-02 10:34:40.088522 aiodeu-0.1.8/aiodeu/__init__.py
--rw-r--r--   0        0        0     1341 2021-03-11 13:55:54.951950 aiodeu-0.1.8/aiodeu/app.py
--rw-r--r--   0        0        0     1137 2021-03-07 12:26:19.493129 aiodeu-0.1.8/aiodeu/codecs.py
--rw-r--r--   0        0        0     1241 2021-03-08 07:53:18.903607 aiodeu-0.1.8/aiodeu/config.py
--rw-r--r--   0        0        0     1852 2021-03-11 13:25:03.020964 aiodeu-0.1.8/aiodeu/console.py
--rw-r--r--   0        0        0     2558 2021-10-21 14:49:29.155573 aiodeu-0.1.8/aiodeu/etl.py
--rw-r--r--   0        0        0      318 2020-11-08 09:58:09.375000 aiodeu-0.1.8/aiodeu/logger.py
--rw-r--r--   0        0        0     2150 2021-03-05 11:18:51.874000 aiodeu-0.1.8/aiodeu/s3.py
--rw-r--r--   0        0        0      816 2021-03-07 16:59:26.395929 aiodeu-0.1.8/aiodeu/utils.py
--rw-r--r--   0        0        0      652 2021-10-21 14:50:39.007185 aiodeu-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      862 2021-10-21 14:53:17.256036 aiodeu-0.1.8/setup.py
--rw-r--r--   0        0        0      561 2021-10-21 14:53:17.256941 aiodeu-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2021-02-02 16:12:52.942988 aiodeu-0.1.9/LICENSE
+-rw-r--r--   0        0        0       22 2021-04-02 10:34:40.088522 aiodeu-0.1.9/aiodeu/__init__.py
+-rw-r--r--   0        0        0     1341 2021-03-11 13:55:54.951950 aiodeu-0.1.9/aiodeu/app.py
+-rw-r--r--   0        0        0     1137 2021-03-07 12:26:19.493129 aiodeu-0.1.9/aiodeu/codecs.py
+-rw-r--r--   0        0        0     1241 2021-03-08 07:53:18.903607 aiodeu-0.1.9/aiodeu/config.py
+-rw-r--r--   0        0        0     1852 2021-03-11 13:25:03.020964 aiodeu-0.1.9/aiodeu/console.py
+-rw-r--r--   0        0        0     2558 2021-10-21 14:49:29.155573 aiodeu-0.1.9/aiodeu/etl.py
+-rw-r--r--   0        0        0      318 2020-11-08 09:58:09.375000 aiodeu-0.1.9/aiodeu/logger.py
+-rw-r--r--   0        0        0     2150 2021-03-05 11:18:51.874000 aiodeu-0.1.9/aiodeu/s3.py
+-rw-r--r--   0        0        0      816 2021-03-07 16:59:26.395929 aiodeu-0.1.9/aiodeu/utils.py
+-rw-r--r--   0        0        0      661 2022-04-27 08:40:01.969098 aiodeu-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      871 2022-04-27 08:42:04.080534 aiodeu-0.1.9/setup.py
+-rw-r--r--   0        0        0      570 2022-04-27 08:42:04.080829 aiodeu-0.1.9/PKG-INFO
```

### Comparing `aiodeu-0.1.8/LICENSE` & `aiodeu-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodeu-0.1.8/aiodeu/app.py` & `aiodeu-0.1.9/aiodeu/app.py`

 * *Files identical despite different names*

### Comparing `aiodeu-0.1.8/aiodeu/codecs.py` & `aiodeu-0.1.9/aiodeu/codecs.py`

 * *Files identical despite different names*

### Comparing `aiodeu-0.1.8/aiodeu/config.py` & `aiodeu-0.1.9/aiodeu/config.py`

 * *Files identical despite different names*

### Comparing `aiodeu-0.1.8/aiodeu/console.py` & `aiodeu-0.1.9/aiodeu/console.py`

 * *Files identical despite different names*

### Comparing `aiodeu-0.1.8/aiodeu/etl.py` & `aiodeu-0.1.9/aiodeu/etl.py`

 * *Files identical despite different names*

### Comparing `aiodeu-0.1.8/aiodeu/s3.py` & `aiodeu-0.1.9/aiodeu/s3.py`

 * *Files identical despite different names*

### Comparing `aiodeu-0.1.8/aiodeu/utils.py` & `aiodeu-0.1.9/aiodeu/utils.py`

 * *Files identical despite different names*

### Comparing `aiodeu-0.1.8/pyproject.toml` & `aiodeu-0.1.9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "aiodeu"
-version = "0.1.8"
+version = "0.1.9"
 description = "aio data engineering utils"
 authors = ["Josh Rowe <s-block@users.noreply.github.com>"]
 homepage = "https://github.com/s-block/aiodeu"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 asyncio-redis = "^0.16.0"
 boto3 = "^1.17.21"
-faust = "^1.10.4"
+faust-streaming = "^0.8.4"
 python-schema-registry-client = "~1.8.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 avro-python3 = "^1.10.1"
 confluent-kafka = "^1.6.0"
 flake8 = "^3.8.4"
```

### Comparing `aiodeu-0.1.8/setup.py` & `aiodeu-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['asyncio-redis>=0.16.0,<0.17.0',
  'boto3>=1.17.21,<2.0.0',
- 'faust>=1.10.4,<2.0.0',
+ 'faust-streaming>=0.8.4,<0.9.0',
  'python-schema-registry-client>=1.8.1,<1.9.0']
 
 entry_points = \
 {'console_scripts': ['aiodeu = aiodeu.console:main']}
 
 setup_kwargs = {
     'name': 'aiodeu',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'aio data engineering utils',
     'long_description': None,
     'author': 'Josh Rowe',
     'author_email': 's-block@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/s-block/aiodeu',
```

