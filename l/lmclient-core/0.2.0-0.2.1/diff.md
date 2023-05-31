# Comparing `tmp/lmclient-core-0.2.0.tar.gz` & `tmp/lmclient-core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmclient-core-0.2.0.tar", max compression
+gzip compressed data, was "lmclient-core-0.2.1.tar", max compression
```

## Comparing `lmclient-core-0.2.0.tar` & `lmclient-core-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient-core-0.2.0/LICENSE
--rw-r--r--   0        0        0      966 2023-05-31 07:37:53.134651 lmclient-core-0.2.0/README.md
--rw-r--r--   0        0        0      187 2023-05-31 03:47:48.079921 lmclient-core-0.2.0/lmclient/__init__.py
--rw-r--r--   0        0        0     5605 2023-05-31 07:39:43.149971 lmclient-core-0.2.0/lmclient/client.py
--rw-r--r--   0        0        0      151 2023-05-31 03:48:41.450228 lmclient-core-0.2.0/lmclient/completions/__init__.py
--rw-r--r--   0        0        0     1421 2023-05-31 06:58:04.718510 lmclient-core-0.2.0/lmclient/completions/azure.py
--rw-r--r--   0        0        0     1223 2023-05-31 06:58:20.810104 lmclient-core-0.2.0/lmclient/completions/openai.py
--rw-r--r--   0        0        0      267 2023-05-31 07:11:15.090406 lmclient-core-0.2.0/lmclient/protocols.py
--rw-r--r--   0        0        0      690 2023-05-31 07:39:36.079759 lmclient-core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 lmclient-core-0.2.0/setup.py
--rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 lmclient-core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient-core-0.2.1/LICENSE
+-rw-r--r--   0        0        0      966 2023-05-31 07:37:53.134651 lmclient-core-0.2.1/README.md
+-rw-r--r--   0        0        0      187 2023-05-31 03:47:48.079921 lmclient-core-0.2.1/lmclient/__init__.py
+-rw-r--r--   0        0        0     6248 2023-05-31 08:19:14.595390 lmclient-core-0.2.1/lmclient/client.py
+-rw-r--r--   0        0        0      151 2023-05-31 03:48:41.450228 lmclient-core-0.2.1/lmclient/completions/__init__.py
+-rw-r--r--   0        0        0     1421 2023-05-31 06:58:04.718510 lmclient-core-0.2.1/lmclient/completions/azure.py
+-rw-r--r--   0        0        0     1223 2023-05-31 06:58:20.810104 lmclient-core-0.2.1/lmclient/completions/openai.py
+-rw-r--r--   0        0        0      267 2023-05-31 07:11:15.090406 lmclient-core-0.2.1/lmclient/protocols.py
+-rw-r--r--   0        0        0      690 2023-05-31 08:36:13.317730 lmclient-core-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 lmclient-core-0.2.1/setup.py
+-rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 lmclient-core-0.2.1/PKG-INFO
```

### Comparing `lmclient-core-0.2.0/LICENSE` & `lmclient-core-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmclient-core-0.2.0/README.md` & `lmclient-core-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lmclient-core-0.2.0/lmclient/client.py` & `lmclient-core-0.2.1/lmclient/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 from __future__ import annotations
 
 import time
 from enum import Enum
-from typing import ClassVar
+from typing import ClassVar, Literal
 
 import anyio
 import asyncer
 import diskcache
 import tqdm
 
 from lmclient.protocols import CompletionModel
 
 
 class ErrorMode(str, Enum):
     RAISE = 'raise'
     IGNORE = 'ignore'
 
 
+class ProgressBarMode(str, Enum):
+    AUTO = 'auto'
+    ALWAYS = 'always'
+    NEVER = 'never'
+
+
 class LMClient:
     NUM_SECONDS_PER_MINUTE: ClassVar[int] = 60
+    PROGRESS_BAR_THRESHOLD: ClassVar[int] = 30
 
     def __init__(
         self,
         completion_model: CompletionModel,
         max_requests_per_minute: int = 20,
         async_capacity: int = 3,
         error_mode: ErrorMode | str = ErrorMode.RAISE,
         cache_dir: str | None = None,
+        progress_bar: ProgressBarMode | str = ProgressBarMode.AUTO,
     ):
         self.completion_model = completion_model
         self.async_capacity = async_capacity
         self.max_requests_per_minute = max_requests_per_minute
         self.error_mode = ErrorMode(error_mode)
+        self.progress_bar_mode = ProgressBarMode(progress_bar)
         self._task_created_time_list: list[int] = []
         self.cache = diskcache.Cache(cache_dir) if cache_dir is not None else None
 
     def run(self, prompts: list[str], **kwargs) -> list[str]:
-        progress_bar = tqdm.tqdm(desc=f'Sync {self.completion_model.__class__.__name__}', total=len(prompts))
+        progress_bar = self._get_progress_bar(num_tasks=len(prompts))
         completions: list[str] = []
         for prompt in prompts:
             completion = self._run_single_task(prompt=prompt, progress_bar=progress_bar, **kwargs)
             completions.append(completion)
         progress_bar.close()
         return completions
 
     @asyncer.runnify
     async def async_run(self, prompts: list[str], **kwargs) -> list[str]:
         limiter = anyio.CapacityLimiter(self.async_capacity)
         task_created_lock = anyio.Lock()
-        progress_bar = tqdm.tqdm(desc=f'Async {self.completion_model.__class__.__name__}', total=len(prompts))
+        progress_bar = self._get_progress_bar(num_tasks=len(prompts))
 
         soon_values: list[asyncer.SoonValue[str]] = []
         async with asyncer.create_task_group() as task_group:
             soon_func = task_group.soonify(self._async_run_single_task)
             for prompt in prompts:
                 soon_value = soon_func(
                     prompt=prompt,
@@ -144,7 +153,16 @@
         else:
             return max(self.NUM_SECONDS_PER_MINUTE - int(current_time - self._task_created_time_list[0]) + 1, 0)
 
     def _gen_task_key(self, prompt: str, **kwargs) -> str:
         items = sorted([f'{key}={value}' for key, value in kwargs.items()])
         items = [prompt, self.completion_model.identifier] + items
         return '---'.join(items)
+
+    def _get_progress_bar(self, num_tasks: int) -> tqdm.tqdm:
+        use_progress_bar = (self.progress_bar_mode is ProgressBarMode.ALWAYS) or (
+            self.progress_bar_mode is ProgressBarMode.AUTO and num_tasks > self.PROGRESS_BAR_THRESHOLD
+        )
+        progress_bar = tqdm.tqdm(
+            desc=f'{self.completion_model.__class__.__name__}', total=num_tasks, disable=not use_progress_bar
+        )
+        return progress_bar
```

### Comparing `lmclient-core-0.2.0/lmclient/completions/azure.py` & `lmclient-core-0.2.1/lmclient/completions/azure.py`

 * *Files identical despite different names*

### Comparing `lmclient-core-0.2.0/lmclient/completions/openai.py` & `lmclient-core-0.2.1/lmclient/completions/openai.py`

 * *Files identical despite different names*

### Comparing `lmclient-core-0.2.0/pyproject.toml` & `lmclient-core-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lmclient-core"
-version = "0.2.0"
+version = "0.2.1"
 description = "LM Async Client, openai client, azure openai client ..."
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "lmclient"}]
 repository = "https://github.com/wangyuxinwhy/lmclient"
 keywords = ["lmclient", "openai", "azure", "async"]
```

### Comparing `lmclient-core-0.2.0/setup.py` & `lmclient-core-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['asyncer==0.0.2',
  'diskcache>=5.6.1,<6.0.0',
  'openai>=0.27.7,<0.28.0',
  'typing-extensions>=4.6.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'lmclient-core',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'LM Async Client, openai client, azure openai client ...',
     'long_description': "# lmclient\n\nLM Async Client, OpenAI, Azure ...\n\n\n## Install\n\n```shell\npip install lmclient-core\n```\n\n## Usage\n\n```python\nfrom lmclient import LMClient, AzureCompletion, OpenAICompletion\n\nopenai_completion = OpenAICompletion(model='gpt-3.5-turbo')\n# azure_completion = AzureCompletion()\nclient = LMClient(openai_completion, async_capacity=5, max_requests_per_minute=20)\nprompts = [\n    'Hello, my name is',\n    'can you please tell me your name?',\n    'i want to know your name',\n    'what is your name?',\n]\nvalues = client.async_run(prompts=prompts)\nprint(values)\n```\n\n## Advanced Usage\n\n```python\n# limit max_requests_per_minute to 20\n# limit async_capacity to 5 (max 5 async requests at the same time)\n# use cache\n# set error_mode to ignore (ignore or raise)\n\nfrom lmclient import LMClient, OpenAICompletion\nopenai_completion = OpenAICompletion(model='gpt-3.5-turbo', max_requests_per_minute=20, async_capacity=5, cache_dir='openai_cache', error_mode='ignore')\n```",
     'author': 'wangyuxin',
     'author_email': 'wangyuxin@mokahr.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/wangyuxinwhy/lmclient',
```

### Comparing `lmclient-core-0.2.0/PKG-INFO` & `lmclient-core-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmclient-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: LM Async Client, openai client, azure openai client ...
 Home-page: https://github.com/wangyuxinwhy/lmclient
 License: Apache-2.0
 Keywords: lmclient,openai,azure,async
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.8,<4.0
```

