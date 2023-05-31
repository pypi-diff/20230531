# Comparing `tmp/yml2cli-0.0.1.tar.gz` & `tmp/yml2cli-0.0.1.post20230531185952.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yml2cli-0.0.1.tar", last modified: Wed May 31 19:07:18 2023, max compression
+gzip compressed data, was "yml2cli-0.0.1.post20230531185952.tar", last modified: Wed May 31 19:01:29 2023, max compression
```

## Comparing `yml2cli-0.0.1.tar` & `yml2cli-0.0.1.post20230531185952.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:07:18.539346 yml2cli-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 19:06:51.000000 yml2cli-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-31 19:07:18.535346 yml2cli-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 19:06:51.000000 yml2cli-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:07:18.539346 yml2cli-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1785 2023-05-31 19:07:07.000000 yml2cli-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:07:18.535346 yml2cli-0.0.1/yml2cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:51.000000 yml2cli-0.0.1/yml2cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-31 19:06:51.000000 yml2cli-0.0.1/yml2cli/yml2cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:07:18.535346 yml2cli-0.0.1/yml2cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-31 19:07:18.000000 yml2cli-0.0.1/yml2cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-31 19:07:18.000000 yml2cli-0.0.1/yml2cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:07:18.000000 yml2cli-0.0.1/yml2cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 19:07:18.000000 yml2cli-0.0.1/yml2cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 19:07:18.000000 yml2cli-0.0.1/yml2cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 19:07:18.000000 yml2cli-0.0.1/yml2cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:01:29.236867 yml2cli-0.0.1.post20230531185952/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 19:01:07.000000 yml2cli-0.0.1.post20230531185952/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 19:01:29.232867 yml2cli-0.0.1.post20230531185952/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 19:01:07.000000 yml2cli-0.0.1.post20230531185952/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:01:29.236867 yml2cli-0.0.1.post20230531185952/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1800 2023-05-31 19:01:22.000000 yml2cli-0.0.1.post20230531185952/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:01:29.232867 yml2cli-0.0.1.post20230531185952/yml2cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:01:07.000000 yml2cli-0.0.1.post20230531185952/yml2cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-31 19:01:07.000000 yml2cli-0.0.1.post20230531185952/yml2cli/yml2cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:01:29.232867 yml2cli-0.0.1.post20230531185952/yml2cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 19:01:29.000000 yml2cli-0.0.1.post20230531185952/yml2cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-31 19:01:29.000000 yml2cli-0.0.1.post20230531185952/yml2cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:01:29.000000 yml2cli-0.0.1.post20230531185952/yml2cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 19:01:29.000000 yml2cli-0.0.1.post20230531185952/yml2cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 19:01:29.000000 yml2cli-0.0.1.post20230531185952/yml2cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 19:01:29.000000 yml2cli-0.0.1.post20230531185952/yml2cli.egg-info/top_level.txt
```

### Comparing `yml2cli-0.0.1/LICENSE` & `yml2cli-0.0.1.post20230531185952/LICENSE`

 * *Files identical despite different names*

### Comparing `yml2cli-0.0.1/setup.py` & `yml2cli-0.0.1.post20230531185952/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 REQUIREMENTS = [
     "pyyaml",
 ]
 
 
 setuptools.setup(
     name="yml2cli",
-    version="v0.0.1",
+    version="v0.0.1-20230531185952",
 
     author="Krishna Miriyala",
     author_email="krishnambm@gmail.com",
     url="https://github.com/krishnamiriyala/yml2cli",
     description="Yaml to cli params converter",
     long_description=open(README, "r").read(),
     packages=setuptools.find_packages(),
```

### Comparing `yml2cli-0.0.1/yml2cli/yml2cli.py` & `yml2cli-0.0.1.post20230531185952/yml2cli/yml2cli.py`

 * *Files identical despite different names*

