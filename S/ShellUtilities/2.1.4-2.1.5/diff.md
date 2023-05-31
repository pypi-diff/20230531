# Comparing `tmp/ShellUtilities-2.1.4.tar.gz` & `tmp/ShellUtilities-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellUtilities-2.1.4.tar", last modified: Wed May 31 15:27:17 2023, max compression
+gzip compressed data, was "ShellUtilities-2.1.5.tar", last modified: Wed May 31 15:34:43 2023, max compression
```

## Comparing `ShellUtilities-2.1.4.tar` & `ShellUtilities-2.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:27:17.895152 ShellUtilities-2.1.4/
--rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:27:17.895152 ShellUtilities-2.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1890 2023-05-26 15:09:33.000000 ShellUtilities-2.1.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:27:17.895152 ShellUtilities-2.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      965 2023-05-31 15:27:00.000000 ShellUtilities-2.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:27:17.893152 ShellUtilities-2.1.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:27:17.894152 ShellUtilities-2.1.4/src/ShellUtilities/
--rw-r--r--   0 root         (0) root         (0)     3727 2023-05-31 15:07:04.000000 ShellUtilities-2.1.4/src/ShellUtilities/Shell.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-04-05 16:00:52.000000 ShellUtilities-2.1.4/src/ShellUtilities/ShellCommandException.py
--rw-r--r--   0 root         (0) root         (0)     5280 2023-05-31 15:27:00.000000 ShellUtilities-2.1.4/src/ShellUtilities/ShellCommandResults.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:52.000000 ShellUtilities-2.1.4/src/ShellUtilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:27:17.894152 ShellUtilities-2.1.4/src/ShellUtilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:27:17.000000 ShellUtilities-2.1.4/src/ShellUtilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-31 15:27:17.000000 ShellUtilities-2.1.4/src/ShellUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:27:17.000000 ShellUtilities-2.1.4/src/ShellUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 15:27:17.000000 ShellUtilities-2.1.4/src/ShellUtilities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:34:43.900412 ShellUtilities-2.1.5/
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:34:43.900412 ShellUtilities-2.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-26 15:09:33.000000 ShellUtilities-2.1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:34:43.900412 ShellUtilities-2.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-31 15:34:30.000000 ShellUtilities-2.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:34:43.894412 ShellUtilities-2.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:34:43.895412 ShellUtilities-2.1.5/src/ShellUtilities/
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-05-31 15:07:04.000000 ShellUtilities-2.1.5/src/ShellUtilities/Shell.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-04-05 16:00:52.000000 ShellUtilities-2.1.5/src/ShellUtilities/ShellCommandException.py
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-05-31 15:34:30.000000 ShellUtilities-2.1.5/src/ShellUtilities/ShellCommandResults.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:00:52.000000 ShellUtilities-2.1.5/src/ShellUtilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:34:43.899412 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-05-31 15:34:43.000000 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-31 15:34:43.000000 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:34:43.000000 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 15:34:43.000000 ShellUtilities-2.1.5/src/ShellUtilities.egg-info/top_level.txt
```

### Comparing `ShellUtilities-2.1.4/PKG-INFO` & `ShellUtilities-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellUtilities
-Version: 2.1.4
+Version: 2.1.5
 Summary: A library for executing shell commands in either a blocking or non-blocking way.
 Home-page: https://github.com/taylor-schneider/ShellUtilities
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ShellUtilities-2.1.4/README.md` & `ShellUtilities-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ShellUtilities-2.1.4/setup.py` & `ShellUtilities-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open('README.md', "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="ShellUtilities",
-    version="2.1.4",
+    version="2.1.5",
     author="tschneider",
     author_email="tschneider@live.com",
     description="A library for executing shell commands in either a blocking or non-blocking way.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(source_code_dir),
     package_dir={
```

### Comparing `ShellUtilities-2.1.4/src/ShellUtilities/Shell.py` & `ShellUtilities-2.1.5/src/ShellUtilities/Shell.py`

 * *Files identical despite different names*

### Comparing `ShellUtilities-2.1.4/src/ShellUtilities/ShellCommandResults.py` & `ShellUtilities-2.1.5/src/ShellUtilities/ShellCommandResults.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             process_running = True
             while process_running:
                 for line in iter(buffer.readline, b''):
                     if line != b'':
                         line = line.decode()
                         line = line.rstrip("\n")
                         buffer_handler_func(line)
-                process_running = process.poll() != None
+                process_running = process.poll() == None
 
         self.stdout_thread = threading.Thread(target=handle_output_line, args=(process.stdout, self._handle_stdout_line))
         self.stderr_thread = threading.Thread(target=handle_output_line, args=(process.stderr, self._handle_stderr_line))
         self.stdout_thread.start()
         self.stderr_thread.start()
 
     def command_running(self):
```

### Comparing `ShellUtilities-2.1.4/src/ShellUtilities.egg-info/PKG-INFO` & `ShellUtilities-2.1.5/src/ShellUtilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellUtilities
-Version: 2.1.4
+Version: 2.1.5
 Summary: A library for executing shell commands in either a blocking or non-blocking way.
 Home-page: https://github.com/taylor-schneider/ShellUtilities
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

