# Comparing `tmp/agenta-0.1.2.tar.gz` & `tmp/agenta-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenta-0.1.2.tar", max compression
+gzip compressed data, was "agenta-0.1.3.tar", max compression
```

## Comparing `agenta-0.1.2.tar` & `agenta-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.2/README.md
--rw-r--r--   0        0        0       53 2023-05-20 06:49:49.205423 agenta-0.1.2/agenta/__init__.py
--rw-r--r--   0        0        0     3045 2023-05-30 19:16:46.669891 agenta-0.1.2/agenta/agenta.py
--rw-r--r--   0        0        0     5924 2023-05-29 13:26:47.815435 agenta-0.1.2/agenta/cli.py
--rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.2/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.2/agenta/client/__init__.py
--rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.2/agenta/client/api_models.py
--rw-r--r--   0        0        0     1479 2023-05-26 07:44:13.475577 agenta-0.1.2/agenta/client/client.py
--rw-r--r--   0        0        0      550 2023-05-11 14:46:01.166162 agenta-0.1.2/agenta/config.py
--rw-r--r--   0        0        0       91 2023-05-12 12:52:29.405049 agenta-0.1.2/agenta/config.toml
--rw-r--r--   0        0        0      337 2023-05-24 09:05:58.092867 agenta-0.1.2/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.2/agenta/docker/docker-assets/README.md
--rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.2/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     2585 2023-05-27 10:11:21.981693 agenta-0.1.2/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0      407 2023-05-22 17:58:10.352282 agenta-0.1.2/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      658 2023-05-31 17:00:44.755699 agenta-0.1.2/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.2/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.2/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0      513 2023-05-31 17:01:05.416017 agenta-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 agenta-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.3/README.md
+-rw-r--r--   0        0        0       53 2023-05-20 06:49:49.205423 agenta-0.1.3/agenta/__init__.py
+-rw-r--r--   0        0        0     3045 2023-05-30 19:16:46.669891 agenta-0.1.3/agenta/agenta.py
+-rw-r--r--   0        0        0     5924 2023-05-29 13:26:47.815435 agenta-0.1.3/agenta/cli.py
+-rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.3/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.3/agenta/client/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.3/agenta/client/api_models.py
+-rw-r--r--   0        0        0     1479 2023-05-26 07:44:13.475577 agenta-0.1.3/agenta/client/client.py
+-rw-r--r--   0        0        0      550 2023-05-11 14:46:01.166162 agenta-0.1.3/agenta/config.py
+-rw-r--r--   0        0        0       91 2023-05-12 12:52:29.405049 agenta-0.1.3/agenta/config.toml
+-rw-r--r--   0        0        0      337 2023-05-24 09:05:58.092867 agenta-0.1.3/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.3/agenta/docker/docker-assets/README.md
+-rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.3/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     2585 2023-05-27 10:11:21.981693 agenta-0.1.3/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0      407 2023-05-22 17:58:10.352282 agenta-0.1.3/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.3/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.3/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.3/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0      513 2023-05-31 17:02:54.646010 agenta-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 agenta-0.1.3/PKG-INFO
```

### Comparing `agenta-0.1.2/agenta/agenta.py` & `agenta-0.1.3/agenta/agenta.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.2/agenta/cli.py` & `agenta-0.1.3/agenta/cli.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.2/agenta/client/client.py` & `agenta-0.1.3/agenta/client/client.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.2/agenta/config.py` & `agenta-0.1.3/agenta/config.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.2/agenta/docker/docker_utils.py` & `agenta-0.1.3/agenta/docker/docker_utils.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.2/agenta/templates/simple_prompt/app.py` & `agenta-0.1.3/agenta/templates/simple_prompt/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from langchain.prompts import PromptTemplate
 
 default_prompt = "What is a good name for a company that makes {product}?"
 
 
 @post
 def generate(product: str, temperature: FloatParam = 0.9, prompt_template: TextParam = default_prompt) -> str:
-    load_dotenv
+    load_dotenv()
     llm = OpenAI(temperature=temperature)
     prompt = PromptTemplate(
         input_variables=["product"],
         template=prompt_template,
     )
     chain = LLMChain(llm=llm, prompt=prompt)
     output = chain.run(product=product)
```

### Comparing `agenta-0.1.2/pyproject.toml` & `agenta-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agenta"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Mahmoud Mabrouk <mahmoudmabrouk.mail@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^6.1.1"
```

### Comparing `agenta-0.1.2/PKG-INFO` & `agenta-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agenta
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Mahmoud Mabrouk
 Author-email: mahmoudmabrouk.mail@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

