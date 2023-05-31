# Comparing `tmp/metal_sdk-1.0.4.tar.gz` & `tmp/metal_sdk-1.0.5.tar.gz`

## Comparing `metal_sdk-1.0.4.tar` & `metal_sdk-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/motorhead.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/motorhead_async.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/tests/test_metal.py
--rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/tests/test_metal_async.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/tests/test_motorhead.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/tests/test_motorhead_async.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/motorhead.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/motorhead_async.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/tests/test_metal.py
+-rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/tests/test_metal_async.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/tests/test_motorhead.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/tests/test_motorhead_async.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/PKG-INFO
```

### Comparing `metal_sdk-1.0.4/.github/workflows/publish.yml` & `metal_sdk-1.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/.github/workflows/test.yml` & `metal_sdk-1.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/examples/example.py` & `metal_sdk-1.0.5/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/examples/example_async.py` & `metal_sdk-1.0.5/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/src/metal_sdk/metal.py` & `metal_sdk-1.0.5/src/metal_sdk/metal_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import httpx
 from typing import List
+import httpx
 from .typings import IndexPayload, SearchPayload, TunePayload, BulkIndexItem
 
 
 BASE_API = "https://api.getmetal.io"
 
 
-class Metal(httpx.Client):
+class Metal(httpx.AsyncClient):
     api_key: str
     client_id: str
     index_id: str
 
     def __init__(self, api_key, client_id, index_id=None, base_url=BASE_API):
         super().__init__()
         self.api_key = api_key
@@ -19,16 +19,16 @@
         self.headers.update({
             'Content-Type': 'application/json',
             'x-metal-api-key': self.api_key,
             'x-metal-client-id': self.client_id,
         })
         self.base_url = base_url
 
-    def request(self, method, url, *args, **kwargs):
-        return super().request(method, url, *args, **kwargs)
+    async def request(self, method, url, *args, **kwargs):
+        return await super().request(method, url, *args, **kwargs)
 
     def __getData(self, index, payload: dict = {}):
         data = {"index": index}
         if payload.get("id") is not None:
             data["id"] = payload["id"]
 
         if payload.get("metadata") is not None:
@@ -56,49 +56,49 @@
             payload.get("imageBase64") is None
             and payload.get("imageUrl") is None
             and payload.get("text") is None
             and payload.get("embedding") is None
         ):
             raise TypeError("imageBase64, imageUrl, text, or embedding required")
 
-    def index(self, payload: IndexPayload = {}, index_id=None):
+    async def index(self, payload: IndexPayload = {}, index_id=None):
         index = self.index_id or index_id
         self.__validateIndexAndSearch(index, payload)
         data = self.__getData(index, payload)
         url = "/v1/index"
 
-        res = self.request("post", url, json=data)
+        res = await self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
-    def index_many(self, payload: List[BulkIndexItem]):
+    async def index_many(self, payload: List[BulkIndexItem]):
         url = "/v1/index/bulk"
         data = {"data": payload}
+        res = await self.request("post", url, json=data)
 
-        res = self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
-    def search(
+    async def search(
         self, payload: SearchPayload = {}, index_id=None, ids_only=False, limit=1
     ):
         index = index_id or self.index_id
         self.__validateIndexAndSearch(index, payload)
         data = self.__getData(index, payload)
 
         url = "/v1/search?limit=" + str(limit)
 
         if ids_only:
             url = url + "&idsOnly=true"
 
-        res = self.request("post", url, json=data)
+        res = await self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
-    def tune(self, payload: TunePayload = {}, index_id=None):
+    async def tune(self, payload: TunePayload = {}, index_id=None):
         index = index_id or self.index_id
 
         if index is None:
             raise TypeError("index_id required")
 
         idA = payload.get("idA")
         idB = payload.get("idB")
@@ -106,40 +106,50 @@
 
         if idA is None or idB is None or label is None:
             raise TypeError("idA, idB, and label required")
 
         url = "/v1/tune"
         data = {"index": index, "idA": idA, "idB": idB, "label": label}
 
-        res = self.request("post", url, json=data)
+        res = await self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
-    def get_one(self, id: str, index_id=None):
+    async def get_one(self, id: str, index_id=None):
+        index = index_id or self.index_id
+
         if id is None:
             raise TypeError("id required")
 
-        url = "/v1/documents/" + id
+        if index is None:
+            raise TypeError("index_id required")
+
+        url = "/v1/indexes/" + index + "/documents/" + id
 
-        res = self.request("get", url)
+        res = await self.request("get", url)
         res.raise_for_status()
         return res.json()
 
-    def delete_one(self, id: str, index_id=None):
+    async def delete_one(self, id: str, index_id=None):
+        index = index_id or self.index_id
+
         if id is None:
             raise TypeError("id required")
 
-        url = "/v1/documents/" + id
+        if index is None:
+            raise TypeError("index_id required")
+
+        url = "/v1/indexes/" + index + "/documents/" + id
 
-        res = self.request("delete", url)
+        res = await self.request("delete", url)
         res.raise_for_status()
         return res.json()
 
-    def delete_many(self, ids: List[str], index_id=None):
+    async def delete_many(self, ids: List[str]):
         if ids is None:
             raise TypeError("ids required")
 
         url = "/v1/documents/bulk"
 
-        res = self.request("delete", url, json={"ids": ids})
+        res = await self.request("delete", url, json={"ids": ids})
         res.raise_for_status()
         return res.json()
```

### Comparing `metal_sdk-1.0.4/src/metal_sdk/metal_async.py` & `metal_sdk-1.0.5/src/metal_sdk/metal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import List
 import httpx
+from typing import List
 from .typings import IndexPayload, SearchPayload, TunePayload, BulkIndexItem
 
 
 BASE_API = "https://api.getmetal.io"
 
 
-class Metal(httpx.AsyncClient):
+class Metal(httpx.Client):
     api_key: str
     client_id: str
     index_id: str
 
     def __init__(self, api_key, client_id, index_id=None, base_url=BASE_API):
         super().__init__()
         self.api_key = api_key
@@ -19,16 +19,16 @@
         self.headers.update({
             'Content-Type': 'application/json',
             'x-metal-api-key': self.api_key,
             'x-metal-client-id': self.client_id,
         })
         self.base_url = base_url
 
-    async def request(self, method, url, *args, **kwargs):
-        return await super().request(method, url, *args, **kwargs)
+    def request(self, method, url, *args, **kwargs):
+        return super().request(method, url, *args, **kwargs)
 
     def __getData(self, index, payload: dict = {}):
         data = {"index": index}
         if payload.get("id") is not None:
             data["id"] = payload["id"]
 
         if payload.get("metadata") is not None:
@@ -56,49 +56,49 @@
             payload.get("imageBase64") is None
             and payload.get("imageUrl") is None
             and payload.get("text") is None
             and payload.get("embedding") is None
         ):
             raise TypeError("imageBase64, imageUrl, text, or embedding required")
 
-    async def index(self, payload: IndexPayload = {}, index_id=None):
+    def index(self, payload: IndexPayload = {}, index_id=None):
         index = self.index_id or index_id
         self.__validateIndexAndSearch(index, payload)
         data = self.__getData(index, payload)
         url = "/v1/index"
 
-        res = await self.request("post", url, json=data)
+        res = self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
-    async def index_many(self, payload: List[BulkIndexItem]):
+    def index_many(self, payload: List[BulkIndexItem]):
         url = "/v1/index/bulk"
         data = {"data": payload}
-        res = await self.request("post", url, json=data)
 
+        res = self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
-    async def search(
+    def search(
         self, payload: SearchPayload = {}, index_id=None, ids_only=False, limit=1
     ):
         index = index_id or self.index_id
         self.__validateIndexAndSearch(index, payload)
         data = self.__getData(index, payload)
 
         url = "/v1/search?limit=" + str(limit)
 
         if ids_only:
             url = url + "&idsOnly=true"
 
-        res = await self.request("post", url, json=data)
+        res = self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
-    async def tune(self, payload: TunePayload = {}, index_id=None):
+    def tune(self, payload: TunePayload = {}, index_id=None):
         index = index_id or self.index_id
 
         if index is None:
             raise TypeError("index_id required")
 
         idA = payload.get("idA")
         idB = payload.get("idB")
@@ -106,40 +106,50 @@
 
         if idA is None or idB is None or label is None:
             raise TypeError("idA, idB, and label required")
 
         url = "/v1/tune"
         data = {"index": index, "idA": idA, "idB": idB, "label": label}
 
-        res = await self.request("post", url, json=data)
+        res = self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
-    async def get_one(self, id: str):
+    def get_one(self, id: str, index_id=None):
+        index = index_id or self.index_id
+
         if id is None:
             raise TypeError("id required")
 
-        url = "/v1/documents/" + id
+        if index is None:
+            raise TypeError("index_id required")
+
+        url = "/v1/indexes/" + index + "/documents/" + id
 
-        res = await self.request("get", url)
+        res = self.request("get", url)
         res.raise_for_status()
         return res.json()
 
-    async def delete_one(self, id: str):
+    def delete_one(self, id: str, index_id=None):
+        index = index_id or self.index_id
+
         if id is None:
             raise TypeError("id required")
 
-        url = "/v1/documents/" + id
+        if index is None:
+            raise TypeError("index_id required")
+
+        url = "/v1/indexes/" + index + "/documents/" + id
 
-        res = await self.request("delete", url)
+        res = self.request("delete", url)
         res.raise_for_status()
         return res.json()
 
-    async def delete_many(self, ids: List[str]):
+    def delete_many(self, ids: List[str], index_id=None):
         if ids is None:
             raise TypeError("ids required")
 
         url = "/v1/documents/bulk"
 
-        res = await self.request("delete", url, json={"ids": ids})
+        res = self.request("delete", url, json={"ids": ids})
         res.raise_for_status()
         return res.json()
```

### Comparing `metal_sdk-1.0.4/src/metal_sdk/motorhead.py` & `metal_sdk-1.0.5/src/metal_sdk/motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/src/metal_sdk/motorhead_async.py` & `metal_sdk-1.0.5/src/metal_sdk/motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/src/metal_sdk/typings.py` & `metal_sdk-1.0.5/src/metal_sdk/typings.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/tests/test_metal.py` & `metal_sdk-1.0.5/tests/test_metal.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,28 +147,28 @@
         metal = Metal(API_KEY, CLIENT_ID, index_id)
         return_value = mock.MagicMock(json=lambda: {"ozzy": "black sabbath"})
         metal.request = mock.MagicMock(return_value=return_value)
 
         metal.get_one(id)
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "get")
-        self.assertEqual(metal.request.call_args[0][1], "/v1/documents/ozzy")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/indexes/index-id/documents/ozzy")
 
     def test_metal_delete_one_with_payload(self):
         index_id = "index-id"
         id = "ozzy"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
         return_value = mock.MagicMock(json=lambda: {"ozzy": "black sabbath"})
         metal.request = mock.MagicMock(return_value=return_value)
 
         metal.delete_one(id)
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
-        self.assertEqual(metal.request.call_args[0][1], "/v1/documents/ozzy")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/indexes/index-id/documents/ozzy")
 
     def test_metal_delete_many_with_payload(self):
         index_id = "index-id"
         id = "ozzy"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
         return_value = mock.MagicMock(json=lambda: {"ozzy": "black sabbath"})
         metal.request = mock.MagicMock(return_value=return_value)
```

### Comparing `metal_sdk-1.0.4/tests/test_metal_async.py` & `metal_sdk-1.0.5/tests/test_metal_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,27 +147,27 @@
         metal = Metal(API_KEY, CLIENT_ID, index_id)
         return_value = mock.MagicMock(json=lambda: {"band": "Megadeth"})
         metal.request = mock.MagicMock(return_value=return_value)
 
         await metal.get_one(id)
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "get")
-        self.assertEqual(metal.request.call_args[0][1], "/v1/documents/dave")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/indexes/index-id/documents/dave")
 
     async def test_metal_delete_one_with_payload(self):
         index_id = "index-id"
         id = "dave"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
         return_value = mock.MagicMock(json=lambda: {"band": "Megadeth"})
         metal.request = mock.MagicMock(return_value=return_value)
 
         await metal.get_one(id)
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
-        self.assertEqual(metal.request.call_args[0][1], "/v1/documents/dave")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/indexes/index-id/documents/dave")
 
     async def test_metal_delete_many_with_payload(self):
         index_id = "index-id"
         id = "ozzy"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
         return_value = mock.MagicMock(json=lambda: {"ozzy": "black sabbath"})
         metal.request = mock.MagicMock(return_value=return_value)
```

### Comparing `metal_sdk-1.0.4/tests/test_motorhead.py` & `metal_sdk-1.0.5/tests/test_motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/tests/test_motorhead_async.py` & `metal_sdk-1.0.5/tests/test_motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/.gitignore` & `metal_sdk-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/LICENSE` & `metal_sdk-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/README.md` & `metal_sdk-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.4/pyproject.toml` & `metal_sdk-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `metal_sdk-1.0.4/PKG-INFO` & `metal_sdk-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

