# Comparing `tmp/ShellUtilities-2.1.2.tar.gz` & `tmp/ShellUtilities-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellUtilities-2.1.2.tar", last modified: Sat May 27 01:41:30 2023, max compression
+gzip compressed data, was "ShellUtilities-2.1.3.tar", last modified: Wed May 31 15:07:30 2023, max compression
```

## Comparing `ShellUtilities-2.1.2.tar` & `ShellUtilities-2.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 01:41:30.161696 ShellUtilities-2.1.2/
--rw-r--r--   0 root         (0) root         (0)     2403 2023-05-27 01:41:30.161696 ShellUtilities-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1890 2023-05-26 15:09:33.000000 ShellUtilities-2.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 01:41:30.161696 ShellUtilities-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      965 2023-05-27 01:41:16.000000 ShellUtilities-2.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 01:41:30.158697 ShellUtilities-2.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 01:41:30.160696 ShellUtilities-2.1.2/src/ShellUtilities/
--rw-r--r--   0 root         (0) root         (0)     8512 2023-05-27 01:41:16.000000 ShellUtilities-2.1.2/src/ShellUtilities/Shell.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-04-05 16:00:52.000000 ShellUtilities-2.1.2/src/ShellUtilities/ShellCommandException.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-05 16:00:52.000000 ShellUtilities-2.1.2/src/ShellUtilities/ShellCommandResults.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:52.000000 ShellUtilities-2.1.2/src/ShellUtilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 01:41:30.160696 ShellUtilities-2.1.2/src/ShellUtilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2403 2023-05-27 01:41:30.000000 ShellUtilities-2.1.2/src/ShellUtilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-27 01:41:30.000000 ShellUtilities-2.1.2/src/ShellUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 01:41:30.000000 ShellUtilities-2.1.2/src/ShellUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-27 01:41:30.000000 ShellUtilities-2.1.2/src/ShellUtilities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:07:30.193438 ShellUtilities-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:07:30.192438 ShellUtilities-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-26 15:09:33.000000 ShellUtilities-2.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:07:30.193438 ShellUtilities-2.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-31 15:07:04.000000 ShellUtilities-2.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:07:30.187438 ShellUtilities-2.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:07:30.191438 ShellUtilities-2.1.3/src/ShellUtilities/
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-05-31 15:07:04.000000 ShellUtilities-2.1.3/src/ShellUtilities/Shell.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-04-05 16:00:52.000000 ShellUtilities-2.1.3/src/ShellUtilities/ShellCommandException.py
+-rw-r--r--   0 root         (0) root         (0)     5277 2023-05-31 15:07:04.000000 ShellUtilities-2.1.3/src/ShellUtilities/ShellCommandResults.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:52.000000 ShellUtilities-2.1.3/src/ShellUtilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:07:30.192438 ShellUtilities-2.1.3/src/ShellUtilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:07:30.000000 ShellUtilities-2.1.3/src/ShellUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-31 15:07:30.000000 ShellUtilities-2.1.3/src/ShellUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:07:30.000000 ShellUtilities-2.1.3/src/ShellUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 15:07:30.000000 ShellUtilities-2.1.3/src/ShellUtilities.egg-info/top_level.txt
```

### Comparing `ShellUtilities-2.1.2/PKG-INFO` & `ShellUtilities-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellUtilities
-Version: 2.1.2
+Version: 2.1.3
 Summary: A library for executing shell commands in either a blocking or non-blocking way.
 Home-page: https://github.com/taylor-schneider/ShellUtilities
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ShellUtilities-2.1.2/README.md` & `ShellUtilities-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ShellUtilities-2.1.2/setup.py` & `ShellUtilities-2.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open('README.md', "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="ShellUtilities",
-    version="2.1.2",
+    version="2.1.3",
     author="tschneider",
     author_email="tschneider@live.com",
     description="A library for executing shell commands in either a blocking or non-blocking way.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(source_code_dir),
     package_dir={
```

### Comparing `ShellUtilities-2.1.2/src/ShellUtilities.egg-info/PKG-INFO` & `ShellUtilities-2.1.3/src/ShellUtilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellUtilities
-Version: 2.1.2
+Version: 2.1.3
 Summary: A library for executing shell commands in either a blocking or non-blocking way.
 Home-page: https://github.com/taylor-schneider/ShellUtilities
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

