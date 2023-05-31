# Comparing `tmp/together_web3-0.1.5.tar.gz` & `tmp/together_web3-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together_web3-0.1.5.tar", max compression
+gzip compressed data, was "together_web3-0.1.6.tar", max compression
```

## Comparing `together_web3-0.1.5.tar` & `together_web3-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1177 2023-04-28 17:37:40.180065 together_web3-0.1.5/README.md
--rw-r--r--   0        0        0     2806 2023-04-28 17:37:40.180065 together_web3-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/__init__.py
--rw-r--r--   0        0        0      167 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/accounts.py
--rw-r--r--   0        0        0    10298 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/computer.py
--rw-r--r--   0        0        0     1315 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/coordinator.py
--rw-r--r--   0        0        0    13998 2023-04-28 17:37:40.184065 together_web3-0.1.5/together_web3/together.py
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 together_web3-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1177 2023-05-31 15:01:08.033636 together_web3-0.1.6/README.md
+-rw-r--r--   0        0        0     2806 2023-05-31 15:01:08.037636 together_web3-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-05-31 15:01:08.037636 together_web3-0.1.6/together_web3/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-31 15:01:08.037636 together_web3-0.1.6/together_web3/accounts.py
+-rw-r--r--   0        0        0    10298 2023-05-31 15:01:08.037636 together_web3-0.1.6/together_web3/computer.py
+-rw-r--r--   0        0        0     1315 2023-05-31 15:01:08.037636 together_web3-0.1.6/together_web3/coordinator.py
+-rw-r--r--   0        0        0    14060 2023-05-31 15:01:08.037636 together_web3-0.1.6/together_web3/together.py
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 together_web3-0.1.6/PKG-INFO
```

### Comparing `together_web3-0.1.5/README.md` & `together_web3-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `together_web3-0.1.5/pyproject.toml` & `together_web3-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "together-web3"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["together <together@together.xyz>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/togethercomputer/web3.py"
 homepage = "https://github.com/togethercomputer/web3.py"
 keywords = [
```

### Comparing `together_web3-0.1.5/together_web3/computer.py` & `together_web3-0.1.6/together_web3/computer.py`

 * *Files identical despite different names*

### Comparing `together_web3-0.1.5/together_web3/coordinator.py` & `together_web3-0.1.6/together_web3/coordinator.py`

 * *Files identical despite different names*

### Comparing `together_web3-0.1.5/together_web3/together.py` & `together_web3-0.1.6/together_web3/together.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 
 @dataclass
 class TogetherClientOptions:
     connect_timeout: int = 10
     reconnect_delay: int = 2
     reconnect: bool = False
+    websocket_max_size: int = 20000000
 
 
 def asdict_filter_none(x):
     return asdict(x, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
 
 
 def dataclass_replace_none_with_default_values(data_class, data):
@@ -124,15 +125,15 @@
             self._subscription = asyncio.create_task(
                 self._handle_events(f"{rpc_namespace}_subscribe", "events", self._handle_event))
 
     async def _handle_events(self, method: str, event: str, handler: Callable[[Dict[str, Any]], Awaitable[None]]) -> None:
         while True:
             ws = None
             try:
-                ws = await asyncio.wait_for(connect(self.websocket_url, max_size=10000000), self.options.connect_timeout)
+                ws = await asyncio.wait_for(connect(self.websocket_url, max_size=self.options.websocket_max_size), self.options.connect_timeout)
                 await ws.send(f'{{"jsonrpc": "2.0", "id": 1, "method": "{method}", "params": ["{event}"]}}')
                 message = await ws.recv()
                 subscription_response = json.loads(message)
                 self._subscription_id = subscription_response["result"]
                 await self._handle_connect()
                 while True:
                     message = await asyncio.wait_for(ws.recv(), 1073741824)
```

### Comparing `together_web3-0.1.5/PKG-INFO` & `together_web3-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together-web3
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/togethercomputer/web3.py
 License: MIT
 Keywords: NLP,vision,speech,deep,learning,transformer,pytorch,tensorflow,BERT,GPT-2
 Author: together
 Author-email: together@together.xyz
 Requires-Python: >=3.7.2,<3.11
```

