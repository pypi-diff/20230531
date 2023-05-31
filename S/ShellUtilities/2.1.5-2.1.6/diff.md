# Comparing `tmp/ShellUtilities-2.1.5.tar.gz` & `tmp/ShellUtilities-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellUtilities-2.1.5.tar", last modified: Wed May 31 15:34:43 2023, max compression
+gzip compressed data, was "ShellUtilities-2.1.6.tar", last modified: Wed May 31 15:54:43 2023, max compression
```

## Comparing `ShellUtilities-2.1.5.tar` & `ShellUtilities-2.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:34:43.900412 ShellUtilities-2.1.5/
--rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:34:43.900412 ShellUtilities-2.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1890 2023-05-26 15:09:33.000000 ShellUtilities-2.1.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:34:43.900412 ShellUtilities-2.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      965 2023-05-31 15:34:30.000000 ShellUtilities-2.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:34:43.894412 ShellUtilities-2.1.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:34:43.895412 ShellUtilities-2.1.5/src/ShellUtilities/
--rw-r--r--   0 root         (0) root         (0)     3727 2023-05-31 15:07:04.000000 ShellUtilities-2.1.5/src/ShellUtilities/Shell.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-04-05 16:00:52.000000 ShellUtilities-2.1.5/src/ShellUtilities/ShellCommandException.py
--rw-r--r--   0 root         (0) root         (0)     5280 2023-05-31 15:34:30.000000 ShellUtilities-2.1.5/src/ShellUtilities/ShellCommandResults.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:52.000000 ShellUtilities-2.1.5/src/ShellUtilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:34:43.899412 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:34:43.000000 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-31 15:34:43.000000 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:34:43.000000 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 15:34:43.000000 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:54:43.209909 ShellUtilities-2.1.6/
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:54:43.209909 ShellUtilities-2.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-26 15:09:33.000000 ShellUtilities-2.1.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:54:43.209909 ShellUtilities-2.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-31 15:54:31.000000 ShellUtilities-2.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:54:43.205909 ShellUtilities-2.1.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:54:43.208909 ShellUtilities-2.1.6/src/ShellUtilities/
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-05-31 15:07:04.000000 ShellUtilities-2.1.6/src/ShellUtilities/Shell.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-05-31 15:54:31.000000 ShellUtilities-2.1.6/src/ShellUtilities/ShellCommandException.py
+-rw-r--r--   0 root         (0) root         (0)     5499 2023-05-31 15:54:31.000000 ShellUtilities-2.1.6/src/ShellUtilities/ShellCommandResults.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:52.000000 ShellUtilities-2.1.6/src/ShellUtilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:54:43.208909 ShellUtilities-2.1.6/src/ShellUtilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:54:43.000000 ShellUtilities-2.1.6/src/ShellUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-31 15:54:43.000000 ShellUtilities-2.1.6/src/ShellUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:54:43.000000 ShellUtilities-2.1.6/src/ShellUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 15:54:43.000000 ShellUtilities-2.1.6/src/ShellUtilities.egg-info/top_level.txt
```

### Comparing `ShellUtilities-2.1.5/PKG-INFO` & `ShellUtilities-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellUtilities
-Version: 2.1.5
+Version: 2.1.6
 Summary: A library for executing shell commands in either a blocking or non-blocking way.
 Home-page: https://github.com/taylor-schneider/ShellUtilities
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ShellUtilities-2.1.5/README.md` & `ShellUtilities-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ShellUtilities-2.1.5/setup.py` & `ShellUtilities-2.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open('README.md', "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="ShellUtilities",
-    version="2.1.5",
+    version="2.1.6",
     author="tschneider",
     author_email="tschneider@live.com",
     description="A library for executing shell commands in either a blocking or non-blocking way.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(source_code_dir),
     package_dir={
```

### Comparing `ShellUtilities-2.1.5/src/ShellUtilities/Shell.py` & `ShellUtilities-2.1.6/src/ShellUtilities/Shell.py`

 * *Files identical despite different names*

### Comparing `ShellUtilities-2.1.5/src/ShellUtilities/ShellCommandResults.py` & `ShellUtilities-2.1.6/src/ShellUtilities/ShellCommandResults.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import threading
 import os
 import time
-
+from ShellUtilities.ShellCommandException import AsynchronousShellCommandException
 
 class ShellCommandResults():
 
     def __init__(self, command, stdout, stderr, exitcode):
         self.Command = command
         self.Stdout = stdout
         self.Stderr = stderr
         self.ExitCode = exitcode
 
-
 class AsynchronousShellCommandResults(ShellCommandResults):
 
     def __init__(self, command, process):
         # Create vars for handling process output
         self.process = process
         self.stdout_lines = []
         self.stderr_lines = []
@@ -107,15 +106,15 @@
 
     def command_running(self):
         poll = self.process.poll()
         if not poll:
             return False
         return self.stdout_thread.is_alive() or self.stderr_thread.is_alive()
 
-    def wait(self):
+    def wait(self, raise_on_error=True):
 
         # This is a blocking function which will safely wait for the shell process and handling threads to complete
 
         # Wait for the process to exit
         self.process.wait()
 
         # Wait for the enqueing threads to complete
@@ -124,7 +123,10 @@
 
         # Make sure we have cleaned up and dont see any warnings like:
         # ResourceWarning: unclosed file <_io.BufferedReader name=4>
         self.process.stdout.close()
         self.process.stderr.close()
 
         self.ExitCode = self.process.returncode
+        
+        if raise_on_error and self.ExitCode != 0:
+            raise AsynchronousShellCommandException(self)
```

### Comparing `ShellUtilities-2.1.5/src/ShellUtilities.egg-info/PKG-INFO` & `ShellUtilities-2.1.6/src/ShellUtilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellUtilities
-Version: 2.1.5
+Version: 2.1.6
 Summary: A library for executing shell commands in either a blocking or non-blocking way.
 Home-page: https://github.com/taylor-schneider/ShellUtilities
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

