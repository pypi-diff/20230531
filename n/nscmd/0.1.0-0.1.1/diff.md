# Comparing `tmp/nscmd-0.1.0.tar.gz` & `tmp/nscmd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nscmd-0.1.0.tar", last modified: Wed May 31 01:19:59 2023, max compression
+gzip compressed data, was "nscmd-0.1.1.tar", last modified: Wed May 31 12:10:24 2023, max compression
```

## Comparing `nscmd-0.1.0.tar` & `nscmd-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 ropbear   (1337) ropbear   (1337)        0 2023-05-31 01:19:59.780893 nscmd-0.1.0/
--rw-r--r--   0 ropbear   (1337) ropbear   (1337)    35149 2023-05-26 03:12:09.000000 nscmd-0.1.0/LICENSE
--rw-r--r--   0 ropbear   (1337) ropbear   (1337)     2476 2023-05-31 01:19:59.780893 nscmd-0.1.0/PKG-INFO
--rw-r--r--   0 ropbear   (1337) ropbear   (1337)     1898 2023-05-31 01:12:20.000000 nscmd-0.1.0/README.md
--rwxr-xr-x   0 ropbear   (1337) ropbear   (1337)      151 2023-05-31 01:17:42.000000 nscmd-0.1.0/pyproject.toml
--rw-r--r--   0 ropbear   (1337) ropbear   (1337)       38 2023-05-31 01:19:59.780893 nscmd-0.1.0/setup.cfg
--rwxr-xr-x   0 ropbear   (1337) ropbear   (1337)      888 2023-05-31 01:19:30.000000 nscmd-0.1.0/setup.py
-drwxr-xr-x   0 ropbear   (1337) ropbear   (1337)        0 2023-05-31 01:19:59.780893 nscmd-0.1.0/src/
-drwxr-xr-x   0 ropbear   (1337) ropbear   (1337)        0 2023-05-31 01:19:59.780893 nscmd-0.1.0/src/nscmd.egg-info/
--rw-r--r--   0 ropbear   (1337) ropbear   (1337)     2476 2023-05-31 01:19:59.000000 nscmd-0.1.0/src/nscmd.egg-info/PKG-INFO
--rw-r--r--   0 ropbear   (1337) ropbear   (1337)      173 2023-05-31 01:19:59.000000 nscmd-0.1.0/src/nscmd.egg-info/SOURCES.txt
--rw-r--r--   0 ropbear   (1337) ropbear   (1337)        1 2023-05-31 01:19:59.000000 nscmd-0.1.0/src/nscmd.egg-info/dependency_links.txt
--rw-r--r--   0 ropbear   (1337) ropbear   (1337)        1 2023-05-31 01:19:59.000000 nscmd-0.1.0/src/nscmd.egg-info/top_level.txt
+drwxr-xr-x   0 ropbear   (1337) ropbear   (1337)        0 2023-05-31 12:10:24.806661 nscmd-0.1.1/
+-rw-r--r--   0 ropbear   (1337) ropbear   (1337)    35149 2023-05-26 03:12:09.000000 nscmd-0.1.1/LICENSE
+-rw-r--r--   0 ropbear   (1337) ropbear   (1337)     2476 2023-05-31 12:10:24.806661 nscmd-0.1.1/PKG-INFO
+-rw-r--r--   0 ropbear   (1337) ropbear   (1337)     1898 2023-05-31 01:12:20.000000 nscmd-0.1.1/README.md
+-rwxr-xr-x   0 ropbear   (1337) ropbear   (1337)      151 2023-05-31 01:17:42.000000 nscmd-0.1.1/pyproject.toml
+-rw-r--r--   0 ropbear   (1337) ropbear   (1337)       38 2023-05-31 12:10:24.806661 nscmd-0.1.1/setup.cfg
+-rwxr-xr-x   0 ropbear   (1337) ropbear   (1337)      888 2023-05-31 12:10:08.000000 nscmd-0.1.1/setup.py
+drwxr-xr-x   0 ropbear   (1337) ropbear   (1337)        0 2023-05-31 12:10:24.806661 nscmd-0.1.1/src/
+drwxr-xr-x   0 ropbear   (1337) ropbear   (1337)        0 2023-05-31 12:10:24.806661 nscmd-0.1.1/src/nscmd/
+-rw-r--r--   0 ropbear   (1337) ropbear   (1337)    24961 2023-05-31 01:11:07.000000 nscmd-0.1.1/src/nscmd/__init__.py
+drwxr-xr-x   0 ropbear   (1337) ropbear   (1337)        0 2023-05-31 12:10:24.806661 nscmd-0.1.1/src/nscmd.egg-info/
+-rw-r--r--   0 ropbear   (1337) ropbear   (1337)     2476 2023-05-31 12:10:24.000000 nscmd-0.1.1/src/nscmd.egg-info/PKG-INFO
+-rw-r--r--   0 ropbear   (1337) ropbear   (1337)      195 2023-05-31 12:10:24.000000 nscmd-0.1.1/src/nscmd.egg-info/SOURCES.txt
+-rw-r--r--   0 ropbear   (1337) ropbear   (1337)        1 2023-05-31 12:10:24.000000 nscmd-0.1.1/src/nscmd.egg-info/dependency_links.txt
+-rw-r--r--   0 ropbear   (1337) ropbear   (1337)        6 2023-05-31 12:10:24.000000 nscmd-0.1.1/src/nscmd.egg-info/top_level.txt
```

### Comparing `nscmd-0.1.0/LICENSE` & `nscmd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nscmd-0.1.0/PKG-INFO` & `nscmd-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nscmd
-Version: 0.1.0
+Version: 0.1.1
 Summary: A terminal user interface (TUI) for GNU/Linux systems which implements namespaces.
 Home-page: https://github.com/ropbear/nscmd
 Author: ropbear
 Author-email: pypi@selfhosted.systems
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/ropbear/nscmd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nscmd-0.1.0/README.md` & `nscmd-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nscmd-0.1.0/setup.py` & `nscmd-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="nscmd",
-    version="0.1.0",
+    version="0.1.1",
     description="A terminal user interface (TUI) for GNU/Linux systems which implements namespaces.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ropbear/nscmd",
     author="ropbear",
     author_email="pypi@selfhosted.systems",
     license="GPLv3",
```

### Comparing `nscmd-0.1.0/src/nscmd.egg-info/PKG-INFO` & `nscmd-0.1.1/src/nscmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nscmd
-Version: 0.1.0
+Version: 0.1.1
 Summary: A terminal user interface (TUI) for GNU/Linux systems which implements namespaces.
 Home-page: https://github.com/ropbear/nscmd
 Author: ropbear
 Author-email: pypi@selfhosted.systems
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/ropbear/nscmd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

