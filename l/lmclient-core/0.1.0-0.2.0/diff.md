# Comparing `tmp/lmclient-core-0.1.0.tar.gz` & `tmp/lmclient-core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmclient-core-0.1.0.tar", max compression
+gzip compressed data, was "lmclient-core-0.2.0.tar", max compression
```

## Comparing `lmclient-core-0.1.0.tar` & `lmclient-core-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient-core-0.1.0/LICENSE
--rw-r--r--   0        0        0      568 2023-05-31 06:21:16.450580 lmclient-core-0.1.0/README.md
--rw-r--r--   0        0        0      187 2023-05-31 03:47:48.079921 lmclient-core-0.1.0/lmclient/__init__.py
--rw-r--r--   0        0        0     4504 2023-05-31 04:00:08.045809 lmclient-core-0.1.0/lmclient/client.py
--rw-r--r--   0        0        0      151 2023-05-31 03:48:41.450228 lmclient-core-0.1.0/lmclient/completions/__init__.py
--rw-r--r--   0        0        0     1320 2023-05-31 03:48:41.467315 lmclient-core-0.1.0/lmclient/completions/azure.py
--rw-r--r--   0        0        0     1117 2023-05-31 03:37:48.433094 lmclient-core-0.1.0/lmclient/completions/openai.py
--rw-r--r--   0        0        0      246 2023-05-31 03:48:41.453236 lmclient-core-0.1.0/lmclient/protocols.py
--rw-r--r--   0        0        0      538 2023-05-31 06:23:34.344800 lmclient-core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 lmclient-core-0.1.0/setup.py
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 lmclient-core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient-core-0.2.0/LICENSE
+-rw-r--r--   0        0        0      966 2023-05-31 07:37:53.134651 lmclient-core-0.2.0/README.md
+-rw-r--r--   0        0        0      187 2023-05-31 03:47:48.079921 lmclient-core-0.2.0/lmclient/__init__.py
+-rw-r--r--   0        0        0     5605 2023-05-31 07:39:43.149971 lmclient-core-0.2.0/lmclient/client.py
+-rw-r--r--   0        0        0      151 2023-05-31 03:48:41.450228 lmclient-core-0.2.0/lmclient/completions/__init__.py
+-rw-r--r--   0        0        0     1421 2023-05-31 06:58:04.718510 lmclient-core-0.2.0/lmclient/completions/azure.py
+-rw-r--r--   0        0        0     1223 2023-05-31 06:58:20.810104 lmclient-core-0.2.0/lmclient/completions/openai.py
+-rw-r--r--   0        0        0      267 2023-05-31 07:11:15.090406 lmclient-core-0.2.0/lmclient/protocols.py
+-rw-r--r--   0        0        0      690 2023-05-31 07:39:36.079759 lmclient-core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 lmclient-core-0.2.0/setup.py
+-rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 lmclient-core-0.2.0/PKG-INFO
```

### Comparing `lmclient-core-0.1.0/LICENSE` & `lmclient-core-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmclient-core-0.1.0/lmclient/client.py` & `lmclient-core-0.2.0/lmclient/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import time
 from enum import Enum
 from typing import ClassVar
 
 import anyio
 import asyncer
+import diskcache
 import tqdm
 
 from lmclient.protocols import CompletionModel
 
 
 class ErrorMode(str, Enum):
     RAISE = 'raise'
@@ -21,89 +22,107 @@
 
     def __init__(
         self,
         completion_model: CompletionModel,
         max_requests_per_minute: int = 20,
         async_capacity: int = 3,
         error_mode: ErrorMode | str = ErrorMode.RAISE,
+        cache_dir: str | None = None,
     ):
         self.completion_model = completion_model
         self.async_capacity = async_capacity
         self.max_requests_per_minute = max_requests_per_minute
         self.error_mode = ErrorMode(error_mode)
         self._task_created_time_list: list[int] = []
+        self.cache = diskcache.Cache(cache_dir) if cache_dir is not None else None
 
     def run(self, prompts: list[str], **kwargs) -> list[str]:
         progress_bar = tqdm.tqdm(desc=f'Sync {self.completion_model.__class__.__name__}', total=len(prompts))
-        values: list[str] = []
+        completions: list[str] = []
         for prompt in prompts:
-            values.append(self._run_single_task(prompt=prompt, progress_bar=progress_bar, **kwargs))
+            completion = self._run_single_task(prompt=prompt, progress_bar=progress_bar, **kwargs)
+            completions.append(completion)
         progress_bar.close()
-        return values
+        return completions
 
     @asyncer.runnify
     async def async_run(self, prompts: list[str], **kwargs) -> list[str]:
         limiter = anyio.CapacityLimiter(self.async_capacity)
         task_created_lock = anyio.Lock()
         progress_bar = tqdm.tqdm(desc=f'Async {self.completion_model.__class__.__name__}', total=len(prompts))
 
         soon_values: list[asyncer.SoonValue[str]] = []
         async with asyncer.create_task_group() as task_group:
             soon_func = task_group.soonify(self._async_run_single_task)
             for prompt in prompts:
-                soon_values.append(
-                    soon_func(
-                        prompt=prompt,
-                        limiter=limiter,
-                        task_created_lock=task_created_lock,
-                        progress_bar=progress_bar,
-                        **kwargs,
-                    )
+                soon_value = soon_func(
+                    prompt=prompt,
+                    limiter=limiter,
+                    task_created_lock=task_created_lock,
+                    progress_bar=progress_bar,
+                    **kwargs,
                 )
+                soon_values.append(soon_value)
 
         progress_bar.close()
         values = [soon_value.value for soon_value in soon_values]
         return values
 
     async def _async_run_single_task(
         self,
         prompt: str,
         limiter: anyio.CapacityLimiter,
         task_created_lock: anyio.Lock,
         progress_bar: tqdm.tqdm,
-        **openai_kwargs,
+        **kwargs,
     ) -> str:
         async with limiter:
+            task_key = self._gen_task_key(prompt=prompt, **kwargs)
+            if self.cache is not None and task_key in self.cache:
+                completion = self.cache[task_key]  # type: ignore
+                progress_bar.update(1)
+                return completion
+
             async with task_created_lock:
                 sleep_time = self._calculate_sleep_time()
                 if sleep_time > 0:
                     await anyio.sleep(sleep_time)
                 self._task_created_time_list.append(int(time.time()))
 
             try:
-                completion = await self.completion_model.async_complete(prompt=prompt, **openai_kwargs)
+                completion = await self.completion_model.async_complete(prompt=prompt, **kwargs)
+                if self.cache is not None:
+                    self.cache[task_key] = completion
             except BaseException as e:
                 if self.error_mode is ErrorMode.RAISE:
                     raise
                 elif self.error_mode is ErrorMode.IGNORE:
                     completion: str = f'Error: {e}'
                 else:
                     raise ValueError(f'Unknown error mode: {self.error_mode}')
 
             progress_bar.update(1)
             return completion
 
     def _run_single_task(self, prompt: str, progress_bar: tqdm.tqdm, **kwargs) -> str:
+        task_key = self._gen_task_key(prompt=prompt, **kwargs)
+        if self.cache is not None and task_key in self.cache:
+            completion = self.cache[task_key]  # type: ignore
+            progress_bar.update(1)
+            return completion
+
         sleep_time = self._calculate_sleep_time()
         if sleep_time > 0:
             time.sleep(sleep_time)
         self._task_created_time_list.append(int(time.time()))
 
         try:
             completion = self.completion_model.complete(prompt=prompt, **kwargs)
+            if self.cache is not None:
+                self.cache[task_key] = completion
         except BaseException as e:
             if self.error_mode is ErrorMode.RAISE:
                 raise
             elif self.error_mode is ErrorMode.IGNORE:
                 completion: str = f'Error: {e}'
             else:
                 raise ValueError(f'Unknown error mode: {self.error_mode}')
@@ -120,7 +139,12 @@
                 break
         self._task_created_time_list = self._task_created_time_list[idx:]
 
         if len(self._task_created_time_list) < self.max_requests_per_minute:
             return 0
         else:
             return max(self.NUM_SECONDS_PER_MINUTE - int(current_time - self._task_created_time_list[0]) + 1, 0)
+
+    def _gen_task_key(self, prompt: str, **kwargs) -> str:
+        items = sorted([f'{key}={value}' for key, value in kwargs.items()])
+        items = [prompt, self.completion_model.identifier] + items
+        return '---'.join(items)
```

### Comparing `lmclient-core-0.1.0/lmclient/completions/azure.py` & `lmclient-core-0.2.0/lmclient/completions/azure.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,30 +6,34 @@
 
 from lmclient.protocols import CompletionModel
 
 
 class AzureCompletion(CompletionModel):
     def __init__(
         self,
-        engine: str | None = None,
+        model: str | None = None,
         api_key: str | None = None,
         api_base: str | None = None,
         api_version: str | None = None,
     ):
-        self.engine = engine or os.environ['AZURE_CHAT_API_ENGINE']
+        self.model = model or os.environ['AZURE_CHAT_API_ENGINE']
 
         openai.api_type = 'azure'
         openai.api_key = api_key or os.environ['AZURE_API_KEY']
         openai.api_base = api_base or os.environ['AZURE_API_BASE']
         openai.api_version = api_version or os.getenv('AZURE_API_VERSION') or '2023-05-15'
 
     def complete(self, prompt: str, **kwargs) -> str:
         messages = [{'role': 'user', 'content': prompt}]
-        response = openai.ChatCompletion.create(engine=self.engine, messages=messages, **kwargs)
+        response = openai.ChatCompletion.create(engine=self.model, messages=messages, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
 
     async def async_complete(self, prompt: str, **kwargs) -> str:
         messages = [{'role': 'user', 'content': prompt}]
-        response = await openai.ChatCompletion.acreate(engine=self.engine, messages=messages, **kwargs)
+        response = await openai.ChatCompletion.acreate(engine=self.model, messages=messages, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
+
+    @property
+    def identifier(self) -> str:
+        return f'{self.__class__.__name__}({self.model})'
```

### Comparing `lmclient-core-0.1.0/lmclient/completions/openai.py` & `lmclient-core-0.2.0/lmclient/completions/openai.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,7 +27,11 @@
         return completion
 
     async def async_complete(self, prompt: str, **kwargs) -> str:
         messages = [{'role': 'user', 'content': prompt}]
         response = await openai.ChatCompletion.acreate(model=self.model, messages=messages, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
+
+    @property
+    def identifier(self) -> str:
+        return f'{self.__class__.__name__}({self.model})'
```

### Comparing `lmclient-core-0.1.0/pyproject.toml` & `lmclient-core-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [tool.poetry]
 name = "lmclient-core"
-version = "0.1.0"
+version = "0.2.0"
 description = "LM Async Client, openai client, azure openai client ..."
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 readme = "README.md"
+license = "Apache-2.0"
 packages = [{include = "lmclient"}]
+repository = "https://github.com/wangyuxinwhy/lmclient"
+keywords = ["lmclient", "openai", "azure", "async"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 openai = "^0.27.7"
 asyncer = "0.0.2"
 typing-extensions = "^4.6.2"
+diskcache = "^5.6.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 blue = "^0.9.1"
 isort = "^5.12.0"
 pyright = "^1.1.310"
```

### Comparing `lmclient-core-0.1.0/setup.py` & `lmclient-core-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 packages = \
 ['lmclient', 'lmclient.completions']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['asyncer==0.0.2', 'openai>=0.27.7,<0.28.0', 'typing-extensions>=4.6.2,<5.0.0']
+['asyncer==0.0.2',
+ 'diskcache>=5.6.1,<6.0.0',
+ 'openai>=0.27.7,<0.28.0',
+ 'typing-extensions>=4.6.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'lmclient-core',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'LM Async Client, openai client, azure openai client ...',
-    'long_description': "# lmclient\n\nLM Async Client, OpenAI, Azure ...\n\n\n## Install\n\n```shell\npip install lmclient-core\n```\n\n## Usage\n\n```python\nfrom lmclient import LMClient, AzureCompletion, OpenAICompletion\n\nopenai_completion = OpenAICompletion(model='gpt-3.5-turbo')\n# azure_completion = AzureCompletion()\nclient = LMClient(openai_completion, async_capacity=5, max_requests_per_minute=20)\nprompts = [\n    'Hello, my name is',\n    'can you please tell me your name?',\n    'i want to know your name',\n    'what is your name?',\n]\nvalues = client.async_run(prompts=prompts)\nprint(values)\n```\n",
+    'long_description': "# lmclient\n\nLM Async Client, OpenAI, Azure ...\n\n\n## Install\n\n```shell\npip install lmclient-core\n```\n\n## Usage\n\n```python\nfrom lmclient import LMClient, AzureCompletion, OpenAICompletion\n\nopenai_completion = OpenAICompletion(model='gpt-3.5-turbo')\n# azure_completion = AzureCompletion()\nclient = LMClient(openai_completion, async_capacity=5, max_requests_per_minute=20)\nprompts = [\n    'Hello, my name is',\n    'can you please tell me your name?',\n    'i want to know your name',\n    'what is your name?',\n]\nvalues = client.async_run(prompts=prompts)\nprint(values)\n```\n\n## Advanced Usage\n\n```python\n# limit max_requests_per_minute to 20\n# limit async_capacity to 5 (max 5 async requests at the same time)\n# use cache\n# set error_mode to ignore (ignore or raise)\n\nfrom lmclient import LMClient, OpenAICompletion\nopenai_completion = OpenAICompletion(model='gpt-3.5-turbo', max_requests_per_minute=20, async_capacity=5, cache_dir='openai_cache', error_mode='ignore')\n```",
     'author': 'wangyuxin',
     'author_email': 'wangyuxin@mokahr.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/wangyuxinwhy/lmclient',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

