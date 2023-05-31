# Comparing `tmp/custom-json-serializer-1234-1.5.tar.gz` & `tmp/custom-json-serializer-1234-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-json-serializer-1234-1.5.tar", last modified: Wed May 31 13:37:37 2023, max compression
+gzip compressed data, was "custom-json-serializer-1234-1.6.tar", last modified: Wed May 31 13:46:27 2023, max compression
```

## Comparing `custom-json-serializer-1234-1.5.tar` & `custom-json-serializer-1234-1.6.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/PKG-INFO
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/core/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      174 2023-05-29 14:08:22.000000 custom-json-serializer-1234-1.5/core/__init__.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      325 2023-05-30 22:15:14.000000 custom-json-serializer-1234-1.5/core/factory.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/core/helpers/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:46:44.000000 custom-json-serializer-1234-1.5/core/helpers/__init__.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1517 2023-05-31 11:21:37.000000 custom-json-serializer-1234-1.5/core/helpers/constants.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     7185 2023-05-31 11:19:21.000000 custom-json-serializer-1234-1.5/core/helpers/functions.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/core/serializers/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:44:29.000000 custom-json-serializer-1234-1.5/core/serializers/__init__.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2640 2023-05-30 22:50:19.000000 custom-json-serializer-1234-1.5/core/serializers/jsonserializer.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2783 2023-05-30 22:50:50.000000 custom-json-serializer-1234-1.5/core/serializers/xmlserializer.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/PKG-INFO
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      470 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/SOURCES.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        1 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/dependency_links.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1511 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/requires.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        5 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/top_level.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)       38 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/setup.cfg
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      602 2023-05-31 13:34:19.000000 custom-json-serializer-1234-1.5/setup.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:46:27.696189 custom-json-serializer-1234-1.6/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 13:46:27.696189 custom-json-serializer-1234-1.6/PKG-INFO
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:46:27.696189 custom-json-serializer-1234-1.6/core/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      174 2023-05-29 14:08:22.000000 custom-json-serializer-1234-1.6/core/__init__.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      325 2023-05-30 22:15:14.000000 custom-json-serializer-1234-1.6/core/factory.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:46:27.696189 custom-json-serializer-1234-1.6/core/helpers/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:46:44.000000 custom-json-serializer-1234-1.6/core/helpers/__init__.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1517 2023-05-31 11:21:37.000000 custom-json-serializer-1234-1.6/core/helpers/constants.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     7185 2023-05-31 11:19:21.000000 custom-json-serializer-1234-1.6/core/helpers/functions.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:46:27.696189 custom-json-serializer-1234-1.6/core/serializers/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:44:29.000000 custom-json-serializer-1234-1.6/core/serializers/__init__.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2640 2023-05-30 22:50:19.000000 custom-json-serializer-1234-1.6/core/serializers/jsonserializer.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2783 2023-05-30 22:50:50.000000 custom-json-serializer-1234-1.6/core/serializers/xmlserializer.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:46:27.696189 custom-json-serializer-1234-1.6/custom_json_serializer_1234.egg-info/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 13:46:27.000000 custom-json-serializer-1234-1.6/custom_json_serializer_1234.egg-info/PKG-INFO
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      420 2023-05-31 13:46:27.000000 custom-json-serializer-1234-1.6/custom_json_serializer_1234.egg-info/SOURCES.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        1 2023-05-31 13:46:27.000000 custom-json-serializer-1234-1.6/custom_json_serializer_1234.egg-info/dependency_links.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        5 2023-05-31 13:46:27.000000 custom-json-serializer-1234-1.6/custom_json_serializer_1234.egg-info/top_level.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)       38 2023-05-31 13:46:27.696189 custom-json-serializer-1234-1.6/setup.cfg
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      602 2023-05-31 13:46:20.000000 custom-json-serializer-1234-1.6/setup.py
```

### Comparing `custom-json-serializer-1234-1.5/core/helpers/constants.py` & `custom-json-serializer-1234-1.6/core/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `custom-json-serializer-1234-1.5/core/helpers/functions.py` & `custom-json-serializer-1234-1.6/core/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `custom-json-serializer-1234-1.5/core/serializers/jsonserializer.py` & `custom-json-serializer-1234-1.6/core/serializers/jsonserializer.py`

 * *Files identical despite different names*

### Comparing `custom-json-serializer-1234-1.5/core/serializers/xmlserializer.py` & `custom-json-serializer-1234-1.6/core/serializers/xmlserializer.py`

 * *Files identical despite different names*

### Comparing `custom-json-serializer-1234-1.5/setup.py` & `custom-json-serializer-1234-1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="custom-json-serializer-1234",
-    version="1.5",
+    version="1.6",
     description="serialization/deserialization package",
     url="https://github.com/donshester/PythonLabs/tree/lab3",
     author="Me",
     author_email="vlad.stepanov.2003@bk.ru",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
```

