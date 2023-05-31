# Comparing `tmp/archytas-0.3.0.tar.gz` & `tmp/archytas-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-0.3.0.tar", max compression
+gzip compressed data, was "archytas-1.0.0.tar", max compression
```

## Comparing `archytas-0.3.0.tar` & `archytas-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32472 2023-05-15 11:48:23.713528 archytas-0.3.0/LICENSE
--rw-r--r--   0        0        0     2088 2023-05-15 11:48:23.713528 archytas-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/__init__.py
--rw-r--r--   0        0        0     8481 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/agent.py
--rw-r--r--   0        0        0     9746 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/demo_tools.py
--rw-r--r--   0        0        0     4129 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/prompt.py
--rw-r--r--   0        0        0     3166 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/python.py
--rw-r--r--   0        0        0     7500 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/react.py
--rw-r--r--   0        0        0     1462 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/repl.py
--rw-r--r--   0        0        0    18038 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/tool_utils.py
--rw-r--r--   0        0        0     4586 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/tools.py
--rw-r--r--   0        0        0     1251 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/utils.py
--rw-r--r--   0        0        0      780 2023-05-15 11:48:23.749529 archytas-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 archytas-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-05-31 19:52:28.418704 archytas-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2088 2023-05-31 19:52:28.418704 archytas-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/__init__.py
+-rw-r--r--   0        0        0     8291 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/agent.py
+-rw-r--r--   0        0        0     9746 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/demo_tools.py
+-rw-r--r--   0        0        0     4129 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/prompt.py
+-rw-r--r--   0        0        0     3166 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/python.py
+-rw-r--r--   0        0        0     7521 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/react.py
+-rw-r--r--   0        0        0     1462 2023-05-31 19:52:28.418704 archytas-1.0.0/archytas/repl.py
+-rw-r--r--   0        0        0    18506 2023-05-31 19:52:28.422704 archytas-1.0.0/archytas/tool_utils.py
+-rw-r--r--   0        0        0     4586 2023-05-31 19:52:28.422704 archytas-1.0.0/archytas/tools.py
+-rw-r--r--   0        0        0     1251 2023-05-31 19:52:28.422704 archytas-1.0.0/archytas/utils.py
+-rw-r--r--   0        0        0      780 2023-05-31 19:52:28.458704 archytas-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 archytas-1.0.0/PKG-INFO
```

### Comparing `archytas-0.3.0/LICENSE` & `archytas-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-0.3.0/README.md` & `archytas-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `archytas-0.3.0/archytas/agent.py` & `archytas-1.0.0/archytas/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 import os
 import openai
 import logging
-from openai.error import Timeout, APIError, APIConnectionError, RateLimitError, ServiceUnavailableError, InvalidRequestError
+from openai.error import Timeout, APIError, APIConnectionError, RateLimitError, ServiceUnavailableError
 from tenacity import before_sleep_log, retry as tenacity_retry, retry_if_exception_type as retry_if, stop_after_attempt, wait_exponential
-from typing import TypedDict, Literal, Callable, ContextManager
-from frozendict import frozendict
+from typing import Literal, Callable, ContextManager
+from enum import Enum
 
 from rich.spinner import Spinner
 from rich.live import Live
 
 
 logger = logging.getLogger(__name__)
 retry = tenacity_retry(
     reraise=True,
     stop=stop_after_attempt(4),
     wait=wait_exponential(multiplier=1, min=4, max=10),
     retry=retry_if((Timeout, APIError, APIConnectionError, RateLimitError, ServiceUnavailableError)),
     before_sleep=before_sleep_log(logger, logging.WARNING),
 )
 
-#TODO: want these to be enums, but Role.role needs to return a string, not an enum member
-class Role:
+class Role(str, Enum):
     system = 'system'
     assistant = 'assistant'
     user = 'user'
-class Message(TypedDict):
-    role: Literal['system', 'assistant', 'user']
-    content: str
+
+class Message(dict):
+    """Message format for communicating with the OpenAI API."""
+    def __init__(self, role:Role, content:str):
+        super().__init__(role=role.value, content=content)
+
+class ContextMessage(Message):
+    """Simple wrapper around a message that adds an id and optional lifetime."""
+    def __init__(self, role:Role, content:str, id:int, lifetime:int|None=None):
+        super().__init__(role=role, content=content)
+        self.id = id
+        self.lifetime = lifetime
 
 
 def cli_spinner(): 
     return Live(Spinner('dots', speed=2, text="thinking..."), refresh_per_second=30, transient=True)
 class no_spinner:
     def __enter__(self): pass
     def __exit__(self, *args): pass
@@ -46,120 +54,109 @@
             api_key (str, optional): The OpenAI API key to use. Defaults to None. If None, the API key will be read from the OPENAI_API_KEY environment variable.
 
         Raises:
             Exception: If no API key is given.
         """
 
         self.model = model
-        self.system_message: Message = {"role": Role.system, "content": prompt }
-        self.messages = []
+        self.system_message = Message(role=Role.system, content=prompt)
+        self.messages: list[Message] = []
         self.spinner = spinner if spinner is not None else no_spinner
 
-        # keep track of injected context messages and their lifetimes
-        self._context_lifetimes = {}
-        self._all_context_messages = []
+        # use to generate unique ids for context messages
+        self._current_context_id = 0
 
         # check that an api key was given, and set it
         if api_key is None:
             api_key = os.environ.get('OPENAI_API_KEY', None)
         if not api_key:
             raise Exception("No OpenAI API key given. Please set the OPENAI_API_KEY environment variable or pass the api_key argument to the Agent constructor.")
         openai.api_key = api_key
 
-
-    def add_timed_context(self, context:str, time:int=1) -> None:
-        """
-        Add a context to the agent's conversation.
-        The context will be added to the conversation for a finite number of time steps.
+    def new_context_id(self) -> int:
+        """Generate a new context id."""
+        self._current_context_id += 1
+        return self._current_context_id
+
+    def add_context(self, context:str, *, lifetime:int|None=None) -> int:
+        """
+        Inject a context message to the agent's conversation.
+
+        Useful for providing the agent with information relevant to the current conversation, e.g. tool state, environment info, etc.
+        If a lifetime is specified, the context message will automatically be deleted from the chat history after that many steps.
+        A context message can be deleted manually by calling clear_context() with the id of the context message.
 
         Args:
             context (str): The context to add to the agent's conversation.
-            time (int, optional): The number of time steps the context will live for. Defaults to 1 (i.e. it gets deleted as soon as the LLM sees it once).
+            lifetime (int, optional): The number of time steps the context will live for. Defaults to None (i.e. it will never be removed).
+
+        Returns:
+            int: The id of the context message.
         """
-        context_message = frozendict({"role": Role.system, "content": context})
+        context_message = ContextMessage(role=Role.system, content=context, id=self.new_context_id(), lifetime=lifetime)
         self.messages.append(context_message)
-        self._context_lifetimes[context_message] = time
-        self._all_context_messages.append(context_message)
-
+        return context_message.id
 
     def update_timed_context(self) -> None:
         """
         Update the lifetimes of all timed contexts, and remove any that have expired.
         This should be called after every LLM response.
         """
-        # Update context lifetimes and remove expired contexts
-        for context_message in list(self._context_lifetimes.keys()):
-            self._context_lifetimes[context_message] -= 1
-            if self._context_lifetimes[context_message] <= 0:
-                self.messages.remove(context_message)
-                self._all_context_messages.remove(context_message)
-                del self._context_lifetimes[context_message]
-
-    
-    def add_permanent_context(self, context:str) -> None:
-        """
-        Add a context to the agent's conversation.
-        The context will be added to the conversation permanently.
+        #decrement lifetimes of all timed context messages
+        for message in self.messages:
+            if isinstance(message, ContextMessage) and message.lifetime is not None:
+                message.lifetime -= 1
 
-        Args:
-            context (str): The context to add to the agent's conversation.
-        """
-        context_message = {"role": Role.system, "content": context}
-        self.messages.append(context_message)
-        self._all_context_messages.append(context_message)
+        #remove expired context messages
+        new_messages = []
+        for message in self.messages:
+            if isinstance(message, ContextMessage) and message.lifetime == 0:
+                continue
+            new_messages.append(message)
+        self.messages = new_messages
 
 
-    def add_managed_context(self, context:str) -> Callable[[], None]:
+    def clear_context(self, id:int) -> None:
         """
-        Add a context to the agent's conversation.
-        The context will be added to the conversation for an arbitrary number of time steps.
-        Returns a function that can be called to remove the context from the conversation.
+        Remove a single context message from the agent's conversation.
 
         Args:
-            context (str): The context to add to the agent's conversation.
-
-        Returns:
-            Callable[[], None]: A function that can be called to remove the context from the conversation.
+            id (int): The id of the context message to remove.
         """
-        context_message = {"role": Role.system, "content": context}
-        self.messages.append(context_message)
-        self._all_context_messages.append(context_message)
-
-        def remove_context():
-            self.messages.remove(context_message)
-            self._all_context_messages.remove(context_message)
+        new_messages = []
+        for message in self.messages:
+            if isinstance(message, ContextMessage) and message.id == id:
+                continue
+            new_messages.append(message)
+        self.messages = new_messages
 
-        return remove_context
 
     def clear_all_context(self) -> None:
-        """Remove all contexts from the agent's conversation."""
-        for context_message in self._all_context_messages:
-            self.messages.remove(context_message)
-        self._all_context_messages = []
-        self._context_lifetimes = {}
+        """Remove all context messages from the agent's conversation."""
+        self.messages = [message for message in self.messages if not isinstance(message, ContextMessage)]
     
     def query(self, message:str) -> str:
         """Send a user query to the agent. Returns the agent's response"""
-        self.messages.append({"role": Role.user, "content": message})
+        self.messages.append(Message(role=Role.user, content=message))
         return self.execute()
     
     def observe(self, observation:str) -> str:
         """Send a system/tool observation to the agent. Returns the agent's response"""
-        self.messages.append({"role": Role.system, "content": observation})
+        self.messages.append(Message(role=Role.system, content=observation))
         return self.execute()
     
     def error(self, error:str, drop_error:bool=True) -> str:
         """
         Send an error message to the agent. Returns the agent's response.
         
         Args:
             error (str): The error message to send to the agent.
             drop_error (bool, optional): If True, the error message and LLMs bad input will be dropped from the chat history. Defaults to `True`.
         """
-        self.messages.append({"role": Role.system, "content": f'ERROR: {error}'})
+        self.messages.append(Message(role=Role.system, content=f'ERROR: {error}'))
         result = self.execute()
 
         # Drop error + LLM's bad input from chat history
         if drop_error:
             del self.messages[-3:-1]
 
         return result
@@ -171,15 +168,15 @@
                 model=self.model, 
                 messages=[self.system_message] + self.messages,
                 temperature=0,
             )
         
         # grab the response and add it to the chat history
         result = completion.choices[0].message.content
-        self.messages.append({"role": Role.assistant, "content": result})
+        self.messages.append(Message(role=Role.assistant, content=result))
 
         # remove any timed contexts that have expired
         self.update_timed_context()
 
         return result
 
     @retry
@@ -195,14 +192,14 @@
 
         Returns:
             str: The agent's response to the user query.
         """
         with self.spinner():
             completion = openai.ChatCompletion.create(
                 model=self.model, 
-                messages=[{"role": Role.system, "content": prompt }, {"role": Role.user, "content": query}],
+                messages=[Message(role=Role.system, content=prompt), Message(role=Role.user, content=query)],
                 temperature=0,
             )
 
         # return the agent's response
         result = completion.choices[0].message.content
         return result
```

### Comparing `archytas-0.3.0/archytas/demo_tools.py` & `archytas-1.0.0/archytas/demo_tools.py`

 * *Files identical despite different names*

### Comparing `archytas-0.3.0/archytas/prompt.py` & `archytas-1.0.0/archytas/prompt.py`

 * *Files identical despite different names*

### Comparing `archytas-0.3.0/archytas/python.py` & `archytas-1.0.0/archytas/python.py`

 * *Files identical despite different names*

### Comparing `archytas-0.3.0/archytas/react.py` & `archytas-1.0.0/archytas/react.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 logger = logging.Logger('archytas')
 
 class FailedTaskError(Exception): ...
 
 
 class LoopController:
     PROCEED = 0
-    STOP = 1
-    ERROR = 2
+    STOP_SUCCESS = 1
+    STOP_FATAL = 2
 
-    state: int|None
+    state: int
 
     def __init__(self) -> None:
         self.reset()
 
     def set_state(self, new_value):
         self.state = new_value
 
@@ -131,17 +131,17 @@
                 tool_output = tool_fn.run(tool_input, tool_context=tool_context)
             except Exception as e:
                 action_str = self.error(f"error running tool \"{tool_name}\": {e}")
 
                 continue
 
             # Check loop controller to see if we need to stop or error
-            if controller.state == LoopController.STOP:
+            if controller.state == LoopController.STOP_SUCCESS:
                 return tool_output
-            if controller.state == LoopController.ERROR:
+            if controller.state == LoopController.STOP_FATAL:
                 raise FailedTaskError(tool_output)
 
             # have the agent observe the result, and get the next action
             if self.verbose:
                 print(f"observation: {tool_output}\n")
             action_str = self.observe(tool_output)
```

### Comparing `archytas-0.3.0/archytas/repl.py` & `archytas-1.0.0/archytas/repl.py`

 * *Files identical despite different names*

### Comparing `archytas-0.3.0/archytas/tool_utils.py` & `archytas-1.0.0/archytas/tool_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -206,45 +206,60 @@
     """checks if a function is part of a class, or a standalone function"""
     assert inspect.isfunction(func), f"is_class_method can only be used on functions. Got {func}"
     return func.__qualname__ != func.__name__
 
 
 def is_tool(obj:Callable|type) -> bool:
     """checks if an object is a tool function, tool method, tool class, or an instance of a class tool"""
-    return hasattr(obj, '_is_function_tool') or hasattr(obj, '_is_method_tool') or hasattr(obj, '_is_class_tool') or hasattr(obj, '_is_class_tool_instance')
-        
+    return is_function_tool(obj) or is_method_tool(obj) or is_class_tool(obj) or is_class_tool_instance(obj)
+
+def is_function_tool(obj:Callable) -> bool:
+    """checks if an object is a tool function"""
+    return inspect.isfunction(obj) and hasattr(obj, '_is_function_tool')
+
+def is_method_tool(obj:Callable) -> bool:
+    """checks if an object is a tool method"""
+    return inspect.ismethod(obj) and hasattr(obj, '_is_method_tool')
+
+def is_class_tool(obj:type) -> bool:
+    """checks if an object is a tool class"""
+    return inspect.isclass(obj) and hasattr(obj, '_is_class_tool')
+
+def is_class_tool_instance(obj:type) -> bool:
+    """checks if an object is an instance of a tool class"""
+    return hasattr(obj, '_is_class_tool_instance')
 
 def get_tool_name(obj:Callable|type) -> str:
     """Get the name of the tool, either from the @tool _name field, or the __name__ attribute"""
     assert is_tool(obj), f"get_tool_name can only be used on decorated @tools. Got {obj}"
     return getattr(obj, '_name')
 
 
 def get_tool_names(obj:Callable|type) -> list[str]:
     """
     Get the tool name, or all method names if tool is a class tool
     """
     assert is_tool(obj), f"get_tool_name can only be used on decorated @tools. Got {obj}"
     
-    if hasattr(obj, '_is_class_tool') or hasattr(obj, '_is_class_tool_instance'):
+    if is_class_tool(obj) or is_class_tool_instance(obj):
         cls_name = get_tool_name(obj)
 
         #construct names as cls_name.method_name
         names = [f"{cls_name}.{get_tool_name(method)}" for method in obj._tool_methods]
 
         return names
     
     #otherwise, just return the name of the tool
     return [get_tool_name(obj)]
 
 
 def get_tool_prompt_description(obj:Callable|type|Any):
-    if hasattr(obj, '_is_class_tool') or hasattr(obj, '_is_class_tool_instance'):
+    if is_class_tool(obj) or is_class_tool_instance(obj):
         return get_tool_class_prompt_description(obj)
-    if hasattr(obj, '_is_function_tool') or hasattr(obj, '_is_method_tool'):
+    if is_function_tool(obj) or is_method_tool(obj):
         return get_tool_func_prompt_description(obj)
 
     raise TypeError(f"get_tool_prompt_description can only be used on @tools. Got {obj}")
 
 
 def get_tool_func_prompt_description(func:Callable):
     assert is_tool(func), f"Function {func.__name__} does not have the @tool decorator attached"
@@ -318,15 +333,15 @@
 
     Args:
         cls (type|Any): The class tool to get the description for, or an instance of a class tool
     
     Returns:
         str: The prompt description for the class tool
     """
-    assert hasattr(cls, '_is_class_tool') or hasattr(cls, '_is_class_tool_instance'), f"class or instance {cls} does not have the @tool decorator attached"
+    assert is_class_tool(cls) or is_class_tool_instance(cls), f"class or instance {cls} does not have the @tool decorator attached"
 
 
     chunks = []
     tab = "    "
 
     ############### NAME/DESCRIPTION ###############
     chunks.append(f"{cls._name} (class):\n")
@@ -428,29 +443,29 @@
     #TODO: extract methods from any class tools
     tool_dict = {}
     for tool in tools:
         assert is_tool(tool), f"make_tool_dict can only be used on wrapped @tools/@toolsets. Got {tool}"
         name = getattr(tool, '_name')
         
         
-        if hasattr(tool, '_is_function_tool'):
+        if is_function_tool(tool):
             if name in tool_dict:
                 raise ValueError(f"Tool name '{name}' is already in use")
             tool_dict[name] = tool
             continue
         
-        if hasattr(tool, '_is_method_tool'):
+        if is_method_tool(tools):
             #TODO: not sure if methods should be allowed since they need usually need a class instance...
             raise NotImplementedError("Free-floating tool methods are not yet supported")
             pdb.set_trace()
         
 
         # collect methods from @toolset. handle if instance of class or class itself
-        assert hasattr(tool, '_is_class_tool'), f"Tool {tool} is not a function, method, or class tool"
-        if hasattr(tool, '_is_class_tool_instance'):
+        assert is_class_tool(tool) or is_class_tool_instance(tool), f"Tool {tool} is not a function, method, or class tool"
+        if is_class_tool_instance(tool):
             instance = tool
         else:
             instance = tool()
 
         # add each method to the tool dictionary under the name 'class_name.method_name'
         methods = inspect.getmembers(instance, predicate=inspect.ismethod)
         for _, method in methods:
```

### Comparing `archytas-0.3.0/archytas/tools.py` & `archytas-1.0.0/archytas/tools.py`

 * *Files identical despite different names*

### Comparing `archytas-0.3.0/archytas/utils.py` & `archytas-1.0.0/archytas/utils.py`

 * *Files identical despite different names*

### Comparing `archytas-0.3.0/pyproject.toml` & `archytas-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "0.3.0"
+version = "1.0.0"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
```

### Comparing `archytas-0.3.0/PKG-INFO` & `archytas-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 0.3.0
+Version: 1.0.0
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

