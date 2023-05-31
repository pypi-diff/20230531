# Comparing `tmp/langchainplus_sdk-0.0.1.tar.gz` & `tmp/langchainplus_sdk-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainplus_sdk-0.0.1.tar", max compression
+gzip compressed data, was "langchainplus_sdk-0.0.1rc1.tar", max compression
```

## Comparing `langchainplus_sdk-0.0.1.tar` & `langchainplus_sdk-0.0.1rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      604 2023-05-31 03:06:17.895497 langchainplus_sdk-0.0.1/README.md
--rw-r--r--   0        0        0      119 2023-05-31 01:18:44.687819 langchainplus_sdk-0.0.1/langchainplus_sdk/__init__.py
--rw-r--r--   0        0        0    17009 2023-05-31 02:59:28.603476 langchainplus_sdk-0.0.1/langchainplus_sdk/client.py
--rw-r--r--   0        0        0     6647 2023-05-31 02:59:33.535466 langchainplus_sdk-0.0.1/langchainplus_sdk/schemas.py
--rw-r--r--   0        0        0     1315 2023-05-31 01:24:33.402976 langchainplus_sdk-0.0.1/langchainplus_sdk/utils.py
--rw-r--r--   0        0        0      791 2023-05-31 02:53:09.155804 langchainplus_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1237 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      604 2023-05-31 03:06:17.895497 langchainplus_sdk-0.0.1rc1/README.md
+-rw-r--r--   0        0        0      119 2023-05-31 01:18:44.687819 langchainplus_sdk-0.0.1rc1/langchainplus_sdk/__init__.py
+-rw-r--r--   0        0        0    17009 2023-05-31 02:59:28.603476 langchainplus_sdk-0.0.1rc1/langchainplus_sdk/client.py
+-rw-r--r--   0        0        0     6647 2023-05-31 02:59:33.535466 langchainplus_sdk-0.0.1rc1/langchainplus_sdk/schemas.py
+-rw-r--r--   0        0        0     1315 2023-05-31 01:24:33.402976 langchainplus_sdk-0.0.1rc1/langchainplus_sdk/utils.py
+-rw-r--r--   0        0        0      796 2023-05-31 04:00:02.925774 langchainplus_sdk-0.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.1rc1/PKG-INFO
```

### Comparing `langchainplus_sdk-0.0.1/README.md` & `langchainplus_sdk-0.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.1/langchainplus_sdk/client.py` & `langchainplus_sdk-0.0.1rc1/langchainplus_sdk/client.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.1/langchainplus_sdk/schemas.py` & `langchainplus_sdk-0.0.1rc1/langchainplus_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.1/langchainplus_sdk/utils.py` & `langchainplus_sdk-0.0.1rc1/langchainplus_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.1/pyproject.toml` & `langchainplus_sdk-0.0.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchainplus-sdk"
-version = "0.0.1"
+version = "0.0.1-rc1"
 description = "Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langchainplus_sdk"}]
 
 [tool.poetry.dependencies]
@@ -31,8 +31,8 @@
   "E",  # pycodestyle
   "F",  # pyflakes
   "I",  # isort
 ]
 
 [tool.mypy]
 ignore_missing_imports = "True"
-disallow_untyped_defs = "True"
+disallow_untyped_defs = "True"
```

### Comparing `langchainplus_sdk-0.0.1/PKG-INFO` & `langchainplus_sdk-0.0.1rc1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchainplus-sdk
-Version: 0.0.1
+Version: 0.0.1rc1
 Summary: Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

