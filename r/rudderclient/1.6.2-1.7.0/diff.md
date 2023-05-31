# Comparing `tmp/rudderclient-1.6.2.tar.gz` & `tmp/rudderclient-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderclient-1.6.2.tar", last modified: Tue May 30 08:54:15 2023, max compression
+gzip compressed data, was "rudderclient-1.7.0.tar", last modified: Wed May 31 09:11:58 2023, max compression
```

## Comparing `rudderclient-1.6.2.tar` & `rudderclient-1.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-30 08:54:15.156264 rudderclient-1.6.2/
--rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-05-30 08:53:43.000000 rudderclient-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-30 08:54:15.155264 rudderclient-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-05-30 08:53:43.000000 rudderclient-1.6.2/README.md
--rw-r--r--   0 runner    (1001) runner    (1001)     1030 2023-05-30 08:54:04.000000 rudderclient-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-05-30 08:54:15.156264 rudderclient-1.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-30 08:54:15.147264 rudderclient-1.6.2/src/
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-30 08:54:15.149264 rudderclient-1.6.2/src/rudderclient/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-30 08:54:15.153264 rudderclient-1.6.2/src/rudderclient/aws/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/aws/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5274 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/aws/requests.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-30 08:54:15.154264 rudderclient-1.6.2/src/rudderclient/gcp/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/gcp/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2747 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/gcp/auth.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1087 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/gcp/http_requests.py
--rw-r--r--   0 runner    (1001) runner    (1001)      943 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/gcp/pubsub.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-30 08:54:15.155264 rudderclient-1.6.2/src/rudderclient/request/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/request/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/request/exceptions.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1316 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/request/helpers.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-30 08:54:15.155264 rudderclient-1.6.2/src/rudderclient/tools/
--rw-r--r--   0 runner    (1001) runner    (1001)     5491 2023-05-30 08:53:43.000000 rudderclient-1.6.2/src/rudderclient/tools/send_account_email.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-30 08:54:15.152264 rudderclient-1.6.2/src/rudderclient.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-30 08:54:15.000000 rudderclient-1.6.2/src/rudderclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      614 2023-05-30 08:54:15.000000 rudderclient-1.6.2/src/rudderclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-05-30 08:54:15.000000 rudderclient-1.6.2/src/rudderclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-05-30 08:54:15.000000 rudderclient-1.6.2/src/rudderclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       13 2023-05-30 08:54:15.000000 rudderclient-1.6.2/src/rudderclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.309699 rudderclient-1.7.0/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-05-31 09:11:31.000000 rudderclient-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-31 09:11:58.309699 rudderclient-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-05-31 09:11:31.000000 rudderclient-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     1030 2023-05-31 09:11:49.000000 rudderclient-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-05-31 09:11:58.309699 rudderclient-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.302698 rudderclient-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.304699 rudderclient-1.7.0/src/rudderclient/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.306699 rudderclient-1.7.0/src/rudderclient/aws/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/aws/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5274 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/aws/requests.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.307699 rudderclient-1.7.0/src/rudderclient/gcp/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2747 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/gcp/auth.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2088 2023-05-31 09:11:47.000000 rudderclient-1.7.0/src/rudderclient/gcp/http_requests.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      943 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/gcp/pubsub.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.308699 rudderclient-1.7.0/src/rudderclient/request/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/request/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/request/exceptions.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1316 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/request/helpers.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.308699 rudderclient-1.7.0/src/rudderclient/tools/
+-rw-r--r--   0 runner    (1001) runner    (1001)     5491 2023-05-31 09:11:31.000000 rudderclient-1.7.0/src/rudderclient/tools/send_account_email.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-31 09:11:58.305699 rudderclient-1.7.0/src/rudderclient.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      614 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       13 2023-05-31 09:11:58.000000 rudderclient-1.7.0/src/rudderclient.egg-info/top_level.txt
```

### Comparing `rudderclient-1.6.2/LICENSE` & `rudderclient-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderclient-1.6.2/PKG-INFO` & `rudderclient-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.6.2
+Version: 1.7.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.6.2/pyproject.toml` & `rudderclient-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0.0", "wheel",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudderclient"
-version = "1.6.2"
+version = "1.7.0"
 description = "Shared helpers for rudder application functions code"
 readme = "README.md"
 classifiers = [ "License :: OSI Approved :: MIT License", "Programming Language :: Python", "Programming Language :: Python :: 3.10",]
 keywords = [ "rudder", "client", "helper",]
 dependencies = [ "google-cloud-secret-manager",]
 requires-python = ">=3.10"
 [[project.authors]]
```

### Comparing `rudderclient-1.6.2/src/rudderclient/aws/requests.py` & `rudderclient-1.7.0/src/rudderclient/aws/requests.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.6.2/src/rudderclient/gcp/auth.py` & `rudderclient-1.7.0/src/rudderclient/gcp/auth.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.6.2/src/rudderclient/gcp/pubsub.py` & `rudderclient-1.7.0/src/rudderclient/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.6.2/src/rudderclient/request/exceptions.py` & `rudderclient-1.7.0/src/rudderclient/request/exceptions.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.6.2/src/rudderclient/request/helpers.py` & `rudderclient-1.7.0/src/rudderclient/request/helpers.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.6.2/src/rudderclient/tools/send_account_email.py` & `rudderclient-1.7.0/src/rudderclient/tools/send_account_email.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.6.2/src/rudderclient.egg-info/PKG-INFO` & `rudderclient-1.7.0/src/rudderclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.6.2
+Version: 1.7.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.6.2/src/rudderclient.egg-info/SOURCES.txt` & `rudderclient-1.7.0/src/rudderclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

