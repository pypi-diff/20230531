# Comparing `tmp/abstract_ai-0.0.705.tar.gz` & `tmp/abstract_ai-0.0.706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.0.705.tar", last modified: Wed May 31 19:40:00 2023, max compression
+gzip compressed data, was "abstract_ai-0.0.706.tar", last modified: Wed May 31 19:45:14 2023, max compression
```

## Comparing `abstract_ai-0.0.705.tar` & `abstract_ai-0.0.706.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:40:00.802854 abstract_ai-0.0.705/
--rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:40:00.802854 abstract_ai-0.0.705/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.705/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.705/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 19:40:00.802854 abstract_ai-0.0.705/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1412 2023-05-31 19:39:44.000000 abstract_ai-0.0.705/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:40:00.794854 abstract_ai-0.0.705/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:40:00.798854 abstract_ai-0.0.705/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.705/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4193 2023-05-31 19:30:00.000000 abstract_ai-0.0.705/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.705/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.705/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.705/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4345 2023-05-31 19:39:32.000000 abstract_ai-0.0.705/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.705/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:40:00.802854 abstract_ai-0.0.705/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:40:00.000000 abstract_ai-0.0.705/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 19:40:00.000000 abstract_ai-0.0.705/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 19:40:00.000000 abstract_ai-0.0.705/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 19:40:00.000000 abstract_ai-0.0.705/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 19:40:00.000000 abstract_ai-0.0.705/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:45:14.578680 abstract_ai-0.0.706/
+-rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:45:14.578680 abstract_ai-0.0.706/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.706/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.706/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 19:45:14.578680 abstract_ai-0.0.706/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1412 2023-05-31 19:44:59.000000 abstract_ai-0.0.706/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:45:14.570680 abstract_ai-0.0.706/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:45:14.574680 abstract_ai-0.0.706/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.706/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4193 2023-05-31 19:30:00.000000 abstract_ai-0.0.706/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.706/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.706/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.706/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4344 2023-05-31 19:44:53.000000 abstract_ai-0.0.706/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     2060 2023-05-31 18:22:52.000000 abstract_ai-0.0.706/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:45:14.574680 abstract_ai-0.0.706/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5549 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 19:45:14.000000 abstract_ai-0.0.706/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.0.705/PKG-INFO` & `abstract_ai-0.0.706/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_ai
-Version: 0.0.705
+Version: 0.0.706
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_ai-0.0.705/README.md` & `abstract_ai-0.0.706/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.705/setup.py` & `abstract_ai-0.0.706/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.0.705',
+      version='0.0.706',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
       classifiers=[
```

### Comparing `abstract_ai-0.0.705/src/abstract_ai/api_calls.py` & `abstract_ai-0.0.706/src/abstract_ai/api_calls.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.705/src/abstract_ai/endpoints.py` & `abstract_ai-0.0.706/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.705/src/abstract_ai/main.py` & `abstract_ai-0.0.706/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.705/src/abstract_ai/prompts.py` & `abstract_ai-0.0.706/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.705/src/abstract_ai/response_handling.py` & `abstract_ai-0.0.706/src/abstract_ai/response_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     try:
         generated_text = json.loads(js['response']['choices'][0]['message']['content'])
         if 'title' in generated_text:
             title = generated_text['title']
     except:
         print()
     path = mkdirs(path_join(mkdirs(path_join(mkdirs('response_data'), get_date())), js['model']))
-    write_to_file(file_path=path_join(path, title + '.json'), contents=json.dumps(js))
+    write_to_file(filepath=path_join(path, title + '.json'), contents=json.dumps(js))
     return generated_text
 
 
 
 def find_keys(data, target_keys):
     """
     Finds the values associated with the specified target keys in a nested dictionary or list.
```

### Comparing `abstract_ai-0.0.705/src/abstract_ai/tokenization.py` & `abstract_ai-0.0.706/src/abstract_ai/tokenization.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.705/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.0.706/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-ai
-Version: 0.0.705
+Version: 0.0.706
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

