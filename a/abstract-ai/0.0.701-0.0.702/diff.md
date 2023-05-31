# Comparing `tmp/abstract_ai-0.0.701.tar.gz` & `tmp/abstract_ai-0.0.702.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.0.701.tar", last modified: Wed May 31 19:30:27 2023, max compression
+gzip compressed data, was "abstract_ai-0.0.702.tar", last modified: Wed May 31 19:32:02 2023, max compression
```

## Comparing `abstract_ai-0.0.701.tar` & `abstract_ai-0.0.702.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:30:27.165393 abstract_ai-0.0.701/
--rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:30:27.165393 abstract_ai-0.0.701/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.701/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.701/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 19:30:27.165393 abstract_ai-0.0.701/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1412 2023-05-31 19:30:07.000000 abstract_ai-0.0.701/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:30:27.157394 abstract_ai-0.0.701/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:30:27.161394 abstract_ai-0.0.701/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.701/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4193 2023-05-31 19:30:00.000000 abstract_ai-0.0.701/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.701/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.701/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.701/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4244 2023-05-31 19:11:42.000000 abstract_ai-0.0.701/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.701/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:30:27.165393 abstract_ai-0.0.701/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:30:27.000000 abstract_ai-0.0.701/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 19:30:27.000000 abstract_ai-0.0.701/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 19:30:27.000000 abstract_ai-0.0.701/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 19:30:27.000000 abstract_ai-0.0.701/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 19:30:27.000000 abstract_ai-0.0.701/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:32:02.400370 abstract_ai-0.0.702/
+-rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:32:02.400370 abstract_ai-0.0.702/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.702/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.702/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 19:32:02.400370 abstract_ai-0.0.702/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1412 2023-05-31 19:31:45.000000 abstract_ai-0.0.702/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:32:02.392370 abstract_ai-0.0.702/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:32:02.396370 abstract_ai-0.0.702/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.702/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4193 2023-05-31 19:30:00.000000 abstract_ai-0.0.702/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.702/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.702/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.702/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4243 2023-05-31 19:31:38.000000 abstract_ai-0.0.702/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.702/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:32:02.400370 abstract_ai-0.0.702/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:32:02.000000 abstract_ai-0.0.702/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 19:32:02.000000 abstract_ai-0.0.702/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 19:32:02.000000 abstract_ai-0.0.702/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 19:32:02.000000 abstract_ai-0.0.702/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 19:32:02.000000 abstract_ai-0.0.702/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.0.701/PKG-INFO` & `abstract_ai-0.0.702/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_ai
-Version: 0.0.701
+Version: 0.0.702
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_ai-0.0.701/README.md` & `abstract_ai-0.0.702/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.701/setup.py` & `abstract_ai-0.0.702/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.0.701',
+      version='0.0.702',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
       classifiers=[
```

### Comparing `abstract_ai-0.0.701/src/abstract_ai/api_calls.py` & `abstract_ai-0.0.702/src/abstract_ai/api_calls.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.701/src/abstract_ai/endpoints.py` & `abstract_ai-0.0.702/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.701/src/abstract_ai/main.py` & `abstract_ai-0.0.702/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.701/src/abstract_ai/prompts.py` & `abstract_ai-0.0.702/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.701/src/abstract_ai/response_handling.py` & `abstract_ai-0.0.702/src/abstract_ai/response_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         print()
     try:
         generated_text = json.loads(js['response']['choices'][0]['message']['content'])
         if 'title' in generated_text:
             title = generated_text['title']
     except:
         print()
-    path = mkdirs(join_paths(mkdirs(join_paths(mkdirs('response_data'), date())), js['model']))
+    path = mkdirs(join_paths(mkdirs(path_join(mkdirs('response_data'), date())), js['model']))
     pen(join_paths(path, title + '.json'), json.dumps(js))
     return generated_text
 
 
 
 def find_keys(data, target_keys):
     """
```

### Comparing `abstract_ai-0.0.701/src/abstract_ai/tokenization.py` & `abstract_ai-0.0.702/src/abstract_ai/tokenization.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.701/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.0.702/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-ai
-Version: 0.0.701
+Version: 0.0.702
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```
