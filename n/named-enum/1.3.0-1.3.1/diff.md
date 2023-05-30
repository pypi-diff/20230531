# Comparing `tmp/named_enum-1.3.0.tar.gz` & `tmp/named_enum-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "named_enum-1.3.0.tar", last modified: Wed May 10 22:04:28 2023, max compression
+gzip compressed data, was "named_enum-1.3.1.tar", last modified: Tue May 30 23:12:12 2023, max compression
```

## Comparing `named_enum-1.3.0.tar` & `named_enum-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:04:28.316132 named_enum-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 22:04:17.000000 named_enum-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:04:17.000000 named_enum-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-05-10 22:04:28.316132 named_enum-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-10 22:04:17.000000 named_enum-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:04:28.316132 named_enum-1.3.0/named_enum/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 22:04:17.000000 named_enum-1.3.0/named_enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20249 2023-05-10 22:04:17.000000 named_enum-1.3.0/named_enum/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    24232 2023-05-10 22:04:17.000000 named_enum-1.3.0/named_enum/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 22:04:17.000000 named_enum-1.3.0/named_enum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:04:28.316132 named_enum-1.3.0/named_enum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-10 22:04:28.316132 named_enum-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-10 22:04:17.000000 named_enum-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:12:12.855071 named_enum-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-30 23:12:01.000000 named_enum-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 23:12:01.000000 named_enum-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-05-30 23:12:12.855071 named_enum-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-30 23:12:01.000000 named_enum-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:12:12.855071 named_enum-1.3.1/named_enum/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 23:12:01.000000 named_enum-1.3.1/named_enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20249 2023-05-30 23:12:01.000000 named_enum-1.3.1/named_enum/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24232 2023-05-30 23:12:01.000000 named_enum-1.3.1/named_enum/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 23:12:01.000000 named_enum-1.3.1/named_enum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:12:12.855071 named_enum-1.3.1/named_enum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-05-30 23:12:12.000000 named_enum-1.3.1/named_enum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-30 23:12:12.000000 named_enum-1.3.1/named_enum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 23:12:12.000000 named_enum-1.3.1/named_enum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 23:12:12.000000 named_enum-1.3.1/named_enum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 23:12:12.000000 named_enum-1.3.1/named_enum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 23:12:12.000000 named_enum-1.3.1/named_enum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-30 23:12:12.859071 named_enum-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-30 23:12:01.000000 named_enum-1.3.1/setup.py
```

### Comparing `named_enum-1.3.0/LICENSE` & `named_enum-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `named_enum-1.3.0/PKG-INFO` & `named_enum-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: named_enum
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python named enumeration, which extends the built-in Enum class with extra features.
 Home-page: https://github.com/zhiwei2017/named_enum
 Author: Zhiwei Zhang
 Author-email: zhiwei2017@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -437,8 +436,7 @@
 Author
 ------
 
 * `Zhiwei Zhang <https://github.com/zhiwei2017>`_ - *Maintainer* - `zhiwei2017@gmail.com <mailto:zhiwei2017@gmail.com?subject=[GitHub]Named%20Enum>`_
 * `Jianlan Shao <https://github.com/Lan314>`_ - *Developer* - `jianlan.shao@gmail.com <mailto:jianlan.shao@gmail.com?subject=[GitHub]Named%20Enum>`_
 
 **[ ~ Dependencies scanned by** `PyUp.io <https://pyup.io>`_ **~ ]**
-
```

### Comparing `named_enum-1.3.0/README.rst` & `named_enum-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `named_enum-1.3.0/named_enum/enum.py` & `named_enum-1.3.1/named_enum/enum.py`

 * *Files identical despite different names*

### Comparing `named_enum-1.3.0/named_enum/meta.py` & `named_enum-1.3.1/named_enum/meta.py`

 * *Files identical despite different names*

### Comparing `named_enum-1.3.0/named_enum.egg-info/PKG-INFO` & `named_enum-1.3.1/named_enum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: named-enum
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python named enumeration, which extends the built-in Enum class with extra features.
 Home-page: https://github.com/zhiwei2017/named_enum
 Author: Zhiwei Zhang
 Author-email: zhiwei2017@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -437,8 +436,7 @@
 Author
 ------
 
 * `Zhiwei Zhang <https://github.com/zhiwei2017>`_ - *Maintainer* - `zhiwei2017@gmail.com <mailto:zhiwei2017@gmail.com?subject=[GitHub]Named%20Enum>`_
 * `Jianlan Shao <https://github.com/Lan314>`_ - *Developer* - `jianlan.shao@gmail.com <mailto:jianlan.shao@gmail.com?subject=[GitHub]Named%20Enum>`_
 
 **[ ~ Dependencies scanned by** `PyUp.io <https://pyup.io>`_ **~ ]**
-
```

### Comparing `named_enum-1.3.0/setup.py` & `named_enum-1.3.1/setup.py`

 * *Files identical despite different names*

