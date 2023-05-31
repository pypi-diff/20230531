# Comparing `tmp/miniscutil-0.2.3.tar.gz` & `tmp/miniscutil-0.2.4.tar.gz`

## Comparing `miniscutil-0.2.3.tar` & `miniscutil-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/__about__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/adapt.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/config.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/deepeq.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/dispatch.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/misc.py
--rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/sum.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/type_util.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/README.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/__init__.py
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/document.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/server.py
--rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/lsp/types.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/__init__.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/extrarpc.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/io_transport.py
--rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/jsonrpc.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/starlette_ws_transport.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/transport.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.3/miniscutil/rpc/websocket_transport.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_classdispatch.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_config.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_deepeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_humansize.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_lsp.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_ofdict.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_typing.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/test_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.3/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.3/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.3/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/__about__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/misc.py
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/sum.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/type_util.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/README.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/__init__.py
+-rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/document.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/server.py
+-rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/__init__.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/extrarpc.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/io_transport.py
+-rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.4/miniscutil/rpc/websocket_transport.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_humansize.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_lsp.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.4/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.4/LICENSE.txt
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.4/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.4/PKG-INFO
```

### Comparing `miniscutil-0.2.3/miniscutil/__init__.py` & `miniscutil-0.2.4/miniscutil/__init__.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/adapt.py` & `miniscutil-0.2.4/miniscutil/adapt.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/asyncio_helpers.py` & `miniscutil-0.2.4/miniscutil/asyncio_helpers.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/config.py` & `miniscutil-0.2.4/miniscutil/config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/current.py` & `miniscutil-0.2.4/miniscutil/current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/deep.py` & `miniscutil-0.2.4/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/deepeq.py` & `miniscutil-0.2.4/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/dispatch.py` & `miniscutil-0.2.4/miniscutil/dispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/misc.py` & `miniscutil-0.2.4/miniscutil/misc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/ofdict.py` & `miniscutil-0.2.4/miniscutil/ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/sum.py` & `miniscutil-0.2.4/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/type_util.py` & `miniscutil-0.2.4/miniscutil/type_util.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/lsp/document.py` & `miniscutil-0.2.4/miniscutil/lsp/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import contextlib
 from contextvars import ContextVar
 from dataclasses import dataclass, replace
 from enum import Enum
 import functools
 import itertools
 from typing import Iterable, Optional, Union
+
 try:
     from typing import TypeAlias, TypeVar
 except:
     from typing_extensions import TypeAlias, TypeVar
 from miniscutil.misc import set_ctx
 
 
@@ -52,17 +53,24 @@
     @classmethod
     def of_offset(cls, offset: int):
         return document_context.get().offset_to_position(offset)
 
     def to_offset(self):
         return document_context.get().position_to_offset(self)
 
-    def __add__(self, offset: int):
-        assert isinstance(offset, int)
-        return document_context.get().add_position(self, offset)
+    def __add__(self, offset: Union[int, tuple[int, int]]):
+        if isinstance(offset, int):
+            return document_context.get().add_position(self, offset)
+        elif isinstance(offset, tuple):
+            line, col = offset
+            return replace(self, self.line + line, self.character + col)
+        else:
+            raise TypeError(
+                f"unsupported operand type(s) for +: 'Position' and '{type(offset)}'"
+            )
 
     def __le__(self, other: "Position"):
         assert isinstance(other, Position)
         return (self.line, self.character) <= (other.line, other.character)
 
     def __eq__(self, other: "Position"):
         assert isinstance(other, Position)
@@ -160,21 +168,30 @@
         assert len(lines) > 0
         offsets = list(cumsum(map(len, lines)))
         assert len(offsets) == len(lines)
         assert offsets[-1] == len(self.text)
         assert offsets[0] == len(lines[0])
         return offsets
 
+    def get_line_start_offset(self, line_index: int) -> int:
+        if line_index == 0:
+            return 0
+        if line_index >= self.line_count:
+            return len(self.text)
+        return self.line_offsets[line_index - 1]
+
+    def get_line_end_offset(self, line_index: int) -> int:
+        if line_index >= self.line_count:
+            return len(self.text)
+        return self.line_offsets[line_index]
+
     def get_line(self, index: int) -> str:
-        if index == 0:
-            return self.text[: self.line_offsets[0]]
-        elif index >= self.line_count:
-            return self.text[self.line_offsets[-2] :]
-        else:
-            return self.text[self.line_offsets[index - 1] : self.line_offsets[index]]
+        return self.text[
+            self.get_line_start_offset(index) : self.get_line_end_offset(index)
+        ]
 
     @property
     def position_encoding(self):
         return position_encoding_context.get()
 
     def position_to_offset(self, position: Position):
         s = self.line_offsets
```

### Comparing `miniscutil-0.2.3/miniscutil/lsp/server.py` & `miniscutil-0.2.4/miniscutil/lsp/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 logger = logging.getLogger("LSP")
 
 
 class LspServer(ExtraRpc):
     capabilities: ServerCapabilities
     position_encoding = "utf-16"
+    # [todo] consider using io.StringIO for the documents because they are mutating.
     documents: dict[lsp.DocumentUri, lsp.TextDocumentItem]
     change_callbacks: defaultdict[lsp.DocumentUri, set[Callable]]
     """ set of open documents, the server will keep these synced with the client
      editor automatically. """
 
     def __init__(self, transport):
         self.change_callbacks = defaultdict(set)
```

### Comparing `miniscutil-0.2.3/miniscutil/lsp/types.py` & `miniscutil-0.2.4/miniscutil/lsp/types.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/rpc/extrarpc.py` & `miniscutil-0.2.4/miniscutil/rpc/extrarpc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/rpc/io_transport.py` & `miniscutil-0.2.4/miniscutil/rpc/io_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/rpc/jsonrpc.py` & `miniscutil-0.2.4/miniscutil/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/rpc/starlette_ws_transport.py` & `miniscutil-0.2.4/miniscutil/rpc/starlette_ws_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/rpc/transport.py` & `miniscutil-0.2.4/miniscutil/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/miniscutil/rpc/websocket_transport.py` & `miniscutil-0.2.4/miniscutil/rpc/websocket_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/tests/test_classdispatch.py` & `miniscutil-0.2.4/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/tests/test_config.py` & `miniscutil-0.2.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/tests/test_current.py` & `miniscutil-0.2.4/tests/test_current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/tests/test_deepeq.py` & `miniscutil-0.2.4/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/tests/test_lsp.py` & `miniscutil-0.2.4/tests/test_lsp.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/tests/test_ofdict.py` & `miniscutil-0.2.4/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/tests/test_typing.py` & `miniscutil-0.2.4/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/.gitignore` & `miniscutil-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/LICENSE.txt` & `miniscutil-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/README.md` & `miniscutil-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/pyproject.toml` & `miniscutil-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.3/PKG-INFO` & `miniscutil-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.2.3
+Version: 0.2.4
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

