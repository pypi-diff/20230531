# Comparing `tmp/gptw-0.4.1.tar.gz` & `tmp/gptw-0.4.2.tar.gz`

## Comparing `gptw-0.4.1.tar` & `gptw-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.4.1/gptw/__init__.py
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 gptw-0.4.1/gptw/gptw.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 gptw-0.4.1/gptw/prompts.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.4.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.4.1/LICENSE
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 gptw-0.4.1/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 gptw-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 gptw-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.4.2/gptw/__init__.py
+-rw-r--r--   0        0        0     6748 2020-02-02 00:00:00.000000 gptw-0.4.2/gptw/gptw.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 gptw-0.4.2/gptw/prompts.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.4.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 gptw-0.4.2/README.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 gptw-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 gptw-0.4.2/PKG-INFO
```

### Comparing `gptw-0.4.1/gptw/gptw.py` & `gptw-0.4.2/gptw/gptw.py`

 * *Files 12% similar despite different names*

```diff
@@ -159,27 +159,40 @@
     )
     response = ""
     for data in chatbot.ask(text):
         response = data["message"]
     return response
 
 
-def ask_azure(token, endpoint, depname, text):
+def ask_azure_multi_pass(token, endpoint, depname, text):
+    msgs = [{"role": "user", "content": text}]
+    for _ in range(5):
+        resp = ask_azure(token, endpoint, depname, msgs)
+        msgs.append({"role": "assistant", "content": resp})
+        msgs.append({"role": "user", "content": "a better one"})
+        print(resp)
+        print("")
+    return ""
+
+
+def ask_azure(token, endpoint, depname, msgs):
     import openai
 
-    logging.debug(f"!!!ask:{text}")
+    logging.debug(f"!!!ask:{msgs}")
     openai.api_key = token
     openai.api_base = endpoint
     openai.api_type = "azure"
     openai.api_version = "2023-05-15"
     completion = openai.ChatCompletion.create(
         engine=depname,
-        messages=[{"role": "user", "content": text}],
+        messages=msgs,
         temperature=0.5,
     )
+    resp = str(completion.choices[0].message.content).strip()
+    logging.debug(f"!!!resp:{resp}")
     return str(completion.choices[0].message.content).strip()
 
 
 def list_commands(prompts):
     print(f'{"cmd":<{3}} | {"meaning":<{30}} | {"example"}')
     for pmt in prompts:
         print(
@@ -238,8 +251,8 @@
         model = get_config("gpt-web-model")
         print(ask_gpt_web(token, proxy, model, msg))
     if get_config("provider") == "azure":
         logging.debug("use azure")
         token = get_config("azure-token")
         endpoint = get_config("azure-endpoint")
         depname = get_config("azure-depname")
-        print(ask_azure(token, endpoint, depname, msg))
+        print(ask_azure_multi_pass(token, endpoint, depname, msg))
```

### Comparing `gptw-0.4.1/gptw/prompts.json` & `gptw-0.4.2/gptw/prompts.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'cmds'": "{'e': {'prompt': 'Please rephrase the text delimited by triple backticks into "*

 * *           'natural-sounding English, adhering to native speaker conventions. Limit your response '*

 * *           "to the translation only.'}}"}*

```diff
@@ -19,15 +19,15 @@
             "_comment": "Dictionary",
             "example": "ww dic dictionary",
             "prompt": "Please provide the definitions of the following English words, including both English and Chinese explanations, an example sentence in English, and the correct pronunciation. Please also correct any spelling errors in the words. Please refrain from providing any additional output beyond the definitions."
         },
         "e": {
             "_comment": "Translate into English",
             "example": "ww e \u4f60\u597d",
-            "prompt": "Please rephrase the following text into natural-sounding English, adhering to native speaker conventions. Limit your response to the translation only."
+            "prompt": "Please rephrase the text delimited by triple backticks into natural-sounding English, adhering to native speaker conventions. Limit your response to the translation only."
         },
         "p": {
             "_comment": "Polish sentence",
             "example": "ww p hwo are you",
             "prompt": "Please review the sentence below for grammar, tense, word choice, and phrasing issues. Edit the sentence to make it sound natural and align with native speaker conventions. Provide a brief explanation for any changes made."
         },
         "r": {
```

### Comparing `gptw-0.4.1/.gitignore` & `gptw-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gptw-0.4.1/LICENSE` & `gptw-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gptw-0.4.1/README.md` & `gptw-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `gptw-0.4.1/pyproject.toml` & `gptw-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gptw-0.4.1/PKG-INFO` & `gptw-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptw
-Version: 0.4.1
+Version: 0.4.2
 Summary: The ChatGPT command-line wrapper simplifies the execution of predetermined tasks through ChatGPT.
 Author: Xin Yang
 Author-email: xinydev@gmail.com
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: ChatGPT,Command Line,English Polishing,English Translation
 Classifier: Development Status :: 3 - Alpha
```

