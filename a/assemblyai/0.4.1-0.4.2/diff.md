# Comparing `tmp/assemblyai-0.4.1.tar.gz` & `tmp/assemblyai-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.4.1.tar", last modified: Wed May 31 19:20:30 2023, max compression
+gzip compressed data, was "assemblyai-0.4.2.tar", last modified: Wed May 31 20:09:39 2023, max compression
```

## Comparing `assemblyai-0.4.1.tar` & `assemblyai-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.358389 assemblyai-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 19:20:18.000000 assemblyai-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-31 19:20:30.358389 assemblyai-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-31 19:20:18.000000 assemblyai-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.354390 assemblyai-0.4.1/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.354390 assemblyai-0.4.1/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:20:30.358389 assemblyai-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-31 19:20:18.000000 assemblyai-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.354390 assemblyai-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.358389 assemblyai-0.4.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.404760 assemblyai-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 20:09:30.000000 assemblyai-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-31 20:09:39.404760 assemblyai-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-31 20:09:30.000000 assemblyai-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.400760 assemblyai-0.4.2/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44904 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.400760 assemblyai-0.4.2/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:09:39.404760 assemblyai-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-31 20:09:30.000000 assemblyai-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.400760 assemblyai-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.404760 assemblyai-0.4.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.4.1/LICENSE` & `assemblyai-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/PKG-INFO` & `assemblyai-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.4.1
+Version: 0.4.2
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
```

### Comparing `assemblyai-0.4.1/README.md` & `assemblyai-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/assemblyai/__init__.py` & `assemblyai-0.4.2/assemblyai/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/assemblyai/api.py` & `assemblyai-0.4.2/assemblyai/api.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/assemblyai/client.py` & `assemblyai-0.4.2/assemblyai/client.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/assemblyai/lemur.py` & `assemblyai-0.4.2/assemblyai/lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/assemblyai/transcriber.py` & `assemblyai-0.4.2/assemblyai/transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/assemblyai/types.py` & `assemblyai-0.4.2/assemblyai/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1068,14 +1068,15 @@
     text: str
     start: int
     end: int
     confidence: float
 
 
 class UtteranceWord(Word):
+    channel: Optional[str]
     speaker: Optional[str]
 
 
 class Utterance(UtteranceWord):
     words: List[UtteranceWord]
```

### Comparing `assemblyai-0.4.1/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.4.2/assemblyai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.4.1
+Version: 0.4.2
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
```

### Comparing `assemblyai-0.4.1/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.4.2/assemblyai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/setup.py` & `assemblyai-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.4.1",
+    version="0.4.2",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.4.1/tests/unit/factories.py` & `assemblyai-0.4.2/tests/unit/factories.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/tests/unit/test_domains.py` & `assemblyai-0.4.2/tests/unit/test_domains.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/tests/unit/test_lemur.py` & `assemblyai-0.4.2/tests/unit/test_lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/tests/unit/test_transcriber.py` & `assemblyai-0.4.2/tests/unit/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.1/tests/unit/test_transcript.py` & `assemblyai-0.4.2/tests/unit/test_transcript.py`

 * *Files identical despite different names*

