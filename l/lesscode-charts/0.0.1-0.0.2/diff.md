# Comparing `tmp/lesscode_charts-0.0.1.tar.gz` & `tmp/lesscode_charts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_charts-0.0.1.tar", last modified: Fri May 19 07:53:45 2023, max compression
+gzip compressed data, was "dist/lesscode_charts-0.0.2.tar", last modified: Wed May 31 09:14:34 2023, max compression
```

## Comparing `lesscode_charts-0.0.1.tar` & `lesscode_charts-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/
--rw-r--r--   0 baai       (501) staff       (20)     6563 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)     6228 2023-05-19 01:12:56.000000 lesscode_charts-0.0.1/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/lesscode_charts/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.1/lesscode_charts/__init__.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/lesscode_charts/utils/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.1/lesscode_charts/utils/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)      966 2023-05-19 07:36:01.000000 lesscode_charts-0.0.1/lesscode_charts/utils/common_utils.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/lesscode_charts/v1/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.1/lesscode_charts/v1/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.1/lesscode_charts/v1/forest_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     2106 2023-05-19 07:48:32.000000 lesscode_charts-0.0.1/lesscode_charts/v1/histogram_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.1/lesscode_charts/v1/k_line_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1437 2023-05-19 03:41:10.000000 lesscode_charts-0.0.1/lesscode_charts/v1/pie_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1058 2023-05-19 07:29:22.000000 lesscode_charts-0.0.1/lesscode_charts/v1/pyramid_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.1/lesscode_charts/v1/radar_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1281 2023-05-19 07:29:21.000000 lesscode_charts-0.0.1/lesscode_charts/v1/sankey_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     3088 2023-05-19 02:50:25.000000 lesscode_charts-0.0.1/lesscode_charts/v1/table_chart.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-05-19 07:50:40.000000 lesscode_charts-0.0.1/lesscode_charts/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/lesscode_charts.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)     6563 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/lesscode_charts.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      611 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/lesscode_charts.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/lesscode_charts.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       16 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/lesscode_charts.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-05-19 07:53:45.000000 lesscode_charts-0.0.1/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1300 2023-05-19 07:52:58.000000 lesscode_charts-0.0.1/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.2/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.2/lesscode_charts/__init__.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts/utils/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.2/lesscode_charts/utils/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.2/lesscode_charts/utils/common_utils.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts/v1/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.2/lesscode_charts/v1/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.2/lesscode_charts/v1/forest_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     2106 2023-05-19 07:48:32.000000 lesscode_charts-0.0.2/lesscode_charts/v1/histogram_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.2/lesscode_charts/v1/k_line_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1437 2023-05-19 03:41:10.000000 lesscode_charts-0.0.2/lesscode_charts/v1/pie_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1058 2023-05-19 07:29:22.000000 lesscode_charts-0.0.2/lesscode_charts/v1/pyramid_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.2/lesscode_charts/v1/radar_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1911 2023-05-31 09:14:31.000000 lesscode_charts-0.0.2/lesscode_charts/v1/sankey_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3088 2023-05-19 02:50:25.000000 lesscode_charts-0.0.2/lesscode_charts/v1/table_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-05-31 09:14:31.000000 lesscode_charts-0.0.2/lesscode_charts/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      611 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       16 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.2/setup.py
```

### Comparing `lesscode_charts-0.0.1/lesscode_charts/utils/common_utils.py` & `lesscode_charts-0.0.2/lesscode_charts/utils/common_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,7 +32,16 @@
                 x["children"] = []
             parent["children"].append(x)
         else:
             if not x.get("children"):
                 x["children"] = []
             result.append(x)
     return result
+
+
+def dict2list(data: dict, data_key="count", key_name="key", value_name="value"):
+    result = []
+    for key, value in data.items():
+        if data_key:
+            value = value.get(data_key)
+        result.append({key_name: key, value_name: value})
+    return result
```

### Comparing `lesscode_charts-0.0.1/lesscode_charts/v1/forest_chart.py` & `lesscode_charts-0.0.2/lesscode_charts/v1/forest_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.1/lesscode_charts/v1/histogram_chart.py` & `lesscode_charts-0.0.2/lesscode_charts/v1/histogram_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.1/lesscode_charts/v1/k_line_chart.py` & `lesscode_charts-0.0.2/lesscode_charts/v1/k_line_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.1/lesscode_charts/v1/pie_chart.py` & `lesscode_charts-0.0.2/lesscode_charts/v1/pie_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.1/lesscode_charts/v1/pyramid_chart.py` & `lesscode_charts-0.0.2/lesscode_charts/v1/pyramid_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.1/lesscode_charts/v1/radar_chart.py` & `lesscode_charts-0.0.2/lesscode_charts/v1/radar_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.1/lesscode_charts/v1/table_chart.py` & `lesscode_charts-0.0.2/lesscode_charts/v1/table_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.1/lesscode_charts.egg-info/SOURCES.txt` & `lesscode_charts-0.0.2/lesscode_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.1/setup.py` & `lesscode_charts-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # -*- coding: utf-8 -*-
 
-import shutil
-
 import setuptools
-from setuptools.command.install_scripts import install_scripts
+
 from lesscode_charts.version import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lesscode_charts",
```

