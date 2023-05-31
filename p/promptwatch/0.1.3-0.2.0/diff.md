# Comparing `tmp/promptwatch-0.1.3.tar.gz` & `tmp/promptwatch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.1.3.tar", last modified: Wed May 24 14:02:38 2023, max compression
+gzip compressed data, was "promptwatch-0.2.0.tar", last modified: Wed May 31 21:52:59 2023, max compression
```

## Comparing `promptwatch-0.1.3.tar` & `promptwatch-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 14:02:38.310160 promptwatch-0.1.3/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-24 14:02:38.308607 promptwatch-0.1.3/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.1.3/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.1.3/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-24 14:02:38.310253 promptwatch-0.1.3/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-19 10:25:10.000000 promptwatch-0.1.3/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 14:02:38.286980 promptwatch-0.1.3/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 14:02:38.293718 promptwatch-0.1.3/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      332 2023-05-24 14:02:26.000000 promptwatch-0.1.3/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11928 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5392 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.1.3/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.1.3/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 14:02:38.301274 promptwatch-0.1.3/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      153 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11067 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    25666 2023-05-23 20:18:59.000000 promptwatch-0.1.3/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17876 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 14:02:38.308117 promptwatch-0.1.3/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.1.3/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13583 2023-05-19 10:25:10.000000 promptwatch-0.1.3/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1105 2023-05-24 13:30:08.000000 promptwatch-0.1.3/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-24 14:02:38.296713 promptwatch-0.1.3/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-24 14:02:38.000000 promptwatch-0.1.3/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-05-24 14:02:38.000000 promptwatch-0.1.3/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-24 14:02:38.000000 promptwatch-0.1.3/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.1.3/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-05-24 14:02:38.000000 promptwatch-0.1.3/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-24 14:02:38.000000 promptwatch-0.1.3/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.873867 promptwatch-0.2.0/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-31 21:52:59.873675 promptwatch-0.2.0/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.0/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.0/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-31 21:52:59.873924 promptwatch-0.2.0/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.0/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.863236 promptwatch-0.2.0/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.866986 promptwatch-0.2.0/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-05-31 21:34:10.000000 promptwatch-0.2.0/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.0/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.0/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.0/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5459 2023-05-30 20:36:31.000000 promptwatch-0.2.0/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.0/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.870533 promptwatch-0.2.0/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.0/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.0/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    29625 2023-05-31 09:25:01.000000 promptwatch-0.2.0/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.0/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17902 2023-05-31 18:53:06.000000 promptwatch-0.2.0/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.872453 promptwatch-0.2.0/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.0/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.0/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.0/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.0/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1105 2023-05-24 13:30:08.000000 promptwatch-0.2.0/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.869110 promptwatch-0.2.0/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.0/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.1.3/PKG-INFO` & `promptwatch-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.1.3
+Version: 0.2.0
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.1.3/README.md` & `promptwatch-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.3/setup.py` & `promptwatch-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.3/src/promptwatch/client.py` & `promptwatch-0.2.0/src/promptwatch/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .data_model import Session, ActivityBase, ActivityList
 import requests
-from typing import List, Optional,Tuple
+from typing import Dict, List, Optional,Tuple
 import os
 import logging
 from datetime import datetime
 from .unit_tests.schema import TestCase,  PromptUnitTestRun, TestCaseResult, TestCaseResultsList
 from pydantic.json import pydantic_encoder
 
 
@@ -64,25 +64,39 @@
     
         if response.status_code==200:
             return Session(**response.json())
         else:
             raise Exception(f"Error response from server: {response.status_code}: {response.text}")
         
 
-    def get_from_cache(self, cache_namespace_key:str,  query_embedding:List[float], min_similarity:float)-> Tuple[str,float]:
-        response = self._request("POST", f"/prompt-cache/{cache_namespace_key}/get", json_dict={"embedding":query_embedding},params={ "min_similarity":min_similarity})
+    def get_from_cache(self, cache_namespace_key:str,  query_embedding:List[float], min_similarity:float,  prompt_template_identity:str=None, prompt_input_values:Dict[str,str]=None)-> Tuple[str,float]:
+        response = self._request("POST", f"/prompt-cache/{cache_namespace_key}/get", 
+                                 json_dict={
+                                     "embedding":query_embedding,
+                                     "prompt_template_identity":prompt_template_identity,
+                                     "prompt_input_values":prompt_input_values,
+                                     },
+                                 params={ "min_similarity":min_similarity})
         if response:
             data = response.json()
             if data:
                 result = data.get("result")
                 similarity = data.get("similarity")
                 return result, similarity
         
-    def add_into_cache(self, cache_namespace_key:str, id:str, embedding:List[float], result:str):
-       response = self._request("POST", f"/prompt-cache/{cache_namespace_key}", json_dict={"embedding":embedding, "id":id,"result":result})
+    def add_into_cache(self, cache_namespace_key:str, id:str, embedding:List[float], result:str,  prompt_template_identity:str=None, prompt_input_values:Dict[str,str]=None):
+       response = self._request("POST", f"/prompt-cache/{cache_namespace_key}", 
+                                json_dict={
+                                     "embedding":embedding,
+                                     "prompt_template_identity":prompt_template_identity,
+                                     "prompt_input_values":prompt_input_values,
+                                     "id":id,
+                                     "result":result
+                                     }
+                                     )
     
     def clear_cache(self, cache_namespace_key:str, until:Optional[datetime]=None):
        response = self._request("POST", f"/prompt-cache/{cache_namespace_key}/clear", params={ "until":until})
     
 
     
     def get_test_cases(self, for_tracking_project=None, for_template_name=None, skip=0, limit=1000)->TestCase:
```

### Comparing `promptwatch-0.1.3/src/promptwatch/data_model.py` & `promptwatch-0.2.0/src/promptwatch/data_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     text:str
 
 class ChatMessagePromptTemplate(PromptTemplateDescription):
     role:Optional[str]
     
     
 class NamedPromptTemplateDescription(PromptTemplateDescription):
-    template_name:Optional[str]
+    template_name:str
     template_version:Optional[str]
 
     
 
 LlmPrompt.update_forward_refs()
 PromptTemplateDescription.update_forward_refs()
 ChatMessagePromptTemplate.update_forward_refs()
```

### Comparing `promptwatch-0.1.3/src/promptwatch/decorators.py` & `promptwatch-0.2.0/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.3/src/promptwatch/langchain/caching.py` & `promptwatch-0.2.0/src/promptwatch/langchain/caching.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from langchain.prompts.chat import ChatPromptValue
 from langchain.llms.base import LLM, BaseLLM
 from langchain.chat_models.base import BaseChatModel
 from langchain.embeddings.base import Embeddings
 from langchain.schema import AIMessage, BaseMessage, ChatGeneration, ChatResult
 from langchain.schema import PromptValue
 from langchain.schema import LLMResult
+
+from ..data_model import LlmPrompt, NamedPromptTemplateDescription
 from ..decorators import FORMATTED_PROMPT_CONTEXT_KEY
 from typing import List
 from .. import PromptWatch
 from langchain.schema import Generation
 from typing import Any, Optional, Union
 import datetime
 from langchain.llms.base import LLM
@@ -45,22 +47,28 @@
         return "cached-llm"
     
     
     
     def _get_from_cache(self,prompt, stop: Optional[List[str]] = None):
         promptwatch_context = PromptWatch.get_active_instance()
 
-        
         if promptwatch_context:
-            
+
+            if isinstance(promptwatch_context.current_activity,LlmPrompt) and isinstance(promptwatch_context.current_activity.prompt_template, NamedPromptTemplateDescription):
+                prompt_input_values = promptwatch_context.current_activity.prompt_input_values
+                named_prompt_template = promptwatch_context.current_activity.prompt_template
+            else:
+                prompt_input_values=None
+                named_prompt_template=None
+
             embed_func = self.cache_embeddings.embed_query if self.cache_embeddings else None
             cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, embed_func, self.token_limit, self.similarity_limit)
             
             cache_prompt_req = f"Stop:[{','.join(stop)}]\n:{prompt}" if stop else prompt
-            cached_res = cache.get(cache_prompt_req)
+            cached_res = cache.get(cache_prompt_req, prompt_template=named_prompt_template, prompt_input_values=prompt_input_values)
            
            
             return  cached_res, lambda cached_res,result : cache.add(cached_res, result) if cached_res is not None else None
         else:
             return None, None
         
     def _call(self, prompt:str, stop: Optional[List[str]] = None) -> str:
@@ -112,44 +120,56 @@
 class CachedChatLLM(BaseChatModel):
     
     inner_llm:Any
     cache_namespace_key:Optional[str]
     cache_embeddings:Optional[Embeddings]
     token_limit:Optional[int]
     similarity_limit:Optional[float]
-    def __init__(self, inner_llm:BaseLLM, cache_namespace_key:str=None, cache_embeddings:Embeddings = None, token_limit:int=None, similarity_limit:float=0.97) -> None:
+    def __init__(self, inner_llm:BaseLLM, cache_namespace_key:str=None, cache_embeddings:Embeddings = None, token_limit:int=None, similarity_limit:float=0.95) -> None:
         
         super().__init__(inner_llm=inner_llm, cache_namespace_key=cache_namespace_key, cache_embeddings=cache_embeddings, token_limit=token_limit, similarity_limit=similarity_limit)
        
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "cached-chat-llm"
     
     def generate_prompt(
         self, prompts: List[PromptValue], stop: Optional[List[str]] = None, **kwargs
     ) -> LLMResult:
         # overriding generate_prompt because we want to pass down the prompts to the inner llm
         promptwatch_context = PromptWatch.get_active_instance()
         if promptwatch_context and len(prompts)==1 :
-            promptwatch_context.add_context(FORMATTED_PROMPT_CONTEXT_KEY, prompts[0])
+            promptwatch_context.add_context(FORMATTED_PROMPT_CONTEXT_KEY, prompts[0]) # .to_messages() or not .to_messages() ... that is the question
         return super().generate_prompt(prompts, stop=stop)
         
     
     def _get_from_cache(self, messages: Union[str, List[BaseMessage]], stop: Optional[List[str]] = None):
         promptwatch_context = PromptWatch.get_active_instance()
         prompt = ChatPromptValue(messages=messages).to_string()
         
         if promptwatch_context:
             
             embed_func = self.cache_embeddings.embed_query if self.cache_embeddings else None
             cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, embed_func, self.token_limit, self.similarity_limit)
             
+            
+            if isinstance(promptwatch_context.current_activity,LlmPrompt) \
+                and isinstance(promptwatch_context.current_activity.prompt_template, NamedPromptTemplateDescription) \
+                and promptwatch_context.current_activity.prompt_template.template_name:
+                    
+                named_prompt_template = promptwatch_context.current_activity.prompt_template
+                prompt_input_values = promptwatch_context.current_activity.prompt_input_values
+            else:
+                prompt_input_values=None
+                named_prompt_template=None
+
+
             cache_prompt_req = f"Stop:[{','.join(stop)}]\n:{prompt}" if stop else prompt
-            cached_res = cache.get(cache_prompt_req)
+            cached_res = cache.get(cache_prompt_req,prompt_template=named_prompt_template, prompt_input_values=prompt_input_values )
            
            
             return  cached_res, lambda cached_res,result : cache.add(cached_res, result) 
         else:
             return None, None
         
     def _call(self, messages: List[BaseMessage], stop: Optional[List[str]] = None, **kwargs) -> str:
```

### Comparing `promptwatch-0.1.3/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.2.0/src/promptwatch/langchain/langchain_support.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """A Tracer implementation that records to LangChain endpoint."""
 from __future__ import annotations
+from ast import Tuple
 import re
 from abc import ABC
+import types
 from typing import Any, Dict, Optional, Union
 import datetime
 from langchain.prompts.base import BasePromptTemplate
 from langchain.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate, AIMessagePromptTemplate, SystemMessagePromptTemplate, MessagesPlaceholder, BaseMessagePromptTemplate
 from langchain.llms.base import LLM
 from langchain.chat_models.base import BaseChatModel
 from langchain.chains import LLMChain
 from langchain.embeddings.base import Embeddings
 from langchain.schema import HumanMessage, ChatMessage as LangChainChatMessage, AIMessage, SystemMessage, BaseMessage
 from langchain.callbacks.base import BaseCallbackHandler
+from langchain.agents import initialize_agent, Tool, Agent, BaseSingleActionAgent
+from langchain.tools.base import BaseTool
+from langchain.chains.base import Chain
 
 from langchain.schema import AgentAction, AgentFinish, LLMResult,  Document
 from ..client import Client
 from ..data_model import NamedPromptTemplateDescription,PromptTemplateDescription, LlmPrompt, ParallelPrompt, ChainSequence, ChatMessage, Answer, Action, Question, RetrievedDocuments, DocumentSnippet, ChatMessagePromptTemplate
 from ..utils import find_the_caller_in_the_stack, is_primitive_type, wrap_a_method
 from .caching import CachedLLM, CachedChatLLM
 from ..decorators import FORMATTED_PROMPT_CONTEXT_KEY, TEMPLATE_NAME_CONTEXT_KEY, LLM_CHAIN_CONTEXT_KEY
@@ -406,37 +411,37 @@
         
     
 
         
 
 
 
-def register_prompt_template(template_name:str,prompt_template, version:Optional[str]=None):
+def register_prompt_template(template_name:str,prompt_template, version:Optional[str]="1.0"):
         """
         Register prompt template into context for more detailed tracking, versioning and evaluation
 
 
         Args:
             template_name (str): arbitrary unique template name (should not contain white spaces, max 126 chars)
             prompt_template (Union[BasePromptTemplate,BaseChatPromptTemplate]): Any langchain prompt template
             version (Optional[str], optional): Optional - (major) (SemVer) version of the template. Minor changes are tracked incrementally automatically. Useful if you are going to make a major change in the template, and you with to dive the version a distinct version number.
 
         ## Examples:
         
         ### Registering regular prompt (completion)
 
         ```
-        from promptwatch import PromptWatch
+        from promptwatch import PromptWatch, register_prompt_template
         from langchain import OpenAI, LLMChain, PromptTemplate
 
         prompt_template = PromptTemplate.from_template("Finish this sentence {input}")
         my_chain = LLMChain(llm=OpenAI(), prompt=prompt_template)
+        register_prompt_template("simple_completion_template",prompt_template, version="1.0")
 
-        with PromptWatch() as pw:
-            pw.register_prompt_template("simple_completion_template",prompt_template, version="1.0")
+        with PromptWatch():    
             my_chain("The quick brown fox jumped over")
         ```
 
         ### Registering chat messages template (completion)
         ...
 
         """
@@ -453,20 +458,110 @@
         decorator_func = format_prompt_decorator(template_name)
         
         
         wrap_a_method(prompt_template, "format_prompt", decorator_func)
         # we need to mark the prompt template somehow... keeping just the reference doesn't work since pydantic is creating copy of it when passed to the constructor
         # that is why we add special field __template_name__ into it... also skipping setattr() since that might be blocked by pydantic as well (depending on the configuration)
         prompt_template.__dict__["__template_name__"]=template_name
+        prompt_template.__dict__["__template_version__"]=version
 
         PromptWatch.prompt_template_register_cache[template_name] = converted_template
         return prompt_template
 
 
 
+
+
+
+def find_templates_recursive(root_chain: Union[Chain,Tool, Agent], template_name_prefix:str, print_code=True, _ignore_chains:List[Chain]=[])-> Tuple[str,BasePromptTemplate]:
+    """This will find all templates in the chain and its subchains, agents, tools recursively. 
+    It return a tuple of (path_to_template, template)
+
+    If print_code==True, it will also print the code to register all templates
+
+
+    Args:
+        root_chain (Union[Chain,Tool, Agent]): _description_
+        template_name_prefix (str): _description_
+        print_code (bool, optional): _description_. Defaults to True.
+        _ignore_chains (List[Chain], optional): _description_. Defaults to [].
+
+
+
+    Yields:
+        Tuple(): _description_
+    """
+
+    is_tool=isinstance(root_chain,BaseTool) 
+    for field_key, field_value in root_chain.__dict__.items():
+        if field_value is None or field_value in _ignore_chains:
+            continue
+        if is_tool and isinstance(field_value, types.MethodType):
+            # tools have a "func" field that is bound to the tool it self
+            if field_value.__self__ in _ignore_chains:
+                continue
+
+            _ignore_chains.append(field_value.__self__)
+            for res_pair in find_templates_recursive(field_value.__self__, f"{template_name_prefix}.{field_key}"):
+                yield res_pair
+        elif isinstance(field_value,Chain):
+              _ignore_chains.append(field_value)
+              for res_pair in find_templates_recursive(field_value, f"{template_name_prefix}.{field_key}"):
+                    yield res_pair
+        elif isinstance(field_value, BaseSingleActionAgent):
+            _ignore_chains.append(field_value)
+            for res_pair in find_templates_recursive(field_value, f"{template_name_prefix}.{field_key}"):
+                yield res_pair
+        elif isinstance(field_value, list):
+            for i,item in enumerate(field_value):
+                
+                if hasattr(item,"name"):
+                    index_key = f"{field_key}.[{item.name}]"
+                else:
+                    index_key = f"{field_key}[{i}]"
+
+                if isinstance(item, BaseTool) or  isinstance(item, Chain):
+                    _ignore_chains.append(item)
+                    for res_pair in find_templates_recursive(item, f"{template_name_prefix}.{index_key}"):
+                        yield res_pair
+        elif isinstance(field_value, BasePromptTemplate):
+            if field_value.__dict__.get("__template_name__") :
+                 continue
+                 raise ValueError(f"PromptTemplate {field_value} has no name")
+            if print_code:
+                print(f"register_prompt_template({template_name_prefix}.{field_key}, '{template_name_prefix}.{field_key}'")
+            yield f"{template_name_prefix}.{field_key}", field_value
+        
+            
+
+def find_and_register_templates_recursive(root_chain: Chain, template_name_prefix:str, ignore_subpaths=[]):
+    paths = []
+    ignore=False
+    for path, template in find_templates_recursive(root_chain, template_name_prefix, print_code=False):
+        for subpath in ignore_subpaths:
+            if subpath in path:
+                ignore=True
+        if ignore:
+            continue
+        register_prompt_template(template_name=path, prompt_template=template)
+        paths.append(path)
+    print(f"Registered {len(paths)} templates: ")
+    print("\n".join(paths))
+    print("WARNING: This method is not fit for production use as it might slow down the startup time.")
+    print("         Please consider using find_and_register_templates_recursive() to generate a code to register all templates instead.")
+
+
+
+
+
+
+
+
+
+
 def convert_chat_messages( msg:Union[BaseMessage, List[BaseMessage]]):
         if isinstance(msg, BaseMessage):
                 if isinstance(msg,HumanMessage):
                     role="user"
                 elif isinstance(msg,LangChainChatMessage):
                     role = msg.role
                 elif isinstance(msg,AIMessage):
@@ -569,8 +664,7 @@
             format=langchain_prompt_template.template_format
     if prompt_template:
         if template_name:
             return NamedPromptTemplateDescription(prompt_template=prompt_template, prompt_input_params=input_params, format=format, template_name=template_name ,template_version=template_version)
         else:
             return PromptTemplateDescription(prompt_template=prompt_template, prompt_input_params=input_params, format=format)
 
-
```

### Comparing `promptwatch-0.1.3/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.2.0/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.3/src/promptwatch/promptwatch_context.py` & `promptwatch-0.2.0/src/promptwatch/promptwatch_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     """
     Singleton metaclass for ensuring only one instance of a class per thread
     """
 
     _thread_local = threading.local()
     _cross_thread_storage = {}
 
-    def __call__(cls, *args, **kwargs):
+    def __call__(cls, *args, **kwargs)->PromptWatch:
         """Call method for the singleton metaclass."""
         if not hasattr(ContextTrackerSingleton._thread_local, "_instance"):
             prompt_watch_context = super(ContextTrackerSingleton, cls).__call__(*args, **kwargs)
             if not prompt_watch_context.session_id:
                 raise Exception("PromptWatch: Session ID was not initialized. Please report this as a bug.")
             ContextTrackerSingleton._cross_thread_storage[prompt_watch_context.session_id] = prompt_watch_context
             ContextTrackerSingleton._thread_local._instance = prompt_watch_context
        
         return ContextTrackerSingleton._thread_local._instance 
         
-    def get_current(session_id:str=None):
+    def get_current(session_id:str=None)->PromptWatch:
         """ return the current instance
         for sync context session_id is not required
         for async context session_id is required, otherwise it the instance wont be found
         """
         if hasattr(ContextTrackerSingleton._thread_local, "_instance"):
             # in thread context ... this will work unless async is used... then we loose track...
             # it is OK for nesting context in single thread...
```

### Comparing `promptwatch-0.1.3/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.2.0/src/promptwatch/unit_tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.3/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.2.0/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.3/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.2.0/src/promptwatch/unit_tests/unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 from datetime import datetime, timezone
 
 
         
 
 class UnitTest:
 
-    def __init__(self, test_name:str, evaluation:EvaluationStrategyBase=DEFAULT_COSINE_SCORE_EVALUATION) -> None:
+    def __init__(self, test_name:str, evaluation:EvaluationStrategyBase=DEFAULT_COSINE_SCORE_EVALUATION, api_key:str=None) -> None:
         """ Initialize new test definition. If called with the same parameters, it will be reused """
         self.test_name=test_name
         self.evaluation_strategy=evaluation
         self._entered=False
         #avoiding circular imports
         
         # it ok to create new instance... PromptWatch is a singleton and if someone want's to initialize extra params, he can wrapping it int  PromptWatch context 
         self.prompt_watch=None 
         self.conditions=None
         self.test_cases_generator=None
         from promptwatch.client import Client
-        self.client=Client()
+        self.client=Client(api_key=api_key)
 
         self.evaluator=None
         
        
             
 
     def for_test_cases(self, examples:List["TestCase"])->"UnitTest":
@@ -121,15 +121,15 @@
     
     def __enter__(self):
         
         self._entered=True
         if not self.test_cases_generator:
             raise Exception("Invalid use. Please define the scope of test by calling one of for_test_cases, for_test_cases_in_file, for_prompt_template or for_project_sessions methods before entering the context")
         
-        self.prompt_watch=PromptWatch(tracking_project=self.conditions.for_tracking_project if self.conditions else None)
+        self.prompt_watch=PromptWatch(tracking_project=self.conditions.for_tracking_project if self.conditions else None, api_key=self.client.api_key)
         self.prompt_watch.__enter__()
         self.prompt_watch.session_id
         self.unit_test_run = PromptUnitTestRun(
             test_name=self.test_name,
             session_id=self.prompt_watch.current_session.id, 
             start_time=datetime.now(tz=timezone.utc), 
             conditions=self.conditions,
```

### Comparing `promptwatch-0.1.3/src/promptwatch/utils.py` & `promptwatch-0.2.0/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.3/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.2.0/src/promptwatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.1.3
+Version: 0.2.0
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.1.3/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.2.0/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

