# Comparing `tmp/abstract_ai-0.0.706.tar.gz` & `tmp/abstract_ai-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.0.706.tar", last modified: Wed May 31 19:45:14 2023, max compression
+gzip compressed data, was "abstract_ai-0.0.71.tar", last modified: Wed May 31 21:49:21 2023, max compression
```

## Comparing `abstract_ai-0.0.706.tar` & `abstract_ai-0.0.71.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:45:14.578680 abstract_ai-0.0.706/
--rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:45:14.578680 abstract_ai-0.0.706/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.706/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.706/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 19:45:14.578680 abstract_ai-0.0.706/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1412 2023-05-31 19:44:59.000000 abstract_ai-0.0.706/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:45:14.570680 abstract_ai-0.0.706/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:45:14.574680 abstract_ai-0.0.706/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.706/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4193 2023-05-31 19:30:00.000000 abstract_ai-0.0.706/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.706/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.706/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.706/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4344 2023-05-31 19:44:53.000000 abstract_ai-0.0.706/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.706/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:45:14.574680 abstract_ai-0.0.706/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:49:21.480196 abstract_ai-0.0.71/
+-rw-r--r--   0 root         (0) root         (0)     5548 2023-05-31 21:49:21.480196 abstract_ai-0.0.71/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.71/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.71/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 21:49:21.480196 abstract_ai-0.0.71/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1411 2023-05-31 21:48:47.000000 abstract_ai-0.0.71/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:49:21.472196 abstract_ai-0.0.71/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:49:21.476196 abstract_ai-0.0.71/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.71/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4502 2023-05-31 21:48:24.000000 abstract_ai-0.0.71/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.71/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.71/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.71/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4344 2023-05-31 19:44:53.000000 abstract_ai-0.0.71/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     2362 2023-05-31 21:48:37.000000 abstract_ai-0.0.71/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:49:21.480196 abstract_ai-0.0.71/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5548 2023-05-31 21:49:21.000000 abstract_ai-0.0.71/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 21:49:21.000000 abstract_ai-0.0.71/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 21:49:21.000000 abstract_ai-0.0.71/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 21:49:21.000000 abstract_ai-0.0.71/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 21:49:21.000000 abstract_ai-0.0.71/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.0.706/PKG-INFO` & `abstract_ai-0.0.71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_ai
-Version: 0.0.706
+Version: 0.0.71
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_ai-0.0.706/README.md` & `abstract_ai-0.0.71/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.706/setup.py` & `abstract_ai-0.0.71/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.0.706',
+      version='0.0.71',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
       classifiers=[
```

### Comparing `abstract_ai-0.0.706/src/abstract_ai/api_calls.py` & `abstract_ai-0.0.71/src/abstract_ai/api_calls.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,20 +80,25 @@
     Returns:
         dict: The response received from the API request.
     """
     if 'prompt' not in js:
         js['prompt'] = prompt
     if 'max_tokens' not in js:
         js['max_tokens'] = default_tokens()
+    js['max_tokens'] = int(js['max_tokens'])
+    pre_max = js['max_tokens']
     token_dist=calculate_token_distribution(max_tokens=js['max_tokens'],prompt=js['prompt'],completion_percentage=40)
     total = len(token_dist['chunks']["data"])
     responses = []
-    pre_max = js['max_tokens']
     for k in range(0,total):
-        js['prompt'] = f'part {k} of {total}:\n{token_dist["chunks"]["data"][k]}'
-        js['max_tokens'] = int(pre_max)-int(count_tokens(js['prompt']))-int(token_dist["prompt"]["used"])
+        bef = int(count_tokens(js['prompt']))
+        formatted_prompt = f'part {k} of {total}:\n{token_dist["chunks"]["data"][k]}'
+        formatted_prompt_length = count_tokens(formatted_prompt)
+        js['prompt'] = formatted_prompt
+        js['max_tokens'] = int(float(token_dist["completion"]["available"] - (formatted_prompt_length - bef))*.95)
+        #js['max_tokens'] = int(js['max_tokens']) -((int(count_tokens(js['prompt']))-int(pre_max)))
         response = requests.post(endpoint, json=create_prompt(js), headers=headers())
         resp = save_response(js, response)
         print(resp)
         responses.append(resp)
     return responses
```

### Comparing `abstract_ai-0.0.706/src/abstract_ai/endpoints.py` & `abstract_ai-0.0.71/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.706/src/abstract_ai/main.py` & `abstract_ai-0.0.71/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.706/src/abstract_ai/prompts.py` & `abstract_ai-0.0.71/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.706/src/abstract_ai/response_handling.py` & `abstract_ai-0.0.71/src/abstract_ai/response_handling.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.706/src/abstract_ai/tokenization.py` & `abstract_ai-0.0.71/src/abstract_ai/tokenization.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,76 @@
 from nltk.tokenize import word_tokenize
+
 def count_tokens(text):
     """
     Counts the number of tokens in the given text.
 
     Args:
         text (str): The input text.
 
     Returns:
         int: The number of tokens.
     """
     return len(word_tokenize(text))
+
+def convert_to_percentage(number):
+    if number > 1:
+        return number / 100
+    else:
+        return number
+
 def create_chunks(content, size_per_chunk):
-    words = content.split()
+    tokens = word_tokenize(content)
     chunks = []
     current_chunk = []
-    for word in words:
-        if len(' '.join(current_chunk)) + len(word) > size_per_chunk:
+    current_size = 0
+    for token in tokens:
+        current_size += 1
+        if current_size > size_per_chunk:
             chunks.append(' '.join(current_chunk))
             current_chunk = []
-        current_chunk.append(word)
+            current_size = 1
+        current_chunk.append(token)
     chunks.append(' '.join(current_chunk))
     return chunks
+
 def calculate_token_distribution(max_tokens, prompt:str, completion_percentage:float=40, size_per_chunk:int=None):
+    max_tokens = int(max_tokens)
+    completion_percentage = convert_to_percentage(completion_percentage)
     prompt_length = count_tokens(prompt)
     prompt_percentage = 1 - completion_percentage
-    prompt_available = int(float(max_tokens) * float(prompt_percentage)) - int(prompt_length)
-    completion_available = float(max_tokens) * float(completion_percentage)
-    completion_desired = float(max_tokens) * float(completion_percentage)
-    if size_per_chunk == None:
-        size_per_chunk =float(max_tokens) * float(prompt_percentage)
+    prompt_desired = int(max_tokens * prompt_percentage)
+    prompt_available = max(0, prompt_desired - prompt_length)
+    completion_available = int(max_tokens * completion_percentage)
+    completion_desired = completion_available
+
+    if size_per_chunk is None:
+        size_per_chunk = prompt_length if prompt_length < max_tokens else max_tokens
+
     num_chunks = prompt_length // size_per_chunk + 1 if prompt_length % size_per_chunk > 0 else prompt_length // size_per_chunk
 
     chunked_data = create_chunks(prompt, size_per_chunk)
 
     token_distribution = {
         "percent_distribution": {
             "prompt": prompt_percentage * 100,
             "completion": completion_percentage * 100
         },
         "prompt": {
             "available": prompt_available,
             "used": prompt_length,
-            "desired": max_tokens * prompt_percentage
+            "desired": prompt_desired
         },
         "completion": {
             "available": prompt_available + completion_available,
             "used": 0,
             "desired": completion_desired
         },
         "chunks": {
             "total": num_chunks,
             "length_per": size_per_chunk,
             "data": chunked_data
         }
     }
 
+    input(token_distribution)
     return token_distribution
-
```

### Comparing `abstract_ai-0.0.706/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.0.71/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-ai
-Version: 0.0.706
+Version: 0.0.71
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

