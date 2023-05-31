# Comparing `tmp/chatstream-0.1.4.tar.gz` & `tmp/chatstream-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatstream-0.1.4.tar", last modified: Fri May 26 02:36:51 2023, max compression
+gzip compressed data, was "chatstream-0.1.5.tar", last modified: Wed May 31 09:18:07 2023, max compression
```

## Comparing `chatstream-0.1.4.tar` & `chatstream-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 02:36:51.025482 chatstream-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-05-26 02:36:51.014081 chatstream-0.1.4/ChatStream.egg-info/
--rw-rw-rw-   0        0        0     7337 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 chatstream-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     7337 2023-05-26 02:36:51.024483 chatstream-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6485 2023-05-22 04:52:49.000000 chatstream-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 02:36:51.021482 chatstream-0.1.4/chatstream/
--rw-rw-rw-   0        0        0      168 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/__init__.py
--rw-rw-rw-   0        0        0     8430 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/chat_core.py
--rw-rw-rw-   0        0        0     8648 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/chat_process.py
--rw-rw-rw-   0        0        0     2907 2023-05-26 02:27:29.000000 chatstream-0.1.4/chatstream/chat_process_mock.py
--rw-rw-rw-   0        0        0     6416 2023-05-22 01:34:57.000000 chatstream-0.1.4/chatstream/chat_prompt.py
--rw-rw-rw-   0        0        0    20900 2023-05-26 02:24:23.000000 chatstream-0.1.4/chatstream/chat_stream.py
--rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/mock_response_example_text.py
-drwxrwxrwx   0        0        0        0 2023-05-26 02:36:51.024483 chatstream-0.1.4/chatstream/request_handler/
--rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/request_handler/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/request_handler/request_handler.py
--rw-rw-rw-   0        0        0     4916 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/request_handler/simple_session_request_handler.py
--rw-rw-rw-   0        0        0     3356 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/sampling_utils.py
--rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/util_request_id.py
--rw-rw-rw-   0        0        0       42 2023-05-26 02:36:51.025482 chatstream-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-05-26 02:33:07.000000 chatstream-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.086113 chatstream-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.065408 chatstream-0.1.5/ChatStream.egg-info/
+-rw-rw-rw-   0        0        0     8598 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 chatstream-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     8598 2023-05-31 09:18:07.085108 chatstream-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7703 2023-05-31 09:10:35.000000 chatstream-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.080605 chatstream-0.1.5/chatstream/
+-rw-rw-rw-   0        0        0      472 2023-05-31 07:50:57.000000 chatstream-0.1.5/chatstream/__init__.py
+-rw-rw-rw-   0        0        0     8430 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/chat_core.py
+-rw-rw-rw-   0        0        0     9316 2023-05-30 07:48:10.000000 chatstream-0.1.5/chatstream/chat_process.py
+-rw-rw-rw-   0        0        0     4447 2023-05-27 07:38:12.000000 chatstream-0.1.5/chatstream/chat_process_mock.py
+-rw-rw-rw-   0        0        0     8831 2023-05-30 07:38:04.000000 chatstream-0.1.5/chatstream/chat_prompt.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.082605 chatstream-0.1.5/chatstream/chat_prompt_presets/
+-rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/chat_prompt_presets/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-05-31 00:36:00.000000 chatstream-0.1.5/chatstream/chat_prompt_presets/chat_prompt_redpajama_incite.py
+-rw-rw-rw-   0        0        0     1452 2023-05-31 00:10:08.000000 chatstream-0.1.5/chatstream/chat_prompt_presets/chat_prompt_rinna.py
+-rw-rw-rw-   0        0        0    21392 2023-05-31 07:35:08.000000 chatstream-0.1.5/chatstream/chat_stream.py
+-rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/mock_response_example_text.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.085108 chatstream-0.1.5/chatstream/request_handler/
+-rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/request_handler/__init__.py
+-rw-rw-rw-   0        0        0     4428 2023-05-31 07:34:47.000000 chatstream-0.1.5/chatstream/request_handler/request_handler.py
+-rw-rw-rw-   0        0        0    10863 2023-05-31 07:35:08.000000 chatstream-0.1.5/chatstream/request_handler/simple_session_request_handler.py
+-rw-rw-rw-   0        0        0     3356 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/sampling_utils.py
+-rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/util_request_id.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 09:18:07.086113 chatstream-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-05-31 09:10:49.000000 chatstream-0.1.5/setup.py
```

### Comparing `chatstream-0.1.4/ChatStream.egg-info/PKG-INFO` & `chatstream-0.1.5/ChatStream.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chatstream
-Version: 0.1.4
-Summary: Streaming chat server building blocks for FastAPI/Starlette
+Version: 0.1.5
+Summary: A streaming chat toolkit for pre-trained large language models(LLM)
 Home-page: https://github.com/riversun/ChatStream
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatStream
 
-A load control utility for large-scale streaming chat servers using pre-trained large language models (LLM)
+[English](https://github.com/riversun/ChatStream/blob/main/README.md) | [&#26085;&#26412;&#35486;](https://github.com/riversun/ChatStream/blob/main/README_ja.md)
+
+
+A streaming chat toolkit for pre-trained large language models(LLM)
 
 ## Installation
 
 ```
 pip install chatstream
 ```
 
@@ -228,7 +231,40 @@
     start_server()
 
 
 if __name__ == "__main__":
     main()
 
 ```
+
+# License
+
+All code in this repository was developed by Tom Misawa except where otherwise noted.  Copyright (c) 2023, Tom Misawa.  All rights reserved. The code is licensed under the Apache 2.0 license.
+
+```
+Copyright 2023 Tom Misawa(riversun.org@gmail.com)
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+```
+
+# Citing ChatStream
+
+```bibtex
+@software{chatstream,
+  title = {{ChatStream: A streaming chat toolkit for pre-trained large language models(LLM)}},
+  author = {Tom Misawa(riversun.org@gmail.com) },
+  url = {https://github.com/riversun/ChatStream}
+  month = {5},
+  year = {2023},
+  version = {0.15},
+}
+```
```

### Comparing `chatstream-0.1.4/ChatStream.egg-info/SOURCES.txt` & `chatstream-0.1.5/ChatStream.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,10 +16,13 @@
 chatstream/sampling_utils.py
 chatstream/util_request_id.py
 chatstream.egg-info/PKG-INFO
 chatstream.egg-info/SOURCES.txt
 chatstream.egg-info/dependency_links.txt
 chatstream.egg-info/requires.txt
 chatstream.egg-info/top_level.txt
+chatstream/chat_prompt_presets/__init__.py
+chatstream/chat_prompt_presets/chat_prompt_redpajama_incite.py
+chatstream/chat_prompt_presets/chat_prompt_rinna.py
 chatstream/request_handler/__init__.py
 chatstream/request_handler/request_handler.py
 chatstream/request_handler/simple_session_request_handler.py
```

### Comparing `chatstream-0.1.4/LICENSE` & `chatstream-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.4/PKG-INFO` & `chatstream-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chatstream
-Version: 0.1.4
-Summary: Streaming chat server building blocks for FastAPI/Starlette
+Version: 0.1.5
+Summary: A streaming chat toolkit for pre-trained large language models(LLM)
 Home-page: https://github.com/riversun/ChatStream
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatStream
 
-A load control utility for large-scale streaming chat servers using pre-trained large language models (LLM)
+[English](https://github.com/riversun/ChatStream/blob/main/README.md) | [&#26085;&#26412;&#35486;](https://github.com/riversun/ChatStream/blob/main/README_ja.md)
+
+
+A streaming chat toolkit for pre-trained large language models(LLM)
 
 ## Installation
 
 ```
 pip install chatstream
 ```
 
@@ -228,7 +231,40 @@
     start_server()
 
 
 if __name__ == "__main__":
     main()
 
 ```
+
+# License
+
+All code in this repository was developed by Tom Misawa except where otherwise noted.  Copyright (c) 2023, Tom Misawa.  All rights reserved. The code is licensed under the Apache 2.0 license.
+
+```
+Copyright 2023 Tom Misawa(riversun.org@gmail.com)
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+```
+
+# Citing ChatStream
+
+```bibtex
+@software{chatstream,
+  title = {{ChatStream: A streaming chat toolkit for pre-trained large language models(LLM)}},
+  author = {Tom Misawa(riversun.org@gmail.com) },
+  url = {https://github.com/riversun/ChatStream}
+  month = {5},
+  year = {2023},
+  version = {0.15},
+}
+```
```

### Comparing `chatstream-0.1.4/README.md` & `chatstream-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # ChatStream
 
-A load control utility for large-scale streaming chat servers using pre-trained large language models (LLM)
+[English](https://github.com/riversun/ChatStream/blob/main/README.md) | [&#26085;&#26412;&#35486;](https://github.com/riversun/ChatStream/blob/main/README_ja.md)
+
+
+A streaming chat toolkit for pre-trained large language models(LLM)
 
 ## Installation
 
 ```
 pip install chatstream
 ```
 
@@ -210,8 +213,41 @@
 def main():
     start_server()
 
 
 if __name__ == "__main__":
     main()
 
-```
+```
+
+# License
+
+All code in this repository was developed by Tom Misawa except where otherwise noted.  Copyright (c) 2023, Tom Misawa.  All rights reserved. The code is licensed under the Apache 2.0 license.
+
+```
+Copyright 2023 Tom Misawa(riversun.org@gmail.com)
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+```
+
+# Citing ChatStream
+
+```bibtex
+@software{chatstream,
+  title = {{ChatStream: A streaming chat toolkit for pre-trained large language models(LLM)}},
+  author = {Tom Misawa(riversun.org@gmail.com) },
+  url = {https://github.com/riversun/ChatStream}
+  month = {5},
+  year = {2023},
+  version = {0.15},
+}
+```
```

### Comparing `chatstream-0.1.4/chatstream/chat_core.py` & `chatstream-0.1.5/chatstream/chat_core.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.4/chatstream/chat_process.py` & `chatstream-0.1.5/chatstream/chat_process.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,16 +111,23 @@
                     response_text = response_text[chat_prompt.get_skip_len():].strip()
             else:
                 # response_text = response_text[len(prompt):].strip()
                 pass
 
             updated_text = response_text[len(prev):]
 
-            updated_text_to_disp = self.tflow_for_updated_text.put(updated_text)
-            response_text_to_disp = self.tflow_for_response_text.put(response_text)
+            updated_text_to_disp=updated_text
+            response_text_to_disp=response_text
+
+            # tokflow 処理が必要な場合はバッファリングしたものをセットする
+            if self.tflow_for_updated_text is not None:
+                updated_text_to_disp = self.tflow_for_updated_text.put(updated_text)
+
+            if self.tflow_for_response_text is not None:
+                response_text_to_disp = self.tflow_for_response_text.put(response_text)
 
             if otype == "updated_text":
                 yield updated_text_to_disp
             elif otype == "response_text":
                 yield response_text_to_disp
             else:
                 yield response_text_to_disp, updated_text_to_disp, pos
@@ -141,17 +148,26 @@
                 # AI側の最後の返信を会話履歴に追加する
                 # この方式の場合は、最後まで（文章生成の正常停止まで）トークンが生成できた場合のみ chat_prompt に履歴を反映する
                 # もし途中で切断されたら履歴は残らない
                 chat_prompt.set_responder_last_msg(response_text.strip())
 
         pos = "end"
 
-        # tokflow 内に未出力のバッファが存在する可能性があるため flush する
-        updated_text_to_disp = self.tflow_for_updated_text.flush()
-        response_text_to_disp = self.tflow_for_response_text.flush()
+
+        if self.tflow_for_updated_text is not None:
+            # tokflow 内に未出力のバッファが存在する可能性があるため flush する
+            updated_text_to_disp = self.tflow_for_updated_text.flush()
+        else:
+            updated_text_to_disp = updated_text
+
+        if self.tflow_for_response_text is not None:
+            # tokflow 内に未出力のバッファが存在する可能性があるため flush する
+            response_text_to_disp = self.tflow_for_response_text.flush()
+        else:
+            response_text_to_disp = response_text
 
         # 最終メッセージを出力タイプごとに出しわける
         if otype == "updated_text":
             yield updated_text_to_disp
         elif otype == "response_text":
             yield response_text_to_disp
         else:
```

### Comparing `chatstream-0.1.4/chatstream/chat_stream.py` & `chatstream-0.1.5/chatstream/chat_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
                  # The number of simultaneous executions for sentence generation tasks in the pre-trained language model
                  max_queue_size: int = 5,
                  # The maximum queue size for sentence generation tasks in the pre-trained language model
                  too_many_request_as_http_error=False,
                  # True: When a 'Too many requests' situation occurs, it returns the status as 429
                  use_mock_response=False,
                  # True: Returns fixed phrases for testing. As it doesn't need to load the model, it starts up immediately
-                 mock_params={type:"round"},  # "round" / "long" - The type of phrases to return when use_mock_response=True
+                 mock_params={type: "round"},
+                 # "round" / "long" - The type of phrases to return when use_mock_response=True
                  chat_prompt_clazz=None,
                  # Specifies the class that manages the prompts sent to the language model. Inherit from AbstractChatPrompt and implement a class that generates chat prompts according to the etiquette of each model
                  max_new_tokens=256,  # The maximum size of the newly generated tokens
                  context_len=1024,  # The size of the context (in terms of the number of tokens)
                  temperature=1.0,  # The temperature value for randomness in prediction
                  top_k=50,  # Value of top K for sampling
                  top_p=1.0,  # Value of top P for sampling
@@ -45,15 +46,16 @@
                  logger=None,  # logging object
                  ):
 
         if logger is None:
             logger = logging.getLogger('chatstream')
             logger.setLevel(logging.NOTSET)
             handler = logging.StreamHandler()
-            handler.setFormatter(logging.Formatter('%(asctime)s [%(name)s][%(levelname)s] #%(funcName)s  %(message)s'))
+            handler.setFormatter(
+                logging.Formatter('%(asctime)s [%(name)s][%(levelname)s] %(module)s#%(funcName)s  %(message)s'))
 
             logger.addHandler(handler)
 
         self.logger = logger
 
         self.request_handler = request_handler
         self.request_handler.logger = logger
@@ -103,15 +105,15 @@
         else:
             self.chat_generator = ChatGenerator(model, tokenizer, device, chat_params)
 
         # request_handler にパラメータをセット
         request_handler.chat_generator = self.chat_generator
         request_handler.chat_prompt_clazz = self.chat_prompt_clazz
 
-    async def handle_starlette_request(self, request: Request):
+    async def handle_starlette_request(self, request: Request, request_body=None, callback=None):
         """
         This method performs sequential text generation based on user input received, using a pre-trained language model.
 
         The 'request' should be a FastAPI/Starlette Request object, with an expected JSON format in the request body as {"user_input": userText}.
 
         The 'response' is a StreamingResponse, which supports streaming text generation on the client side.
 
@@ -142,16 +144,18 @@
 
         # 非同期操作の結果を保持するための Future オブジェクトをつくる
         future_result = asyncio.Future()
 
         try:
             # リクエストキュー（処理待ち行列）にリクエストタスク(request, this_request_semaphore, future_result)を追加する
             self.request_queue.put_nowait(
-                (request, this_request_semaphore, future_result))  # put_nowait=>キューが一杯でない場合にのみ要求を追加
-            self.logger.debug(f"{req_id(request)} このリクエストを'リクエストキュー'に追加")
+                (request, request_body, callback, this_request_semaphore,
+                 future_result))  # put_nowait=>キューが一杯でない場合にのみ要求を追加
+            self.logger.debug(
+                f"{req_id(request)} このリクエストを'リクエストキュー'に追加 キューサイズ:{self.request_queue.qsize()}/{self.request_queue.maxsize}")
 
         except asyncio.QueueFull:
 
             # リクエストキュー（処理ち行列）を超えるリクエストがあった場合はエラーを返す
             # クライアント側ではこのエラーを受け取ったたら、エラーの旨と、再送のボタンなどを表示する
 
             self.logger.debug(f"{req_id(request)} このリクエストを'リクエストキュー'に追加失敗。リクエストキューがいっぱい")
@@ -201,15 +205,15 @@
 
         try:
             while True:
                 # request_queue.get()　でクライアントからのリクエストが発生するのを待つ
                 # クライアントからのリクエストが発生したとき
                 # 即座にそのリクエストタスク（request, this_request_semaphore, future_resultのタプル）はリクエストキュー(request_queue)から取りだされ
                 # 次実行キュー(run_on_next_queue) に詰められる
-                request, this_request_semaphore, future_result = await self.request_queue.get()
+                request, request_body, callback, this_request_semaphore, future_result = await self.request_queue.get()
 
                 self.logger.debug(f"{req_id(request)} 'リクエストキュー'からリクエストタスク取り出し")
 
                 # 同時処理カウントセマフォ(concurrent_processing_semaphore) がロックされているときに
                 # 短時間（１秒以内）に大量リクエストが来た場合、　次実行キュー(run_on_next_queue) に詰める前に
                 # リクエストキュー(request_queue) がいっぱいになるため、実際には run_on_next_queue のサイズ -1 の同時リクエストで
                 # too_many_request が発生するので注意。
@@ -218,61 +222,64 @@
                 # リクエストキュー(request_queue) のみだと、 request_queue.get したあと、 connection_semaphore.acquire の間で宙に浮く
                 # リクエストタスク（request, this_request_semaphore, resultのタプル）が発生してしまい、現在の待ち行列の大きさが直接的に
                 # 把握しづらくなるため、次に実行されるべきリクエストタスクを一時格納するために導入した
 
                 # リクエストが立て込んでいる場合、　基本的に　次実行キュー(run_on_next_queue) のサイズは 1 となる
                 # が、同時処理カウントセマフォ(concurrent_processing_semaphore)が取得され
                 # 次実行キュー(run_on_next_queue)からリクエストタスクが dequeue されてから、ループが1周まわるまでの短時間 0 になる
-                self.run_on_next_queue.put_nowait((request, this_request_semaphore, future_result))
+                self.run_on_next_queue.put_nowait(
+                    (request, request_body, callback, this_request_semaphore, future_result))
 
                 self.logger.debug(f"{req_id(request)} リクエストタスクを'次処理キュー'に追加")
 
                 # 同時処理カウントセマフォ(concurrent_processing_semaphore)を１つ取得
                 await self.concurrent_processing_semaphore.acquire()
 
                 request_task = await self.run_on_next_queue.get()  # 次実行キューを dequeue
                 self.processing_queue.put_nowait(request_task)  # 処理中キューに enqueue
 
                 self.logger.debug(f"{req_id(request)} リクエストタスク処理中： 実行権を獲得")
 
                 async def request_processing_finished_callback(request, message):
-
+                    self.logger.debug(f"{req_id(request)} 終了コールバックあり {message}")
                     """
                     文章生成ストリームの終了時に呼び出されるコールバック関数
                     ストリーム終了原因
                     ・message=="success" ストリームがクライアントに向け正常に送出された
-                    ・message=="client_disconnected_1" ストリーム送出中にクライアントから切断された
-                    ・message=="client_disconnected_2" ストリーム送出前にクライアントから切断されていた
+                    ・message=="client_disconnected_while_streaming" ストリーム送出中にクライアントから切断された
+                    ・message=="client_disconnected_before_streaming" ストリーム送出前にクライアントから切断されていた
                     ・message=="unknown_error_occurred" ストリーム送出中に予期せぬエラーが発生した
                     :param message:
                     :return:
                     """
 
                     # message は現在のところ、これより先には通知しない
                     # この結果を TODO 上位に伝えられるようにする
                     self.concurrent_processing_semaphore.release()  # 同時処理管理セマフォをリリースする Release the concurrent processing semaphore
                     await self.processing_queue.get()  # 現在の request を、リクエスト処理中キューから取り出す Get the current request from the request processing queue
                     self.logger.debug(f"{req_id(request)} リクエストタスク処理中： 文章生成終了　終了メッセージ:'{message}'")
-
+                    if callback:
+                        callback(request, message)
                     # 上の2つ（セマフォと、キュー）を解放したので、次に処理されるべきリクエストタスクが処理(モデルによる文章生成)できるようになる。
 
                 # concurrent_processing_semaphore を取得した request のみ、ここに入れる
                 final_response = None
                 try:
                     # request を処理する。responseは逐次出力を担当する StreamResponse になっているため、
                     # response を得たあともストリーミングが続いていることを忘れてはいけない
 
                     self.logger.debug(f"{req_id(request)} リクエストタスク処理中： リクエストハンドラにより処理開始")
-                    final_response = await self.request_handler.process_request(request,
-                                                                                streaming_finished_callback=request_processing_finished_callback)
+                    final_response = await self.request_handler.process_request(
+                        request, request_body,
+                        streaming_finished_callback=request_processing_finished_callback)
 
                 except ClientDisconnect as e:
                     # ストリーム送出開始時にクライアントから切断されていたとき
 
-                    await request_processing_finished_callback(request, "client_disconnected_2")
+                    await request_processing_finished_callback(request, "client_disconnected_before_streaming")
                 except Exception as e:
                     #  ストリーム送出開始時に想定していないエラーが発生したとき
 
                     self.logger.warning(f"{req_id(request)} 予期せぬエラーが発生しました: {e}\n{traceback.format_exc()}")
 
                     final_response = JSONResponse(
                         content={"error": "internal_server_error", "detail": "generating response"}, status_code=500,
```

### Comparing `chatstream-0.1.4/chatstream/mock_response_example_text.py` & `chatstream-0.1.5/chatstream/mock_response_example_text.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.4/chatstream/request_handler/request_handler.py` & `chatstream-0.1.5/chatstream/request_handler/request_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
 from abc import ABC, abstractmethod
 
 from fastapi import Request
 import traceback
 
+from chatstream.util_request_id import req_id
+
 
 class AbstractRequestHandler(ABC):
     """
     リクエストハンドラの基底抽象クラス
     本クラスを継承した独自のリクエストハンドラを作成し、
 
     process_request　をオーバーライドすることで以下のような要件を実装できる
@@ -25,47 +27,54 @@
     """
 
     def __init__(self):
         self.chat_generator = None
         self.chat_prompt_clazz = None
         self.logger = None
 
-    async def generate(self, chat_prompt, chat_generation_finished_callback):
+    async def generate(self, chat_prompt, chat_generation_finished_callback,request):
         f"""
         事前学習済言語モデルから逐次生成されたトークンを送出する非同期ジェネレーターを返す
         
         非同期ジェネレーターにより逐次トークンが生成され最終的に
         クライアントへのレスポンスストリームに送出されるが、
-        その送出中にクライアント側からの切断が検出された場合、コールバック関数に "client_disconnected_1"
+        その送出中にクライアント側からの切断が検出された場合、コールバック関数に "client_disconnected_while_streaming"
         をコールバックする
         
         :param chat_prompt: 
         :param chat_generation_finished_callback: 事前学習済言語モデルでの文章生成終了時に受け取るコールバック関数
         コールバック関数のパラメータは message
         文章生成状況に応じて、コールバックされるパラメータは以下の通りとなる
         
         "success" ... 文章生成が無事終了
-        "client_disconnected_1" ... レスポンス送出中にクライアントからの切断またはネットワーク切断が発生した
+        "client_disconnected_while_streaming" ... レスポンス送出中にクライアントからの切断またはネットワーク切断が発生した
         "unknown_error" ... 文章生成中に予期せぬエラーが発生した場合
         :return:                                 
         """
 
         # chat_generator.generate をラッピングすることで、 CancelledError をキャッチしてコールバックできるようにしている
         try:
             async for tok in self.chat_generator.generate(chat_prompt,
                                                           {"output_type": "response_text",
                                                            "post_process_callback": chat_generation_finished_callback
                                                            }):
                 yield tok
         except asyncio.CancelledError:
             # レスポンス送出中にクライアントからの切断が発生した場合
             # request 処理が異常終了(送出中にクライアントからの切断、ネットワーク断)したことを指定されたコールバック関数に通知
-            await chat_generation_finished_callback("client_disconnected_1")
+            await chat_generation_finished_callback("client_disconnected_while_streaming")
 
         except Exception as e:
             #  ストリーム送出開始時に想定していないエラーが発生したとき
-            print(f"予期せぬエラーが発生しました: {e}\n{traceback.format_exc()}")
+
+            self.logger.warning(f"{req_id(request)} 予期せぬエラーが発生しました: {e}\n{traceback.format_exc()}")
+
+            # エラーのコールバックを返す
             await chat_generation_finished_callback("unknown_error_occurred,while chat_generator.generate")
 
+            # エラーを上位に投げる
+            # (このエラーは、generator が yield しはじめた場合、上位にあがらない)
+            raise e
+
     @abstractmethod
     async def process_request(self, request: Request, streaming_finished_callback):
         pass
```

### Comparing `chatstream-0.1.4/chatstream/sampling_utils.py` & `chatstream-0.1.5/chatstream/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.4/chatstream/util_request_id.py` & `chatstream-0.1.5/chatstream/util_request_id.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.4/setup.py` & `chatstream-0.1.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chatstream",
-    version="0.1.4",
+    version="0.1.5",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
-    description="Streaming chat server building blocks for FastAPI/Starlette",
+    description="A streaming chat toolkit for pre-trained large language models(LLM)",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/ChatStream",
-    packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
+    packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples","doc","doc.*"]),
     tests_require=["pytest", "httpx", "transformers", "torch"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

