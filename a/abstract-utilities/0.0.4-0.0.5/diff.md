# Comparing `tmp/abstract_utilities-0.0.4.tar.gz` & `tmp/abstract_utilities-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_utilities-0.0.4.tar", last modified: Wed May 31 04:42:19 2023, max compression
+gzip compressed data, was "abstract_utilities-0.0.5.tar", last modified: Wed May 31 04:44:44 2023, max compression
```

## Comparing `abstract_utilities-0.0.4.tar` & `abstract_utilities-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:42:19.516248 abstract_utilities-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     4706 2023-05-31 04:42:19.516248 abstract_utilities-0.0.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3953 2023-05-26 08:32:45.000000 abstract_utilities-0.0.4/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_utilities-0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 04:42:19.516248 abstract_utilities-0.0.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1205 2023-05-31 04:42:03.000000 abstract_utilities-0.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:42:19.508248 abstract_utilities-0.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:42:19.516248 abstract_utilities-0.0.4/src/abstract_utilities/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 06:03:57.000000 abstract_utilities-0.0.4/src/abstract_utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8064 2023-05-31 04:41:41.000000 abstract_utilities-0.0.4/src/abstract_utilities/class_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1346 2023-05-31 02:00:01.000000 abstract_utilities-0.0.4/src/abstract_utilities/collator_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1538 2023-05-26 09:14:05.000000 abstract_utilities-0.0.4/src/abstract_utilities/compare_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2176 2023-05-31 04:38:20.000000 abstract_utilities-0.0.4/src/abstract_utilities/global_utils.py
--rw-rw-r--   0 root         (0) root         (0)     6569 2023-05-31 02:30:30.000000 abstract_utilities-0.0.4/src/abstract_utilities/json_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1016 2023-05-26 06:03:57.000000 abstract_utilities-0.0.4/src/abstract_utilities/list_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_utilities-0.0.4/src/abstract_utilities/main.py
--rw-rw-r--   0 root         (0) root         (0)      810 2023-05-26 06:03:57.000000 abstract_utilities-0.0.4/src/abstract_utilities/math_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3961 2023-05-31 02:05:43.000000 abstract_utilities-0.0.4/src/abstract_utilities/read_write_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4568 2023-05-31 02:01:18.000000 abstract_utilities-0.0.4/src/abstract_utilities/string_clean.py
--rw-rw-r--   0 root         (0) root         (0)     1407 2023-05-31 02:21:17.000000 abstract_utilities-0.0.4/src/abstract_utilities/thread_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4660 2023-05-26 06:03:57.000000 abstract_utilities-0.0.4/src/abstract_utilities/time_utils.py
--rw-rw-r--   0 root         (0) root         (0)    18229 2023-05-26 22:18:18.000000 abstract_utilities-0.0.4/src/abstract_utilities/type_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:42:19.516248 abstract_utilities-0.0.4/src/abstract_utilities.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     4706 2023-05-31 04:42:19.000000 abstract_utilities-0.0.4/src/abstract_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      747 2023-05-31 04:42:19.000000 abstract_utilities-0.0.4/src/abstract_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-31 04:42:19.000000 abstract_utilities-0.0.4/src/abstract_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       19 2023-05-31 04:42:19.000000 abstract_utilities-0.0.4/src/abstract_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:44:44.046858 abstract_utilities-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     4706 2023-05-31 04:44:44.046858 abstract_utilities-0.0.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3953 2023-05-26 08:32:45.000000 abstract_utilities-0.0.5/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_utilities-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 04:44:44.046858 abstract_utilities-0.0.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1205 2023-05-31 04:44:25.000000 abstract_utilities-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:44:44.038858 abstract_utilities-0.0.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:44:44.042858 abstract_utilities-0.0.5/src/abstract_utilities/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-26 06:03:57.000000 abstract_utilities-0.0.5/src/abstract_utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8064 2023-05-31 04:41:41.000000 abstract_utilities-0.0.5/src/abstract_utilities/class_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1346 2023-05-31 02:00:01.000000 abstract_utilities-0.0.5/src/abstract_utilities/collator_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1538 2023-05-26 09:14:05.000000 abstract_utilities-0.0.5/src/abstract_utilities/compare_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2176 2023-05-31 04:44:16.000000 abstract_utilities-0.0.5/src/abstract_utilities/global_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     6569 2023-05-31 02:30:30.000000 abstract_utilities-0.0.5/src/abstract_utilities/json_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1016 2023-05-26 06:03:57.000000 abstract_utilities-0.0.5/src/abstract_utilities/list_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-05-29 11:40:08.000000 abstract_utilities-0.0.5/src/abstract_utilities/main.py
+-rw-rw-r--   0 root         (0) root         (0)      810 2023-05-26 06:03:57.000000 abstract_utilities-0.0.5/src/abstract_utilities/math_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3961 2023-05-31 02:05:43.000000 abstract_utilities-0.0.5/src/abstract_utilities/read_write_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4568 2023-05-31 02:01:18.000000 abstract_utilities-0.0.5/src/abstract_utilities/string_clean.py
+-rw-rw-r--   0 root         (0) root         (0)     1407 2023-05-31 02:21:17.000000 abstract_utilities-0.0.5/src/abstract_utilities/thread_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4660 2023-05-26 06:03:57.000000 abstract_utilities-0.0.5/src/abstract_utilities/time_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    18229 2023-05-26 22:18:18.000000 abstract_utilities-0.0.5/src/abstract_utilities/type_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:44:44.046858 abstract_utilities-0.0.5/src/abstract_utilities.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     4706 2023-05-31 04:44:44.000000 abstract_utilities-0.0.5/src/abstract_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      747 2023-05-31 04:44:44.000000 abstract_utilities-0.0.5/src/abstract_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-31 04:44:44.000000 abstract_utilities-0.0.5/src/abstract_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       19 2023-05-31 04:44:44.000000 abstract_utilities-0.0.5/src/abstract_utilities.egg-info/top_level.txt
```

### Comparing `abstract_utilities-0.0.4/PKG-INFO` & `abstract_utilities-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_utilities
-Version: 0.0.4
+Version: 0.0.5
 Summary: abstract_utilities is a collection of utility modules providing a variety of functions to aid in tasks such as data comparison, list manipulation, JSON handling, string manipulation, mathematical computations, and time operations.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_utilities
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_utilities-0.0.4/README.md` & `abstract_utilities-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/setup.py` & `abstract_utilities-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_utilities',
-    version='0.0.4',
+    version='0.0.5',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_utilities is a collection of utility modules providing a variety of functions to aid in tasks such as data comparison, list manipulation, JSON handling, string manipulation, mathematical computations, and time operations.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/abstract_endeavors/abstract_essentials/abstract_utilities',
     classifiers=[
```

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/class_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/class_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/collator_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/collator_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/compare_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/compare_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/global_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/global_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 def global_registry(name:str,glob:dict):
-    global_registry = if_none_default(string='global_registry',glob=globals(),default={"registry_names":[],"registry_index":[]))
+    global_registry = if_none_default(string='global_registry',glob=globals(),default={"registry_names":[],"registry_index":[]})
     if name not in global_registry['registry_names']:
         if glob == None:
             return None
         global_registry['registry_names'].append(name)
         global_registry['registry_index'].append(glob)
     length = len(global_registry['registry_names']) 
     change_glob('global_registry',global_registry)
```

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/json_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/json_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/list_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/list_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/main.py` & `abstract_utilities-0.0.5/src/abstract_utilities/main.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/math_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/math_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/read_write_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/read_write_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/string_clean.py` & `abstract_utilities-0.0.5/src/abstract_utilities/string_clean.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/thread_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/thread_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/time_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/time_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities/type_utils.py` & `abstract_utilities-0.0.5/src/abstract_utilities/type_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities.egg-info/PKG-INFO` & `abstract_utilities-0.0.5/src/abstract_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-utilities
-Version: 0.0.4
+Version: 0.0.5
 Summary: abstract_utilities is a collection of utility modules providing a variety of functions to aid in tasks such as data comparison, list manipulation, JSON handling, string manipulation, mathematical computations, and time operations.
 Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_utilities
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_utilities-0.0.4/src/abstract_utilities.egg-info/SOURCES.txt` & `abstract_utilities-0.0.5/src/abstract_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

