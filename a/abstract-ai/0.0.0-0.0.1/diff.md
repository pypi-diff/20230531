# Comparing `tmp/abstract_ai-0.0.0.tar.gz` & `tmp/abstract_ai-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.0.0.tar", last modified: Wed May 31 17:34:53 2023, max compression
+gzip compressed data, was "abstract_ai-0.0.1.tar", last modified: Wed May 31 18:01:26 2023, max compression
```

## Comparing `abstract_ai-0.0.0.tar` & `abstract_ai-0.0.1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:34:53.487869 abstract_ai-0.0.0/
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-31 17:34:53.487869 abstract_ai-0.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.0/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 17:34:53.487869 abstract_ai-0.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:34:53.483869 abstract_ai-0.0.0/src/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.0/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:34:53.487869 abstract_ai-0.0.0/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.0/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3954 2023-05-31 17:28:34.000000 abstract_ai-0.0.0/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.0/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.0/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9736 2023-05-31 14:41:56.000000 abstract_ai-0.0.0/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4110 2023-05-31 16:43:30.000000 abstract_ai-0.0.0/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     1990 2023-05-31 17:17:32.000000 abstract_ai-0.0.0/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:34:53.487869 abstract_ai-0.0.0/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-31 17:34:53.000000 abstract_ai-0.0.0/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-31 17:34:53.000000 abstract_ai-0.0.0/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 17:34:53.000000 abstract_ai-0.0.0/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-31 17:34:53.000000 abstract_ai-0.0.0/src/abstract_ai.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:34:53.487869 abstract_ai-0.0.0/tests/
--rw-rw-r--   0 root         (0) root         (0)     4839 2023-05-31 13:44:23.000000 abstract_ai-0.0.0/tests/test.py
--rw-rw-r--   0 root         (0) root         (0)     9599 2023-05-31 10:50:09.000000 abstract_ai-0.0.0/tests/test3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:01:26.311575 abstract_ai-0.0.1/
+-rw-r--r--   0 root         (0) root         (0)     5537 2023-05-31 18:01:26.311575 abstract_ai-0.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.0.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:01:26.311575 abstract_ai-0.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1400 2023-05-31 17:59:34.000000 abstract_ai-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:01:26.303575 abstract_ai-0.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:01:26.307575 abstract_ai-0.0.1/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.0.1/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3954 2023-05-31 17:28:34.000000 abstract_ai-0.0.1/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.0.1/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.0.1/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.0.1/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4110 2023-05-31 16:43:30.000000 abstract_ai-0.0.1/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     1990 2023-05-31 17:17:32.000000 abstract_ai-0.0.1/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:01:26.307575 abstract_ai-0.0.1/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5537 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 18:01:26.000000 abstract_ai-0.0.1/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.0.0/README.md` & `abstract_ai-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.0/src/abstract_ai/api_calls.py` & `abstract_ai-0.0.1/src/abstract_ai/api_calls.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.0/src/abstract_ai/endpoints.py` & `abstract_ai-0.0.1/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.0/src/abstract_ai/main.py` & `abstract_ai-0.0.1/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.0/src/abstract_ai/prompts.py` & `abstract_ai-0.0.1/src/abstract_ai/prompts.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         js = {"model": model, "prompt": prompt, "max_tokens": max_tokens}
     else:
         js.setdefault("model", model)
         js.setdefault("prompt", prompt)
         js.setdefault("max_tokens", max_tokens)
     prompt_data = {"model": js['model'], "messages": [{"role": "user", "content": f'{js["prompt"]}'}],
                    "max_tokens": js['max_tokens']}
-    prompt_data["max_tokens"] = check_token_size(prompt_data, prompt_data['max_tokens'])
     return prompt_data
 
 
 def get_json_response():
     """
     Returns the description for the 'response' key in JSON format.
```

### Comparing `abstract_ai-0.0.0/src/abstract_ai/response_handling.py` & `abstract_ai-0.0.1/src/abstract_ai/response_handling.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.0.0/src/abstract_ai/tokenization.py` & `abstract_ai-0.0.1/src/abstract_ai/tokenization.py`

 * *Files identical despite different names*

