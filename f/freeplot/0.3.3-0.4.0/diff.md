# Comparing `tmp/freeplot-0.3.3.tar.gz` & `tmp/freeplot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplot-0.3.3.tar", last modified: Thu May 25 05:28:26 2023, max compression
+gzip compressed data, was "freeplot-0.4.0.tar", last modified: Wed May 31 09:24:05 2023, max compression
```

## Comparing `freeplot-0.3.3.tar` & `freeplot-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 05:28:26.037920 freeplot-0.3.3/
--rw-rw-rw-   0        0        0     1085 2022-09-19 12:06:04.000000 freeplot-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     7420 2023-05-25 05:28:26.036897 freeplot-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     6937 2023-01-01 10:56:12.000000 freeplot-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 05:28:25.972587 freeplot-0.3.3/freeplot/
--rw-rw-rw-   0        0        0       51 2023-05-25 05:27:37.000000 freeplot-0.3.3/freeplot/__init__.py
--rw-rw-rw-   0        0        0    17958 2023-02-17 05:04:04.000000 freeplot-0.3.3/freeplot/base.py
--rw-rw-rw-   0        0        0     3682 2023-04-20 05:14:16.000000 freeplot-0.3.3/freeplot/config.py
--rw-rw-rw-   0        0        0    25144 2023-04-17 13:09:51.000000 freeplot-0.3.3/freeplot/unit.py
--rw-rw-rw-   0        0        0     2303 2023-02-17 05:04:16.000000 freeplot-0.3.3/freeplot/utils.py
--rw-rw-rw-   0        0        0     6226 2022-09-19 12:06:04.000000 freeplot-0.3.3/freeplot/zoo.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:28:26.035886 freeplot-0.3.3/freeplot.egg-info/
--rw-rw-rw-   0        0        0     7420 2023-05-25 05:28:25.000000 freeplot-0.3.3/freeplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-25 05:28:25.000000 freeplot-0.3.3/freeplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 05:28:25.000000 freeplot-0.3.3/freeplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-05-25 05:28:25.000000 freeplot-0.3.3/freeplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 05:28:25.000000 freeplot-0.3.3/freeplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 05:28:26.038937 freeplot-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-05-25 05:27:04.000000 freeplot-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:24:05.662125 freeplot-0.4.0/
+-rw-rw-rw-   0        0        0     1085 2022-09-19 12:06:04.000000 freeplot-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     7420 2023-05-31 09:24:05.661126 freeplot-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6937 2023-01-01 10:56:12.000000 freeplot-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 09:24:05.645080 freeplot-0.4.0/freeplot/
+-rw-rw-rw-   0        0        0       51 2023-05-31 09:24:01.000000 freeplot-0.4.0/freeplot/__init__.py
+-rw-rw-rw-   0        0        0    17958 2023-02-17 05:04:04.000000 freeplot-0.4.0/freeplot/base.py
+-rw-rw-rw-   0        0        0     3682 2023-04-20 05:14:16.000000 freeplot-0.4.0/freeplot/config.py
+-rw-rw-rw-   0        0        0    25144 2023-04-17 13:09:51.000000 freeplot-0.4.0/freeplot/unit.py
+-rw-rw-rw-   0        0        0     2303 2023-02-17 05:04:16.000000 freeplot-0.4.0/freeplot/utils.py
+-rw-rw-rw-   0        0        0     6226 2022-09-19 12:06:04.000000 freeplot-0.4.0/freeplot/zoo.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:24:05.661126 freeplot-0.4.0/freeplot.egg-info/
+-rw-rw-rw-   0        0        0     7420 2023-05-31 09:24:05.000000 freeplot-0.4.0/freeplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-31 09:24:05.000000 freeplot-0.4.0/freeplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 09:24:05.000000 freeplot-0.4.0/freeplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-05-31 09:24:05.000000 freeplot-0.4.0/freeplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 09:24:05.000000 freeplot-0.4.0/freeplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 09:24:05.662125 freeplot-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-05-25 05:27:04.000000 freeplot-0.4.0/setup.py
```

### Comparing `freeplot-0.3.3/LICENSE` & `freeplot-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.3/PKG-INFO` & `freeplot-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplot
-Version: 0.3.3
+Version: 0.4.0
 Summary: a Python data visualization library based on matplotlib
 Home-page: https://github.com/MTandHJ/freeplot
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freeplot-0.3.3/README.md` & `freeplot-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.3/freeplot/base.py` & `freeplot-0.4.0/freeplot/base.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.3/freeplot/config.py` & `freeplot-0.4.0/freeplot/config.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.3/freeplot/unit.py` & `freeplot-0.4.0/freeplot/unit.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.3/freeplot/utils.py` & `freeplot-0.4.0/freeplot/utils.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.3/freeplot/zoo.py` & `freeplot-0.4.0/freeplot/zoo.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.3/freeplot.egg-info/PKG-INFO` & `freeplot-0.4.0/freeplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplot
-Version: 0.3.3
+Version: 0.4.0
 Summary: a Python data visualization library based on matplotlib
 Home-page: https://github.com/MTandHJ/freeplot
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freeplot-0.3.3/setup.py` & `freeplot-0.4.0/setup.py`

 * *Files identical despite different names*

