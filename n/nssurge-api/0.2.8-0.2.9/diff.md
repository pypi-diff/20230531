# Comparing `tmp/nssurge-api-0.2.8.tar.gz` & `tmp/nssurge-api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nssurge-api-0.2.8.tar", max compression
+gzip compressed data, was "nssurge-api-0.2.9.tar", max compression
```

## Comparing `nssurge-api-0.2.8.tar` & `nssurge-api-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1100 2022-05-13 09:10:56.006089 nssurge-api-0.2.8/LICENSE
--rw-r--r--   0        0        0        0 2022-05-13 09:10:48.912889 nssurge-api-0.2.8/README.md
--rw-r--r--   0        0        0       75 2022-05-15 02:25:27.604188 nssurge-api-0.2.8/nssurge_api/__init__.py
--rw-r--r--   0        0        0    10277 2022-05-15 01:51:13.732497 nssurge-api-0.2.8/nssurge_api/api.py
--rw-r--r--   0        0        0     2140 2022-05-14 14:12:39.911453 nssurge-api-0.2.8/nssurge_api/types.py
--rw-r--r--   0        0        0      833 2022-05-15 02:25:27.603458 nssurge-api-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      684 2022-05-15 02:25:31.478816 nssurge-api-0.2.8/setup.py
--rw-r--r--   0        0        0      763 2022-05-15 02:25:31.479288 nssurge-api-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-05-13 09:10:56.006089 nssurge-api-0.2.9/LICENSE
+-rw-r--r--   0        0        0        0 2022-05-13 09:10:48.912889 nssurge-api-0.2.9/README.md
+-rw-r--r--   0        0        0       75 2022-05-15 04:23:30.592184 nssurge-api-0.2.9/nssurge_api/__init__.py
+-rw-r--r--   0        0        0    10364 2022-05-15 04:22:53.673609 nssurge-api-0.2.9/nssurge_api/api.py
+-rw-r--r--   0        0        0     2140 2022-05-14 14:12:39.911453 nssurge-api-0.2.9/nssurge_api/types.py
+-rw-r--r--   0        0        0      833 2022-05-15 04:23:30.591625 nssurge-api-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      684 2022-05-15 04:23:34.774329 nssurge-api-0.2.9/setup.py
+-rw-r--r--   0        0        0      763 2022-05-15 04:23:34.775281 nssurge-api-0.2.9/PKG-INFO
```

### Comparing `nssurge-api-0.2.8/LICENSE` & `nssurge-api-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nssurge-api-0.2.8/nssurge_api/api.py` & `nssurge-api-0.2.9/nssurge_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,19 @@
 # @dataclass
 class SurgeAPIClient:
     """
     Surge HTTP API Client
     https://manual.nssurge.com/others/http-api.html
     """
 
-    def __init__(self, endpoint: str = "http://127.0.0.1:9999", api_key: str = ""):
+    def __init__(self, endpoint: str = "http://127.0.0.1:9999", api_key: str = "", trust_env: bool = False):
         self.endpoint: str = endpoint
         self.api_key: str = api_key
-        self.session: ClientSession = ClientSession()
+        # self.trust_env: bool = trust_env
+        self.session: ClientSession = ClientSession(trust_env=trust_env)
 
     # session: ClientSession
 
     # @classmethod
     # async def create(cls, endpoint, api_key, session):
     # 	return cls(endpoint, api_key, session)
```

### Comparing `nssurge-api-0.2.8/nssurge_api/types.py` & `nssurge-api-0.2.9/nssurge_api/types.py`

 * *Files identical despite different names*

### Comparing `nssurge-api-0.2.8/pyproject.toml` & `nssurge-api-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nssurge-api"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/nssurge-api"
 repository = "https://github.com/tddschn/nssurge-api"
 classifiers = [
```

### Comparing `nssurge-api-0.2.8/setup.py` & `nssurge-api-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.1,<4.0.0', 'typing-extensions>=4.2.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'nssurge-api',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '',
     'long_description': '',
     'author': 'Xinyuan Chen',
     'author_email': '45612704+tddschn@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/tddschn/nssurge-api',
```

### Comparing `nssurge-api-0.2.8/PKG-INFO` & `nssurge-api-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nssurge-api
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Home-page: https://github.com/tddschn/nssurge-api
 License: MIT
 Keywords: nssurge,api
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

