# Comparing `tmp/httplus-0.0.0.tar.gz` & `tmp/httplus-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httplus-0.0.0.tar", max compression
+gzip compressed data, was "httplus-0.1.0.tar", max compression
```

## Comparing `httplus-0.0.0.tar` & `httplus-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-05-28 07:57:55.312570 httplus-0.0.0/LICENSE
--rw-r--r--   0        0        0       37 2023-05-28 08:10:00.266418 httplus-0.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-28 08:07:59.849959 httplus-0.0.0/httplus/__init__.py
--rw-r--r--   0        0        0     3000 2023-05-28 10:03:57.117649 httplus-0.0.0/httplus/client.py
--rw-r--r--   0        0        0     1250 2023-05-28 10:01:08.774733 httplus-0.0.0/httplus/request.py
--rw-r--r--   0        0        0       26 2023-05-28 08:50:51.206044 httplus-0.0.0/httplus/response.py
--rw-r--r--   0        0        0      398 2023-05-29 10:33:33.656659 httplus-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 httplus-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-28 07:57:55.312570 httplus-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1267 2023-05-31 08:40:24.812091 httplus-0.1.0/README.md
+-rw-r--r--   0        0        0       47 2023-05-30 11:55:36.148288 httplus-0.1.0/httplus/__init__.py
+-rw-r--r--   0        0        0     3464 2023-05-30 10:58:20.428873 httplus-0.1.0/httplus/client.py
+-rw-r--r--   0        0        0     1872 2023-05-30 09:13:58.586047 httplus-0.1.0/httplus/request.py
+-rw-r--r--   0        0        0     1161 2023-05-30 09:17:26.535355 httplus-0.1.0/httplus/response.py
+-rw-r--r--   0        0        0      398 2023-05-31 08:38:03.138203 httplus-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 httplus-0.1.0/PKG-INFO
```

### Comparing `httplus-0.0.0/LICENSE` & `httplus-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httplus-0.0.0/httplus/client.py` & `httplus-0.1.0/httplus/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,69 +13,81 @@
 
     def __aenter__(self):
         ...
 
     def __aexit__(self, exc_type, exc_val, exc_tb):
         self.writer.close()
 
-    async def execute(self, host, port, data) -> bytes:
+    async def execute(self, host, port, data) -> Response:
+        context = None
         if self.verify:
             context = ssl.SSLContext(ssl.PROTOCOL_TLS)
             context.load_verify_locations(self.verify)
             context.verify_mode = ssl.CERT_REQUIRED
             context.check_hostname = True
-            self.reader, self.writer = await asyncio.open_connection(host, port, ssl=context)
-        else:
-            self.reader, self.writer = await asyncio.open_connection(host, port)
-        if data:
-            self.writer.write(data.encode())
-        data_res = b''
+        reader, writer = await asyncio.open_connection(host, port, ssl=context)
+        writer.write(data)
+        await writer.drain()
+        response = Response()
+        line = await reader.readline()
+        response.set_controller(line)
         while True:
-            res = await self.reader.read(100)
-            if not res:
+            line = await reader.readline()
+            if not line or line == b'\r\n':
                 break
-            data_res += res
-        self.writer.close()
-        return data_res
+            response.set_header_pair(line)
+        if response.content_length:
+            while True:
+                line = await reader.read(1000)
+                if not line:
+                    break
+                response.body += line
+        writer.close()
+        await writer.wait_closed()
+        return response
 
     async def request(
             self,
             method: str,
             url: str,
             data: ... = None,
             headers: dict = None
     ) -> Response:
+        headers = headers or {}
         req = Request(url=url, method=method, headers=headers)
-        req.body = data or ''
+        req.set_data(data)
         content = req.render()
         res = await self.execute(req.host, req.port, content)
-        response = Response()
-        return response
+        return res
 
     async def get(
             self,
             url: str,
             headers: dict = None
     ) -> Response:
         return await self.request('GET', url, headers=headers)
 
     async def post(
             self,
             url: str,
             data: ... = None,
             headers: dict = None
     ) -> Response:
+        if not data:
+            raise Exception(f'Data must be set!')
         return await self.request('POST', url, data, headers)
 
     async def put(
             self,
             url: str,
             data: ... = None,
             headers: dict = None
     ) -> Response:
+        if not data:
+            raise Exception(f'Data must be set!')
         return await self.request('PUT', url, data, headers)
 
     async def delete(
             self,
             url: str,
             data: ... = None,
             headers: dict = None
@@ -84,14 +96,16 @@
 
     async def patch(
             self,
             url: str,
             data: ... = None,
             headers: dict = None
     ) -> Response:
+        if not data:
+            raise Exception(f'Data must be set!')
         return await self.request('PATCH', url, data, headers)
 
     async def options(
             self,
             url: str,
             data: ... = None,
             headers: dict = None
```

