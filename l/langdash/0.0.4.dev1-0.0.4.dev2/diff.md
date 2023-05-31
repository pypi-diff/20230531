# Comparing `tmp/langdash-0.0.4.dev1.tar.gz` & `tmp/langdash-0.0.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-0.0.4.dev1.tar", last modified: Wed May 31 21:24:12 2023, max compression
+gzip compressed data, was "langdash-0.0.4.dev2.tar", last modified: Wed May 31 21:54:53 2023, max compression
```

## Comparing `langdash-0.0.4.dev1.tar` & `langdash-0.0.4.dev2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.4.dev1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-0.0.4.dev1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3484 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2670 2023-05-30 08:29:06.000000 langdash-0.0.4.dev1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       66 2023-05-31 20:08:48.000000 langdash-0.0.4.dev1/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    17611 2023-05-31 19:50:04.000000 langdash-0.0.4.dev1/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.498655 langdash-0.0.4.dev1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.4.dev1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.4.dev1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     4126 2023-05-31 20:08:59.000000 langdash-0.0.4.dev1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      690 2023-05-31 17:39:51.000000 langdash-0.0.4.dev1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-05-31 17:04:37.000000 langdash-0.0.4.dev1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7520 2023-05-31 19:52:12.000000 langdash-0.0.4.dev1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.498655 langdash-0.0.4.dev1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.4.dev1/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      682 2023-05-31 21:23:49.000000 langdash-0.0.4.dev1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     7041 2023-05-31 20:11:04.000000 langdash-0.0.4.dev1/langdash/models/rwkvcpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      958 2023-05-31 20:11:54.000000 langdash-0.0.4.dev1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6134 2023-05-31 20:11:31.000000 langdash-0.0.4.dev1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      835 2023-05-31 17:40:54.000000 langdash-0.0.4.dev1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2436 2023-05-31 17:34:53.000000 langdash-0.0.4.dev1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.4.dev1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.4.dev1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.4.dev1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.4.dev1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3484 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1214 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1405 2023-05-31 20:04:55.000000 langdash-0.0.4.dev1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.4.dev2/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-0.0.4.dev2/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3575 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2690 2023-05-31 21:54:27.000000 langdash-0.0.4.dev2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       66 2023-05-31 21:53:10.000000 langdash-0.0.4.dev2/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17611 2023-05-31 19:50:04.000000 langdash-0.0.4.dev2/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.484769 langdash-0.0.4.dev2/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.4.dev2/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.4.dev2/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4126 2023-05-31 20:08:59.000000 langdash-0.0.4.dev2/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      690 2023-05-31 17:39:51.000000 langdash-0.0.4.dev2/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-05-31 17:04:37.000000 langdash-0.0.4.dev2/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7520 2023-05-31 19:52:12.000000 langdash-0.0.4.dev2/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.484769 langdash-0.0.4.dev2/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.4.dev2/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      682 2023-05-31 21:23:49.000000 langdash-0.0.4.dev2/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7041 2023-05-31 20:11:04.000000 langdash-0.0.4.dev2/langdash/models/rwkvcpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      958 2023-05-31 20:11:54.000000 langdash-0.0.4.dev2/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6134 2023-05-31 20:11:31.000000 langdash-0.0.4.dev2/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      835 2023-05-31 17:40:54.000000 langdash-0.0.4.dev2/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2436 2023-05-31 17:34:53.000000 langdash-0.0.4.dev2/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.4.dev2/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.4.dev2/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.4.dev2/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.4.dev2/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3575 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1214 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1474 2023-05-31 21:52:17.000000 langdash-0.0.4.dev2/setup.py
```

### Comparing `langdash-0.0.4.dev1/LICENSE.txt` & `langdash-0.0.4.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/PKG-INFO` & `langdash-0.0.4.dev2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.4.dev1
+Version: 0.0.4.dev2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
+Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
@@ -20,22 +21,24 @@
 Provides-Extra: sentence_transformers
 License-File: LICENSE.txt
 
 # langdash
 
 A simple library for interfacing with language models.
 
+**Currently in alpha!**
+
 Features:
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends (currently rwkv.cpp is supported).
 
-**Currently in alpha! Documentation might be missing, but the library should work OOTB**
+Documentation: [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
 
 ## Installation
 
 Use [pip](https://pip.pypa.io/en/stable/) to install. By default, langdash does not come preinstalled with any additional modules, so you'll have to specify what you need like in the following command:
 
 ```
 pip install --user langdash[embeddings,sentence_transformers]
```

### Comparing `langdash-0.0.4.dev1/README.md` & `langdash-0.0.4.dev2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # langdash
 
 A simple library for interfacing with language models.
 
+**Currently in alpha!**
+
 Features:
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends (currently rwkv.cpp is supported).
 
-**Currently in alpha! Documentation might be missing, but the library should work OOTB**
+Documentation: [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
 
 ## Installation
 
 Use [pip](https://pip.pypa.io/en/stable/) to install. By default, langdash does not come preinstalled with any additional modules, so you'll have to specify what you need like in the following command:
 
 ```
 pip install --user langdash[embeddings,sentence_transformers]
```

### Comparing `langdash-0.0.4.dev1/langdash/chains.py` & `langdash-0.0.4.dev2/langdash/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/classify/token_qa.py` & `langdash-0.0.4.dev2/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/core.py` & `langdash-0.0.4.dev2/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/infer.py` & `langdash-0.0.4.dev2/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/llm.py` & `langdash-0.0.4.dev2/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/llm_session.py` & `langdash-0.0.4.dev2/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/models/mock.py` & `langdash-0.0.4.dev2/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/models/rwkvcpp.py` & `langdash-0.0.4.dev2/langdash/models/rwkvcpp.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/models/sentence_transformers.py` & `langdash-0.0.4.dev2/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/models/transformers.py` & `langdash-0.0.4.dev2/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/response.py` & `langdash-0.0.4.dev2/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/sampling.py` & `langdash-0.0.4.dev2/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/search/embedding_search.py` & `langdash-0.0.4.dev2/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash/search/multichoice_search.py` & `langdash-0.0.4.dev2/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/langdash.egg-info/PKG-INFO` & `langdash-0.0.4.dev2/langdash.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.4.dev1
+Version: 0.0.4.dev2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
+Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
@@ -20,22 +21,24 @@
 Provides-Extra: sentence_transformers
 License-File: LICENSE.txt
 
 # langdash
 
 A simple library for interfacing with language models.
 
+**Currently in alpha!**
+
 Features:
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends (currently rwkv.cpp is supported).
 
-**Currently in alpha! Documentation might be missing, but the library should work OOTB**
+Documentation: [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
 
 ## Installation
 
 Use [pip](https://pip.pypa.io/en/stable/) to install. By default, langdash does not come preinstalled with any additional modules, so you'll have to specify what you need like in the following command:
 
 ```
 pip install --user langdash[embeddings,sentence_transformers]
```

### Comparing `langdash-0.0.4.dev1/langdash.egg-info/SOURCES.txt` & `langdash-0.0.4.dev2/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev1/setup.py` & `langdash-0.0.4.dev2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
       'Topic :: Software Development :: Libraries',
       'License :: OSI Approved :: Apache Software License',
       'Programming Language :: Python :: 3',
       'Programming Language :: Python :: 3.8',
     ],
     project_urls={
       'Source': 'https://git.mysymphony.jp.net/nana/langdash',
+      'Documentation': 'https://langdash.readthedocs.io/en/latest/',
     },
     # requirements
     python_requires='>=3.8',
     packages=find_packages(include=['langdash', 'langdash.*'], exclude=['extern']),
     install_requires=[
       'torch',
     ],
```

