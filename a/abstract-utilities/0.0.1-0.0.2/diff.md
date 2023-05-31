# Comparing `tmp/abstract_utilities-0.0.1.tar.gz` & `tmp/abstract_utilities-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_utilities-0.0.1.tar", last modified: Wed May 31 02:08:47 2023, max compression
+gzip compressed data, was "abstract_utilities-0.0.2.tar", last modified: Wed May 31 02:26:57 2023, max compression
```

## Comparing `abstract_utilities-0.0.1.tar` & `abstract_utilities-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:47.025282 abstract_utilities-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     4706 2023-05-31 02:08:47.025282 abstract_utilities-0.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3953 2023-05-26 08:32:45.000000 abstract_utilities-0.0.1/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_utilities-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 02:08:47.025282 abstract_utilities-0.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1205 2023-05-31 02:07:51.000000 abstract_utilities-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:47.013282 abstract_utilities-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:47.021282 abstract_utilities-0.0.1/src/abstract_utilities/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 06:03:57.000000 abstract_utilities-0.0.1/src/abstract_utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9005 2023-05-26 13:06:56.000000 abstract_utilities-0.0.1/src/abstract_utilities/class_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1346 2023-05-31 02:00:01.000000 abstract_utilities-0.0.1/src/abstract_utilities/collator_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1538 2023-05-26 09:14:05.000000 abstract_utilities-0.0.1/src/abstract_utilities/compare_utils.py
--rw-rw-r--   0 root         (0) root         (0)      305 2023-05-29 06:30:45.000000 abstract_utilities-0.0.1/src/abstract_utilities/global_utils.py
--rw-rw-r--   0 root         (0) root         (0)     7101 2023-05-29 06:28:49.000000 abstract_utilities-0.0.1/src/abstract_utilities/json_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1016 2023-05-26 06:03:57.000000 abstract_utilities-0.0.1/src/abstract_utilities/list_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_utilities-0.0.1/src/abstract_utilities/main.py
--rw-rw-r--   0 root         (0) root         (0)      810 2023-05-26 06:03:57.000000 abstract_utilities-0.0.1/src/abstract_utilities/math_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3961 2023-05-31 02:05:43.000000 abstract_utilities-0.0.1/src/abstract_utilities/read_write_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4568 2023-05-31 02:01:18.000000 abstract_utilities-0.0.1/src/abstract_utilities/string_clean.py
--rw-rw-r--   0 root         (0) root         (0)     4660 2023-05-26 06:03:57.000000 abstract_utilities-0.0.1/src/abstract_utilities/time_utils.py
--rw-rw-r--   0 root         (0) root         (0)    18229 2023-05-26 22:18:18.000000 abstract_utilities-0.0.1/src/abstract_utilities/type_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:47.021282 abstract_utilities-0.0.1/src/abstract_utilities.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     4706 2023-05-31 02:08:46.000000 abstract_utilities-0.0.1/src/abstract_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      708 2023-05-31 02:08:47.000000 abstract_utilities-0.0.1/src/abstract_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-31 02:08:46.000000 abstract_utilities-0.0.1/src/abstract_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       19 2023-05-31 02:08:46.000000 abstract_utilities-0.0.1/src/abstract_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:26:57.228634 abstract_utilities-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     4706 2023-05-31 02:26:57.228634 abstract_utilities-0.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3953 2023-05-26 08:32:45.000000 abstract_utilities-0.0.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_utilities-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 02:26:57.228634 abstract_utilities-0.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1205 2023-05-31 02:26:02.000000 abstract_utilities-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:26:57.220634 abstract_utilities-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:26:57.228634 abstract_utilities-0.0.2/src/abstract_utilities/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 06:03:57.000000 abstract_utilities-0.0.2/src/abstract_utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9005 2023-05-26 13:06:56.000000 abstract_utilities-0.0.2/src/abstract_utilities/class_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1346 2023-05-31 02:00:01.000000 abstract_utilities-0.0.2/src/abstract_utilities/collator_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1538 2023-05-26 09:14:05.000000 abstract_utilities-0.0.2/src/abstract_utilities/compare_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      305 2023-05-29 06:30:45.000000 abstract_utilities-0.0.2/src/abstract_utilities/global_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     7101 2023-05-29 06:28:49.000000 abstract_utilities-0.0.2/src/abstract_utilities/json_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1016 2023-05-26 06:03:57.000000 abstract_utilities-0.0.2/src/abstract_utilities/list_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_utilities-0.0.2/src/abstract_utilities/main.py
+-rw-rw-r--   0 root         (0) root         (0)      810 2023-05-26 06:03:57.000000 abstract_utilities-0.0.2/src/abstract_utilities/math_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3961 2023-05-31 02:05:43.000000 abstract_utilities-0.0.2/src/abstract_utilities/read_write_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4568 2023-05-31 02:01:18.000000 abstract_utilities-0.0.2/src/abstract_utilities/string_clean.py
+-rw-rw-r--   0 root         (0) root         (0)     1407 2023-05-31 02:21:17.000000 abstract_utilities-0.0.2/src/abstract_utilities/thread_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4660 2023-05-26 06:03:57.000000 abstract_utilities-0.0.2/src/abstract_utilities/time_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    18229 2023-05-26 22:18:18.000000 abstract_utilities-0.0.2/src/abstract_utilities/type_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:26:57.228634 abstract_utilities-0.0.2/src/abstract_utilities.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     4706 2023-05-31 02:26:57.000000 abstract_utilities-0.0.2/src/abstract_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      747 2023-05-31 02:26:57.000000 abstract_utilities-0.0.2/src/abstract_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-31 02:26:57.000000 abstract_utilities-0.0.2/src/abstract_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       19 2023-05-31 02:26:57.000000 abstract_utilities-0.0.2/src/abstract_utilities.egg-info/top_level.txt
```

### Comparing `abstract_utilities-0.0.1/PKG-INFO` & `abstract_utilities-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_utilities
-Version: 0.0.1
+Version: 0.0.2
 Summary: abstract_utilities is a collection of utility modules providing a variety of functions to aid in tasks such as data comparison, list manipulation, JSON handling, string manipulation, mathematical computations, and time operations.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_utilities
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_utilities-0.0.1/README.md` & `abstract_utilities-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/setup.py` & `abstract_utilities-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_utilities',
-    version='0.0.1',
+    version='0.0.2',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_utilities is a collection of utility modules providing a variety of functions to aid in tasks such as data comparison, list manipulation, JSON handling, string manipulation, mathematical computations, and time operations.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/abstract_endeavors/abstract_essentials/abstract_utilities',
     classifiers=[
```

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/class_utils.py` & `abstract_utilities-0.0.2/src/abstract_utilities/class_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/collator_utils.py` & `abstract_utilities-0.0.2/src/abstract_utilities/collator_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/compare_utils.py` & `abstract_utilities-0.0.2/src/abstract_utilities/compare_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/json_utils.py` & `abstract_utilities-0.0.2/src/abstract_utilities/json_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/list_utils.py` & `abstract_utilities-0.0.2/src/abstract_utilities/list_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/main.py` & `abstract_utilities-0.0.2/src/abstract_utilities/main.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/math_utils.py` & `abstract_utilities-0.0.2/src/abstract_utilities/math_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/read_write_utils.py` & `abstract_utilities-0.0.2/src/abstract_utilities/read_write_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/string_clean.py` & `abstract_utilities-0.0.2/src/abstract_utilities/string_clean.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/time_utils.py` & `abstract_utilities-0.0.2/src/abstract_utilities/time_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities/type_utils.py` & `abstract_utilities-0.0.2/src/abstract_utilities/type_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities.egg-info/PKG-INFO` & `abstract_utilities-0.0.2/src/abstract_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-utilities
-Version: 0.0.1
+Version: 0.0.2
 Summary: abstract_utilities is a collection of utility modules providing a variety of functions to aid in tasks such as data comparison, list manipulation, JSON handling, string manipulation, mathematical computations, and time operations.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_utilities
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_utilities-0.0.1/src/abstract_utilities.egg-info/SOURCES.txt` & `abstract_utilities-0.0.2/src/abstract_utilities.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 src/abstract_utilities/global_utils.py
 src/abstract_utilities/json_utils.py
 src/abstract_utilities/list_utils.py
 src/abstract_utilities/main.py
 src/abstract_utilities/math_utils.py
 src/abstract_utilities/read_write_utils.py
 src/abstract_utilities/string_clean.py
+src/abstract_utilities/thread_utils.py
 src/abstract_utilities/time_utils.py
 src/abstract_utilities/type_utils.py
 src/abstract_utilities.egg-info/PKG-INFO
 src/abstract_utilities.egg-info/SOURCES.txt
 src/abstract_utilities.egg-info/dependency_links.txt
 src/abstract_utilities.egg-info/top_level.txt
```

