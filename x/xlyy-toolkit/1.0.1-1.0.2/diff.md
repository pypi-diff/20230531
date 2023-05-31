# Comparing `tmp/xlyy_toolkit-1.0.1.tar.gz` & `tmp/xlyy_toolkit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlyy_toolkit-1.0.1.tar", last modified: Wed May 31 12:57:05 2023, max compression
+gzip compressed data, was "xlyy_toolkit-1.0.2.tar", last modified: Wed May 31 13:01:43 2023, max compression
```

## Comparing `xlyy_toolkit-1.0.1.tar` & `xlyy_toolkit-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:05.523677 xlyy_toolkit-1.0.1/
--rw-rw-rw-   0        0        0      210 2023-05-31 12:57:05.522681 xlyy_toolkit-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-31 12:57:05.523677 xlyy_toolkit-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      308 2023-05-31 12:56:01.000000 xlyy_toolkit-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:05.507731 xlyy_toolkit-1.0.1/xlyy_toolkit/
--rw-rw-rw-   0        0        0       65 2023-05-31 10:27:34.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:05.518695 xlyy_toolkit-1.0.1/xlyy_toolkit/common/
--rw-rw-rw-   0        0        0      109 2023-05-31 11:27:25.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/common/__init__.py
--rw-rw-rw-   0        0        0      309 2023-05-31 09:50:50.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/common/container_utils.py
--rw-rw-rw-   0        0        0      791 2023-05-31 09:46:40.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/common/file_utils.py
--rw-rw-rw-   0        0        0      870 2023-05-31 11:58:00.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/common/out_utils.py
--rw-rw-rw-   0        0        0     2339 2023-05-31 09:53:23.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/common/str_utils.py
--rw-rw-rw-   0        0        0       42 2023-05-31 10:30:31.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/common/test.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:05.520687 xlyy_toolkit-1.0.1/xlyy_toolkit/mysql/
--rw-rw-rw-   0        0        0       28 2023-05-31 10:22:29.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/mysql/__init__.py
--rw-rw-rw-   0        0        0     8665 2023-05-31 11:52:18.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/mysql/connect_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:05.521684 xlyy_toolkit-1.0.1/xlyy_toolkit/pyqt6/
--rw-rw-rw-   0        0        0       22 2023-05-31 10:22:29.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/pyqt6/__init__.py
--rw-rw-rw-   0        0        0     1137 2023-05-31 09:42:50.000000 xlyy_toolkit-1.0.1/xlyy_toolkit/pyqt6/w_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:05.512714 xlyy_toolkit-1.0.1/xlyy_toolkit.egg-info/
--rw-rw-rw-   0        0        0      210 2023-05-31 12:57:05.000000 xlyy_toolkit-1.0.1/xlyy_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-31 12:57:05.000000 xlyy_toolkit-1.0.1/xlyy_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 12:57:05.000000 xlyy_toolkit-1.0.1/xlyy_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-31 12:57:05.000000 xlyy_toolkit-1.0.1/xlyy_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 13:01:43.729966 xlyy_toolkit-1.0.2/
+-rw-rw-rw-   0        0        0      282 2023-05-31 13:01:43.728969 xlyy_toolkit-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2023-05-31 12:59:53.000000 xlyy_toolkit-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 13:01:43.729966 xlyy_toolkit-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      490 2023-05-31 13:01:39.000000 xlyy_toolkit-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:01:43.713023 xlyy_toolkit-1.0.2/xlyy_toolkit/
+-rw-rw-rw-   0        0        0       65 2023-05-31 10:27:34.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:01:43.723990 xlyy_toolkit-1.0.2/xlyy_toolkit/common/
+-rw-rw-rw-   0        0        0      109 2023-05-31 11:27:25.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/common/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-05-31 09:50:50.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/common/container_utils.py
+-rw-rw-rw-   0        0        0      791 2023-05-31 09:46:40.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/common/file_utils.py
+-rw-rw-rw-   0        0        0      870 2023-05-31 11:58:00.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/common/out_utils.py
+-rw-rw-rw-   0        0        0     2339 2023-05-31 09:53:23.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/common/str_utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 10:30:31.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/common/test.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:01:43.725979 xlyy_toolkit-1.0.2/xlyy_toolkit/mysql/
+-rw-rw-rw-   0        0        0       28 2023-05-31 10:22:29.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/mysql/__init__.py
+-rw-rw-rw-   0        0        0     8665 2023-05-31 11:52:18.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/mysql/connect_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:01:43.727974 xlyy_toolkit-1.0.2/xlyy_toolkit/pyqt6/
+-rw-rw-rw-   0        0        0       22 2023-05-31 10:22:29.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/pyqt6/__init__.py
+-rw-rw-rw-   0        0        0     1137 2023-05-31 09:42:50.000000 xlyy_toolkit-1.0.2/xlyy_toolkit/pyqt6/w_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:01:43.717009 xlyy_toolkit-1.0.2/xlyy_toolkit.egg-info/
+-rw-rw-rw-   0        0        0      282 2023-05-31 13:01:43.000000 xlyy_toolkit-1.0.2/xlyy_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-05-31 13:01:43.000000 xlyy_toolkit-1.0.2/xlyy_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 13:01:43.000000 xlyy_toolkit-1.0.2/xlyy_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 13:01:43.000000 xlyy_toolkit-1.0.2/xlyy_toolkit.egg-info/top_level.txt
```

### Comparing `xlyy_toolkit-1.0.1/xlyy_toolkit/common/file_utils.py` & `xlyy_toolkit-1.0.2/xlyy_toolkit/common/file_utils.py`

 * *Files identical despite different names*

### Comparing `xlyy_toolkit-1.0.1/xlyy_toolkit/common/out_utils.py` & `xlyy_toolkit-1.0.2/xlyy_toolkit/common/out_utils.py`

 * *Files identical despite different names*

### Comparing `xlyy_toolkit-1.0.1/xlyy_toolkit/common/str_utils.py` & `xlyy_toolkit-1.0.2/xlyy_toolkit/common/str_utils.py`

 * *Files identical despite different names*

### Comparing `xlyy_toolkit-1.0.1/xlyy_toolkit/mysql/connect_utils.py` & `xlyy_toolkit-1.0.2/xlyy_toolkit/mysql/connect_utils.py`

 * *Files identical despite different names*

### Comparing `xlyy_toolkit-1.0.1/xlyy_toolkit/pyqt6/w_utils.py` & `xlyy_toolkit-1.0.2/xlyy_toolkit/pyqt6/w_utils.py`

 * *Files identical despite different names*

