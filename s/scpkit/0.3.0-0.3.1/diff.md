# Comparing `tmp/scpkit-0.3.0.tar.gz` & `tmp/scpkit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpkit-0.3.0.tar", last modified: Fri May 19 18:56:08 2023, max compression
+gzip compressed data, was "scpkit-0.3.1.tar", last modified: Wed May 31 12:49:38 2023, max compression
```

## Comparing `scpkit-0.3.0.tar` & `scpkit-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 18:55:59.000000 scpkit-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-19 18:56:08.132303 scpkit-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-19 18:55:59.000000 scpkit-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 18:55:59.000000 scpkit-0.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/scpkit/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/scpkit/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/scpkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:56:07.000000 scpkit-0.3.0/scpkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-19 18:56:08.132303 scpkit-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:55:59.000000 scpkit-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-19 18:55:59.000000 scpkit-0.3.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.043012 scpkit-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 12:49:24.000000 scpkit-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-31 12:49:38.043012 scpkit-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-31 12:49:24.000000 scpkit-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 12:49:24.000000 scpkit-0.3.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.039012 scpkit-0.3.1/scpkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.043012 scpkit-0.3.1/scpkit/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.043012 scpkit-0.3.1/scpkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:49:37.000000 scpkit-0.3.1/scpkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-31 12:49:38.043012 scpkit-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:49:24.000000 scpkit-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.043012 scpkit-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-31 12:49:24.000000 scpkit-0.3.1/tests/test.py
```

### Comparing `scpkit-0.3.0/LICENSE` & `scpkit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.0/PKG-INFO` & `scpkit-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.3.0
+Version: 0.3.1
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 # SCPkit
 [![GitHub Super-Linter](https://github.com/aquia-inc/scpkit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/aquia-inc/scpkit/actions/workflows/linter.yaml)
 
 ## Overview
 
-This project provides a python module to aid in Service Control Policy management in AWS accounts.
+This project provides a Python module to aid in Service Control Policy (SCP) management in AWS accounts.
 
 SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespace characters as they count toward the byte limit.
 
 
 ```mermaid
   stateDiagram-v2
       [SCPTool] --> Validate
```

### Comparing `scpkit-0.3.0/README.md` & `scpkit-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SCPkit
 [![GitHub Super-Linter](https://github.com/aquia-inc/scpkit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/aquia-inc/scpkit/actions/workflows/linter.yaml)
 
 ## Overview
 
-This project provides a python module to aid in Service Control Policy management in AWS accounts.
+This project provides a Python module to aid in Service Control Policy (SCP) management in AWS accounts.
 
 SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespace characters as they count toward the byte limit.
 
 
 ```mermaid
   stateDiagram-v2
       [SCPTool] --> Validate
```

### Comparing `scpkit-0.3.0/scpkit/main.py` & `scpkit-0.3.1/scpkit/main.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.0/scpkit/src/merge.py` & `scpkit-0.3.1/scpkit/src/merge.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.0/scpkit/src/model.py` & `scpkit-0.3.1/scpkit/src/model.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.0/scpkit/src/util.py` & `scpkit-0.3.1/scpkit/src/util.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.0/scpkit/src/validate.py` & `scpkit-0.3.1/scpkit/src/validate.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.0/scpkit.egg-info/PKG-INFO` & `scpkit-0.3.1/scpkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.3.0
+Version: 0.3.1
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 # SCPkit
 [![GitHub Super-Linter](https://github.com/aquia-inc/scpkit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/aquia-inc/scpkit/actions/workflows/linter.yaml)
 
 ## Overview
 
-This project provides a python module to aid in Service Control Policy management in AWS accounts.
+This project provides a Python module to aid in Service Control Policy (SCP) management in AWS accounts.
 
 SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespace characters as they count toward the byte limit.
 
 
 ```mermaid
   stateDiagram-v2
       [SCPTool] --> Validate
```

### Comparing `scpkit-0.3.0/setup.cfg` & `scpkit-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 project_urls = 
 	Bug Tracker = https://github.com/aquia-inc/scpkit/issues
 	Source = https://github.com/aquia-inc/scpkit
 description = This package helps consolidate service control policies in AWS
 license = Apache License 2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.3.0
+version = 0.3.1
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = file: requirements.txt
```

### Comparing `scpkit-0.3.0/tests/test.py` & `scpkit-0.3.1/tests/test.py`

 * *Files identical despite different names*

