# Comparing `tmp/chatsnack-0.1.6.tar.gz` & `tmp/chatsnack-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatsnack-0.1.6.tar", max compression
+gzip compressed data, was "chatsnack-0.1.7.tar", max compression
```

## Comparing `chatsnack-0.1.6.tar` & `chatsnack-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3795 2023-04-15 22:05:43.794976 chatsnack-0.1.6/chatsnack/__init__.py
--rw-r--r--   0        0        0    10772 2023-05-28 00:42:51.456671 chatsnack-0.1.6/chatsnack/aiwrapper.py
--rw-r--r--   0        0        0     1498 2023-04-09 18:26:53.563580 chatsnack-0.1.6/chatsnack/asynchelpers.py
--rw-r--r--   0        0        0     4737 2023-05-24 19:12:12.474715 chatsnack-0.1.6/chatsnack/chat/__init__.py
--rw-r--r--   0        0        0     6844 2023-04-29 03:01:10.662761 chatsnack-0.1.6/chatsnack/chat/mixin_messages.py
--rw-r--r--   0        0        0     6080 2023-05-26 23:20:36.198540 chatsnack-0.1.6/chatsnack/chat/mixin_params.py
--rw-r--r--   0        0        0    11473 2023-05-26 19:48:45.244560 chatsnack-0.1.6/chatsnack/chat/mixin_query.py
--rw-r--r--   0        0        0     3345 2023-05-24 21:40:51.429802 chatsnack-0.1.6/chatsnack/chat/mixin_serialization.py
--rw-r--r--   0        0        0      929 2023-04-09 15:02:47.382274 chatsnack-0.1.6/chatsnack/defaults.py
--rw-r--r--   0        0        0     1306 2023-04-09 15:11:16.782131 chatsnack-0.1.6/chatsnack/fillings.py
--rw-r--r--   0        0        0       25 2023-04-09 16:04:20.190406 chatsnack-0.1.6/chatsnack/packs/__init__.py
--rw-r--r--   0        0        0    19461 2023-04-14 02:01:22.528095 chatsnack-0.1.6/chatsnack/packs/default_packs/ChatsnackHelper.yml
--rw-r--r--   0        0        0      762 2023-04-14 02:00:30.545934 chatsnack-0.1.6/chatsnack/packs/default_packs/Chester.yml
--rw-r--r--   0        0        0      811 2023-04-14 01:57:06.309659 chatsnack-0.1.6/chatsnack/packs/default_packs/Confectioner.yml
--rw-r--r--   0        0        0      889 2023-04-14 01:57:06.272212 chatsnack-0.1.6/chatsnack/packs/default_packs/Data.yml
--rw-r--r--   0        0        0      736 2023-04-14 01:57:06.293264 chatsnack-0.1.6/chatsnack/packs/default_packs/Jane.yml
--rw-r--r--   0        0        0      905 2023-04-14 01:57:06.327853 chatsnack-0.1.6/chatsnack/packs/default_packs/Jolly.yml
--rw-r--r--   0        0        0     1244 2023-04-23 18:55:56.684760 chatsnack-0.1.6/chatsnack/packs/default_packs/Summarizer.yml
--rw-r--r--   0        0        0     2877 2023-05-03 23:27:38.108990 chatsnack-0.1.6/chatsnack/packs/module_help_vendor.py
--rw-r--r--   0        0        0     4028 2023-04-20 15:50:28.683064 chatsnack-0.1.6/chatsnack/packs/snackpacks.py
--rw-r--r--   0        0        0     1229 2023-04-06 15:39:54.021402 chatsnack-0.1.6/chatsnack/txtformat.py
--rw-r--r--   0        0        0     3976 2023-04-20 00:41:01.746999 chatsnack-0.1.6/chatsnack/yamlformat.py
--rw-r--r--   0        0        0     1091 2023-04-14 18:33:08.190283 chatsnack-0.1.6/LICENSE
--rw-r--r--   0        0        0     1030 2023-05-28 00:54:26.275409 chatsnack-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     9186 2023-04-29 00:10:57.640242 chatsnack-0.1.6/README.md
--rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 chatsnack-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3795 2023-04-15 22:05:43.794976 chatsnack-0.1.7/chatsnack/__init__.py
+-rw-r--r--   0        0        0    10772 2023-05-28 18:10:12.638570 chatsnack-0.1.7/chatsnack/aiwrapper.py
+-rw-r--r--   0        0        0     1498 2023-04-09 18:26:53.563580 chatsnack-0.1.7/chatsnack/asynchelpers.py
+-rw-r--r--   0        0        0     4681 2023-05-28 16:12:34.901207 chatsnack-0.1.7/chatsnack/chat/__init__.py
+-rw-r--r--   0        0        0     7561 2023-05-28 01:40:33.437804 chatsnack-0.1.7/chatsnack/chat/mixin_messages.py
+-rw-r--r--   0        0        0     6080 2023-05-26 23:20:36.198540 chatsnack-0.1.7/chatsnack/chat/mixin_params.py
+-rw-r--r--   0        0        0    11531 2023-05-28 19:30:49.305433 chatsnack-0.1.7/chatsnack/chat/mixin_query.py
+-rw-r--r--   0        0        0     3345 2023-05-24 21:40:51.429802 chatsnack-0.1.7/chatsnack/chat/mixin_serialization.py
+-rw-r--r--   0        0        0      929 2023-04-09 15:02:47.382274 chatsnack-0.1.7/chatsnack/defaults.py
+-rw-r--r--   0        0        0     1306 2023-04-09 15:11:16.782131 chatsnack-0.1.7/chatsnack/fillings.py
+-rw-r--r--   0        0        0       25 2023-04-09 16:04:20.190406 chatsnack-0.1.7/chatsnack/packs/__init__.py
+-rw-r--r--   0        0        0    19461 2023-04-14 02:01:22.528095 chatsnack-0.1.7/chatsnack/packs/default_packs/ChatsnackHelper.yml
+-rw-r--r--   0        0        0      762 2023-04-14 02:00:30.545934 chatsnack-0.1.7/chatsnack/packs/default_packs/Chester.yml
+-rw-r--r--   0        0        0      811 2023-04-14 01:57:06.309659 chatsnack-0.1.7/chatsnack/packs/default_packs/Confectioner.yml
+-rw-r--r--   0        0        0      889 2023-04-14 01:57:06.272212 chatsnack-0.1.7/chatsnack/packs/default_packs/Data.yml
+-rw-r--r--   0        0        0      736 2023-04-14 01:57:06.293264 chatsnack-0.1.7/chatsnack/packs/default_packs/Jane.yml
+-rw-r--r--   0        0        0      905 2023-04-14 01:57:06.327853 chatsnack-0.1.7/chatsnack/packs/default_packs/Jolly.yml
+-rw-r--r--   0        0        0     1244 2023-04-23 18:55:56.684760 chatsnack-0.1.7/chatsnack/packs/default_packs/Summarizer.yml
+-rw-r--r--   0        0        0     2877 2023-05-03 23:27:38.108990 chatsnack-0.1.7/chatsnack/packs/module_help_vendor.py
+-rw-r--r--   0        0        0     4028 2023-04-20 15:50:28.683064 chatsnack-0.1.7/chatsnack/packs/snackpacks.py
+-rw-r--r--   0        0        0     1229 2023-04-06 15:39:54.021402 chatsnack-0.1.7/chatsnack/txtformat.py
+-rw-r--r--   0        0        0     3976 2023-04-20 00:41:01.746999 chatsnack-0.1.7/chatsnack/yamlformat.py
+-rw-r--r--   0        0        0     1091 2023-04-14 18:33:08.190283 chatsnack-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1030 2023-05-31 14:21:19.659626 chatsnack-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9186 2023-04-29 00:10:57.640242 chatsnack-0.1.7/README.md
+-rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 chatsnack-0.1.7/PKG-INFO
```

### Comparing `chatsnack-0.1.6/chatsnack/__init__.py` & `chatsnack-0.1.7/chatsnack/__init__.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/aiwrapper.py` & `chatsnack-0.1.7/chatsnack/aiwrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         user = "_not_set"
     # prompt will be in JSON format, let us translate it to a python list
     # if the prompt is a list already, we will just use it as is
     if isinstance(prompt, list):
         messages = prompt
     else:
         messages = json.loads(prompt)
-    logger.debug("""Chat Query:
+    logger.trace("""Chat Query:
     Prompt: {0}
     Model: {2}, Max Tokens: {3}, Stop: {5}, Temperature: {1}, Top-P: {4}, Presence Penalty {6}, Frequency Penalty: {7}, N: {8}, Stream: {9}, User: {10}
     """,prompt, temperature, engine, max_tokens, top_p, stop, presence_penalty, frequency_penalty, n, stream, user)
     additional_args = {}
     if deployment is not None:
         additional_args["deployment_id"] = deployment
     if api_key_env is not None:
```

### Comparing `chatsnack-0.1.6/chatsnack/asynchelpers.py` & `chatsnack-0.1.7/chatsnack/asynchelpers.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/chat/__init__.py` & `chatsnack-0.1.7/chatsnack/chat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,16 @@
                 # if we get two args, the first is the name and the second is the system message
                 self.system_message = args[1]
         
         self._initial_name = self.name
         self._initial_params = copy.copy(self.params)
         self._initial_messages = copy.copy(self.messages)
         self._initial_system_message = self.system_message
-        self._ready = True
    
     def reset(self) -> object:
         """ Resets the chat prompt to its initial state, returns itself """
         self.name = self._initial_name
         self.params = self._initial_params
         self.messages = self._initial_messages
         if self._initial_system_message is not None:
             self.system_message = self._initial_system_message
-        self._ready = True
         return self
```

### Comparing `chatsnack-0.1.6/chatsnack/chat/mixin_messages.py` & `chatsnack-0.1.7/chatsnack/chat/mixin_messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,31 @@
                 if escape:
                     # escape the { and } characters
                     message["content"] = message["content"].replace("{", "{{").replace("}", "}}")
                     message["role"] = message["role"].replace("{", "{{").replace("}", "}}")
                 self.add_message(message["role"], message["content"])
             else:
                 raise ValueError("Invalid message format, a 'role' or 'content' key was missing")
+    def add_or_update_last_assistant_message(self, content: str):
+        """
+        Adds a final assistant message (or appends to the end of the last assistant message)
+        """
+        # get the last message in the list
+        last_message = self.messages[-1]
+        # get the dict version
+        last_message = self._msg_dict(last_message)
+
+        # if it's an assistant message, append to it
+        if "assistant" in last_message:
+            last_message["assistant"] += content
+            # replace the last message with the updated one
+            self.messages[-1] = last_message
+        else:
+            # otherwise add a new assistant message
+            self.assistant(content)
 
     # define a read-only attribute "last" that returns the last message in the list
     @property
     def last(self) -> str:
         """ Returns the value of the last message in the chat prompt (any)"""
         # last message is a dictionary, we need the last value in the dictionary
         if len(self.messages) > 0:
```

### Comparing `chatsnack-0.1.6/chatsnack/chat/mixin_params.py` & `chatsnack-0.1.7/chatsnack/chat/mixin_params.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/chat/mixin_query.py` & `chatsnack-0.1.7/chatsnack/chat/mixin_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,60 +98,46 @@
      
     async def _build_final_prompt(self, additional_vars = {}):
         promptvars = {}
         promptvars.update(additional_vars)
         # format the prompt text with the passed-in variables as well as doing internal expansion
         prompt = await self._gather_format(aformatter.async_format, **filling_machine(promptvars))
         return prompt
-    def _update_after_stream(self, response):
-        self.assistant(response)
-        self._ready = True
     async def _submit_for_response_and_prompt(self, **additional_vars):
         """ Executes the query as-is and returns a tuple of the final prompt and the response"""
-        if not self.ready:
-            raise Exception("Chat is not ready for a response")
         prompter = self
         # if the user in additional_vars, we're going to instead deepcopy this prompt into a new prompt and add the .user() to it
         if "__user" in additional_vars:
             new_chatprompt = self.copy()
             new_chatprompt.user(additional_vars["__user"])
             prompter = new_chatprompt
             # remove __user from additional_vars
             del additional_vars["__user"]
         prompt = await prompter._build_final_prompt(additional_vars)
         if self.params is None:
             return prompt, await cleaned_chat_completion(prompt)
         else:
             pparams = prompter.params._get_non_none_params()
             if self.params.stream:
-                self._ready = False
                 # we're streaming so we need to use the wrapper object
                 listener = ChatStreamListener(prompt, **self.params._get_non_none_params())
                 return prompt, listener
             else:
                 return prompt, await cleaned_chat_completion(prompt, **pparams)
 
     @property
-    def ready(self) -> bool:
-        """ Returns True if the chat is done, False otherwise ⭐"""
-        return self._ready
-    
-    @property
     def response(self) -> str:
         """ Returns the value of the last assistant message in the chat prompt ⭐"""
         last_assistant_message = None
-        if self.ready:
-            for _message in self.messages:
-                message = self._msg_dict(_message)
-                if "assistant" in message:
-                    last_assistant_message = message["assistant"]
-            # filter the response if we have a pattern
-            last_assistant_message = self.filter_by_pattern(last_assistant_message)
-        else:
-            last_assistant_message = self._response_so_far
+        for _message in self.messages:
+            message = self._msg_dict(_message)
+            if "assistant" in message:
+                last_assistant_message = message["assistant"]
+        # filter the response if we have a pattern
+        last_assistant_message = self.filter_by_pattern(last_assistant_message)
         return last_assistant_message
 
     def __str__(self):
         """ Returns the most recent response from the chat prompt ⭐"""
         if self.response is None:
             return ""
         else:
@@ -185,61 +171,70 @@
         """
         Executes the internal chat query as-is and returns a listener object that can be iterated on for the text.
         If usermsg is passed in, it will be added as a user message to the chat before executing the query. ⭐
         """
         if usermsg is not None:
             additional_vars["__user"] = usermsg
         _, response = asyncio.run(self._submit_for_response_and_prompt(**additional_vars))
-        if not self.ready:
+        if self.params.stream:
             # response is a ChatStreamListener so lets start it
             response.start()
         return response
     async def listen_a(self, usermsg=None, async_listen=True, **additional_vars) -> ChatStreamListener:
         """ Executes the query as-is, async version of listen()"""
         if not self.stream:
             raise Exception("Cannot use listen() without a stream")
         if usermsg is not None:
             additional_vars["__user"] = usermsg
         _, response = await self._submit_for_response_and_prompt(**additional_vars)
-        if not self.ready:
+        if self.params.stream:
             # response is a ChatStreamListener so lets start it
             await response.start_a()
         return response
     def chat(self, usermsg=None, **additional_vars) -> object:
         """ 
         Executes the query as-is and returns a new Chat for continuation 
         If usermsg is passed in, it will be added as a user message to the chat before executing the query. ⭐
         """
         if usermsg is not None:
             additional_vars["__user"] = usermsg
-        return asyncio.run(self.chat_a(**additional_vars))    
+        return asyncio.run(self.chat_a(**additional_vars))
     async def chat_a(self, usermsg=None, **additional_vars) -> object:
         """ Executes the query as-is, and returns a ChatPrompt object that contains the response. Async version of chat()"""
         if usermsg is not None:
             additional_vars["__user"] = usermsg
         if self.stream:
             raise Exception("Cannot use chat() with a stream")
         prompt, response = await self._submit_for_response_and_prompt(**additional_vars)
         # create a new chatprompt with the new name, copy it from this one
         new_chatprompt = self.__class__()
         new_chatprompt.params = self.params
         logger.trace("Expanded prompt: " + prompt)
         new_chatprompt.add_messages_json(prompt)
         # append the recent message
-        new_chatprompt.assistant(response)
+        new_chatprompt.add_or_update_last_assistant_message(response)
         return new_chatprompt
     
     # clone function to create a new chatprompt with the same name and data
     def copy(self, name: str = None, system = None, expand_includes: bool = False, expand_fillings: bool = False, **additional_vars) -> object:
         """ Returns a new ChatPrompt object that is a copy of this one, optionally with a new name ⭐"""
         import copy
         if name is not None:
             new_chat = self.__class__(name=name)
         else:
-            new_chat = self.__class__(name=self.name + f"_{datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}-{uuid.uuid4()}")
+            # if the existing name ends with _{datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}-{uuid.uuid4()}" then we need to trim that off and add a new one
+            # use a regex to match at the end of the name
+            import re
+            match = re.search(r"_(\d{4}-\d{2}-\d{2}_\d{2}-\d{2}-\d{2})-([a-f0-9]{8}-([a-f0-9]{4}-){3}[a-f0-9]{12})", self.name)
+            if match is not None:
+                # trim off the end
+                name = self.name[:match.start()]
+            else:
+                name = self.name
+            new_chat = self.__class__(name=name + f"_{datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}-{uuid.uuid4()}")
         new_chat.params = copy.copy(self.params)
         if expand_fillings:
             if not expand_includes:
                 raise NotImplementedError("Cannot expand fillings without expanding includes")
             prompt = asyncio.run(self._build_final_prompt(additional_vars))
             new_chat.add_messages_json(prompt, escape=True)
         else:
```

### Comparing `chatsnack-0.1.6/chatsnack/chat/mixin_serialization.py` & `chatsnack-0.1.7/chatsnack/chat/mixin_serialization.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/defaults.py` & `chatsnack-0.1.7/chatsnack/defaults.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/fillings.py` & `chatsnack-0.1.7/chatsnack/fillings.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/packs/default_packs/ChatsnackHelper.yml` & `chatsnack-0.1.7/chatsnack/packs/default_packs/ChatsnackHelper.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/packs/default_packs/Chester.yml` & `chatsnack-0.1.7/chatsnack/packs/default_packs/Chester.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/packs/default_packs/Confectioner.yml` & `chatsnack-0.1.7/chatsnack/packs/default_packs/Confectioner.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/packs/default_packs/Data.yml` & `chatsnack-0.1.7/chatsnack/packs/default_packs/Data.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/packs/default_packs/Jane.yml` & `chatsnack-0.1.7/chatsnack/packs/default_packs/Jane.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/packs/default_packs/Jolly.yml` & `chatsnack-0.1.7/chatsnack/packs/default_packs/Jolly.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/packs/default_packs/Summarizer.yml` & `chatsnack-0.1.7/chatsnack/packs/default_packs/Summarizer.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/packs/module_help_vendor.py` & `chatsnack-0.1.7/chatsnack/packs/module_help_vendor.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/packs/snackpacks.py` & `chatsnack-0.1.7/chatsnack/packs/snackpacks.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/txtformat.py` & `chatsnack-0.1.7/chatsnack/txtformat.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/chatsnack/yamlformat.py` & `chatsnack-0.1.7/chatsnack/yamlformat.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/LICENSE` & `chatsnack-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/pyproject.toml` & `chatsnack-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatsnack"
-version = "0.1.6"
+version = "0.1.7"
 description = "chatsnack is the easiest Python library for rapid development with OpenAI's ChatGPT API. It provides an intuitive interface for creating and managing chat-based prompts and responses, making it convenient to build complex, interactive conversations with AI."
 authors = ["Mattie Casper"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `chatsnack-0.1.6/README.md` & `chatsnack-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.6/PKG-INFO` & `chatsnack-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatsnack
-Version: 0.1.6
+Version: 0.1.7
 Summary: chatsnack is the easiest Python library for rapid development with OpenAI's ChatGPT API. It provides an intuitive interface for creating and managing chat-based prompts and responses, making it convenient to build complex, interactive conversations with AI.
 License: MIT
 Author: Mattie Casper
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

