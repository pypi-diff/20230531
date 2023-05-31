# Comparing `tmp/vnpy_xex-2023.5.30.1.tar.gz` & `tmp/vnpy_xex-2023.5.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_xex-2023.5.30.1.tar", last modified: Tue May 30 10:26:27 2023, max compression
+gzip compressed data, was "vnpy_xex-2023.5.31.1.tar", last modified: Wed May 31 01:36:22 2023, max compression
```

## Comparing `vnpy_xex-2023.5.30.1.tar` & `vnpy_xex-2023.5.31.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-05-30 10:26:27.851005 vnpy_xex-2023.5.30.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.5.30.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      986 2023-05-30 10:26:27.851134 vnpy_xex-2023.5.30.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.5.30.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      972 2023-05-30 10:26:27.851803 vnpy_xex-2023.5.30.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.5.30.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-05-30 10:26:27.847579 vnpy_xex-2023.5.30.1/vnpy_xex/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.5.30.1/vnpy_xex/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    23922 2023-05-30 10:05:30.000000 vnpy_xex-2023.5.30.1/vnpy_xex/xex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-05-30 10:26:27.850752 vnpy_xex-2023.5.30.1/vnpy_xex.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      986 2023-05-30 10:26:27.000000 vnpy_xex-2023.5.30.1/vnpy_xex.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-05-30 10:26:27.000000 vnpy_xex-2023.5.30.1/vnpy_xex.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:26:27.000000 vnpy_xex-2023.5.30.1/vnpy_xex.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.5.30.1/vnpy_xex.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-05-30 10:26:27.000000 vnpy_xex-2023.5.30.1/vnpy_xex.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-05-30 10:26:27.000000 vnpy_xex-2023.5.30.1/vnpy_xex.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-05-31 01:36:22.562964 vnpy_xex-2023.5.31.1/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.5.31.1/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1008 2023-05-31 01:36:22.563068 vnpy_xex-2023.5.31.1/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.5.31.1/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      994 2023-05-31 01:36:22.563659 vnpy_xex-2023.5.31.1/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.5.31.1/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-05-31 01:36:22.559061 vnpy_xex-2023.5.31.1/vnpy_xex/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.5.31.1/vnpy_xex/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    23922 2023-05-30 10:05:30.000000 vnpy_xex-2023.5.31.1/vnpy_xex/xex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-05-31 01:36:22.562760 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1008 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/top_level.txt
```

### Comparing `vnpy_xex-2023.5.30.1/LICENSE` & `vnpy_xex-2023.5.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.5.30.1/PKG-INFO` & `vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: vnpy_xex
-Version: 2023.5.30.1
+Name: vnpy-xex
+Version: 2023.5.31.1
 Summary: gateway of xex exchange for vnpy
-Home-page: https://www.vnpy.com
+Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vnpy_xex-2023.5.30.1/setup.cfg` & `vnpy_xex-2023.5.31.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = vnpy_xex
-version = 2023.5.30.1
-url = https://www.vnpy.com
+version = 2023.5.31.1
+url = https://github.com/monk-after-90s/vnpy_xex
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = gateway of xex exchange for vnpy
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords =
```

### Comparing `vnpy_xex-2023.5.30.1/vnpy_xex/__init__.py` & `vnpy_xex-2023.5.31.1/vnpy_xex/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.5.30.1/vnpy_xex/xex_gateway.py` & `vnpy_xex-2023.5.31.1/vnpy_xex/xex_gateway.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.5.30.1/vnpy_xex.egg-info/PKG-INFO` & `vnpy_xex-2023.5.31.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: vnpy-xex
-Version: 2023.5.30.1
+Name: vnpy_xex
+Version: 2023.5.31.1
 Summary: gateway of xex exchange for vnpy
-Home-page: https://www.vnpy.com
+Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

