# Comparing `tmp/talk_codebase-0.1.27.tar.gz` & `tmp/talk_codebase-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.27.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.28.tar", max compression
```

## Comparing `talk_codebase-0.1.27.tar` & `talk_codebase-0.1.28.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2866 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/README.md
--rw-r--r--   0        0        0      888 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/pyproject.toml
--rw-r--r--   0        0        0     4442 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/LLM.py
--rw-r--r--   0        0        0        0 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/__init__.py
--rw-r--r--   0        0        0     2880 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/cli.py
--rw-r--r--   0        0        0     1717 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/consts.py
--rw-r--r--   0        0        0     2403 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/utils.py
--rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 talk_codebase-0.1.27/PKG-INFO
+-rw-r--r--   0        0        0     2866 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/README.md
+-rw-r--r--   0        0        0      888 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/pyproject.toml
+-rw-r--r--   0        0        0     4442 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/LLM.py
+-rw-r--r--   0        0        0        0 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     2880 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/cli.py
+-rw-r--r--   0        0        0     1717 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2474 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/utils.py
+-rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 talk_codebase-0.1.28/PKG-INFO
```

### Comparing `talk_codebase-0.1.27/README.md` & `talk_codebase-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.27/pyproject.toml` & `talk_codebase-0.1.28/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.27"
+version = "0.1.28"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.27/talk_codebase/LLM.py` & `talk_codebase-0.1.28/talk_codebase/LLM.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.27/talk_codebase/cli.py` & `talk_codebase-0.1.28/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.27/talk_codebase/consts.py` & `talk_codebase-0.1.28/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.27/talk_codebase/utils.py` & `talk_codebase-0.1.28/talk_codebase/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import glob
 import multiprocessing
 import os
 import sys
 
 import tiktoken
 from git import Repo
+from halo import Halo
 from langchain import FAISS
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
 from talk_codebase.consts import LOADER_MAPPING, EXCLUDE_FILES
 
 
 def get_repo(root_dir):
@@ -37,14 +38,15 @@
         sys.stdout.write("🤖 ")
 
     def on_llm_end(self, response, **kwargs):
         sys.stdout.write("\n")
         sys.stdout.flush()
 
 
+@Halo(text='📂 Loading files', spinner='dots')
 def load_files(root_dir):
     num_cpus = multiprocessing.cpu_count()
     loaded_files = []
     with multiprocessing.Pool(num_cpus) as pool:
         futures = []
         for file_path in glob.glob(os.path.join(root_dir, '**/*'), recursive=True):
             if is_ignored(file_path, root_dir):
```

### Comparing `talk_codebase-0.1.27/PKG-INFO` & `talk_codebase-0.1.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.27
+Version: 0.1.28
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

