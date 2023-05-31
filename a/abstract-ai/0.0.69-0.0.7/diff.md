# Comparing `tmp/abstract_ai-0.0.69.tar.gz` & `tmp/abstract_ai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.0.69.tar", last modified: Wed May 31 19:25:30 2023, max compression
+gzip compressed data, was "abstract_ai-0.0.7.tar", last modified: Wed May 31 19:27:48 2023, max compression
```

## Comparing `abstract_ai-0.0.69.tar` & `abstract_ai-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:25:30.420573 abstract_ai-0.0.69/
--rw-r--r--   0 root         (0) root         (0)     5548 2023-05-31 19:25:30.420573 abstract_ai-0.0.69/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.69/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.69/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 19:25:30.420573 abstract_ai-0.0.69/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1411 2023-05-31 19:25:09.000000 abstract_ai-0.0.69/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:25:30.412573 abstract_ai-0.0.69/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:25:30.416573 abstract_ai-0.0.69/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.69/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4213 2023-05-31 19:01:14.000000 abstract_ai-0.0.69/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.69/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.69/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.69/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4244 2023-05-31 19:11:42.000000 abstract_ai-0.0.69/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.69/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:25:30.420573 abstract_ai-0.0.69/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5548 2023-05-31 19:25:30.000000 abstract_ai-0.0.69/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 19:25:30.000000 abstract_ai-0.0.69/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 19:25:30.000000 abstract_ai-0.0.69/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 19:25:30.000000 abstract_ai-0.0.69/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 19:25:30.000000 abstract_ai-0.0.69/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:27:48.959091 abstract_ai-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-05-31 19:27:48.955091 abstract_ai-0.0.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.7/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 19:27:48.959091 abstract_ai-0.0.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1410 2023-05-31 19:27:32.000000 abstract_ai-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:27:48.951091 abstract_ai-0.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:27:48.955091 abstract_ai-0.0.7/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.7/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4201 2023-05-31 19:27:22.000000 abstract_ai-0.0.7/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.7/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.7/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.7/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4244 2023-05-31 19:11:42.000000 abstract_ai-0.0.7/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.7/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:27:48.955091 abstract_ai-0.0.7/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-05-31 19:27:48.000000 abstract_ai-0.0.7/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 19:27:48.000000 abstract_ai-0.0.7/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 19:27:48.000000 abstract_ai-0.0.7/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 19:27:48.000000 abstract_ai-0.0.7/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 19:27:48.000000 abstract_ai-0.0.7/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.0.69/PKG-INFO` & `abstract_ai-0.0.7/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract_ai
-Version: 0.0.69
+Name: abstract-ai
+Version: 0.0.7
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_ai-0.0.69/README.md` & `abstract_ai-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.69/setup.py` & `abstract_ai-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.0.69',
+      version='0.0.7',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
       classifiers=[
```

### Comparing `abstract_ai-0.0.69/src/abstract_ai/api_calls.py` & `abstract_ai-0.0.7/src/abstract_ai/api_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Returns:
         dict: The headers containing the 'Content-Type' and 'Authorization' information.
     """
     return {'Content-Type': content_type, 'Authorization': f'Bearer {api_key}'}
 def post_request(endpoint:str=default_endpoint(), prompt:(str or dict)=create_prompt(),content_type:str='application/json',api_key:str=get_openai_key()):
         response = requests.post(endpoint, headers=headers(content_type,api_key), json=prompt)
         if response.status_code == 200:
-            return response.json()
+            return response
         else:
             raise Exception(f'Request failed with status code {response.status_code}')
 
 def hard_request(prompt:str=default_prompt(),model:str=default_model(),max_tokens:int=default_tokens(),temperature:float=0.5,top_p:int=1,frequency_penalty:int=0,presence_penalty:int=0):
     input([prompt,max_tokens,model])
     """
     Sends a hard request to the OpenAI API using the provided parameters.
@@ -89,11 +89,11 @@
     responses = []
     pre_max = js['max_tokens']
     for k in range(0,total):
         js['prompt'] = f'part {k} of {total}:\n{token_dist["chunks"]["data"][k]}'
         js['max_tokens'] = int(pre_max)-int(count_tokens(js['prompt']))-int(token_dist["prompt"]["used"])
         response = requests.post(endpoint, json=create_prompt(js), headers=headers())
         save_response(js, response.json())
-        print(response.text)
+        print(response)
         responses.append(response)
     return responses
```

### Comparing `abstract_ai-0.0.69/src/abstract_ai/endpoints.py` & `abstract_ai-0.0.7/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.69/src/abstract_ai/main.py` & `abstract_ai-0.0.7/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.69/src/abstract_ai/prompts.py` & `abstract_ai-0.0.7/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.69/src/abstract_ai/response_handling.py` & `abstract_ai-0.0.7/src/abstract_ai/response_handling.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.69/src/abstract_ai/tokenization.py` & `abstract_ai-0.0.7/src/abstract_ai/tokenization.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.69/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract-ai
-Version: 0.0.69
+Name: abstract_ai
+Version: 0.0.7
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

