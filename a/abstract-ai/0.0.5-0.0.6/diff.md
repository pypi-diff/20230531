# Comparing `tmp/abstract_ai-0.0.5.tar.gz` & `tmp/abstract_ai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.0.5.tar", last modified: Wed May 31 18:25:23 2023, max compression
+gzip compressed data, was "abstract_ai-0.0.6.tar", last modified: Wed May 31 18:27:00 2023, max compression
```

## Comparing `abstract_ai-0.0.5.tar` & `abstract_ai-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:25:23.953917 abstract_ai-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     5547 2023-05-31 18:25:23.953917 abstract_ai-0.0.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.5/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:25:23.953917 abstract_ai-0.0.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1410 2023-05-31 18:25:07.000000 abstract_ai-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:25:23.945917 abstract_ai-0.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:25:23.949917 abstract_ai-0.0.5/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.5/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3985 2023-05-31 18:25:03.000000 abstract_ai-0.0.5/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.5/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.5/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.5/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4110 2023-05-31 16:43:30.000000 abstract_ai-0.0.5/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.5/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:25:23.949917 abstract_ai-0.0.5/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5547 2023-05-31 18:25:23.000000 abstract_ai-0.0.5/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 18:25:23.000000 abstract_ai-0.0.5/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:25:23.000000 abstract_ai-0.0.5/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 18:25:23.000000 abstract_ai-0.0.5/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 18:25:23.000000 abstract_ai-0.0.5/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:27:00.244852 abstract_ai-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-05-31 18:27:00.244852 abstract_ai-0.0.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.6/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:27:00.244852 abstract_ai-0.0.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1410 2023-05-31 18:26:42.000000 abstract_ai-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:27:00.236852 abstract_ai-0.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:27:00.240852 abstract_ai-0.0.6/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.6/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3981 2023-05-31 18:26:38.000000 abstract_ai-0.0.6/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.6/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.6/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.6/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4110 2023-05-31 16:43:30.000000 abstract_ai-0.0.6/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.6/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:27:00.244852 abstract_ai-0.0.6/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-05-31 18:27:00.000000 abstract_ai-0.0.6/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 18:27:00.000000 abstract_ai-0.0.6/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:27:00.000000 abstract_ai-0.0.6/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 18:27:00.000000 abstract_ai-0.0.6/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 18:27:00.000000 abstract_ai-0.0.6/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.0.5/PKG-INFO` & `abstract_ai-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_ai
-Version: 0.0.5
+Version: 0.0.6
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_ai-0.0.5/README.md` & `abstract_ai-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.5/setup.py` & `abstract_ai-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.0.5',
+      version='0.0.6',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
       classifiers=[
```

### Comparing `abstract_ai-0.0.5/src/abstract_ai/api_calls.py` & `abstract_ai-0.0.6/src/abstract_ai/api_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,13 +80,13 @@
         dict: The response received from the API request.
     """
     if 'prompt' not in js:
         js['prompt'] = prompt
     if 'max_tokens' not in js:
         js['max_tokens'] = default_tokens()
     token_dist=calculate_token_distribution(max_tokens=js['max_tokens'],prompt=js['prompt'],completion_percentage=40)
-    total = len(token_dist['chunks']['total'])
+    total = token_dist['chunks']['total']
     for k in range(0,):
         js['prompt'] = count_tokens(f'part {k} of {total}:\n){token_dist["chunks"]["data"][k]}')
-        js['max_tokens'] = count_tokens(js['prompt'])-token_dist["prompt"]["used"]
+        js['max_tokens'] += count_tokens(js['prompt'])-token_dist["prompt"]["used"]
         return save_response(js, requests.post(endpoint, json=create_prompt(js), headers=headers()))
```

### Comparing `abstract_ai-0.0.5/src/abstract_ai/endpoints.py` & `abstract_ai-0.0.6/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.5/src/abstract_ai/main.py` & `abstract_ai-0.0.6/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.5/src/abstract_ai/prompts.py` & `abstract_ai-0.0.6/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.5/src/abstract_ai/response_handling.py` & `abstract_ai-0.0.6/src/abstract_ai/response_handling.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.5/src/abstract_ai/tokenization.py` & `abstract_ai-0.0.6/src/abstract_ai/tokenization.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.5/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.0.6/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-ai
-Version: 0.0.5
+Version: 0.0.6
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

