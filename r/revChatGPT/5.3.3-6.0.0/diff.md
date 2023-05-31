# Comparing `tmp/revChatGPT-5.3.3.tar.gz` & `tmp/revChatGPT-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.3.3.tar", last modified: Tue May 30 03:32:19 2023, max compression
+gzip compressed data, was "revChatGPT-6.0.0.tar", last modified: Wed May 31 09:30:09 2023, max compression
```

## Comparing `revChatGPT-5.3.3.tar` & `revChatGPT-6.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:32:19.065348 revChatGPT-5.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-30 03:32:19.065348 revChatGPT-5.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-30 03:32:18.000000 revChatGPT-5.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 03:32:19.065348 revChatGPT-5.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:32:19.061347 revChatGPT-5.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:32:19.065348 revChatGPT-5.3.3/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    53881 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:32:19.065348 revChatGPT-5.3.3/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:32:19.065348 revChatGPT-5.3.3/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-30 03:32:19.000000 revChatGPT-5.3.3/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-30 03:32:19.000000 revChatGPT-5.3.3/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:32:19.000000 revChatGPT-5.3.3/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 03:32:19.000000 revChatGPT-5.3.3/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 03:32:19.000000 revChatGPT-5.3.3/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:32:19.065348 revChatGPT-5.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-30 03:31:50.000000 revChatGPT-5.3.3/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.186348 revChatGPT-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.186348 revChatGPT-6.0.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/tests/test_recipient.py
```

### Comparing `revChatGPT-5.3.3/LICENSE` & `revChatGPT-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.3/PKG-INFO` & `revChatGPT-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.3.3
+Version: 6.0.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-5.3.3/README.md` & `revChatGPT-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.3/setup.py` & `revChatGPT-6.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.3.3",
+    version="6.0.0",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-5.3.3/src/revChatGPT/V1.py` & `revChatGPT-6.0.0/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -862,14 +862,15 @@
         self.session.headers = headers_transfer
 
     async def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
+            **kwargs
     ) -> AsyncGenerator[dict, None]:
         cid, pid = data["conversation_id"], data["parent_message_id"]
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         message = ""
 
@@ -921,28 +922,40 @@
                 except json.decoder.JSONDecodeError:
                     continue
                 if not self.__check_fields(line):
                     raise ValueError(f"Field missing. Details: {str(line)}")
                 if line.get("message").get("author").get("role") != "assistant":
                     continue
 
-                message: str = line["message"]["content"]["parts"][0]
                 cid = line["conversation_id"]
                 pid = line["message"]["id"]
                 metadata = line["message"].get("metadata", {})
+                message_exists = False
+                author = {}
+                if line.get("message"):
+                    author = metadata.get("author", {}) or line["message"].get("author", {})
+                    if line["message"].get("content"):
+                        if line["message"]["content"].get("parts"):
+                            if len(line["message"]["content"]["parts"]) > 0:
+                                message_exists = True
+                message: str = (
+                    line["message"]["content"]["parts"][0] if message_exists else ""
+                )
                 model = metadata.get("model_slug", None)
                 finish_details = metadata.get("finish_details", {"type": None})["type"]
                 yield {
+                    "author": author,
                     "message": message,
                     "conversation_id": cid,
                     "parent_id": pid,
                     "model": model,
                     "finish_details": finish_details,
                     "end_turn": line["message"].get("end_turn", True),
                     "recipient": line["message"].get("recipient", "all"),
+                    "citations": metadata.get("citations", []),
                 }
 
             self.conversation_mapping[cid] = pid
             if pid:
                 self.parent_id = pid
             if cid:
                 self.conversation_id = cid
@@ -958,14 +971,15 @@
             yield msg
 
     async def post_messages(
         self,
         messages: list[dict],
         conversation_id: str | None = None,
         parent_id: str = "",
+        plugin_ids: list = [],
         model: str = "",
         auto_continue: bool = False,
         timeout: int = 360,
     ) -> AsyncGenerator[dict, None]:
         """Post messages to the chatbot
 
         Args:
@@ -1021,30 +1035,35 @@
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
             "history_and_training_disabled": self.disable_history,
         }
+        plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
+        if len(plugin_ids) > 0 and not conversation_id:
+            data["plugin_ids"] = plugin_ids
 
         async for msg in self.__send_request(
             data=data,
             auto_continue=auto_continue,
             timeout=timeout,
         ):
             yield msg
 
     async def ask(
-        self,
-        prompt: str,
-        conversation_id: str | None = None,
-        parent_id: str = "",
-        model: str = "",
-        auto_continue: bool = False,
-        timeout: int = 360,
+            self,
+            prompt: str,
+            conversation_id: str | None = None,
+            parent_id: str = "",
+            model: str = "",
+            plugin_ids: list = [],
+            auto_continue: bool = False,
+            timeout: int = 360,
+            **kwargs,
     ) -> AsyncGenerator[dict, None]:
         """Ask a question to the chatbot
 
         Args:
             prompt (str): The question to ask
             conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
             parent_id (str, optional): UUID for the message to continue on. Defaults to "".
@@ -1073,14 +1092,15 @@
             },
         ]
 
         async for msg in self.post_messages(
             messages=messages,
             conversation_id=conversation_id,
             parent_id=parent_id,
+            plugin_ids=plugin_ids,
             model=model,
             auto_continue=auto_continue,
             timeout=timeout,
         ):
             yield msg
 
     async def continue_write(
```

### Comparing `revChatGPT-5.3.3/src/revChatGPT/V3.py` & `revChatGPT-6.0.0/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.3/src/revChatGPT/__init__.py` & `revChatGPT-6.0.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.3/src/revChatGPT/__main__.py` & `revChatGPT-6.0.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.3/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.0.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.3/src/revChatGPT/recipient.py` & `revChatGPT-6.0.0/src/revChatGPT/recipient.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.3/src/revChatGPT/typings.py` & `revChatGPT-6.0.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.3/src/revChatGPT/utils.py` & `revChatGPT-6.0.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.3/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.0.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.3.3
+Version: 6.0.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-5.3.3/tests/test_recipient.py` & `revChatGPT-6.0.0/tests/test_recipient.py`

 * *Files identical despite different names*

