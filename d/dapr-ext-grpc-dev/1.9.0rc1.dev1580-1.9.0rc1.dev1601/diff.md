# Comparing `tmp/dapr-ext-grpc-dev-1.9.0rc1.dev1580.tar.gz` & `tmp/dapr-ext-grpc-dev-1.9.0rc1.dev1601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-grpc-dev-1.9.0rc1.dev1580.tar", last modified: Wed May 24 16:45:21 2023, max compression
+gzip compressed data, was "dist/dapr-ext-grpc-dev-1.9.0rc1.dev1601.tar", last modified: Wed May 31 15:44:20 2023, max compression
```

## Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580.tar` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-24 16:44:46.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-24 16:44:46.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-24 16:44:46.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-24 16:44:46.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/grpc/_servicier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-24 16:44:46.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/grpc/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 16:44:46.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/grpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr_ext_grpc_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr_ext_grpc_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr_ext_grpc_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr_ext_grpc_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr_ext_grpc_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr_ext_grpc_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-24 16:45:21.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-24 16:44:46.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1580/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-31 15:43:49.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 15:43:49.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-31 15:43:49.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-31 15:43:49.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/grpc/_servicier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-31 15:43:49.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/grpc/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 15:43:49.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/grpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr_ext_grpc_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr_ext_grpc_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr_ext_grpc_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr_ext_grpc_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr_ext_grpc_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr_ext_grpc_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-31 15:44:20.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-31 15:43:49.000000 dapr-ext-grpc-dev-1.9.0rc1.dev1601/setup.py
```

### Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580/LICENSE` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580/PKG-INFO` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-grpc-dev
-Version: 1.9.0rc1.dev1580
+Version: 1.9.0rc1.dev1601
 Summary: The developmental release for Dapr gRPC AppCallback.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/grpc/__init__.py` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/grpc/_servicier.py` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/grpc/_servicier.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/grpc/app.py` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/grpc/app.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr/ext/grpc/version.py` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr/ext/grpc/version.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580/dapr_ext_grpc_dev.egg-info/PKG-INFO` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601/dapr_ext_grpc_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-grpc-dev
-Version: 1.9.0rc1.dev1580
+Version: 1.9.0rc1.dev1601
 Summary: The developmental release for Dapr gRPC AppCallback.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580/setup.cfg` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-ext-grpc-dev-1.9.0rc1.dev1580/setup.py` & `dapr-ext-grpc-dev-1.9.0rc1.dev1601/setup.py`

 * *Files identical despite different names*
