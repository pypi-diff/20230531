# Comparing `tmp/cosmian_py_ggml-0.1.0-1-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/cosmian_py_ggml-0.2.0-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 272197 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-31 13:07 cosmian_py_ggml-0.1.0.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-31 13:07 cosmian_py_ggml.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-31 13:07 cosmian_py_ggml/
--rw-r--r--  2.0 unx     1252 b- defN 23-May-31 13:07 cosmian_py_ggml-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx     1064 b- defN 23-May-31 13:07 cosmian_py_ggml-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      592 b- defN 23-May-31 13:07 cosmian_py_ggml-0.1.0.dist-info/RECORD
--rw-r--r--  2.0 unx      165 b- defN 23-May-31 13:07 cosmian_py_ggml-0.1.0.dist-info/WHEEL
--rwxr-xr-x  2.0 unx   684448 b- defN 23-May-31 13:07 cosmian_py_ggml/libggml-gptneox.so
--rw-r--r--  2.0 unx     5334 b- defN 23-May-31 13:07 cosmian_py_ggml/gpt_neox.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-31 13:07 cosmian_py_ggml/__init__.py
-10 files, 692855 bytes uncompressed, 270793 bytes compressed:  60.9%
+Zip file size: 272221 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-31 13:20 cosmian_py_ggml.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-31 13:20 cosmian_py_ggml/
+-rw-r--r--  2.0 unx     1315 b- defN 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx     1064 b- defN 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      592 b- defN 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      165 b- defN 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx   684448 b- defN 23-May-31 13:20 cosmian_py_ggml/libggml-gptneox.so
+-rw-r--r--  2.0 unx     5334 b- defN 23-May-31 13:20 cosmian_py_ggml/gpt_neox.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 13:20 cosmian_py_ggml/__init__.py
+10 files, 692918 bytes uncompressed, 270817 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,26 +1,26 @@
-Filename: cosmian_py_ggml-0.1.0.dist-info/
+Filename: cosmian_py_ggml.libs/
 Comment: 
 
-Filename: cosmian_py_ggml.libs/
+Filename: cosmian_py_ggml-0.2.0.dist-info/
 Comment: 
 
 Filename: cosmian_py_ggml/
 Comment: 
 
-Filename: cosmian_py_ggml-0.1.0.dist-info/METADATA
+Filename: cosmian_py_ggml-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: cosmian_py_ggml-0.1.0.dist-info/LICENSE
+Filename: cosmian_py_ggml-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: cosmian_py_ggml-0.1.0.dist-info/RECORD
+Filename: cosmian_py_ggml-0.2.0.dist-info/RECORD
 Comment: 
 
-Filename: cosmian_py_ggml-0.1.0.dist-info/WHEEL
+Filename: cosmian_py_ggml-0.2.0.dist-info/WHEEL
 Comment: 
 
 Filename: cosmian_py_ggml/libggml-gptneox.so
 Comment: 
 
 Filename: cosmian_py_ggml/gpt_neox.py
 Comment:
```

## Comparing `cosmian_py_ggml-0.1.0.dist-info/METADATA` & `cosmian_py_ggml-0.2.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmian-py-ggml
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python bindings for GGML
 License: MIT
 Author: Hugo Rosenkranz-Costa
 Author-email: hugo.rosenkranz@cosmian.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,17 +23,20 @@
 - [gpt-neox](https://huggingface.co/docs/transformers/model_doc/gpt_neox)
 
 ```python
 from cosmian_py_ggml import gpt_neox
 from transformers import AutoTokenizer
 
 tokenizer = AutoTokenizer.from_pretrained("EleutherAI/gpt-neox-20b")
-res = gpt_neox.generate("ggml_model_path", tokenizer.encode(query))
+model = gpt_neox.load_model("ggml_model_path")
 
+res = gpt_neox.generate(model, tokenizer.encode(query))
 print("Response:", tokenizer.decode(res))
+
+gpt_neox.free_model(model)
 ```
 
 ## Build from sources
 
 ```bash
 git clone --recursive git@github.com:Cosmian/cosmian_py_ggml.git
 scripts/build.sh
```

## Comparing `cosmian_py_ggml-0.1.0.dist-info/LICENSE` & `cosmian_py_ggml-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

