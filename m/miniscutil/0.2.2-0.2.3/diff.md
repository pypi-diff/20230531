# Comparing `tmp/miniscutil-0.2.2.tar.gz` & `tmp/miniscutil-0.2.3.tar.gz`

## Comparing `miniscutil-0.2.2.tar` & `miniscutil-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/__about__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/adapt.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/config.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/deepeq.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/dispatch.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/misc.py
--rw-r--r--   0        0        0    13847 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/sum.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/type_util.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/README.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/__init__.py
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/document.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/server.py
--rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/types.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/__init__.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/extrarpc.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/io_transport.py
--rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/jsonrpc.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/starlette_ws_transport.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/transport.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/websocket_transport.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_classdispatch.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_config.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_deepeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_humansize.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_lsp.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_ofdict.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_typing.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.2/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.2/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/__about__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/misc.py
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/sum.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/type_util.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/README.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/__init__.py
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/document.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/server.py
+-rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/__init__.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/extrarpc.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/io_transport.py
+-rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/websocket_transport.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_humansize.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_lsp.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.3/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.3/PKG-INFO
```

### Comparing `miniscutil-0.2.2/miniscutil/__init__.py` & `miniscutil-0.2.3/miniscutil/__init__.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/adapt.py` & `miniscutil-0.2.3/miniscutil/adapt.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/asyncio_helpers.py` & `miniscutil-0.2.3/miniscutil/asyncio_helpers.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/config.py` & `miniscutil-0.2.3/miniscutil/config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/current.py` & `miniscutil-0.2.3/miniscutil/current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/deep.py` & `miniscutil-0.2.3/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/deepeq.py` & `miniscutil-0.2.3/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/dispatch.py` & `miniscutil-0.2.3/miniscutil/dispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/misc.py` & `miniscutil-0.2.3/miniscutil/misc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/ofdict.py` & `miniscutil-0.2.3/miniscutil/ofdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,23 +47,23 @@
 
 
 def ofdict_dataclass(A: Type[T], a: JsonLike) -> T:
     assert is_dataclass(A)
     d2 = {}
     for f in fields(A):
         if not isinstance(a, dict):
-            raise TypeError(
+            raise OfDictError(
                 f"Error while decoding dataclass {A}, expected a dict but got {a} : {type(a)}"
             )
         k = f.name
         if k not in a:
             if f.type is not None and is_optional(f.type):
                 v = None
             else:
-                raise ValueError(
+                raise OfDictError(
                     f"Missing {f.name} on input dict. Decoding {a} to type {A}."
                 )
         else:
             v = a[k]
         if f.type is not None:
             with dpath(k):
                 d2[k] = ofdict(f.type, v)
```

### Comparing `miniscutil-0.2.2/miniscutil/sum.py` & `miniscutil-0.2.3/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/type_util.py` & `miniscutil-0.2.3/miniscutil/type_util.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/lsp/document.py` & `miniscutil-0.2.3/miniscutil/lsp/document.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/lsp/server.py` & `miniscutil-0.2.3/miniscutil/lsp/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
         kwargs: Any = dict(before=document, after=document_after, changes=params)
 
         callbacks: list[Any] = [
             callback(**kwargs) for callback in self.change_callbacks[item_id.uri]
         ]
         callbacks.append(self.on_change(**kwargs))
-        await asyncio.wait(callbacks)
+        await asyncio.wait(map(asyncio.ensure_future, callbacks))
 
     def register_change_callback(self, callback, uri: lsp.DocumentUri):
         """Register a callback to be called when the document changes"""
         self.change_callbacks[uri].add(callback)
 
     async def on_change(
         self,
```

### Comparing `miniscutil-0.2.2/miniscutil/lsp/types.py` & `miniscutil-0.2.3/miniscutil/lsp/types.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/rpc/extrarpc.py` & `miniscutil-0.2.3/miniscutil/rpc/extrarpc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/rpc/io_transport.py` & `miniscutil-0.2.3/miniscutil/rpc/io_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/rpc/jsonrpc.py` & `miniscutil-0.2.3/miniscutil/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/rpc/starlette_ws_transport.py` & `miniscutil-0.2.3/miniscutil/rpc/starlette_ws_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/rpc/transport.py` & `miniscutil-0.2.3/miniscutil/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/miniscutil/rpc/websocket_transport.py` & `miniscutil-0.2.3/miniscutil/rpc/websocket_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/tests/test_classdispatch.py` & `miniscutil-0.2.3/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/tests/test_config.py` & `miniscutil-0.2.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/tests/test_current.py` & `miniscutil-0.2.3/tests/test_current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/tests/test_deepeq.py` & `miniscutil-0.2.3/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/tests/test_lsp.py` & `miniscutil-0.2.3/tests/test_lsp.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/tests/test_ofdict.py` & `miniscutil-0.2.3/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/tests/test_typing.py` & `miniscutil-0.2.3/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/.gitignore` & `miniscutil-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/LICENSE.txt` & `miniscutil-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/README.md` & `miniscutil-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/pyproject.toml` & `miniscutil-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.2/PKG-INFO` & `miniscutil-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.2.2
+Version: 0.2.3
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

