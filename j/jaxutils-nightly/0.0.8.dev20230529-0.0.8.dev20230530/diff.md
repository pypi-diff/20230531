# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230529.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230529.tar", last modified: Mon May 29 00:06:36 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230530.tar", last modified: Tue May 30 00:06:22 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230529.tar` & `jaxutils-nightly-0.0.8.dev20230530.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-29 00:06:36.675398 jaxutils-nightly-0.0.8.dev20230529/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-29 00:06:36.675398 jaxutils-nightly-0.0.8.dev20230529/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-05-29 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230529/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-29 00:06:36.679398 jaxutils-nightly-0.0.8.dev20230529/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-05-29 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-05-29 00:06:36.679398 jaxutils-nightly-0.0.8.dev20230529/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-05-29 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-05-29 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-05-29 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-05-29 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-05-29 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-29 00:06:36.675398 jaxutils-nightly-0.0.8.dev20230529/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-29 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-05-29 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-29 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-05-29 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-05-29 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230529/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-05-29 00:06:36.679398 jaxutils-nightly-0.0.8.dev20230529/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-05-29 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230529/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-05-29 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230529/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 00:06:22.834913 jaxutils-nightly-0.0.8.dev20230530/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-30 00:06:22.834913 jaxutils-nightly-0.0.8.dev20230530/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-05-30 00:06:15.000000 jaxutils-nightly-0.0.8.dev20230530/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 00:06:22.834913 jaxutils-nightly-0.0.8.dev20230530/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-05-30 00:06:15.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-05-30 00:06:22.834913 jaxutils-nightly-0.0.8.dev20230530/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-05-30 00:06:15.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-05-30 00:06:15.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-05-30 00:06:15.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-05-30 00:06:15.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-05-30 00:06:15.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 00:06:22.834913 jaxutils-nightly-0.0.8.dev20230530/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-30 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-05-30 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-30 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-05-30 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-05-30 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230530/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-05-30 00:06:22.834913 jaxutils-nightly-0.0.8.dev20230530/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-05-30 00:06:15.000000 jaxutils-nightly-0.0.8.dev20230530/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-05-30 00:06:15.000000 jaxutils-nightly-0.0.8.dev20230530/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230529/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230530/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230529
+Version: 0.0.8.dev20230530
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230529/README.md` & `jaxutils-nightly-0.0.8.dev20230530/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230529/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230530/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230529/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230530/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230529/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230530/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230529/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230530/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230529/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230530/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230529/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230530/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230529/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230530/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230529
+Version: 0.0.8.dev20230530
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230529/setup.py` & `jaxutils-nightly-0.0.8.dev20230530/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230529/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230530/versioneer.py`

 * *Files identical despite different names*

