# Comparing `tmp/serialization_tool-1.51.tar.gz` & `tmp/serialization_tool-1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialization_tool-1.51.tar", last modified: Tue May 30 20:40:15 2023, max compression
+gzip compressed data, was "serialization_tool-1.52.tar", last modified: Wed May 31 14:00:16 2023, max compression
```

## Comparing `serialization_tool-1.51.tar` & `serialization_tool-1.52.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.806386 serialization_tool-1.51/
--rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-1.51/LICENSE.txt
--rw-rw-rw-   0        0        0      314 2023-05-30 20:40:15.807387 serialization_tool-1.51/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-1.51/README.md
--rw-rw-rw-   0        0        0      115 2023-05-30 20:40:15.821301 serialization_tool-1.51/setup.cfg
--rw-rw-rw-   0        0        0      490 2023-05-30 20:40:12.000000 serialization_tool-1.51/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.705177 serialization_tool-1.51/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.718501 serialization_tool-1.51/src/serialization_tool/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.51/src/serialization_tool/__init__.py
--rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-1.51/src/serialization_tool/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.783801 serialization_tool-1.51/src/serialization_tool/serialization/
--rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-1.51/src/serialization_tool/serialization/__init__.py
--rw-rw-rw-   0        0        0     2240 2023-05-30 17:28:57.000000 serialization_tool-1.51/src/serialization_tool/serialization/constants.py
--rw-rw-rw-   0        0        0    11717 2023-05-30 20:39:01.000000 serialization_tool-1.51/src/serialization_tool/serialization/serializer.py
--rw-rw-rw-   0        0        0      725 2023-05-18 09:47:32.000000 serialization_tool-1.51/src/serialization_tool/serialization_factory.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.787309 serialization_tool-1.51/src/serialization_tool/types/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.51/src/serialization_tool/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.797368 serialization_tool-1.51/src/serialization_tool/types/json/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.51/src/serialization_tool/types/json/__init__.py
--rw-rw-rw-   0        0        0      850 2023-05-30 16:17:26.000000 serialization_tool-1.51/src/serialization_tool/types/json/constants.py
--rw-rw-rw-   0        0        0      536 2023-05-30 18:02:49.000000 serialization_tool-1.51/src/serialization_tool/types/json/json.py
--rw-rw-rw-   0        0        0     2032 2023-05-30 20:38:34.000000 serialization_tool-1.51/src/serialization_tool/types/json/utilities.py
--rw-rw-rw-   0        0        0     1012 2023-05-18 09:50:41.000000 serialization_tool-1.51/src/serialization_tool/types/serialization.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.805385 serialization_tool-1.51/src/serialization_tool/types/xml/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.51/src/serialization_tool/types/xml/__init__.py
--rw-rw-rw-   0        0        0      371 2023-05-30 17:50:19.000000 serialization_tool-1.51/src/serialization_tool/types/xml/constants.py
--rw-rw-rw-   0        0        0     2264 2023-05-30 20:38:44.000000 serialization_tool-1.51/src/serialization_tool/types/xml/utilities.py
--rw-rw-rw-   0        0        0     1038 2023-05-30 18:00:48.000000 serialization_tool-1.51/src/serialization_tool/types/xml/xml.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.778793 serialization_tool-1.51/src/serialization_tool.egg-info/
--rw-rw-rw-   0        0        0      314 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      984 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 14:00:16.159007 serialization_tool-1.52/
+-rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-1.52/LICENSE.txt
+-rw-rw-rw-   0        0        0      314 2023-05-31 14:00:16.159007 serialization_tool-1.52/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-1.52/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-31 14:00:16.163003 serialization_tool-1.52/setup.cfg
+-rw-rw-rw-   0        0        0      476 2023-05-31 14:00:12.000000 serialization_tool-1.52/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:00:16.051016 serialization_tool-1.52/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 14:00:16.079001 serialization_tool-1.52/src/serialization_tool/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.52/src/serialization_tool/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-1.52/src/serialization_tool/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:00:16.123014 serialization_tool-1.52/src/serialization_tool/serialization/
+-rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-1.52/src/serialization_tool/serialization/__init__.py
+-rw-rw-rw-   0        0        0     2240 2023-05-31 12:52:30.000000 serialization_tool-1.52/src/serialization_tool/serialization/constants.py
+-rw-rw-rw-   0        0        0    11717 2023-05-31 12:52:30.000000 serialization_tool-1.52/src/serialization_tool/serialization/serializer.py
+-rw-rw-rw-   0        0        0      725 2023-05-18 09:47:32.000000 serialization_tool-1.52/src/serialization_tool/serialization_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:00:16.131004 serialization_tool-1.52/src/serialization_tool/types/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.52/src/serialization_tool/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:00:16.143001 serialization_tool-1.52/src/serialization_tool/types/json/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.52/src/serialization_tool/types/json/__init__.py
+-rw-rw-rw-   0        0        0      850 2023-05-31 12:52:30.000000 serialization_tool-1.52/src/serialization_tool/types/json/constants.py
+-rw-rw-rw-   0        0        0      536 2023-05-31 12:52:30.000000 serialization_tool-1.52/src/serialization_tool/types/json/json.py
+-rw-rw-rw-   0        0        0     2032 2023-05-31 12:52:30.000000 serialization_tool-1.52/src/serialization_tool/types/json/utilities.py
+-rw-rw-rw-   0        0        0     1012 2023-05-18 09:50:41.000000 serialization_tool-1.52/src/serialization_tool/types/serialization.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:00:16.155014 serialization_tool-1.52/src/serialization_tool/types/xml/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.52/src/serialization_tool/types/xml/__init__.py
+-rw-rw-rw-   0        0        0      371 2023-05-31 12:52:30.000000 serialization_tool-1.52/src/serialization_tool/types/xml/constants.py
+-rw-rw-rw-   0        0        0     2264 2023-05-31 12:52:30.000000 serialization_tool-1.52/src/serialization_tool/types/xml/utilities.py
+-rw-rw-rw-   0        0        0     1038 2023-05-31 12:52:30.000000 serialization_tool-1.52/src/serialization_tool/types/xml/xml.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:00:16.115006 serialization_tool-1.52/src/serialization_tool.egg-info/
+-rw-rw-rw-   0        0        0      314 2023-05-31 14:00:15.000000 serialization_tool-1.52/src/serialization_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2023-05-31 14:00:15.000000 serialization_tool-1.52/src/serialization_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:00:15.000000 serialization_tool-1.52/src/serialization_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 14:00:15.000000 serialization_tool-1.52/src/serialization_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-31 14:00:15.000000 serialization_tool-1.52/src/serialization_tool.egg-info/top_level.txt
```

### Comparing `serialization_tool-1.51/LICENSE.txt` & `serialization_tool-1.52/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool/serialization/constants.py` & `serialization_tool-1.52/src/serialization_tool/serialization/constants.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool/serialization/serializer.py` & `serialization_tool-1.52/src/serialization_tool/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool/serialization_factory.py` & `serialization_tool-1.52/src/serialization_tool/serialization_factory.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool/types/json/constants.py` & `serialization_tool-1.52/src/serialization_tool/types/json/constants.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool/types/json/json.py` & `serialization_tool-1.52/src/serialization_tool/types/json/json.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool/types/json/utilities.py` & `serialization_tool-1.52/src/serialization_tool/types/json/utilities.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool/types/serialization.py` & `serialization_tool-1.52/src/serialization_tool/types/serialization.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool/types/xml/utilities.py` & `serialization_tool-1.52/src/serialization_tool/types/xml/utilities.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool/types/xml/xml.py` & `serialization_tool-1.52/src/serialization_tool/types/xml/xml.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.51/src/serialization_tool.egg-info/SOURCES.txt` & `serialization_tool-1.52/src/serialization_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

