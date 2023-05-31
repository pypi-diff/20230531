# Comparing `tmp/llmspec-0.3.6.tar.gz` & `tmp/llmspec-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmspec-0.3.6.tar", last modified: Tue May 30 03:30:26 2023, max compression
+gzip compressed data, was "llmspec-0.3.7.tar", last modified: Wed May 31 08:16:23 2023, max compression
```

## Comparing `llmspec-0.3.6.tar` & `llmspec-0.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11098 2023-05-30 03:30:13.033159 llmspec-0.3.6/LICENSE
--rw-r--r--   0        0        0       33 2023-05-30 03:30:13.033159 llmspec-0.3.6/README.md
--rw-r--r--   0        0        0      659 2023-05-30 03:30:13.033159 llmspec-0.3.6/llmspec/__init__.py
--rw-r--r--   0        0        0     9640 2023-05-30 03:30:13.033159 llmspec-0.3.6/llmspec/llmspec.py
--rw-r--r--   0        0        0      215 2023-05-30 03:30:13.033159 llmspec-0.3.6/llmspec/mixins.py
--rw-r--r--   0        0        0     1130 2023-05-30 03:30:26.501390 llmspec-0.3.6/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-30 03:30:13.033159 llmspec-0.3.6/tests/dummy_test.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11098 2023-05-31 08:16:07.065581 llmspec-0.3.7/LICENSE
+-rw-r--r--   0        0        0       33 2023-05-31 08:16:07.065581 llmspec-0.3.7/README.md
+-rw-r--r--   0        0        0      659 2023-05-31 08:16:07.065581 llmspec-0.3.7/llmspec/__init__.py
+-rw-r--r--   0        0        0     9917 2023-05-31 08:16:07.065581 llmspec-0.3.7/llmspec/llmspec.py
+-rw-r--r--   0        0        0      215 2023-05-31 08:16:07.065581 llmspec-0.3.7/llmspec/mixins.py
+-rw-r--r--   0        0        0     1130 2023-05-31 08:16:23.211062 llmspec-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-31 08:16:07.065581 llmspec-0.3.7/tests/dummy_test.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.7/PKG-INFO
```

### Comparing `llmspec-0.3.6/LICENSE` & `llmspec-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.6/llmspec/__init__.py` & `llmspec-0.3.7/llmspec/__init__.py`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.6/llmspec/llmspec.py` & `llmspec-0.3.7/llmspec/llmspec.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     assistant_token: str = ""
     system_token: str = ""
     sep_token: str = ""
     append_assistant_token: bool = False
 
     # model class name in `transformers`
     transformer_model_cls: str = "AutoModelForCausalLM"
+    tokenizer_cls: str = "AutoTokenizer"
 
     # model structure
     is_encoder_decoder: bool = True
 
     def get_conversation_prompt(self, messages: List[ChatMessage]) -> str:
         """Get the prompt for a conversation using the specific tokens of the model."""
         formatted_messages = []
@@ -105,15 +106,23 @@
     user_token="USER: ",
     assistant_token="ASSISTANT: ",
     system_token="",
     sep_token="\n",
     append_assistant_token=True,
     is_encoder_decoder=False,
 )
-FastChatT5 = Vicuna
+FastChatT5 = LanguageModelInfo(
+    user_token="USER: ",
+    assistant_token="ASSISTANT: ",
+    system_token="",
+    sep_token="\n### ",
+    append_assistant_token=True,
+    transformer_model_cls="AutoModelForSeq2SeqLM",
+    tokenizer_cls="T5Tokenizer",
+)
 Unknown = LanguageModelInfo()
 
 
 class CompletionRequest(msgspec.Struct, JSONSerializableMixin, kw_only=True):
     suffix: Optional[str] = None
     max_tokens: int = 16
     temperature: float = 1.0
```

### Comparing `llmspec-0.3.6/pyproject.toml` & `llmspec-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "msgspec>=0.15.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.6"
+version = "0.3.7"
 
 [project.license]
 text = "Apache-2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
```

