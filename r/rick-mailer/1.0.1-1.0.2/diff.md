# Comparing `tmp/rick-mailer-1.0.1.tar.gz` & `tmp/rick-mailer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rick-mailer-1.0.1.tar", last modified: Mon May 22 07:45:12 2023, max compression
+gzip compressed data, was "rick-mailer-1.0.2.tar", last modified: Wed May 31 15:13:41 2023, max compression
```

## Comparing `rick-mailer-1.0.1.tar` & `rick-mailer-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.008975 rick-mailer-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-22 07:45:12.008975 rick-mailer-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.004975 rick-mailer-1.0.1/rick_mailer/
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.004975 rick-mailer-1.0.1/rick_mailer/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/locmem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/smtp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.004975 rick-mailer-1.0.1/rick_mailer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-22 07:45:12.008975 rick-mailer-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.008975 rick-mailer-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/custombackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    38249 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/test_mailer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:13:41.162247 rick-mailer-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-31 15:13:41.162247 rick-mailer-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:13:41.158247 rick-mailer-1.0.2/rick_mailer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/rick_mailer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:13:41.158247 rick-mailer-1.0.2/rick_mailer/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/rick_mailer/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/rick_mailer/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/rick_mailer/backends/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/rick_mailer/backends/locmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/rick_mailer/backends/smtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/rick_mailer/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/rick_mailer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:13:41.158247 rick-mailer-1.0.2/rick_mailer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-31 15:13:41.000000 rick-mailer-1.0.2/rick_mailer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-31 15:13:41.000000 rick-mailer-1.0.2/rick_mailer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:13:41.000000 rick-mailer-1.0.2/rick_mailer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:13:41.000000 rick-mailer-1.0.2/rick_mailer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 15:13:41.000000 rick-mailer-1.0.2/rick_mailer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 15:13:41.000000 rick-mailer-1.0.2/rick_mailer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-31 15:13:41.162247 rick-mailer-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:13:41.158247 rick-mailer-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/tests/custombackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38249 2023-05-31 15:13:25.000000 rick-mailer-1.0.2/tests/test_mailer.py
```

### Comparing `rick-mailer-1.0.1/LICENSE` & `rick-mailer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/PKG-INFO` & `rick-mailer-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rick-mailer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple library to send emails
 Home-page: https://git.oddbit.org/OddBit/rick-mailer
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/rick-mailer/
 Project-URL: Source, https://git.oddbit.org/OddBit/rick-mailer
 Classifier: Environment :: Web Environment
```

### Comparing `rick-mailer-1.0.1/README.md` & `rick-mailer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/rick_mailer/__init__.py` & `rick-mailer-1.0.2/rick_mailer/__init__.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/rick_mailer/backends/base.py` & `rick-mailer-1.0.2/rick_mailer/backends/base.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/rick_mailer/backends/console.py` & `rick-mailer-1.0.2/rick_mailer/backends/console.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/rick_mailer/backends/locmem.py` & `rick-mailer-1.0.2/rick_mailer/backends/locmem.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/rick_mailer/backends/smtp.py` & `rick-mailer-1.0.2/rick_mailer/backends/smtp.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/rick_mailer/message.py` & `rick-mailer-1.0.2/rick_mailer/message.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/rick_mailer/utils.py` & `rick-mailer-1.0.2/rick_mailer/utils.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/rick_mailer.egg-info/PKG-INFO` & `rick-mailer-1.0.2/rick_mailer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rick-mailer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple library to send emails
 Home-page: https://git.oddbit.org/OddBit/rick-mailer
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/rick-mailer/
 Project-URL: Source, https://git.oddbit.org/OddBit/rick-mailer
 Classifier: Environment :: Web Environment
```

### Comparing `rick-mailer-1.0.1/rick_mailer.egg-info/SOURCES.txt` & `rick-mailer-1.0.2/rick_mailer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/setup.cfg` & `rick-mailer-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rick-mailer
-version = 1.0.1
+version = 1.0.2
 url = https://git.oddbit.org/OddBit/rick-mailer
 author = João Pinheiro
 description = Simple library to send emails
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
 classifiers =
```

### Comparing `rick-mailer-1.0.1/tests/common.py` & `rick-mailer-1.0.2/tests/common.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/tests/test_backends.py` & `rick-mailer-1.0.2/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.1/tests/test_mailer.py` & `rick-mailer-1.0.2/tests/test_mailer.py`

 * *Files identical despite different names*

