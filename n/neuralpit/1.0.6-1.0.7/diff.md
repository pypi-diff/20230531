# Comparing `tmp/neuralpit-1.0.6.tar.gz` & `tmp/neuralpit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-1.0.6.tar", last modified: Thu May 25 08:05:06 2023, max compression
+gzip compressed data, was "neuralpit-1.0.7.tar", last modified: Wed May 31 14:10:03 2023, max compression
```

## Comparing `neuralpit-1.0.6.tar` & `neuralpit-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:05:06.031378 neuralpit-1.0.6/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 08:04:32.000000 neuralpit-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-25 08:05:06.031378 neuralpit-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-25 08:04:32.000000 neuralpit-1.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-25 08:04:32.000000 neuralpit-1.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 08:05:06.031378 neuralpit-1.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:05:06.027378 neuralpit-1.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:05:06.027378 neuralpit-1.0.6/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      204 2023-05-25 08:04:32.000000 neuralpit-1.0.6/src/neuralpit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:05:06.031378 neuralpit-1.0.6/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 08:04:32.000000 neuralpit-1.0.6/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-25 08:04:32.000000 neuralpit-1.0.6/src/neuralpit/services/api.py
--rw-r--r--   0 root         (0) root         (0)     1134 2023-05-25 08:04:32.000000 neuralpit-1.0.6/src/neuralpit/services/convert.py
--rw-r--r--   0 root         (0) root         (0)     1375 2023-05-25 08:04:32.000000 neuralpit-1.0.6/src/neuralpit/services/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:05:06.031378 neuralpit-1.0.6/src/neuralpit/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 08:04:32.000000 neuralpit-1.0.6/src/neuralpit/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2380 2023-05-25 08:04:32.000000 neuralpit-1.0.6/src/neuralpit/tools/chat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:05:06.031378 neuralpit-1.0.6/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-25 08:05:06.000000 neuralpit-1.0.6/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-25 08:05:06.000000 neuralpit-1.0.6/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:05:06.000000 neuralpit-1.0.6/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-25 08:05:06.000000 neuralpit-1.0.6/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-25 08:05:06.000000 neuralpit-1.0.6/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:05:06.031378 neuralpit-1.0.6/test/
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-25 08:04:32.000000 neuralpit-1.0.6/test/testDocChat.py
--rw-r--r--   0 root         (0) root         (0)      592 2023-05-25 08:04:32.000000 neuralpit-1.0.6/test/testGetServiceProfile.py
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-25 08:04:32.000000 neuralpit-1.0.6/test/testGetUserProfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 14:09:22.000000 neuralpit-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 14:10:03.672956 neuralpit-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-31 14:09:22.000000 neuralpit-1.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-31 14:09:22.000000 neuralpit-1.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 14:10:03.672956 neuralpit-1.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/services/api.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/services/converter.py
+-rw-r--r--   0 root         (0) root         (0)      368 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/services/converterFactory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/tools/chat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit/utils/
+-rw-r--r--   0 root         (0) root         (0)      631 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/utils/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     2003 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/utils/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      613 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/test/
+-rw-r--r--   0 root         (0) root         (0)      546 2023-05-31 14:09:22.000000 neuralpit-1.0.7/test/testDocChat.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-05-31 14:09:22.000000 neuralpit-1.0.7/test/testGetServiceProfile.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-31 14:09:22.000000 neuralpit-1.0.7/test/testGetUserProfile.py
```

### Comparing `neuralpit-1.0.6/PKG-INFO` & `neuralpit-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.6
+Version: 1.0.7
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-1.0.6/pyproject.toml` & `neuralpit-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "1.0.6"
+version = "1.0.7"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-1.0.6/src/neuralpit/services/api.py` & `neuralpit-1.0.7/src/neuralpit/services/api.py`

 * *Files identical despite different names*

### Comparing `neuralpit-1.0.6/src/neuralpit/services/convert.py` & `neuralpit-1.0.7/src/neuralpit/services/converter.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     def __init__(self) -> None:
         super().__init__()
 
     def convertFileToString(self, file) -> List[str]:
         pass
 
     def convertImageToString(self, file) -> List[str]:
-        pass
+        pass
```

### Comparing `neuralpit-1.0.6/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-1.0.7/src/neuralpit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.6
+Version: 1.0.7
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-1.0.6/src/neuralpit.egg-info/SOURCES.txt` & `neuralpit-1.0.7/src/neuralpit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/neuralpit/__init__.py
+src/neuralpit/context.py
 src/neuralpit.egg-info/PKG-INFO
 src/neuralpit.egg-info/SOURCES.txt
 src/neuralpit.egg-info/dependency_links.txt
 src/neuralpit.egg-info/requires.txt
 src/neuralpit.egg-info/top_level.txt
 src/neuralpit/services/__init__.py
 src/neuralpit/services/api.py
-src/neuralpit/services/convert.py
-src/neuralpit/services/document.py
+src/neuralpit/services/converter.py
+src/neuralpit/services/converterFactory.py
 src/neuralpit/tools/__init__.py
 src/neuralpit/tools/chat.py
+src/neuralpit/utils/indexer.py
+src/neuralpit/utils/loader.py
 test/testDocChat.py
 test/testGetServiceProfile.py
 test/testGetUserProfile.py
```

### Comparing `neuralpit-1.0.6/test/testGetServiceProfile.py` & `neuralpit-1.0.7/test/testGetServiceProfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from neuralpit.services.api import NeuralPitAPIService
-from neuralpit.services.convert import TikaConverterService
+from neuralpit.services.converter import TikaConverterService
 import os
 
 def main():
    client = NeuralPitAPIService()
    service = client.getServiceProfile('DOC_CHAT')
    print(service)
    server_url = service['converter']['server_url']
```

