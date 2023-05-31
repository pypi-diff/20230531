# Comparing `tmp/custom-json-serializer-1234-1.2.tar.gz` & `tmp/custom-json-serializer-1234-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-json-serializer-1234-1.2.tar", last modified: Mon May 29 14:30:18 2023, max compression
+gzip compressed data, was "custom-json-serializer-1234-1.3.tar", last modified: Wed May 31 11:05:26 2023, max compression
```

## Comparing `custom-json-serializer-1234-1.2.tar` & `custom-json-serializer-1234-1.3.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-29 14:30:18.915149 custom-json-serializer-1234-1.2/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-29 14:30:18.915149 custom-json-serializer-1234-1.2/PKG-INFO
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-29 14:30:18.915149 custom-json-serializer-1234-1.2/core/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)       34 2023-05-29 13:37:10.000000 custom-json-serializer-1234-1.2/core/__init__.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1004 2023-05-23 20:56:03.000000 custom-json-serializer-1234-1.2/core/constants.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      302 2023-05-27 12:00:33.000000 custom-json-serializer-1234-1.2/core/factory.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-29 14:30:18.915149 custom-json-serializer-1234-1.2/core/formats/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-04-10 21:22:27.000000 custom-json-serializer-1234-1.2/core/formats/__init__.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-29 14:30:18.915149 custom-json-serializer-1234-1.2/core/formats/json/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-27 11:57:10.000000 custom-json-serializer-1234-1.2/core/formats/json/__init__.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      515 2023-05-27 11:57:29.000000 custom-json-serializer-1234-1.2/core/formats/json/json.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     4101 2023-05-27 12:02:36.000000 custom-json-serializer-1234-1.2/core/formats/parsers.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-29 14:30:18.915149 custom-json-serializer-1234-1.2/core/formats/xml/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-27 11:55:53.000000 custom-json-serializer-1234-1.2/core/formats/xml/__init__.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      682 2023-05-27 11:56:34.000000 custom-json-serializer-1234-1.2/core/formats/xml/constants.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      543 2023-05-27 12:02:44.000000 custom-json-serializer-1234-1.2/core/formats/xml/xml.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     7576 2023-05-29 11:01:17.000000 custom-json-serializer-1234-1.2/core/serializer.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-29 14:30:18.915149 custom-json-serializer-1234-1.2/custom_json_serializer_1234.egg-info/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-29 14:30:18.000000 custom-json-serializer-1234-1.2/custom_json_serializer_1234.egg-info/PKG-INFO
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      520 2023-05-29 14:30:18.000000 custom-json-serializer-1234-1.2/custom_json_serializer_1234.egg-info/SOURCES.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        1 2023-05-29 14:30:18.000000 custom-json-serializer-1234-1.2/custom_json_serializer_1234.egg-info/dependency_links.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      158 2023-05-29 14:30:18.000000 custom-json-serializer-1234-1.2/custom_json_serializer_1234.egg-info/requires.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        5 2023-05-29 14:30:18.000000 custom-json-serializer-1234-1.2/custom_json_serializer_1234.egg-info/top_level.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)       38 2023-05-29 14:30:18.915149 custom-json-serializer-1234-1.2/setup.cfg
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      602 2023-05-29 14:30:11.000000 custom-json-serializer-1234-1.2/setup.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/PKG-INFO
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/core/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      174 2023-05-29 14:08:22.000000 custom-json-serializer-1234-1.3/core/__init__.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      325 2023-05-30 22:15:14.000000 custom-json-serializer-1234-1.3/core/factory.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/core/helpers/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:46:44.000000 custom-json-serializer-1234-1.3/core/helpers/__init__.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1665 2023-05-30 12:10:09.000000 custom-json-serializer-1234-1.3/core/helpers/constants.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     7436 2023-05-31 10:37:09.000000 custom-json-serializer-1234-1.3/core/helpers/functions.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/core/serializers/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:44:29.000000 custom-json-serializer-1234-1.3/core/serializers/__init__.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2640 2023-05-30 22:50:19.000000 custom-json-serializer-1234-1.3/core/serializers/jsonserializer.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2783 2023-05-30 22:50:50.000000 custom-json-serializer-1234-1.3/core/serializers/xmlserializer.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/PKG-INFO
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      470 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/SOURCES.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        1 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/dependency_links.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1591 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/requires.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        5 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/top_level.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)       38 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/setup.cfg
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      602 2023-05-31 11:04:03.000000 custom-json-serializer-1234-1.3/setup.py
```

### Comparing `custom-json-serializer-1234-1.2/setup.py` & `custom-json-serializer-1234-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="custom-json-serializer-1234",
-    version="1.2",
+    version="1.3",
     description="serialization/deserialization package",
     url="https://github.com/donshester/PythonLabs/tree/lab3",
     author="Me",
     author_email="vlad.stepanov.2003@bk.ru",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
```

