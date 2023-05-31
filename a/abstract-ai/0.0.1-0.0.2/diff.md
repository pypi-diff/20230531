# Comparing `tmp/abstract_ai-0.0.1.tar.gz` & `tmp/abstract_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.0.1.tar", last modified: Wed May 31 18:01:26 2023, max compression
+gzip compressed data, was "abstract_ai-0.0.2.tar", last modified: Wed May 31 18:04:28 2023, max compression
```

## Comparing `abstract_ai-0.0.1.tar` & `abstract_ai-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:01:26.311575 abstract_ai-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     5537 2023-05-31 18:01:26.311575 abstract_ai-0.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.1/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:01:26.311575 abstract_ai-0.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1400 2023-05-31 17:59:34.000000 abstract_ai-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:01:26.303575 abstract_ai-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:01:26.307575 abstract_ai-0.0.1/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.1/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3954 2023-05-31 17:28:34.000000 abstract_ai-0.0.1/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.1/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.1/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.1/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4110 2023-05-31 16:43:30.000000 abstract_ai-0.0.1/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     1990 2023-05-31 17:17:32.000000 abstract_ai-0.0.1/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:01:26.307575 abstract_ai-0.0.1/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5537 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:04:28.758359 abstract_ai-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     5537 2023-05-31 18:04:28.754359 abstract_ai-0.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:04:28.758359 abstract_ai-0.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1400 2023-05-31 18:04:12.000000 abstract_ai-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:04:28.750359 abstract_ai-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:04:28.754359 abstract_ai-0.0.2/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.2/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3983 2023-05-31 18:03:41.000000 abstract_ai-0.0.2/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.2/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.2/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.2/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4110 2023-05-31 16:43:30.000000 abstract_ai-0.0.2/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     1990 2023-05-31 17:17:32.000000 abstract_ai-0.0.2/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:04:28.754359 abstract_ai-0.0.2/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5537 2023-05-31 18:04:28.000000 abstract_ai-0.0.2/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 18:04:28.000000 abstract_ai-0.0.2/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:04:28.000000 abstract_ai-0.0.2/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 18:04:28.000000 abstract_ai-0.0.2/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 18:04:28.000000 abstract_ai-0.0.2/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.0.1/PKG-INFO` & `abstract_ai-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_ai-0.0.1/README.md` & `abstract_ai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.1/setup.py` & `abstract_ai-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.0.1',
+      version='0.0.2',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_ai',
       classifiers=[
```

### Comparing `abstract_ai-0.0.1/src/abstract_ai/api_calls.py` & `abstract_ai-0.0.2/src/abstract_ai/api_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import requests
 import openai
 from abstract_security.envy_it import get_env_value
-from .tokenization import count_tokens
+from .tokenization import count_tokens,calculate_token_distribution
 from .prompts import default_prompt,create_prompt
 from .endpoints import default_model,default_endpoint,default_tokens
 def get_openai_key(key:str='OPENAI_API_KEY'):
     """
     Retrieves the OpenAI API key from the environment variables.
 
     Args:
```

### Comparing `abstract_ai-0.0.1/src/abstract_ai/endpoints.py` & `abstract_ai-0.0.2/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.1/src/abstract_ai/main.py` & `abstract_ai-0.0.2/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.1/src/abstract_ai/prompts.py` & `abstract_ai-0.0.2/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.1/src/abstract_ai/response_handling.py` & `abstract_ai-0.0.2/src/abstract_ai/response_handling.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.1/src/abstract_ai/tokenization.py` & `abstract_ai-0.0.2/src/abstract_ai/tokenization.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.1/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.0.2/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

