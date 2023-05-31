# Comparing `tmp/openplugin-0.0.1.tar.gz` & `tmp/openplugin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-0.0.1.tar", max compression
+gzip compressed data, was "openplugin-0.0.2.tar", max compression
```

## Comparing `openplugin-0.0.1.tar` & `openplugin-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,13 @@
--rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-25 21:13:03.569284 openplugin-0.0.1/openplugin/__init__.py
--rw-r--r--   0        0        0      414 2023-05-23 20:38:25.155316 openplugin-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7116 1970-01-01 00:00:00.000000 openplugin-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.2/README.md
+-rw-r--r--   0        0        0      659 2023-05-31 17:20:20.388850 openplugin-0.0.2/openplugin/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-31 18:34:59.726797 openplugin-0.0.2/openplugin/__main__.py
+-rw-r--r--   0        0        0      855 2023-05-31 17:18:40.367458 openplugin-0.0.2/openplugin/api/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-23 18:12:55.625523 openplugin-0.0.2/openplugin/api/http_error.py
+-rw-r--r--   0        0        0      873 2023-05-31 17:17:32.611062 openplugin-0.0.2/openplugin/api/imprompt.py
+-rw-r--r--   0        0        0      857 2023-05-31 17:18:40.370699 openplugin-0.0.2/openplugin/api/langchain.py
+-rw-r--r--   0        0        0     8095 2023-05-31 17:14:33.045786 openplugin-0.0.2/openplugin/bindings/imprompt/imprompt_plugin_selector.py
+-rw-r--r--   0        0        0     5322 2023-05-31 17:14:46.276595 openplugin-0.0.2/openplugin/bindings/langchain/langchain_plugin_selector.py
+-rw-r--r--   0        0        0     7329 2023-05-30 21:50:10.184387 openplugin-0.0.2/openplugin/interfaces/plugin_selector.py
+-rw-r--r--   0        0        0      562 2023-05-31 19:01:14.915142 openplugin-0.0.2/openplugin/main.py
+-rw-r--r--   0        0        0      521 2023-05-31 19:01:50.001865 openplugin-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7160 1970-01-01 00:00:00.000000 openplugin-0.0.2/PKG-INFO
```

### Comparing `openplugin-0.0.1/README.md` & `openplugin-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.1/PKG-INFO` & `openplugin-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: openplugin
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.2,<0.96.0)
 Requires-Dist: langchain (>=0.0.178,<0.0.179)
 Requires-Dist: load-dotenv (>=0.1.0,<0.2.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: pydantic (>=1.0.0,<2.0.0)
 Requires-Dist: requests (==2.29.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 ![Alt text](docs/openplugin_logo.jpg?raw=75x75 "Logo")
 #### Do you want to create a plugin?
 
 If you want to create a plugin, this project is NOT FOR YOU.
```

