# Comparing `tmp/access_nri_intake-0.0.5.tar.gz` & `tmp/access_nri_intake-0.0.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_nri_intake-0.0.5.tar", last modified: Tue May 30 06:16:49 2023, max compression
+gzip compressed data, was "access_nri_intake-0.0.5.post1.tar", last modified: Wed May 31 03:31:26 2023, max compression
```

## Comparing `access_nri_intake-0.0.5.tar` & `access_nri_intake-0.0.5.post1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.972885 access_nri_intake-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/src/access_nri_intake/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/src/access_nri_intake/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.972885 access_nri_intake-0.0.5/src/access_nri_intake/cat/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/cat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/src/access_nri_intake/esmcat/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/esmcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/esmcat/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/esmcat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/src/access_nri_intake/metacat/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/metacat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/metacat/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/metacat/translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.972885 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/cat/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/cat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/cat/catalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/versioneer.py
```

### Comparing `access_nri_intake-0.0.5/LICENSE` & `access_nri_intake-0.0.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5/PKG-INFO` & `access_nri_intake-0.0.5.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_nri_intake
-Version: 0.0.5
+Version: 0.0.5.post1
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.0.5/README.rst` & `access_nri_intake-0.0.5.post1/README.rst`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5/pyproject.toml` & `access_nri_intake-0.0.5.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   "versioneer[toml]",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-access_nri_intake = ["cat/metacatalog.yaml"]
+access_nri_intake = ["cat/catalog.yaml"]
 
 [tool.versioneer]
 VCS = "git"
 style = "pep440"
 versionfile_source = "src/access_nri_intake/_version.py"
 versionfile_build = "access_nri_intake/_version.py"
 tag_prefix = "v"
```

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake/cli.py` & `access_nri_intake-0.0.5.post1/src/access_nri_intake/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,25 +144,25 @@
 
     if not version.startswith("v"):
         version = f"v{version}"
 
     # Create the build directories
     build_base_path = os.path.abspath(build_base_path)
     build_path = os.path.join(build_base_path, version, "source")
-    metacatalog_file = os.path.join(build_base_path, version, metacatalog_file)
+    metacatalog_path = os.path.join(build_base_path, version, metacatalog_file)
     os.makedirs(build_path, exist_ok=True)
 
     # Parse inputs to pass to MetacatManager
     parsed_sources = _parse_inputs(config_yamls, build_path)
     _check_args([parsed_source[1] for parsed_source in parsed_sources])
 
     # Build the catalog
     for (method, args) in parsed_sources:
-        man = manager.MetacatManager(path=metacatalog_file)
-        logger.info(f"Adding '{args['name']}' to metacatalog '{metacatalog_file}'")
+        man = manager.MetacatManager(path=metacatalog_path)
+        logger.info(f"Adding '{args['name']}' to metacatalog '{metacatalog_path}'")
         getattr(man, method)(**args).add()
 
     # Write catalog yaml file
     storage = set()
     for (_, args) in parsed_sources:
         storage |= {
             f"gdata/{os.path.normpath(path).split(os.sep)[3]}" for path in args["path"]
```

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake/esmcat/__init__.py` & `access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake/esmcat/builders.py` & `access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/builders.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake/esmcat/utils.py` & `access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake/metacat/__init__.py` & `access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake/metacat/manager.py` & `access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/manager.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake/metacat/translators.py` & `access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/translators.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake/utils.py` & `access_nri_intake-0.0.5.post1/src/access_nri_intake/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake.egg-info/PKG-INFO` & `access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-nri-intake
-Version: 0.0.5
+Version: 0.0.5.post1
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.0.5/src/access_nri_intake.egg-info/SOURCES.txt` & `access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 src/access_nri_intake.egg-info/PKG-INFO
 src/access_nri_intake.egg-info/SOURCES.txt
 src/access_nri_intake.egg-info/dependency_links.txt
 src/access_nri_intake.egg-info/entry_points.txt
 src/access_nri_intake.egg-info/requires.txt
 src/access_nri_intake.egg-info/top_level.txt
 src/access_nri_intake/cat/__init__.py
+src/access_nri_intake/cat/catalog.yaml
 src/access_nri_intake/esmcat/__init__.py
 src/access_nri_intake/esmcat/builders.py
 src/access_nri_intake/esmcat/utils.py
 src/access_nri_intake/metacat/__init__.py
 src/access_nri_intake/metacat/manager.py
 src/access_nri_intake/metacat/translators.py
```

### Comparing `access_nri_intake-0.0.5/versioneer.py` & `access_nri_intake-0.0.5.post1/versioneer.py`

 * *Files identical despite different names*

