# Comparing `tmp/balder-0.1.8.tar.gz` & `tmp/balder-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balder-0.1.8.tar", max compression
+gzip compressed data, was "balder-0.1.9.tar", max compression
```

## Comparing `balder-0.1.8.tar` & `balder-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     1325 2021-09-15 16:34:37.245336 balder-0.1.8/balder/autodiscover.py
--rw-r--r--   0        0        0      927 2021-09-23 10:57:41.500614 balder-0.1.8/balder/consumers.py
--rw-r--r--   0        0        0      499 2021-03-10 08:37:38.223880 balder-0.1.8/balder/enum.py
--rw-r--r--   0        0        0        0 2021-02-23 10:29:42.833994 balder-0.1.8/balder/fields/__init__.py
--rw-r--r--   0        0        0     3553 2021-04-20 07:35:12.632786 balder-0.1.8/balder/fields/filtered.py
--rw-r--r--   0        0        0     3965 2021-09-23 10:47:54.414327 balder-0.1.8/balder/fields/offsetfiltered.py
--rw-r--r--   0        0        0       28 2021-09-23 11:01:17.051988 balder-0.1.8/balder/filters/__init__.py
--rw-r--r--   0        0        0     1058 2021-09-23 10:46:17.430622 balder-0.1.8/balder/filters/enum.py
--rw-r--r--   0        0        0     2424 2021-09-22 08:22:31.065634 balder-0.1.8/balder/registry.py
--rw-r--r--   0        0        0      408 2021-09-23 10:46:54.786507 balder-0.1.8/balder/schema.py
--rw-r--r--   0        0        0     2406 2021-10-18 12:22:05.076000 balder-0.1.8/balder/templates/balder/graphiql-ws.html
--rw-r--r--   0        0        0     2453 2021-10-18 12:22:05.121000 balder-0.1.8/balder/templates/balder/graphiql.html
--rw-r--r--   0        0        0      145 2021-02-24 13:48:18.781400 balder-0.1.8/balder/types/__init__.py
--rw-r--r--   0        0        0       32 2021-02-23 13:38:31.845806 balder-0.1.8/balder/types/mutation/__init__.py
--rw-r--r--   0        0        0     1656 2021-09-23 10:49:52.541978 balder-0.1.8/balder/types/mutation/base.py
--rw-r--r--   0        0        0     1033 2021-02-24 09:50:35.831539 balder-0.1.8/balder/types/mutation/meta.py
--rw-r--r--   0        0        0      309 2021-09-23 10:57:41.500614 balder-0.1.8/balder/types/object.py
--rw-r--r--   0        0        0       29 2021-02-23 13:03:39.300754 balder-0.1.8/balder/types/query/__init__.py
--rw-r--r--   0        0        0     3877 2021-09-23 11:18:27.319641 balder-0.1.8/balder/types/query/base.py
--rw-r--r--   0        0        0     1038 2021-09-23 11:22:14.919350 balder-0.1.8/balder/types/query/meta.py
--rw-r--r--   0        0        0       39 2021-09-23 10:53:51.765281 balder-0.1.8/balder/types/subscription/__init__.py
--rw-r--r--   0        0        0     3404 2021-09-23 10:57:41.500614 balder-0.1.8/balder/types/subscription/base.py
--rw-r--r--   0        0        0     1098 2021-02-24 11:37:04.269996 balder-0.1.8/balder/types/subscription/meta.py
--rw-r--r--   0        0        0     1259 2021-09-23 10:53:51.765281 balder-0.1.8/balder/types/subscription/serializer.py
--rw-r--r--   0        0        0      175 2021-02-24 09:51:02.595465 balder-0.1.8/balder/types/utils.py
--rw-r--r--   0        0        0        0 2021-10-18 08:45:15.686418 balder-0.1.8/balder/urls.py
--rw-r--r--   0        0        0      572 2021-10-18 08:45:56.434416 balder-0.1.8/balder/views.py
--rw-r--r--   0        0        0      583 2021-10-18 12:22:08.139593 balder-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      969 2021-10-18 12:22:08.456443 balder-0.1.8/setup.py
--rw-r--r--   0        0        0      593 2021-10-18 12:22:08.456674 balder-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1216 2021-10-25 08:40:46.817924 balder-0.1.9/balder/.vscode/settings.json
+-rw-r--r--   0        0        0     1325 2021-09-15 16:34:37.245336 balder-0.1.9/balder/autodiscover.py
+-rw-r--r--   0        0        0      927 2021-09-23 10:57:41.500614 balder-0.1.9/balder/consumers.py
+-rw-r--r--   0        0        0      499 2021-03-10 08:37:38.223880 balder-0.1.9/balder/enum.py
+-rw-r--r--   0        0        0        0 2021-02-23 10:29:42.833994 balder-0.1.9/balder/fields/__init__.py
+-rw-r--r--   0        0        0     3553 2021-04-20 07:35:12.632786 balder-0.1.9/balder/fields/filtered.py
+-rw-r--r--   0        0        0     3965 2021-09-23 10:47:54.414327 balder-0.1.9/balder/fields/offsetfiltered.py
+-rw-r--r--   0        0        0       28 2021-09-23 11:01:17.051988 balder-0.1.9/balder/filters/__init__.py
+-rw-r--r--   0        0        0     1058 2021-10-25 08:44:00.873427 balder-0.1.9/balder/filters/enum.py
+-rw-r--r--   0        0        0     1170 2021-10-25 09:18:59.613633 balder-0.1.9/balder/filters/multi_enum.py
+-rw-r--r--   0        0        0     2424 2021-09-22 08:22:31.065634 balder-0.1.9/balder/registry.py
+-rw-r--r--   0        0        0      408 2021-09-23 10:46:54.786507 balder-0.1.9/balder/schema.py
+-rw-r--r--   0        0        0     2406 2021-10-18 12:22:05.076000 balder-0.1.9/balder/templates/balder/graphiql-ws.html
+-rw-r--r--   0        0        0     2453 2021-10-18 12:22:05.121000 balder-0.1.9/balder/templates/balder/graphiql.html
+-rw-r--r--   0        0        0      145 2021-02-24 13:48:18.781400 balder-0.1.9/balder/types/__init__.py
+-rw-r--r--   0        0        0       32 2021-02-23 13:38:31.845806 balder-0.1.9/balder/types/mutation/__init__.py
+-rw-r--r--   0        0        0     1656 2021-09-23 10:49:52.541978 balder-0.1.9/balder/types/mutation/base.py
+-rw-r--r--   0        0        0     1033 2021-02-24 09:50:35.831539 balder-0.1.9/balder/types/mutation/meta.py
+-rw-r--r--   0        0        0      309 2021-09-23 10:57:41.500614 balder-0.1.9/balder/types/object.py
+-rw-r--r--   0        0        0       29 2021-02-23 13:03:39.300754 balder-0.1.9/balder/types/query/__init__.py
+-rw-r--r--   0        0        0     3877 2021-09-23 11:18:27.319641 balder-0.1.9/balder/types/query/base.py
+-rw-r--r--   0        0        0     1038 2021-09-23 11:22:14.919350 balder-0.1.9/balder/types/query/meta.py
+-rw-r--r--   0        0        0       39 2021-09-23 10:53:51.765281 balder-0.1.9/balder/types/subscription/__init__.py
+-rw-r--r--   0        0        0     3404 2021-09-23 10:57:41.500614 balder-0.1.9/balder/types/subscription/base.py
+-rw-r--r--   0        0        0     1098 2021-02-24 11:37:04.269996 balder-0.1.9/balder/types/subscription/meta.py
+-rw-r--r--   0        0        0     1259 2021-09-23 10:53:51.765281 balder-0.1.9/balder/types/subscription/serializer.py
+-rw-r--r--   0        0        0      175 2021-02-24 09:51:02.595465 balder-0.1.9/balder/types/utils.py
+-rw-r--r--   0        0        0        0 2021-10-18 08:45:15.686418 balder-0.1.9/balder/urls.py
+-rw-r--r--   0        0        0      572 2021-10-18 08:45:56.434416 balder-0.1.9/balder/views.py
+-rw-r--r--   0        0        0      583 2021-10-25 09:19:54.657544 balder-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      982 2021-10-25 09:19:54.969558 balder-0.1.9/setup.py
+-rw-r--r--   0        0        0      593 2021-10-25 09:19:54.969707 balder-0.1.9/PKG-INFO
```

### Comparing `balder-0.1.8/balder/autodiscover.py` & `balder-0.1.9/balder/autodiscover.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/consumers.py` & `balder-0.1.9/balder/consumers.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/fields/filtered.py` & `balder-0.1.9/balder/fields/filtered.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/fields/offsetfiltered.py` & `balder-0.1.9/balder/fields/offsetfiltered.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/filters/enum.py` & `balder-0.1.9/balder/filters/enum.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/registry.py` & `balder-0.1.9/balder/registry.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/templates/balder/graphiql-ws.html` & `balder-0.1.9/balder/templates/balder/graphiql-ws.html`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/templates/balder/graphiql.html` & `balder-0.1.9/balder/templates/balder/graphiql.html`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/types/mutation/base.py` & `balder-0.1.9/balder/types/mutation/base.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/types/mutation/meta.py` & `balder-0.1.9/balder/types/mutation/meta.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/types/query/base.py` & `balder-0.1.9/balder/types/query/base.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/types/query/meta.py` & `balder-0.1.9/balder/types/query/meta.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/types/subscription/base.py` & `balder-0.1.9/balder/types/subscription/base.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/types/subscription/meta.py` & `balder-0.1.9/balder/types/subscription/meta.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/types/subscription/serializer.py` & `balder-0.1.9/balder/types/subscription/serializer.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/balder/views.py` & `balder-0.1.9/balder/views.py`

 * *Files identical despite different names*

### Comparing `balder-0.1.8/pyproject.toml` & `balder-0.1.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balder"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Django = "^3.1"
 graphene-django = "^2.15.0"
```

### Comparing `balder-0.1.8/setup.py` & `balder-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,28 +7,28 @@
  'balder.filters',
  'balder.types',
  'balder.types.mutation',
  'balder.types.query',
  'balder.types.subscription']
 
 package_data = \
-{'': ['*'], 'balder': ['templates/balder/*']}
+{'': ['*'], 'balder': ['.vscode/*', 'templates/balder/*']}
 
 install_requires = \
 ['Django>=3.1,<4.0',
  'django-filter>=2.4.0,<3.0.0',
  'graphene-django>=2.15.0,<3.0.0']
 
 extras_require = \
 {'subscription': ['channels>=3.0.3,<4.0.0',
                   'django-channels-graphql-ws>=0.8.0,<0.9.0']}
 
 setup_kwargs = {
     'name': 'balder',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `balder-0.1.8/PKG-INFO` & `balder-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balder
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

