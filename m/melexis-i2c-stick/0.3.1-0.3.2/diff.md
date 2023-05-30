# Comparing `tmp/melexis-i2c-stick-0.3.1.tar.gz` & `tmp/melexis-i2c-stick-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melexis-i2c-stick-0.3.1.tar", last modified: Tue May 30 21:52:44 2023, max compression
+gzip compressed data, was "melexis-i2c-stick-0.3.2.tar", last modified: Tue May 30 22:39:11 2023, max compression
```

## Comparing `melexis-i2c-stick-0.3.1.tar` & `melexis-i2c-stick-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/melexis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/melexis/i2c_stick/
--rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/melexis/i2c_stick/I2CStick.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/melexis/i2c_stick/MemoryFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/melexis/i2c_stick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/melexis/i2c_stick/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:39:11.175042 melexis-i2c-stick-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-30 22:39:11.171042 melexis-i2c-stick-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:39:11.171042 melexis-i2c-stick-0.3.2/melexis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:39:11.171042 melexis-i2c-stick-0.3.2/melexis/i2c_stick/
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/melexis/i2c_stick/I2CStick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/melexis/i2c_stick/MemoryFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/melexis/i2c_stick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/melexis/i2c_stick/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:39:11.171042 melexis-i2c-stick-0.3.2/melexis_i2c_stick.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-30 22:39:11.000000 melexis-i2c-stick-0.3.2/melexis_i2c_stick.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 22:39:11.000000 melexis-i2c-stick-0.3.2/melexis_i2c_stick.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:39:11.000000 melexis-i2c-stick-0.3.2/melexis_i2c_stick.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 22:39:11.000000 melexis-i2c-stick-0.3.2/melexis_i2c_stick.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:39:11.000000 melexis-i2c-stick-0.3.2/melexis_i2c_stick.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 22:39:11.000000 melexis-i2c-stick-0.3.2/melexis_i2c_stick.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-30 22:38:49.000000 melexis-i2c-stick-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:39:11.175042 melexis-i2c-stick-0.3.2/setup.cfg
```

### Comparing `melexis-i2c-stick-0.3.1/CONTRIBUTING.md` & `melexis-i2c-stick-0.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.3.1/LICENSE` & `melexis-i2c-stick-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.3.1/PKG-INFO` & `melexis-i2c-stick-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.3.1
+Version: 0.3.2
 Summary: Melexis I2C Stick, python interface
 Author-email: Karel Vanroye <kva@melexis.com>
 License:    Copyright 2023 Melexis
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
```

### Comparing `melexis-i2c-stick-0.3.1/melexis/i2c_stick/I2CStick.py` & `melexis-i2c-stick-0.3.2/melexis/i2c_stick/I2CStick.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,14 +407,15 @@
             return None
         if a[2] == "FAIL":
             return "FAIL:" + a[3]
         result = {}
         result = {}
         result['time_ms'] = int(a[2])
         result['values'] = [int(x, 16) for x in a[3].split(',')]
+        result['values'] = [x if x < 2**15 else x - 2**16 for x in result['values']]
         return result
 
 
     def pwm(self, pin, pwm):
         a = self.run_cmd("pwm:{}:{}".format(pin, pwm))
         return a
```

### Comparing `melexis-i2c-stick-0.3.1/melexis/i2c_stick/MemoryFile.py` & `melexis-i2c-stick-0.3.2/melexis/i2c_stick/MemoryFile.py`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/PKG-INFO` & `melexis-i2c-stick-0.3.2/melexis_i2c_stick.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.3.1
+Version: 0.3.2
 Summary: Melexis I2C Stick, python interface
 Author-email: Karel Vanroye <kva@melexis.com>
 License:    Copyright 2023 Melexis
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
```

### Comparing `melexis-i2c-stick-0.3.1/pyproject.toml` & `melexis-i2c-stick-0.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=63.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "melexis-i2c-stick"
-version = "0.3.1"
+version = "0.3.2"
 description = "Melexis I2C Stick, python interface"
 readme = "README.md"
 authors = [{ name = "Karel Vanroye", email = "kva@melexis.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -32,15 +32,15 @@
 Homepage = "https://github.com/melexis/i2c-stick"
 
 [project.scripts]
 melexis_i2c_stick = "melexis.i2c_stick.__main__:main"
 
 
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "0.3.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

