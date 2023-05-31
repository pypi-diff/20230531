# Comparing `tmp/abstract_ai-0.0.3.tar.gz` & `tmp/abstract_ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.0.3.tar", last modified: Wed May 31 18:08:27 2023, max compression
+gzip compressed data, was "abstract_ai-0.0.4.tar", last modified: Wed May 31 18:23:16 2023, max compression
```

## Comparing `abstract_ai-0.0.3.tar` & `abstract_ai-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:08:27.564390 abstract_ai-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     5537 2023-05-31 18:08:27.564390 abstract_ai-0.0.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.3/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:08:27.564390 abstract_ai-0.0.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1400 2023-05-31 18:08:08.000000 abstract_ai-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:08:27.556390 abstract_ai-0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:08:27.560390 abstract_ai-0.0.3/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.3/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3985 2023-05-31 18:07:53.000000 abstract_ai-0.0.3/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.3/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.3/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.3/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4110 2023-05-31 16:43:30.000000 abstract_ai-0.0.3/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     1990 2023-05-31 17:17:32.000000 abstract_ai-0.0.3/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:08:27.564390 abstract_ai-0.0.3/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5537 2023-05-31 18:08:27.000000 abstract_ai-0.0.3/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 18:08:27.000000 abstract_ai-0.0.3/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:08:27.000000 abstract_ai-0.0.3/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 18:08:27.000000 abstract_ai-0.0.3/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 18:08:27.000000 abstract_ai-0.0.3/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:23:16.479318 abstract_ai-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-05-31 18:23:16.479318 abstract_ai-0.0.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.4/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:23:16.479318 abstract_ai-0.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1410 2023-05-31 18:23:00.000000 abstract_ai-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:23:16.471318 abstract_ai-0.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:23:16.475318 abstract_ai-0.0.4/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.4/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3985 2023-05-31 18:07:53.000000 abstract_ai-0.0.4/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.4/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.4/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.4/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4110 2023-05-31 16:43:30.000000 abstract_ai-0.0.4/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.4/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:23:16.475318 abstract_ai-0.0.4/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-05-31 18:23:16.000000 abstract_ai-0.0.4/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 18:23:16.000000 abstract_ai-0.0.4/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:23:16.000000 abstract_ai-0.0.4/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 18:23:16.000000 abstract_ai-0.0.4/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 18:23:16.000000 abstract_ai-0.0.4/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.0.3/PKG-INFO` & `abstract_ai-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: abstract_ai
-Version: 0.0.3
+Version: 0.0.4
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
-Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_ai
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_ai-0.0.3/README.md` & `abstract_ai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.3/setup.py` & `abstract_ai-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.0.3',
+      version='0.0.4',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
-      url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_ai',
+      url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.11',
       ],
```

### Comparing `abstract_ai-0.0.3/src/abstract_ai/api_calls.py` & `abstract_ai-0.0.4/src/abstract_ai/api_calls.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.3/src/abstract_ai/endpoints.py` & `abstract_ai-0.0.4/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.3/src/abstract_ai/main.py` & `abstract_ai-0.0.4/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.3/src/abstract_ai/prompts.py` & `abstract_ai-0.0.4/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.3/src/abstract_ai/response_handling.py` & `abstract_ai-0.0.4/src/abstract_ai/response_handling.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.3/src/abstract_ai/tokenization.py` & `abstract_ai-0.0.4/src/abstract_ai/tokenization.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     for word in words:
         if len(' '.join(current_chunk)) + len(word) > size_per_chunk:
             chunks.append(' '.join(current_chunk))
             current_chunk = []
         current_chunk.append(word)
     chunks.append(' '.join(current_chunk))
     return chunks
-def calculate_token_distribution(max_tokens, prompt, completion_percentage:float=40, size_per_chunk:int=None):
+def calculate_token_distribution(max_tokens, prompt:str, completion_percentage:float=40, size_per_chunk:int=None):
     prompt_length = count_tokens(prompt)
     prompt_percentage = 1 - completion_percentage
-    prompt_available = max_tokens * prompt_percentage - prompt_length
-    completion_available = max_tokens * completion_percentage
-    completion_desired = max_tokens * completion_percentage
+    prompt_available = int(float(max_tokens) * float(prompt_percentage)) - int(prompt_length)
+    completion_available = float(max_tokens) * float(completion_percentage)
+    completion_desired = float(max_tokens) * float(completion_percentage)
     if size_per_chunk == None:
-        size_per_chunk =max_tokens * prompt_percentage
+        size_per_chunk =float(max_tokens) * float(prompt_percentage)
     num_chunks = prompt_length // size_per_chunk + 1 if prompt_length % size_per_chunk > 0 else prompt_length // size_per_chunk
 
     chunked_data = create_chunks(prompt, size_per_chunk)
 
     token_distribution = {
         "percent_distribution": {
             "prompt": prompt_percentage * 100,
```

### Comparing `abstract_ai-0.0.3/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.0.4/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: abstract-ai
-Version: 0.0.3
+Version: 0.0.4
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
-Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_ai
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

