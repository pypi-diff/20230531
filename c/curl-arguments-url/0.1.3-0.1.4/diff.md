# Comparing `tmp/curl_arguments_url-0.1.3.tar.gz` & `tmp/curl_arguments_url-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_arguments_url-0.1.3.tar", last modified: Sun Apr 30 18:00:15 2023, max compression
+gzip compressed data, was "curl_arguments_url-0.1.4.tar", last modified: Wed May 31 17:57:01 2023, max compression
```

## Comparing `curl_arguments_url-0.1.3.tar` & `curl_arguments_url-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:15.899566 curl_arguments_url-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-30 18:00:15.899566 curl_arguments_url-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:15.895566 curl_arguments_url-0.1.3/curl_arguments_url/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/click_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    57514 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/curl_arguments_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:15.899566 curl_arguments_url-0.1.3/curl_arguments_url/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/models/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/models/open_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/curl_arguments_url/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:00:15.895566 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 18:00:15.000000 curl_arguments_url-0.1.3/curl_arguments_url.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-30 18:00:15.899566 curl_arguments_url-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 18:00:07.000000 curl_arguments_url-0.1.3/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:01.839968 curl_arguments_url-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-31 17:57:01.839968 curl_arguments_url-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:01.835968 curl_arguments_url-0.1.4/curl_arguments_url/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/curl_arguments_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/curl_arguments_url/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57514 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/curl_arguments_url/curl_arguments_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:01.839968 curl_arguments_url-0.1.4/curl_arguments_url/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/curl_arguments_url/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/curl_arguments_url/models/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/curl_arguments_url/models/open_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/curl_arguments_url/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:01.839968 curl_arguments_url-0.1.4/curl_arguments_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-31 17:57:01.000000 curl_arguments_url-0.1.4/curl_arguments_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-31 17:57:01.000000 curl_arguments_url-0.1.4/curl_arguments_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:57:01.000000 curl_arguments_url-0.1.4/curl_arguments_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 17:57:01.000000 curl_arguments_url-0.1.4/curl_arguments_url.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:57:01.000000 curl_arguments_url-0.1.4/curl_arguments_url.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 17:57:01.000000 curl_arguments_url-0.1.4/curl_arguments_url.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 17:57:01.000000 curl_arguments_url-0.1.4/curl_arguments_url.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 17:57:01.839968 curl_arguments_url-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 17:56:49.000000 curl_arguments_url-0.1.4/version.txt
```

### Comparing `curl_arguments_url-0.1.3/LICENSE` & `curl_arguments_url-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.3/PKG-INFO` & `curl_arguments_url-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl_arguments_url
-Version: 0.1.3
+Version: 0.1.4
 Summary: Curl with Arguments for Url
 Home-page: https://github.com/valmikirao/curl_arguments_url
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: Apache Software License 2.0
 Keywords: curl_arguments_url,carl,curl,zsh,completions,swagger,openapi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `curl_arguments_url-0.1.3/README.md` & `curl_arguments_url-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.3/curl_arguments_url/cli.py` & `curl_arguments_url-0.1.4/curl_arguments_url/cli.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.3/curl_arguments_url/curl_arguments_url.py` & `curl_arguments_url-0.1.4/curl_arguments_url/curl_arguments_url.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.3/curl_arguments_url/models/open_api.py` & `curl_arguments_url-0.1.4/curl_arguments_url/models/open_api.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.3/curl_arguments_url.egg-info/PKG-INFO` & `curl_arguments_url-0.1.4/curl_arguments_url.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl-arguments-url
-Version: 0.1.3
+Version: 0.1.4
 Summary: Curl with Arguments for Url
 Home-page: https://github.com/valmikirao/curl_arguments_url
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: Apache Software License 2.0
 Keywords: curl_arguments_url,carl,curl,zsh,completions,swagger,openapi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `curl_arguments_url-0.1.3/curl_arguments_url.egg-info/SOURCES.txt` & `curl_arguments_url-0.1.4/curl_arguments_url.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 version.txt
 curl_arguments_url/__init__.py
 curl_arguments_url/cli.py
-curl_arguments_url/click_test.py
 curl_arguments_url/curl_arguments_url.py
 curl_arguments_url/yaml.py
 curl_arguments_url.egg-info/PKG-INFO
 curl_arguments_url.egg-info/SOURCES.txt
 curl_arguments_url.egg-info/dependency_links.txt
 curl_arguments_url.egg-info/entry_points.txt
 curl_arguments_url.egg-info/not-zip-safe
```

### Comparing `curl_arguments_url-0.1.3/setup.py` & `curl_arguments_url-0.1.4/setup.py`

 * *Files identical despite different names*

