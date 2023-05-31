# Comparing `tmp/neuralpit-1.0.8.tar.gz` & `tmp/neuralpit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-1.0.8.tar", last modified: Wed May 31 15:08:25 2023, max compression
+gzip compressed data, was "neuralpit-1.0.9.tar", last modified: Wed May 31 17:40:20 2023, max compression
```

## Comparing `neuralpit-1.0.8.tar` & `neuralpit-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:07:42.000000 neuralpit-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 15:08:25.458119 neuralpit-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-31 15:07:42.000000 neuralpit-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-31 15:07:42.000000 neuralpit-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:08:25.458119 neuralpit-1.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.454119 neuralpit-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.454119 neuralpit-1.0.8/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/services/api.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/services/converter.py
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/services/converterFactory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/src/neuralpit/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/tools/chat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/src/neuralpit/utils/
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/utils/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.454119 neuralpit-1.0.8/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/test/
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-31 15:07:42.000000 neuralpit-1.0.8/test/testDocChat.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-05-31 15:07:42.000000 neuralpit-1.0.8/test/testGetServiceProfile.py
--rw-r--r--   0 root         (0) root         (0)      264 2023-05-31 15:07:42.000000 neuralpit-1.0.8/test/testGetUserProfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.378085 neuralpit-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 17:39:38.000000 neuralpit-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 17:40:20.378085 neuralpit-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-31 17:39:38.000000 neuralpit-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-31 17:39:38.000000 neuralpit-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 17:40:20.378085 neuralpit-1.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/services/api.py
+-rw-r--r--   0 root         (0) root         (0)      986 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/services/converter.py
+-rw-r--r--   0 root         (0) root         (0)      368 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/services/converterFactory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/tools/chat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit/utils/
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/utils/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/test/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-31 17:39:38.000000 neuralpit-1.0.9/test/testDocChat.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-05-31 17:39:38.000000 neuralpit-1.0.9/test/testGetServiceProfile.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-31 17:39:38.000000 neuralpit-1.0.9/test/testGetUserProfile.py
```

### Comparing `neuralpit-1.0.8/PKG-INFO` & `neuralpit-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.8
+Version: 1.0.9
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-1.0.8/pyproject.toml` & `neuralpit-1.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "1.0.8"
+version = "1.0.9"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-1.0.8/src/neuralpit/context.py` & `neuralpit-1.0.9/src/neuralpit/context.py`

 * *Files identical despite different names*

### Comparing `neuralpit-1.0.8/src/neuralpit/services/api.py` & `neuralpit-1.0.9/src/neuralpit/services/api.py`

 * *Files identical despite different names*

### Comparing `neuralpit-1.0.8/src/neuralpit/services/converter.py` & `neuralpit-1.0.9/src/neuralpit/services/converter.py`

 * *Files identical despite different names*

### Comparing `neuralpit-1.0.8/src/neuralpit/utils/loader.py` & `neuralpit-1.0.9/src/neuralpit/utils/loader.py`

 * *Files identical despite different names*

### Comparing `neuralpit-1.0.8/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-1.0.9/src/neuralpit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.8
+Version: 1.0.9
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-1.0.8/src/neuralpit.egg-info/SOURCES.txt` & `neuralpit-1.0.9/src/neuralpit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuralpit-1.0.8/test/testGetServiceProfile.py` & `neuralpit-1.0.9/test/testGetServiceProfile.py`

 * *Files identical despite different names*

