# Comparing `tmp/userfs-1.1.0.tar.gz` & `tmp/userfs-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userfs-1.1.0.tar", last modified: Mon May  8 06:30:34 2023, max compression
+gzip compressed data, was "userfs-1.1.1.tar", last modified: Wed May 31 05:50:26 2023, max compression
```

## Comparing `userfs-1.1.0.tar` & `userfs-1.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 06:29:23.000000 userfs-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-08 06:30:34.034633 userfs-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 06:29:23.000000 userfs-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-08 06:29:23.000000 userfs-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 06:30:34.034633 userfs-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-08 06:29:23.000000 userfs-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.030634 userfs-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 06:29:23.000000 userfs-1.1.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-08 06:29:23.000000 userfs-1.1.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.030634 userfs-1.1.0/userfs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.030634 userfs-1.1.0/userfs/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/commands/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/config/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/data/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/data/schemas/ProjectSpecification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/data/schemas/SourceSpecification.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/project/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.034633 userfs-1.1.0/userfs/update/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-08 06:29:23.000000 userfs-1.1.0/userfs/update/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:30:34.030634 userfs-1.1.0/userfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 06:30:34.000000 userfs-1.1.0/userfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 05:49:01.000000 userfs-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-31 05:50:26.263870 userfs-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-31 05:49:01.000000 userfs-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 05:49:01.000000 userfs-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 05:50:26.263870 userfs-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-31 05:49:01.000000 userfs-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.255869 userfs-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 05:49:01.000000 userfs-1.1.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 05:49:01.000000 userfs-1.1.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.255869 userfs-1.1.1/userfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.259869 userfs-1.1.1/userfs/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.259869 userfs-1.1.1/userfs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/config/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/data/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/data/schemas/ProjectSpecification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/data/schemas/SourceSpecification.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/update/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.259869 userfs-1.1.1/userfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/top_level.txt
```

### Comparing `userfs-1.1.0/LICENSE` & `userfs-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/PKG-INFO` & `userfs-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 1.1.0
+Version: 1.1.1
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=a1d4bf97f19efef60eb4f55ef88be7ee
+    hash=c140d059bd4f3630373f891ee3b3cc15
     =====================================
 -->
 
-# userfs ([1.1.0](https://pypi.org/project/userfs/))
+# userfs ([1.1.1](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
```

### Comparing `userfs-1.1.0/README.md` & `userfs-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=a1d4bf97f19efef60eb4f55ef88be7ee
+    hash=c140d059bd4f3630373f891ee3b3cc15
     =====================================
 -->
 
-# userfs ([1.1.0](https://pypi.org/project/userfs/))
+# userfs ([1.1.1](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
```

### Comparing `userfs-1.1.0/pyproject.toml` & `userfs-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "userfs"
-version = "1.1.0"
+version = "1.1.1"
 description = "A system-bootstrapping automation and introspection tool."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `userfs-1.1.0/setup.py` & `userfs-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/tests/test_entry.py` & `userfs-1.1.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/app.py` & `userfs-1.1.1/userfs/app.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/build/__init__.py` & `userfs-1.1.1/userfs/build/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/commands/all.py` & `userfs-1.1.1/userfs/commands/all.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/commands/build.py` & `userfs-1.1.1/userfs/commands/build.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/commands/common.py` & `userfs-1.1.1/userfs/commands/common.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/commands/custom.py` & `userfs-1.1.1/userfs/commands/custom.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/commands/fetch.py` & `userfs-1.1.1/userfs/commands/fetch.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/config/__init__.py` & `userfs-1.1.1/userfs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/config/project.py` & `userfs-1.1.1/userfs/config/project.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/config/source.py` & `userfs-1.1.1/userfs/config/source.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/data/schemas/Config.yaml` & `userfs-1.1.1/userfs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/data/schemas/ProjectSpecification.yaml` & `userfs-1.1.1/userfs/data/schemas/ProjectSpecification.yaml`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/entry.py` & `userfs-1.1.1/userfs/entry.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/fetch/__init__.py` & `userfs-1.1.1/userfs/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/hooks/__init__.py` & `userfs-1.1.1/userfs/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/paths.py` & `userfs-1.1.1/userfs/paths.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/project/__init__.py` & `userfs-1.1.1/userfs/project/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/schemas.py` & `userfs-1.1.1/userfs/schemas.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs/update/__init__.py` & `userfs-1.1.1/userfs/update/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.0/userfs.egg-info/PKG-INFO` & `userfs-1.1.1/userfs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 1.1.0
+Version: 1.1.1
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=a1d4bf97f19efef60eb4f55ef88be7ee
+    hash=c140d059bd4f3630373f891ee3b3cc15
     =====================================
 -->
 
-# userfs ([1.1.0](https://pypi.org/project/userfs/))
+# userfs ([1.1.1](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
```

### Comparing `userfs-1.1.0/userfs.egg-info/SOURCES.txt` & `userfs-1.1.1/userfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

