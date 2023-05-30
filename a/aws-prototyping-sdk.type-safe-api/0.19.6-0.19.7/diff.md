# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.19.6.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.19.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.19.6.tar", last modified: Tue May 30 03:52:39 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.19.7.tar", last modified: Tue May 30 06:40:35 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.19.6.tar` & `aws_prototyping_sdk.type_safe_api-0.19.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    64124 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.511908 aws_prototyping_sdk.type_safe_api-0.19.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.511908 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   624082 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   979031 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.515909 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:40:35.705304 aws_prototyping_sdk.type_safe_api-0.19.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 06:40:20.000000 aws_prototyping_sdk.type_safe_api-0.19.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 06:40:20.000000 aws_prototyping_sdk.type_safe_api-0.19.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 06:40:35.705304 aws_prototyping_sdk.type_safe_api-0.19.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    64124 2023-05-30 06:40:20.000000 aws_prototyping_sdk.type_safe_api-0.19.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-30 06:40:20.000000 aws_prototyping_sdk.type_safe_api-0.19.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:40:35.705304 aws_prototyping_sdk.type_safe_api-0.19.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-30 06:40:20.000000 aws_prototyping_sdk.type_safe_api-0.19.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:40:35.697305 aws_prototyping_sdk.type_safe_api-0.19.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:40:35.697305 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:40:35.705304 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   624082 2023-05-30 06:40:20.000000 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:40:35.705304 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-30 06:40:20.000000 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   979197 2023-05-30 06:40:20.000000 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:40:20.000000 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:40:35.697305 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 06:40:35.000000 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 06:40:35.000000 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:40:35.000000 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 06:40:35.000000 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 06:40:35.000000 aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.6/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.19.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.6/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.19.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.type_safe_api
-Version: 0.19.6
+Version: 0.19.7
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.6/README.md` & `aws_prototyping_sdk.type_safe_api-0.19.7/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.6/setup.py` & `aws_prototyping_sdk.type_safe_api-0.19.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.19.6",
+    "version": "0.19.7",
     "description": "@aws-prototyping-sdk/type-safe-api",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_prototyping_sdk.type_safe_api",
         "aws_prototyping_sdk.type_safe_api._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.type_safe_api._jsii": [
-            "type-safe-api@0.19.6.jsii.tgz"
+            "type-safe-api@0.19.7.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/__init__.py` & `aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk/type_safe_api/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.type-safe-api
-Version: 0.19.6
+Version: 0.19.7
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.19.7/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.6.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.7.jsii.tgz
```

