# Comparing `tmp/aleph-alpha-client-3.1.1.tar.gz` & `tmp/aleph-alpha-client-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-alpha-client-3.1.1.tar", last modified: Tue May 16 07:18:49 2023, max compression
+gzip compressed data, was "aleph-alpha-client-3.1.2.tar", last modified: Wed May 31 10:01:53 2023, max compression
```

## Comparing `aleph-alpha-client-3.1.1.tar` & `aleph-alpha-client-3.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:18:49.565080 aleph-alpha-client-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-16 07:18:49.565080 aleph-alpha-client-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:18:49.561080 aleph-alpha-client-3.1.1/aleph_alpha_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35139 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/aleph_alpha_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/detokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:18:49.561080 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:18:49.565080 aleph-alpha-client-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:18:49.565080 aleph-alpha-client-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/aleph_alpha_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/aleph_alpha_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/detokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/aleph_alpha_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 10:01:52.000000 aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:01:52.992418 aleph-alpha-client-3.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-31 10:01:42.000000 aleph-alpha-client-3.1.2/tests/test_tokenize.py
```

### Comparing `aleph-alpha-client-3.1.1/LICENSE` & `aleph-alpha-client-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/PKG-INFO` & `aleph-alpha-client-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.1
+Version: 3.1.2
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.1/README.md` & `aleph-alpha-client-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/__init__.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/aleph_alpha_client.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/aleph_alpha_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import aleph_alpha_client
 from aleph_alpha_client.explanation import (
     ExplanationRequest,
     ExplanationResponse,
     ExplanationRequest,
     ExplanationResponse,
 )
-from aleph_alpha_client.prompt import _to_json, _to_serializable_prompt
 from aleph_alpha_client.summarization import SummarizationRequest, SummarizationResponse
 from aleph_alpha_client.qa import QaRequest, QaResponse
 from aleph_alpha_client.completion import CompletionRequest, CompletionResponse
 from aleph_alpha_client.evaluation import EvaluationRequest, EvaluationResponse
 from aleph_alpha_client.tokenization import TokenizationRequest, TokenizationResponse
 from aleph_alpha_client.detokenization import (
     DetokenizationRequest,
@@ -557,14 +556,15 @@
         self.hosting = hosting
         self.request_timeout_seconds = request_timeout_seconds
         self.token = token
         self.nice = nice
 
         retry_options = ExponentialRetry(
             attempts=total_retries + 1,
+            exceptions={aiohttp.ClientConnectionError},
             start_timeout=0.25,
             statuses=set(RETRY_STATUS_CODES),
         )
         self.session = RetryClient(
             trust_env=True,  # same behaviour as requests/(Sync)Client wrt. http_proxy
             raise_for_status=False,
             retry_options=retry_options,
```

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/completion.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/completion.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/detokenization.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/detokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/document.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/document.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/embedding.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/embedding.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/evaluation.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/evaluation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/explanation.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/prompt.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -474,28 +474,7 @@
         return {"type": "text", "data": item}
     elif isinstance(item, List):
         return {"type": "token_ids", "data": item}
     else:
         raise ValueError(
             "The item in the prompt is not valid. Try either a string or an Image."
         )
-
-
-def _to_serializable_prompt(
-    prompt, at_least_one_token=False
-) -> Union[str, Sequence[Mapping[str, str]]]:
-    """
-    Validates that a prompt and emits the format suitable for serialization as JSON
-    """
-    if isinstance(prompt, str):
-        if at_least_one_token:
-            if len(prompt) == 0:
-                raise ValueError("prompt must contain at least one character")
-        # Just pass the string through as is.
-        return prompt
-
-    elif isinstance(prompt, list):
-        return [_to_json(item) for item in prompt]
-
-    raise ValueError(
-        "Invalid prompt. Prompt must either be a string, or a list of valid multimodal propmt items."
-    )
```

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/qa.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/search.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/search.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/summarization.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/summarization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client/tokenization.py` & `aleph-alpha-client-3.1.2/aleph_alpha_client/tokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/PKG-INFO` & `aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.1
+Version: 3.1.2
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/SOURCES.txt` & `aleph-alpha-client-3.1.2/aleph_alpha_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/setup.py` & `aleph-alpha-client-3.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_clients.py` & `aleph-alpha-client-3.1.2/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_complete.py` & `aleph-alpha-client-3.1.2/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_detokenize.py` & `aleph-alpha-client-3.1.2/tests/test_detokenize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_embed.py` & `aleph-alpha-client-3.1.2/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_error_handling.py` & `aleph-alpha-client-3.1.2/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_evaluate.py` & `aleph-alpha-client-3.1.2/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_explanation.py` & `aleph-alpha-client-3.1.2/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_image.py` & `aleph-alpha-client-3.1.2/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_prompt.py` & `aleph-alpha-client-3.1.2/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_qa.py` & `aleph-alpha-client-3.1.2/tests/test_qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_search.py` & `aleph-alpha-client-3.1.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_summarize.py` & `aleph-alpha-client-3.1.2/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.1/tests/test_tokenize.py` & `aleph-alpha-client-3.1.2/tests/test_tokenize.py`

 * *Files identical despite different names*

