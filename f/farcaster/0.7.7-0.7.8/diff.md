# Comparing `tmp/farcaster-0.7.7.tar.gz` & `tmp/farcaster-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "farcaster-0.7.7.tar", max compression
+gzip compressed data, was "farcaster-0.7.8.tar", max compression
```

## Comparing `farcaster-0.7.7.tar` & `farcaster-0.7.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2023-04-09 17:35:25.675298 farcaster-0.7.7/LICENSE
--rw-r--r--   0        0        0     4755 2023-04-09 17:35:25.675298 farcaster-0.7.7/README.md
--rw-r--r--   0        0        0      479 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/__init__.py
--rw-r--r--   0        0        0    37303 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/client.py
--rw-r--r--   0        0        0      516 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/config.py
--rw-r--r--   0        0        0    14393 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/models.py
--rw-r--r--   0        0        0        0 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/py.typed
--rw-r--r--   0        0        0        0 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/utils/__init__.py
--rw-r--r--   0        0        0     4797 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/utils/stream_generator.py
--rw-r--r--   0        0        0     3985 2023-04-09 17:35:25.679298 farcaster-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     6228 1970-01-01 00:00:00.000000 farcaster-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-31 20:18:35.497591 farcaster-0.7.8/LICENSE
+-rw-r--r--   0        0        0     4807 2023-05-31 20:18:35.497591 farcaster-0.7.8/README.md
+-rw-r--r--   0        0        0      479 2023-05-31 20:18:35.497591 farcaster-0.7.8/farcaster/__init__.py
+-rw-r--r--   0        0        0    37303 2023-05-31 20:18:35.497591 farcaster-0.7.8/farcaster/client.py
+-rw-r--r--   0        0        0      516 2023-05-31 20:18:35.497591 farcaster-0.7.8/farcaster/config.py
+-rw-r--r--   0        0        0    15088 2023-05-31 20:18:35.497591 farcaster-0.7.8/farcaster/models.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:18:35.497591 farcaster-0.7.8/farcaster/py.typed
+-rw-r--r--   0        0        0        0 2023-05-31 20:18:35.497591 farcaster-0.7.8/farcaster/utils/__init__.py
+-rw-r--r--   0        0        0     4797 2023-05-31 20:18:35.497591 farcaster-0.7.8/farcaster/utils/stream_generator.py
+-rw-r--r--   0        0        0     3994 2023-05-31 20:18:35.501591 farcaster-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     6081 1970-01-01 00:00:00.000000 farcaster-0.7.8/PKG-INFO
```

### Comparing `farcaster-0.7.7/LICENSE` & `farcaster-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `farcaster-0.7.7/README.md` & `farcaster-0.7.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 To use the Warpcast API you need to have a Farcaster account. We will use the mnemonic or private key of the Farcaster custody account (not your main wallet) to connect to the API.
 
 First, save your Farcaster mnemonic or private key to a `.env` file. Now you can initialize the client, and automatically connect to the Farcaster API!
 
 ```python
 import os
 from farcaster import Warpcast
-from dotenv import load_dotenv
+from dotenv import load_dotenv # can be installed with `pip install python-dotenv`
 
 load_dotenv()
 
 client = Warpcast(mnemonic=os.environ.get("<MNEMONIC_ENV_VAR>"))
 
 print(client.get_healthcheck())
 ```
```

### Comparing `farcaster-0.7.7/farcaster/client.py` & `farcaster-0.7.8/farcaster/client.py`

 * *Files identical despite different names*

### Comparing `farcaster-0.7.7/farcaster/config.py` & `farcaster-0.7.8/farcaster/config.py`

 * *Files identical despite different names*

### Comparing `farcaster-0.7.7/farcaster/models.py` & `farcaster-0.7.8/farcaster/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,23 +225,57 @@
 
 class ViewerContext2(BaseModel):
     reacted: Optional[bool] = None
     recast: Optional[bool] = None
     watched: Optional[bool] = None
 
 
+class ParentSource(BaseModel):
+    type: str
+    url: str
+
+
+class ApiCastUrlEmbed(BaseModel):
+    type: str
+    open_graph: ApiOpenGraphMetadata
+    user: Optional[ApiUser]
+    asset: Optional[ApiAsset]
+    collection: Optional[ApiAssetCollection]
+
+
+class ApiCastImageEmbed(BaseModel):
+    type: str
+    url: str
+    sourceUrl: str
+    alt: str
+
+
+class ApiCastUnknownEmbed(BaseModel):
+    type: str
+    source: str
+
+
+class ApiCastEmbeds(BaseModel):
+    images: List[ApiCastImageEmbed]
+    urls: List[ApiCastUrlEmbed]
+    unknowns: List[ApiCastUnknownEmbed]
+
+
 class ApiCast(BaseModel):
     hash: str
     thread_hash: NoneStr
     parent_hash: NoneStr
     author: ApiUser
+    parent_author: Optional[ApiUser] = None
+    parent_source: Optional[ParentSource] = None
     text: str
     timestamp: PositiveInt
     mentions: Optional[List[ApiUser]] = None
     attachments: Optional[ApiCastAttachments] = None
+    embeds: Optional[ApiCastEmbeds] = None
     ancestors: Optional[Ancestors] = None
     replies: Replies
     reactions: Reactions
     recasts: Recasts
     watches: Watches
     deleted: Optional[bool] = None
     recast: Optional[bool] = None
```

### Comparing `farcaster-0.7.7/farcaster/utils/stream_generator.py` & `farcaster-0.7.8/farcaster/utils/stream_generator.py`

 * *Files identical despite different names*

### Comparing `farcaster-0.7.7/pyproject.toml` & `farcaster-0.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "farcaster"
-version = "0.7.7"
+version = "0.7.8"
 description = "farcaster-py is a Python SDK for the Farcaster Protocol"
 readme = "README.md"
 authors = ["Andreessen Horowitz <crypto-engineering@a16z.com>"]
 license = "MIT"
 repository = "https://github.com/a16z/farcaster-py"
 homepage = "https://github.com/a16z/farcaster-py"
 
@@ -60,15 +60,15 @@
 pytest-html = "^3.1.1"
 pytest-cov = "^4.0.0"
 pytest-recording = "^0.12.1"
 docconvert = "^2.0.0"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.0.5"
 mkdocstrings = ">=0.19.1,<0.22.0"
-mkdocstrings-python = "^0.8.3"
+mkdocstrings-python = ">=0.8.3,<0.11.0"
 pillow = "^9.4.0"
 cairosvg = "^2.6.0"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py310"]
 line-length = 88
```

### Comparing `farcaster-0.7.7/PKG-INFO` & `farcaster-0.7.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: farcaster
-Version: 0.7.7
+Version: 0.7.8
 Summary: farcaster-py is a Python SDK for the Farcaster Protocol
 Home-page: https://github.com/a16z/farcaster-py
 License: MIT
 Author: Andreessen Horowitz
 Author-email: crypto-engineering@a16z.com
 Requires-Python: >3.7.1,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: canonicaljson (>=1.6.4,<3.0.0)
 Requires-Dist: eth-account (>=0.8.0,<0.9.0)
 Requires-Dist: importlib_metadata (>=4.5.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: parsimonious (>=0.8.1,<0.10.0)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: pyhumps (>=3.7.2,<4.0.0)
@@ -72,15 +68,15 @@
 To use the Warpcast API you need to have a Farcaster account. We will use the mnemonic or private key of the Farcaster custody account (not your main wallet) to connect to the API.
 
 First, save your Farcaster mnemonic or private key to a `.env` file. Now you can initialize the client, and automatically connect to the Farcaster API!
 
 ```python
 import os
 from farcaster import Warpcast
-from dotenv import load_dotenv
+from dotenv import load_dotenv # can be installed with `pip install python-dotenv`
 
 load_dotenv()
 
 client = Warpcast(mnemonic=os.environ.get("<MNEMONIC_ENV_VAR>"))
 
 print(client.get_healthcheck())
 ```
```

