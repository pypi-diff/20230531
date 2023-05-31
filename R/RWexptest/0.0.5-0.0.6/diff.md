# Comparing `tmp/RWexptest-0.0.5.tar.gz` & `tmp/RWexptest-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RWexptest-0.0.5.tar", last modified: Fri Apr 28 11:06:48 2023, max compression
+gzip compressed data, was "RWexptest-0.0.6.tar", last modified: Wed May 31 03:21:43 2023, max compression
```

## Comparing `RWexptest-0.0.5.tar` & `RWexptest-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 11:06:48.755585 RWexptest-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 RWexptest-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      687 2023-04-28 11:06:48.755585 RWexptest-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-25 08:29:52.000000 RWexptest-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 11:06:48.741439 RWexptest-0.0.5/RWexptest/
--rw-rw-rw-   0        0        0        0 2023-04-24 09:02:16.000000 RWexptest-0.0.5/RWexptest/_init_.py
--rw-rw-rw-   0        0        0      466 2023-04-28 08:54:19.000000 RWexptest-0.0.5/RWexptest/example.py
--rw-rw-rw-   0        0        0     2126 2023-04-25 09:28:17.000000 RWexptest-0.0.5/RWexptest/toml.py
-drwxrwxrwx   0        0        0        0 2023-04-28 11:06:48.755585 RWexptest-0.0.5/RWexptest.egg-info/
--rw-rw-rw-   0        0        0      687 2023-04-28 11:06:48.000000 RWexptest-0.0.5/RWexptest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-28 11:06:48.000000 RWexptest-0.0.5/RWexptest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 11:06:48.000000 RWexptest-0.0.5/RWexptest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-28 11:06:48.000000 RWexptest-0.0.5/RWexptest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-28 11:06:48.000000 RWexptest-0.0.5/RWexptest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      637 2023-04-28 11:06:06.000000 RWexptest-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 11:06:48.755585 RWexptest-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 03:21:43.964779 RWexptest-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 RWexptest-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      687 2023-05-31 03:21:43.964779 RWexptest-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-25 08:29:52.000000 RWexptest-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 03:21:43.926265 RWexptest-0.0.6/RWexptest/
+-rw-rw-rw-   0        0        0        0 2023-04-24 09:02:16.000000 RWexptest-0.0.6/RWexptest/_init_.py
+-rw-rw-rw-   0        0        0      466 2023-04-28 08:54:19.000000 RWexptest-0.0.6/RWexptest/example.py
+-rw-rw-rw-   0        0        0     3512 2023-05-31 03:03:44.000000 RWexptest-0.0.6/RWexptest/mnist.py
+-rw-rw-rw-   0        0        0     2126 2023-04-25 09:28:17.000000 RWexptest-0.0.6/RWexptest/toml.py
+drwxrwxrwx   0        0        0        0 2023-05-31 03:21:43.963271 RWexptest-0.0.6/RWexptest.egg-info/
+-rw-rw-rw-   0        0        0      687 2023-05-31 03:21:43.000000 RWexptest-0.0.6/RWexptest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-05-31 03:21:43.000000 RWexptest-0.0.6/RWexptest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 03:21:43.000000 RWexptest-0.0.6/RWexptest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-31 03:21:43.000000 RWexptest-0.0.6/RWexptest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-31 03:21:43.000000 RWexptest-0.0.6/RWexptest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      637 2023-05-31 03:20:21.000000 RWexptest-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 03:21:43.964779 RWexptest-0.0.6/setup.cfg
```

### Comparing `RWexptest-0.0.5/LICENSE.txt` & `RWexptest-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RWexptest-0.0.5/PKG-INFO` & `RWexptest-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RWexptest
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: RuiwangW <2219312248@qq.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RWexptest-0.0.5/RWexptest/toml.py` & `RWexptest-0.0.6/RWexptest/toml.py`

 * *Files identical despite different names*

### Comparing `RWexptest-0.0.5/RWexptest.egg-info/PKG-INFO` & `RWexptest-0.0.6/RWexptest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RWexptest
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: RuiwangW <2219312248@qq.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RWexptest-0.0.5/pyproject.toml` & `RWexptest-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RWexptest"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="RuiwangW", email="2219312248@qq.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

