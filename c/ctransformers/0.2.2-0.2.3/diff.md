# Comparing `tmp/ctransformers-0.2.2.tar.gz` & `tmp/ctransformers-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctransformers-0.2.2.tar", last modified: Sun May 28 12:01:01 2023, max compression
+gzip compressed data, was "ctransformers-0.2.3.tar", last modified: Tue May 30 23:11:24 2023, max compression
```

## Comparing `ctransformers-0.2.2.tar` & `ctransformers-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,59 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-28 12:01:01.937186 ctransformers-0.2.2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18596 2023-05-28 12:01:01.937186 ctransformers-0.2.2/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13696 2023-05-28 11:45:59.000000 ctransformers-0.2.2/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-28 12:01:01.927186 ctransformers-0.2.2/ctransformers/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.2.2/ctransformers/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5866 2023-05-19 19:43:30.000000 ctransformers-0.2.2/ctransformers/hub.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2616 2023-05-21 14:15:12.000000 ctransformers-0.2.2/ctransformers/langchain.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-28 12:01:01.927186 ctransformers-0.2.2/ctransformers/lib/
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-28 12:01:01.927186 ctransformers-0.2.2/ctransformers/lib/avx/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   630272 2023-05-28 11:54:15.000000 ctransformers-0.2.2/ctransformers/lib/avx/ctransformers.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)  1321155 2023-05-28 11:54:15.000000 ctransformers-0.2.2/ctransformers/lib/avx/libctransformers.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   785472 2023-05-28 11:54:15.000000 ctransformers-0.2.2/ctransformers/lib/avx/libctransformers.so
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-28 12:01:01.937186 ctransformers-0.2.2/ctransformers/lib/avx2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   616448 2023-05-28 11:54:15.000000 ctransformers-0.2.2/ctransformers/lib/avx2/ctransformers.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)  1321155 2023-05-28 11:54:15.000000 ctransformers-0.2.2/ctransformers/lib/avx2/libctransformers.dylib
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   789568 2023-05-28 11:54:15.000000 ctransformers-0.2.2/ctransformers/lib/avx2/libctransformers.so
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-28 12:01:01.937186 ctransformers-0.2.2/ctransformers/lib/basic/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   624128 2023-05-28 11:54:15.000000 ctransformers-0.2.2/ctransformers/lib/basic/ctransformers.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)  1321155 2023-05-28 11:54:15.000000 ctransformers-0.2.2/ctransformers/lib/basic/libctransformers.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   752664 2023-05-28 11:54:15.000000 ctransformers-0.2.2/ctransformers/lib/basic/libctransformers.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1033 2023-05-12 14:01:41.000000 ctransformers-0.2.2/ctransformers/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    15408 2023-05-28 11:38:52.000000 ctransformers-0.2.2/ctransformers/llm.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1146 2023-05-27 21:21:35.000000 ctransformers-0.2.2/ctransformers/utils.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-28 12:01:01.927186 ctransformers-0.2.2/ctransformers.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18596 2023-05-28 12:01:01.000000 ctransformers-0.2.2/ctransformers.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      767 2023-05-28 12:01:01.000000 ctransformers-0.2.2/ctransformers.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-28 12:01:01.000000 ctransformers-0.2.2/ctransformers.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-28 12:01:01.000000 ctransformers-0.2.2/ctransformers.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-05-28 12:01:01.000000 ctransformers-0.2.2/ctransformers.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-05-28 12:01:01.000000 ctransformers-0.2.2/ctransformers.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-28 12:01:01.937186 ctransformers-0.2.2/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1451 2023-05-28 11:58:39.000000 ctransformers-0.2.2/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.464320 ctransformers-0.2.3/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       43 2023-05-08 17:08:45.000000 ctransformers-0.2.3/.gitattributes
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.434320 ctransformers-0.2.3/.github/
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.444320 ctransformers-0.2.3/.github/workflows/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1325 2023-05-29 18:06:10.000000 ctransformers-0.2.3/.github/workflows/build.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      981 2023-05-14 22:40:02.000000 ctransformers-0.2.3/.github/workflows/tests.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13506 2023-05-14 12:42:43.000000 ctransformers-0.2.3/.gitignore
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      211 2023-05-29 14:27:39.000000 ctransformers-0.2.3/.gitmodules
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4266 2023-05-30 20:08:54.000000 ctransformers-0.2.3/CMakeLists.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1078 2023-05-08 17:08:55.000000 ctransformers-0.2.3/LICENSE
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18486 2023-05-30 23:11:24.464320 ctransformers-0.2.3/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13658 2023-05-30 23:09:34.000000 ctransformers-0.2.3/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.444320 ctransformers-0.2.3/ctransformers/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.2.3/ctransformers/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5866 2023-05-19 19:43:30.000000 ctransformers-0.2.3/ctransformers/hub.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2616 2023-05-21 14:15:12.000000 ctransformers-0.2.3/ctransformers/langchain.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1251 2023-05-29 21:19:55.000000 ctransformers-0.2.3/ctransformers/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    15833 2023-05-30 15:15:11.000000 ctransformers-0.2.3/ctransformers/llm.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1146 2023-05-27 21:21:35.000000 ctransformers-0.2.3/ctransformers/utils.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.444320 ctransformers-0.2.3/ctransformers.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18486 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      998 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-30 23:11:23.000000 ctransformers-0.2.3/ctransformers.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.444320 ctransformers-0.2.3/models/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4905 2023-05-29 15:42:12.000000 ctransformers-0.2.3/models/common.h
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.454320 ctransformers-0.2.3/models/ggml/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    34896 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/ggml-cuda.cu
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      906 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/ggml-cuda.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   506603 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/ggml.c
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    38058 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/ggml.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13668 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/llama-util.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    96303 2023-05-30 14:35:21.000000 ctransformers-0.2.3/models/ggml/llama.cpp
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    14098 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/llama.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2924 2023-05-30 12:22:12.000000 ctransformers-0.2.3/models/llm.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7218 2023-05-30 12:18:34.000000 ctransformers-0.2.3/models/llm.h
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.464320 ctransformers-0.2.3/models/llms/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21413 2023-05-30 20:22:27.000000 ctransformers-0.2.3/models/llms/dolly.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21973 2023-05-30 20:20:35.000000 ctransformers-0.2.3/models/llms/gpt-neox.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    22306 2023-05-30 20:19:06.000000 ctransformers-0.2.3/models/llms/gpt2.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    19234 2023-05-30 20:17:33.000000 ctransformers-0.2.3/models/llms/gptj.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3324 2023-05-30 13:26:40.000000 ctransformers-0.2.3/models/llms/llama.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18424 2023-05-30 20:16:14.000000 ctransformers-0.2.3/models/llms/mpt.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    24167 2023-05-30 20:13:06.000000 ctransformers-0.2.3/models/llms/starcoder.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      150 2023-05-29 18:34:56.000000 ctransformers-0.2.3/pyproject.toml
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.464320 ctransformers-0.2.3/scripts/
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)      107 2023-05-29 18:06:51.000000 ctransformers-0.2.3/scripts/build.sh
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)     1427 2023-05-30 12:31:41.000000 ctransformers-0.2.3/scripts/docs.py
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)      550 2023-05-30 19:39:09.000000 ctransformers-0.2.3/scripts/release.sh
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)      603 2023-05-29 14:52:08.000000 ctransformers-0.2.3/scripts/sync.sh
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-30 23:11:24.464320 ctransformers-0.2.3/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1801 2023-05-30 23:10:19.000000 ctransformers-0.2.3/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.464320 ctransformers-0.2.3/tests/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 17:05:29.000000 ctransformers-0.2.3/tests/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      285 2023-05-14 17:57:20.000000 ctransformers-0.2.3/tests/conftest.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1678 2023-05-17 19:46:10.000000 ctransformers-0.2.3/tests/test_llm.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      618 2023-05-27 19:08:53.000000 ctransformers-0.2.3/tests/test_model.py
```

### Comparing `ctransformers-0.2.2/PKG-INFO` & `ctransformers-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
         
         Python bindings for the Transformer models implemented in C/C++ using [GGML](https://github.com/ggerganov/ggml) library.
         
         - [Supported Models](#supported-models)
         - [Installation](#installation)
         - [Usage](#usage)
           - [Hugging Face Hub](#hugging-face-hub)
           - [LangChain](#langchain)
+          - [GPU](#gpu)
         - [Documentation](#documentation)
         - [License](#license)
         
         ## Supported Models
         
         | Models             | Model Type  |
         | :----------------- | ----------- |
@@ -34,14 +35,39 @@
         
         ## Installation
         
         ```sh
         pip install ctransformers
         ```
         
+        For GPU (CUDA) support, set environment variable `CT_CUBLAS=1` and install from source using:
+        
+        ```sh
+        CT_CUBLAS=1 pip install ctransformers --no-binary ctransformers
+        ```
+        
+        <details>
+        <summary><strong>Show commands for Windows</strong></summary><br>
+        
+        On Windows PowerShell run:
+        
+        ```sh
+        $env:CT_CUBLAS=1
+        pip install ctransformers --no-binary ctransformers
+        ```
+        
+        On Windows Command Prompt run:
+        
+        ```sh
+        set CT_CUBLAS=1
+        pip install ctransformers --no-binary ctransformers
+        ```
+        
+        </details>
+        
         ## Usage
         
         It provides a unified interface for all models:
         
         ```py
         from ctransformers import AutoModelForCausalLM
         
@@ -63,15 +89,26 @@
         ```py
         tokens = llm.tokenize('AI is going to')
         
         for token in llm.generate(tokens):
             print(llm.detokenize(token))
         ```
         
-        This allows you to use a custom tokenizer.
+        It can be used with a custom or Hugging Face tokenizer:
+        
+        ```py
+        from transformers import AutoTokenizer
+        
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+        
+        tokens = tokenizer.encode('AI is going to')
+        
+        for token in llm.generate(tokens):
+            print(tokenizer.decode(token))
+        ```
         
         It also provides access to the low-level C API. See [Documentation](#documentation) section below.
         
         ### Hugging Face Hub
         
         It can be used with models hosted on the Hub:
         
@@ -91,80 +128,33 @@
         
         ```json
         {
           "model_type": "gpt2"
         }
         ```
         
-        You can also specify additional parameters under `task_specific_params.text-generation`:
-        
-        ```json
-        {
-          "model_type": "gpt2",
-          "task_specific_params": {
-            "text-generation": {
-              "top_k": 40,
-              "top_p": 0.95,
-              "temperature": 0.8,
-              "repetition_penalty": 1.1,
-              "last_n_tokens": 64
-            }
-          }
-        }
-        ```
+        You can also specify additional parameters under `task_specific_params.text-generation`.
         
         See [marella/gpt-2-ggml](https://huggingface.co/marella/gpt-2-ggml/blob/main/config.json) for a minimal example and [marella/gpt-2-ggml-example](https://huggingface.co/marella/gpt-2-ggml-example/blob/main/config.json) for a full example.
         
         ### LangChain
         
-        [LangChain](https://python.langchain.com/) is a framework for developing applications powered by language models. A LangChain LLM object can be created using:
-        
-        ```py
-        from ctransformers.langchain import CTransformers
-        
-        llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2')
-        
-        print(llm('AI is going to'))
-        ```
-        
-        If you are getting `illegal instruction` error, try using `lib='avx'` or `lib='basic'`:
-        
-        ```py
-        llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2', lib='avx')
-        ```
+        It is integrated into LangChain. See [LangChain docs](https://python.langchain.com/en/latest/integrations/ctransformers.html).
         
-        It can also be used with models hosted on the Hugging Face Hub:
+        ### GPU
         
-        ```py
-        llm = CTransformers(model='marella/gpt-2-ggml')
-        ```
+        > **Note:** Currently only LLaMA models have GPU support.
         
-        Additional parameters can be passed using the `config` parameter:
+        To run some of the model layers on GPU, set the `gpu_layers` parameter:
         
         ```py
-        config = {'max_new_tokens': 256, 'repetition_penalty': 1.1}
-        
-        llm = CTransformers(model='marella/gpt-2-ggml', config=config)
+        llm = AutoModelForCausalLM.from_pretrained('/path/to/ggml-llama.bin', model_type='llama', gpu_layers=50)
         ```
         
-        It can be used with other LangChain modules:
-        
-        ```py
-        from langchain import PromptTemplate, LLMChain
-        
-        template = """Question: {question}
-        
-        Answer:"""
-        
-        prompt = PromptTemplate(template=template, input_variables=['question'])
-        
-        llm_chain = LLMChain(prompt=prompt, llm=llm)
-        
-        print(llm_chain.run('What is AI?'))
-        ```
+        [Run in Google Colab](https://colab.research.google.com/drive/1Ihn7iPCYiqlTotpkqa1tOhUIpJBrJ1Tp)
         
         ## Documentation
         
         <!-- API_DOCS -->
         
         ### Config
         
@@ -179,16 +169,17 @@
         | `max_new_tokens`     | `int`       | The maximum number of new tokens to generate.            | `256`   |
         | `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `None`  |
         | `stream`             | `bool`      | Whether to stream the generated text.                    | `False` |
         | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
         | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
         | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | `-1`    |
         | `context_length`     | `int`       | The maximum context length to use.                       | `-1`    |
+        | `gpu_layers`         | `int`       | The number of layers to run on GPU.                      | `0`     |
         
-        > **Note:** Currently only LLaMA models support the `context_length` parameter.
+        > **Note:** Currently only LLaMA models support the `context_length` and `gpu_layers` parameters.
         
         ### <kbd>class</kbd> `AutoModelForCausalLM`
         
         ---
         
         #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
```

### Comparing `ctransformers-0.2.2/README.md` & `ctransformers-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Python bindings for the Transformer models implemented in C/C++ using [GGML](https://github.com/ggerganov/ggml) library.
 
 - [Supported Models](#supported-models)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Hugging Face Hub](#hugging-face-hub)
   - [LangChain](#langchain)
+  - [GPU](#gpu)
 - [Documentation](#documentation)
 - [License](#license)
 
 ## Supported Models
 
 | Models             | Model Type  |
 | :----------------- | ----------- |
@@ -26,14 +27,39 @@
 
 ## Installation
 
 ```sh
 pip install ctransformers
 ```
 
+For GPU (CUDA) support, set environment variable `CT_CUBLAS=1` and install from source using:
+
+```sh
+CT_CUBLAS=1 pip install ctransformers --no-binary ctransformers
+```
+
+<details>
+<summary><strong>Show commands for Windows</strong></summary><br>
+
+On Windows PowerShell run:
+
+```sh
+$env:CT_CUBLAS=1
+pip install ctransformers --no-binary ctransformers
+```
+
+On Windows Command Prompt run:
+
+```sh
+set CT_CUBLAS=1
+pip install ctransformers --no-binary ctransformers
+```
+
+</details>
+
 ## Usage
 
 It provides a unified interface for all models:
 
 ```py
 from ctransformers import AutoModelForCausalLM
 
@@ -55,15 +81,26 @@
 ```py
 tokens = llm.tokenize('AI is going to')
 
 for token in llm.generate(tokens):
     print(llm.detokenize(token))
 ```
 
-This allows you to use a custom tokenizer.
+It can be used with a custom or Hugging Face tokenizer:
+
+```py
+from transformers import AutoTokenizer
+
+tokenizer = AutoTokenizer.from_pretrained('gpt2')
+
+tokens = tokenizer.encode('AI is going to')
+
+for token in llm.generate(tokens):
+    print(tokenizer.decode(token))
+```
 
 It also provides access to the low-level C API. See [Documentation](#documentation) section below.
 
 ### Hugging Face Hub
 
 It can be used with models hosted on the Hub:
 
@@ -83,80 +120,33 @@
 
 ```json
 {
   "model_type": "gpt2"
 }
 ```
 
-You can also specify additional parameters under `task_specific_params.text-generation`:
-
-```json
-{
-  "model_type": "gpt2",
-  "task_specific_params": {
-    "text-generation": {
-      "top_k": 40,
-      "top_p": 0.95,
-      "temperature": 0.8,
-      "repetition_penalty": 1.1,
-      "last_n_tokens": 64
-    }
-  }
-}
-```
+You can also specify additional parameters under `task_specific_params.text-generation`.
 
 See [marella/gpt-2-ggml](https://huggingface.co/marella/gpt-2-ggml/blob/main/config.json) for a minimal example and [marella/gpt-2-ggml-example](https://huggingface.co/marella/gpt-2-ggml-example/blob/main/config.json) for a full example.
 
 ### LangChain
 
-[LangChain](https://python.langchain.com/) is a framework for developing applications powered by language models. A LangChain LLM object can be created using:
-
-```py
-from ctransformers.langchain import CTransformers
-
-llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2')
-
-print(llm('AI is going to'))
-```
-
-If you are getting `illegal instruction` error, try using `lib='avx'` or `lib='basic'`:
-
-```py
-llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2', lib='avx')
-```
+It is integrated into LangChain. See [LangChain docs](https://python.langchain.com/en/latest/integrations/ctransformers.html).
 
-It can also be used with models hosted on the Hugging Face Hub:
+### GPU
 
-```py
-llm = CTransformers(model='marella/gpt-2-ggml')
-```
+> **Note:** Currently only LLaMA models have GPU support.
 
-Additional parameters can be passed using the `config` parameter:
+To run some of the model layers on GPU, set the `gpu_layers` parameter:
 
 ```py
-config = {'max_new_tokens': 256, 'repetition_penalty': 1.1}
-
-llm = CTransformers(model='marella/gpt-2-ggml', config=config)
+llm = AutoModelForCausalLM.from_pretrained('/path/to/ggml-llama.bin', model_type='llama', gpu_layers=50)
 ```
 
-It can be used with other LangChain modules:
-
-```py
-from langchain import PromptTemplate, LLMChain
-
-template = """Question: {question}
-
-Answer:"""
-
-prompt = PromptTemplate(template=template, input_variables=['question'])
-
-llm_chain = LLMChain(prompt=prompt, llm=llm)
-
-print(llm_chain.run('What is AI?'))
-```
+[Run in Google Colab](https://colab.research.google.com/drive/1Ihn7iPCYiqlTotpkqa1tOhUIpJBrJ1Tp)
 
 ## Documentation
 
 <!-- API_DOCS -->
 
 ### Config
 
@@ -171,16 +161,17 @@
 | `max_new_tokens`     | `int`       | The maximum number of new tokens to generate.            | `256`   |
 | `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `None`  |
 | `stream`             | `bool`      | Whether to stream the generated text.                    | `False` |
 | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
 | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
 | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | `-1`    |
 | `context_length`     | `int`       | The maximum context length to use.                       | `-1`    |
+| `gpu_layers`         | `int`       | The number of layers to run on GPU.                      | `0`     |
 
-> **Note:** Currently only LLaMA models support the `context_length` parameter.
+> **Note:** Currently only LLaMA models support the `context_length` and `gpu_layers` parameters.
 
 ### <kbd>class</kbd> `AutoModelForCausalLM`
 
 ---
 
 #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
```

### Comparing `ctransformers-0.2.2/ctransformers/hub.py` & `ctransformers-0.2.3/ctransformers/hub.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.2/ctransformers/langchain.py` & `ctransformers-0.2.3/ctransformers/langchain.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.2/ctransformers/llm.py` & `ctransformers-0.2.3/ctransformers/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import os
 import re
 from collections import OrderedDict
 from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
 from ctypes import (
     CDLL,
@@ -49,14 +50,15 @@
     max_new_tokens: int = 256
     stop: Optional[Sequence[str]] = None
     stream: bool = False
     reset: bool = True
 
     # model
     context_length: int = -1
+    gpu_layers: int = 0
 
 
 docs = OrderedDict(
     top_k='The top-k value to use for sampling.',
     top_p='The top-p value to use for sampling.',
     temperature='The temperature to use for sampling.',
     repetition_penalty='The repetition penalty to use for sampling.',
@@ -65,14 +67,15 @@
     max_new_tokens='The maximum number of new tokens to generate.',
     stop='A list of sequences to stop generation when encountered.',
     stream='Whether to stream the generated text.',
     reset='Whether to reset the model state before generating text.',
     batch_size='The batch size to use for evaluating tokens.',
     threads='The number of threads to use for evaluating tokens.',
     context_length='The maximum context length to use.',
+    gpu_layers='The number of layers to run on GPU.',
 )
 
 
 def doc(fn):
     doc = []
     for param in inspect.signature(fn).parameters:
         if param in docs:
@@ -86,21 +89,27 @@
 def get(*values):
     for value in values:
         if value is not None:
             return value
 
 
 def load_library(path: Optional[str] = None) -> Any:
+    # https://docs.python.org/3.8/whatsnew/3.8.html#bpo-36085-whatsnew
+    # https://github.com/abetlen/llama-cpp-python/pull/225
+    if hasattr(os, 'add_dll_directory') and 'CUDA_PATH' in os.environ:
+        os.add_dll_directory(os.path.join(os.environ['CUDA_PATH'], 'bin'))
+
     path = find_library(path)
     lib = CDLL(path)
 
     lib.ctransformers_llm_create.argtypes = [
         c_char_p,  # model_path
         c_char_p,  # model_type
         c_int,  # context_length
+        c_int,  # gpu_layers
     ]
     lib.ctransformers_llm_create.restype = llm_p
 
     lib.ctransformers_llm_delete.argtypes = [llm_p]
     lib.ctransformers_llm_delete.restype = None
 
     lib.ctransformers_llm_tokenize.argtypes = [
@@ -187,14 +196,15 @@
             raise ValueError(f"Model path '{model_path}' doesn't exist.")
 
         self._lib = load_library(lib)
         self._llm = self._lib.ctransformers_llm_create(
             model_path.encode(),
             model_type.encode(),
             config.context_length,
+            config.gpu_layers,
         )
         if self._llm is None:
             raise RuntimeError(
                 f"Failed to create LLM '{model_type}' from '{model_path}'.")
 
     @property
     def model_path(self) -> str:
```

### Comparing `ctransformers-0.2.2/ctransformers/utils.py` & `ctransformers-0.2.3/ctransformers/utils.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.2/ctransformers.egg-info/PKG-INFO` & `ctransformers-0.2.3/ctransformers.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
         
         Python bindings for the Transformer models implemented in C/C++ using [GGML](https://github.com/ggerganov/ggml) library.
         
         - [Supported Models](#supported-models)
         - [Installation](#installation)
         - [Usage](#usage)
           - [Hugging Face Hub](#hugging-face-hub)
           - [LangChain](#langchain)
+          - [GPU](#gpu)
         - [Documentation](#documentation)
         - [License](#license)
         
         ## Supported Models
         
         | Models             | Model Type  |
         | :----------------- | ----------- |
@@ -34,14 +35,39 @@
         
         ## Installation
         
         ```sh
         pip install ctransformers
         ```
         
+        For GPU (CUDA) support, set environment variable `CT_CUBLAS=1` and install from source using:
+        
+        ```sh
+        CT_CUBLAS=1 pip install ctransformers --no-binary ctransformers
+        ```
+        
+        <details>
+        <summary><strong>Show commands for Windows</strong></summary><br>
+        
+        On Windows PowerShell run:
+        
+        ```sh
+        $env:CT_CUBLAS=1
+        pip install ctransformers --no-binary ctransformers
+        ```
+        
+        On Windows Command Prompt run:
+        
+        ```sh
+        set CT_CUBLAS=1
+        pip install ctransformers --no-binary ctransformers
+        ```
+        
+        </details>
+        
         ## Usage
         
         It provides a unified interface for all models:
         
         ```py
         from ctransformers import AutoModelForCausalLM
         
@@ -63,15 +89,26 @@
         ```py
         tokens = llm.tokenize('AI is going to')
         
         for token in llm.generate(tokens):
             print(llm.detokenize(token))
         ```
         
-        This allows you to use a custom tokenizer.
+        It can be used with a custom or Hugging Face tokenizer:
+        
+        ```py
+        from transformers import AutoTokenizer
+        
+        tokenizer = AutoTokenizer.from_pretrained('gpt2')
+        
+        tokens = tokenizer.encode('AI is going to')
+        
+        for token in llm.generate(tokens):
+            print(tokenizer.decode(token))
+        ```
         
         It also provides access to the low-level C API. See [Documentation](#documentation) section below.
         
         ### Hugging Face Hub
         
         It can be used with models hosted on the Hub:
         
@@ -91,80 +128,33 @@
         
         ```json
         {
           "model_type": "gpt2"
         }
         ```
         
-        You can also specify additional parameters under `task_specific_params.text-generation`:
-        
-        ```json
-        {
-          "model_type": "gpt2",
-          "task_specific_params": {
-            "text-generation": {
-              "top_k": 40,
-              "top_p": 0.95,
-              "temperature": 0.8,
-              "repetition_penalty": 1.1,
-              "last_n_tokens": 64
-            }
-          }
-        }
-        ```
+        You can also specify additional parameters under `task_specific_params.text-generation`.
         
         See [marella/gpt-2-ggml](https://huggingface.co/marella/gpt-2-ggml/blob/main/config.json) for a minimal example and [marella/gpt-2-ggml-example](https://huggingface.co/marella/gpt-2-ggml-example/blob/main/config.json) for a full example.
         
         ### LangChain
         
-        [LangChain](https://python.langchain.com/) is a framework for developing applications powered by language models. A LangChain LLM object can be created using:
-        
-        ```py
-        from ctransformers.langchain import CTransformers
-        
-        llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2')
-        
-        print(llm('AI is going to'))
-        ```
-        
-        If you are getting `illegal instruction` error, try using `lib='avx'` or `lib='basic'`:
-        
-        ```py
-        llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2', lib='avx')
-        ```
+        It is integrated into LangChain. See [LangChain docs](https://python.langchain.com/en/latest/integrations/ctransformers.html).
         
-        It can also be used with models hosted on the Hugging Face Hub:
+        ### GPU
         
-        ```py
-        llm = CTransformers(model='marella/gpt-2-ggml')
-        ```
+        > **Note:** Currently only LLaMA models have GPU support.
         
-        Additional parameters can be passed using the `config` parameter:
+        To run some of the model layers on GPU, set the `gpu_layers` parameter:
         
         ```py
-        config = {'max_new_tokens': 256, 'repetition_penalty': 1.1}
-        
-        llm = CTransformers(model='marella/gpt-2-ggml', config=config)
+        llm = AutoModelForCausalLM.from_pretrained('/path/to/ggml-llama.bin', model_type='llama', gpu_layers=50)
         ```
         
-        It can be used with other LangChain modules:
-        
-        ```py
-        from langchain import PromptTemplate, LLMChain
-        
-        template = """Question: {question}
-        
-        Answer:"""
-        
-        prompt = PromptTemplate(template=template, input_variables=['question'])
-        
-        llm_chain = LLMChain(prompt=prompt, llm=llm)
-        
-        print(llm_chain.run('What is AI?'))
-        ```
+        [Run in Google Colab](https://colab.research.google.com/drive/1Ihn7iPCYiqlTotpkqa1tOhUIpJBrJ1Tp)
         
         ## Documentation
         
         <!-- API_DOCS -->
         
         ### Config
         
@@ -179,16 +169,17 @@
         | `max_new_tokens`     | `int`       | The maximum number of new tokens to generate.            | `256`   |
         | `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `None`  |
         | `stream`             | `bool`      | Whether to stream the generated text.                    | `False` |
         | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
         | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
         | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | `-1`    |
         | `context_length`     | `int`       | The maximum context length to use.                       | `-1`    |
+        | `gpu_layers`         | `int`       | The number of layers to run on GPU.                      | `0`     |
         
-        > **Note:** Currently only LLaMA models support the `context_length` parameter.
+        > **Note:** Currently only LLaMA models support the `context_length` and `gpu_layers` parameters.
         
         ### <kbd>class</kbd> `AutoModelForCausalLM`
         
         ---
         
         #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
```

