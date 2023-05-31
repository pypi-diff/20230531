# Comparing `tmp/catgpt-0.0.2.tar.gz` & `tmp/catgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catgpt-0.0.2.tar", max compression
+gzip compressed data, was "catgpt-0.0.4.tar", max compression
```

## Comparing `catgpt-0.0.2.tar` & `catgpt-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0       45 2023-04-29 02:44:31.917850 catgpt-0.0.2/catgpt/__init__.py
--rw-r--r--   0        0        0     3362 2023-04-29 02:44:27.522118 catgpt-0.0.2/catgpt/model.py
--rw-r--r--   0        0        0      404 2023-04-29 02:52:36.690391 catgpt-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      684 2023-04-29 02:53:21.677480 catgpt-0.0.2/setup.py
--rw-r--r--   0        0        0      512 2023-04-29 02:53:21.678281 catgpt-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       46 2023-04-29 02:55:42.000000 catgpt-0.0.4/catgpt/__init__.py
+-rw-r--r--   0        0        0     4396 2023-05-30 06:39:23.426058 catgpt-0.0.4/catgpt/model.py
+-rw-r--r--   0        0        0      404 2023-05-31 06:30:54.371070 catgpt-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 catgpt-0.0.4/PKG-INFO
```

### Comparing `catgpt-0.0.2/catgpt/model.py` & `catgpt-0.0.4/catgpt/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,51 +26,75 @@
         return resp
 
 
 class GPT(object):
     def __init__(self, api: str,
                  token: str,
                  model: str = 'gpt-3.5-turbo',
-                 history_path: str = None) -> None:
+                 openai_key:str = '',
+                 history_path: str = None,
+                 history_length: int = 5,
+                 proxy: dict = None) -> None:
+        """
+        Args:
+            api: api url
+            token: api token
+            openai_key: openai key
+            model: model name
+            history_path: path to save chat history
+            history_length: number of history to show
+            proxy: proxy dict
+        
+        1. if no openai_key is specified, then the server side will use the default openai key
+        2. otherwise, input `openai_key` will be used.
+        """
         self.api = api
         self.token = token
         self.model = model
+        self.history_length = history_length
+        self.openai_key=openai_key
         if history_path is None:
-            history_path = os.path.join('/tmp', cf.random_string(10) + '.txt')
+            today = time.strftime("%Y-%m-%d", time.localtime())
+            history_path = os.path.join('/tmp', 'chat-' + today + '.txt')
         self.chatdb = ChatDB(history_path)
+        self.proxy = proxy
 
     def get_headers(self):
         return {
             "Content-Type": "application/json",
             "token": self.token,
+            "openai_key": self.openai_key
         }
 
     def get_history(self, n: int = 5) -> list:
+        if n == 0:
+            return []
         history = self.chatdb.latest(n)
         return [h for h in history if h]
 
     def update_history(self, item: Dict[str, str]) -> None:
         self.chatdb.save(item)
 
     def make_post(self, prompt: str, stream: bool) -> requests.Response:
         """ Generate a post request to the API
         """
         prompt_dict = {"role": "user", "content": prompt}
-        history = self.get_history(5)
+        history = self.get_history(self.history_length)
         data = {
             "model":  self.model,
             "messages": history + [prompt_dict],
             "stream": stream
         }
         self.update_history(prompt_dict)
         return cf.net.post(
             self.api,
             stream=True,
             headers=self.get_headers(),
             json=data,
+            proxies=self.proxy,
         )
 
     def get_stream(self, prompt: str) -> str:
         request = self.make_post(prompt, stream=True)
         client = sseclient.SSEClient(request)
         contents_str = ''
         for _, event in enumerate(client.events()):
@@ -84,17 +108,23 @@
             'role': 'assistant',
             'content': contents_str
         })
         yield "\n"
 
     def get_response(self, prompt: str) -> str:
         request = self.make_post(prompt, stream=False)
-        response = json.loads(request.text)
-        if response:
-            return response['choices'][0]['message']['content']
+        try:
+            response = json.loads(request.text)
+            if response:
+                return response['choices'][0]['message']['content']
+        except Exception:
+            cf.warning({
+                'prompt': prompt,
+                'response': request.text
+            })
         return 'FOUND NO RESPONSE'
 
     def __call__(self, prompt: str, stream: bool = False) -> str:
         if stream:
             return self.get_stream(prompt)
         else:
             return self.get_response(prompt)
```

### Comparing `catgpt-0.0.2/PKG-INFO` & `catgpt-0.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: catgpt
-Version: 0.0.2
+Version: 0.0.4
 Summary: A simple cli tool to generate text using GPT-turbo
 Author: tom
 Author-email: tom@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: codefast (>=23.4.18,<24.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: sseclient-py (>=1.7.2,<2.0.0)
```

