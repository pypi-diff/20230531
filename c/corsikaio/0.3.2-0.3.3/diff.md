# Comparing `tmp/corsikaio-0.3.2.tar.gz` & `tmp/corsikaio-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corsikaio-0.3.2.tar", last modified: Wed Mar 29 13:51:18 2023, max compression
+gzip compressed data, was "corsikaio-0.3.3.tar", last modified: Wed May 31 16:10:10 2023, max compression
```

## Comparing `corsikaio-0.3.2.tar` & `corsikaio-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:51:18.557168 corsikaio-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-29 13:51:04.000000 corsikaio-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-29 13:51:04.000000 corsikaio-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-29 13:51:04.000000 corsikaio-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-29 13:51:18.557168 corsikaio-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-29 13:51:04.000000 corsikaio-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:51:18.553168 corsikaio-0.3.2/corsikaio/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-29 13:51:17.000000 corsikaio-0.3.2/corsikaio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:51:18.557168 corsikaio-0.3.2/corsikaio/subblocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/subblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/subblocks/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/subblocks/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/subblocks/event_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/subblocks/event_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/subblocks/longitudinal.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/subblocks/run_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/subblocks/run_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-29 13:51:04.000000 corsikaio-0.3.2/corsikaio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:51:18.553168 corsikaio-0.3.2/corsikaio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-29 13:51:17.000000 corsikaio-0.3.2/corsikaio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-29 13:51:18.000000 corsikaio-0.3.2/corsikaio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:51:17.000000 corsikaio-0.3.2/corsikaio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:51:16.000000 corsikaio-0.3.2/corsikaio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-29 13:51:17.000000 corsikaio-0.3.2/corsikaio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-29 13:51:17.000000 corsikaio-0.3.2/corsikaio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-29 13:51:04.000000 corsikaio-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-29 13:51:18.557168 corsikaio-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 13:51:04.000000 corsikaio-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:10:10.082941 corsikaio-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-31 16:09:55.000000 corsikaio-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 16:09:55.000000 corsikaio-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 16:09:55.000000 corsikaio-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-31 16:10:10.082941 corsikaio-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-31 16:09:55.000000 corsikaio-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:10:10.078941 corsikaio-0.3.3/corsikaio/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 16:10:09.000000 corsikaio-0.3.3/corsikaio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:10:10.082941 corsikaio-0.3.3/corsikaio/subblocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/subblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/subblocks/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/subblocks/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/subblocks/event_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/subblocks/event_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/subblocks/longitudinal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/subblocks/run_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/subblocks/run_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-31 16:09:55.000000 corsikaio-0.3.3/corsikaio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:10:10.082941 corsikaio-0.3.3/corsikaio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-31 16:10:09.000000 corsikaio-0.3.3/corsikaio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-31 16:10:10.000000 corsikaio-0.3.3/corsikaio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:10:09.000000 corsikaio-0.3.3/corsikaio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:10:07.000000 corsikaio-0.3.3/corsikaio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-31 16:10:09.000000 corsikaio-0.3.3/corsikaio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 16:10:09.000000 corsikaio-0.3.3/corsikaio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 16:09:55.000000 corsikaio-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-31 16:10:10.086942 corsikaio-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 16:09:55.000000 corsikaio-0.3.3/setup.py
```

### Comparing `corsikaio-0.3.2/.gitignore` & `corsikaio-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/LICENSE` & `corsikaio-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/PKG-INFO` & `corsikaio-0.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corsikaio
-Version: 0.3.2
+Version: 0.3.3
 Summary: Reader for corsika binary output files using numpy
 Home-page: http://github.com/cta-observatory/corsikaio
 Author: Maximilian Linhoff
 Author-email: maximilian.linhoff@tu-dortmund.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `corsikaio-0.3.2/README.md` & `corsikaio-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/__init__.py` & `corsikaio-0.3.3/corsikaio/__init__.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/file.py` & `corsikaio-0.3.3/corsikaio/file.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/io.py` & `corsikaio-0.3.3/corsikaio/io.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/subblocks/__init__.py` & `corsikaio-0.3.3/corsikaio/subblocks/__init__.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/subblocks/data.py` & `corsikaio-0.3.3/corsikaio/subblocks/data.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/subblocks/dtypes.py` & `corsikaio-0.3.3/corsikaio/subblocks/dtypes.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/subblocks/event_end.py` & `corsikaio-0.3.3/corsikaio/subblocks/event_end.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/subblocks/event_header.py` & `corsikaio-0.3.3/corsikaio/subblocks/event_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     Field(4, "total_energy", unit="GeV"),
     Field(5, "starting_altitude", unit="g/cm2"),
     Field(6, "first_target_id"),
     Field(7, "first_interaction_height", unit="cm"),
     Field(8, "momentum_x", unit="GeV/c"),
     Field(9, "momentum_y", unit="GeV/c"),
     Field(10, "momentum_minus_z", unit="GeV/c"),
-    Field(11, "zenith", unit="deg"),
-    Field(12, "azimuth", unit="deg"),
+    Field(11, "zenith", unit="rad"),
+    Field(12, "azimuth", unit="rad"),
     Field(13, "n_random_sequences"),
     Field(13 + 1, "random_seeds", shape=(10, 3)),
     Field(44, "run_number"),
     Field(45, "date"),
     Field(46, "version"),
     Field(47, "n_observation_levels"),
     Field(47 + 1, "observation_height", unit="cm", shape=10),
```

### Comparing `corsikaio-0.3.2/corsikaio/subblocks/longitudinal.py` & `corsikaio-0.3.3/corsikaio/subblocks/longitudinal.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/subblocks/run_header.py` & `corsikaio-0.3.3/corsikaio/subblocks/run_header.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio/version.py` & `corsikaio-0.3.3/corsikaio/version.py`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/corsikaio.egg-info/PKG-INFO` & `corsikaio-0.3.3/corsikaio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corsikaio
-Version: 0.3.2
+Version: 0.3.3
 Summary: Reader for corsika binary output files using numpy
 Home-page: http://github.com/cta-observatory/corsikaio
 Author: Maximilian Linhoff
 Author-email: maximilian.linhoff@tu-dortmund.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `corsikaio-0.3.2/corsikaio.egg-info/SOURCES.txt` & `corsikaio-0.3.3/corsikaio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `corsikaio-0.3.2/setup.cfg` & `corsikaio-0.3.3/setup.cfg`

 * *Files identical despite different names*

