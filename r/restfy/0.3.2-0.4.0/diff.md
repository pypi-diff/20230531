# Comparing `tmp/restfy-0.3.2.tar.gz` & `tmp/restfy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restfy-0.3.2.tar", max compression
+gzip compressed data, was "restfy-0.4.0.tar", max compression
```

## Comparing `restfy-0.3.2.tar` & `restfy-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1071 2022-04-20 08:46:49.388615 restfy-0.3.2/LICENSE
--rw-r--r--   0        0        0     3778 2022-04-20 09:19:13.685984 restfy-0.3.2/README.md
--rw-r--r--   0        0        0      399 2022-09-17 15:30:10.516961 restfy-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      224 2022-09-17 15:28:17.721482 restfy-0.3.2/restfy/__init__.py
--rw-r--r--   0        0        0     3706 2022-09-17 15:28:17.722126 restfy-0.3.2/restfy/application.py
--rw-r--r--   0        0        0      391 2022-04-20 08:46:49.389472 restfy-0.3.2/restfy/file.py
--rw-r--r--   0        0        0      145 2022-04-20 08:46:49.389649 restfy-0.3.2/restfy/http/__init__.py
--rw-r--r--   0        0        0      855 2022-04-20 08:46:49.389772 restfy-0.3.2/restfy/http/cors.py
--rw-r--r--   0        0        0     3415 2022-04-20 08:46:49.389908 restfy-0.3.2/restfy/http/request.py
--rw-r--r--   0        0        0     2454 2022-09-17 15:28:17.722483 restfy-0.3.2/restfy/http/response.py
--rw-r--r--   0        0        0      347 2022-09-17 15:28:17.724041 restfy-0.3.2/restfy/middleware.py
--rw-r--r--   0        0        0     5356 2022-09-17 15:28:38.802933 restfy-0.3.2/restfy/router.py
--rw-r--r--   0        0        0      439 2022-09-17 15:28:17.724619 restfy-0.3.2/restfy/server.py
--rw-r--r--   0        0        0     4509 1970-01-01 00:00:00.000000 restfy-0.3.2/setup.py
--rw-r--r--   0        0        0     4316 1970-01-01 00:00:00.000000 restfy-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 09:49:25.883825 restfy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4564 2023-05-31 10:31:39.962791 restfy-0.4.0/README.md
+-rw-r--r--   0        0        0      514 2023-05-31 09:32:27.497218 restfy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-05-27 10:05:30.008092 restfy-0.4.0/restfy/__init__.py
+-rw-r--r--   0        0        0     5863 2023-05-27 10:08:18.948024 restfy-0.4.0/restfy/application.py
+-rw-r--r--   0        0        0        0 2023-05-27 10:08:18.940024 restfy-0.4.0/restfy/cors.py
+-rw-r--r--   0        0        0      391 2023-05-04 09:49:25.883825 restfy-0.4.0/restfy/file.py
+-rw-r--r--   0        0        0     2098 2023-05-27 10:14:12.191194 restfy-0.4.0/restfy/handler.py
+-rw-r--r--   0        0        0     1189 2023-05-31 10:31:39.954791 restfy-0.4.0/restfy/http.py
+-rw-r--r--   0        0        0      343 2023-05-27 10:05:30.012091 restfy-0.4.0/restfy/middleware.py
+-rw-r--r--   0        0        0     4176 2023-05-27 11:38:52.551360 restfy-0.4.0/restfy/request.py
+-rw-r--r--   0        0        0     3025 2023-05-23 11:15:26.608705 restfy-0.4.0/restfy/response.py
+-rw-r--r--   0        0        0     5316 2023-05-27 10:05:30.004091 restfy-0.4.0/restfy/router.py
+-rw-r--r--   0        0        0     1036 2023-05-27 10:35:29.074926 restfy-0.4.0/restfy/server.py
+-rw-r--r--   0        0        0     1970 2023-05-24 11:35:36.204879 restfy-0.4.0/restfy/testing.py
+-rw-r--r--   0        0        0      724 2023-05-04 09:49:25.883825 restfy-0.4.0/restfy/websocket.py
+-rw-r--r--   0        0        0     5181 1970-01-01 00:00:00.000000 restfy-0.4.0/PKG-INFO
```

### Comparing `restfy-0.3.2/LICENSE` & `restfy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `restfy-0.3.2/README.md` & `restfy-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -153,8 +153,38 @@
 
 
 app = Application()
 app.register_middleware(DefaultMiddleware)
 
 ```
 
+### HTTP client requests
+With http module, you can realize asynchronous requests to other services.
+The most simple request can be seen below.
+```python
+from restfy import http
+...
+res = await http.get('https://someserver.api/endpoint')
+print(res.status)
+# 200
+```
+In addition to the get function, others functions are available like 
+post(), put(), delete() and patch(). 
+If other request method are necessary, we can use request() function passing method param.
+The next example shows a more complex example.
+```python
+from restfy import http
 
+...
+url = 'https://someserver.api/endpoint'
+data = {
+    'name': 'Nick',
+    'surname': 'Lauda'
+}
+headers = {
+    'Content-Type': 'application/json'
+}
+...
+res = await http.post(url=url, data=data, headers=headers)
+print(res.status)
+# 200
+```
```

### Comparing `restfy-0.3.2/restfy/http/request.py` & `restfy-0.4.0/restfy/response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,101 @@
 import json
-from restfy.file import File
-
-
-class Request:
-    def __init__(self, method, version):
-        self.app = None
-        self.method = method
-        self.url = ''
-        self.version = version
-        self.body = None
-        self.type = ''
-        self.query = ''
-        self.length = 0
+import datetime
+import decimal
+from typing import Any
+
+status_title = {
+    101: 'Switching Protocols',
+    200: 'OK',
+    201: 'CREATED',
+    202: 'ACCEPTED',
+    203: 'NON-AUTHORITATIVE INFORMATION',
+    204: 'NO CONTENT',
+    205: 'RESET CONTENT',
+    206: 'PARTIAL CONTENT',
+    400: 'BAD REQUEST',
+    401: 'UNAUTHORIZED',
+    402: 'PAYMENT REQUIRED',
+    403: 'FORBIDDEN',
+    404: 'NOT FOUND',
+    405: 'METHOD NOT ALLOWED',
+    406: 'NOT ACCEPTABLE',
+    407: 'PROXY AUTHENTICATION REQUIRED',
+    408: 'REQUEST TIMEOUT',
+    409: 'CONFLIT',
+    410: 'GONE',
+    500: 'INTERNAL SERVER ERROR',
+    501: 'NOT IMPLEMENTED',
+    502: 'BAD GATEWAY',
+    503: 'SERVICE UNAVAILABLE',
+    504: 'GATEWAY TIMEOUT',
+    505: 'HTTP VERSION NOT SUPORTED'
+}
+
+
+class JSONEncoder(json.JSONEncoder):
+    def default(self, o: Any) -> Any:
+        if hasattr(o, "dict"):
+            return self.default(o.dict())
+        if isinstance(o, datetime.date):
+            return o.strftime('%Y-%m-%d')
+        if isinstance(o, datetime.datetime):
+            return o.isoformat()
+        if isinstance(o, decimal.Decimal):
+            return float(o)
+        return o
+
+
+class Response:
+    def __init__(
+            self,
+            data: Any = None,
+            *,
+            status: int = 200,
+            content_type: str = '',
+            headers: dict = None
+    ):
+        self.version = 'HTTP/1.1'
+        self.status = status
+        self.data = data if status != 204 else None
         self.headers = {}
-        self.files = {}
-        self.origin = ''
-        self.request_method = ''
-        self.request_headers = ''
-        self.preflight = False
-        self.multipart = False
-        self.boundary = ''
-        self.data = {}
-
-    def add_header(self, key, value):
-        self.headers[key] = value
-        if key == 'Content-Type':
-            if 'multipart/form-data' in value:
-                self.multipart = True
-                (content, boundary) = value.split(';')
-                self.type = content.strip()
-                self.boundary = boundary.replace('boundary=', '').strip()
-            else:
-                self.type = value
-        elif key == 'Content-Length':
-            self.length = int(value)
-        elif key == 'Origin':
-            self.origin = value
-            self.preflight = True if self.method == 'OPTIONS' else False
-        elif key == 'Access-Control-Request-Method':
-            self.request_method = value
-        elif key == 'Access-Control-Request-Headers':
-            self.request_headers = value
-
-    def dict(self):
-        if self.body:
-            if self.type == 'application/json':
-                return json.loads(self.body)
-            elif self.type == 'multipart/form-data':
-                return self._process_form_data()
-            elif self.type == 'application/x-www-form-urlencoded':
-                return self._url_decoded_data()
-        return {}
-
-    def args(self):
-        args = {}
-        if self.query:
-            pairs = self.query.split('&')
-            for pair in pairs:
-                (key, value) = pair.split('=')
-                args[key] = value
-        return args
-
-    def prepare_url(self, url):
-        if '?' in url:
-            (path, query) = url.split('?')
-        else:
-            path = url
-            query = ''
-        self.url = path
-        self.query = query
-
-    def prepare_data(self):
-        self.data = self.dict()
-
-    def _process_form_data(self):
-        data = {}
-        parts = self.body.split(f'--{self.boundary}'.encode())
-        for part in parts:
-            if not part or part == b'--\r\n':
-                continue
-            if b'filename=' in part:
-                splt = part.split(b';', maxsplit=2)
-                key = splt[1].decode().strip()[6:-1]
-                (info, content) = splt[2].split(b'\r\n\r\n', maxsplit=1)
-                (filename, kind) = info.decode().split('\r\n')
-                filename = filename.strip()[10:-1]
-                kind = kind.strip()[14:]
-                file = File(name=filename, kind=kind, content=content)
-                self.files[key] = file
-            else:
-                splt = part.split(b';')
-                key, value = splt[1].split(b'\r\n\r\n')
-                key = key.decode().replace('name=', '').strip()[1:-1]
-                data[key] = value.strip().decode()
-        return data
-
-    def _url_decoded_data(self):
-        data = {}
-        pairs = self.body.decode().split('&')
-        for pair in pairs:
-            (key, value) = pair.split('=')
-            data[key] = value
-        return data
+        self.content_type = content_type
+        self._prepare_headers(headers)
+        self.content = b''
+        self.text = ''
+
+    def render(self):
+        title = status_title.get(self.status, 'STATUS WITHOUT TITLE')
+        headers = '\r\n'.join([f"{k}:{v}" for k, v in self.headers.items()])
+        body = self.data
+        content = f'{self.version} {self.status} {title}\r\n{headers}\r\n\r\n'
+        if body:
+            content = f'{content}{body}'
+            self.content = body.encode()
+        return content
+
+    def parser(self, model: Any = None):
+        res = json.loads(self.data)
+        if model:
+            res = model(**res)
+        return res
+
+    def _prepare_headers(self, headers):
+        if not headers:
+            headers = {}
+        if self.data is None:
+            self.data = ''
+        if self.content_type:
+            self.headers['Content-Type'] = self.content_type
+        if isinstance(self.data, dict) or isinstance(self.data, list):
+            self.data = json.dumps(self.data, cls=JSONEncoder)
+            self.headers['Content-Type'] = 'application/json'
+        elif isinstance(self.data, bytes):
+            self._identify_binary_data()
+        elif isinstance(self.data, str):
+            self.headers['Content-Type'] = 'text/plain'
+        self.headers['Content-Length'] = len(self.data)
+        self.headers.update(headers)
+
+    def _identify_binary_data(self):
+        if self.data[1:4] == 'PDF':
+            self.headers['Content-Type'] = 'application/pdf'
```

### Comparing `restfy-0.3.2/restfy/router.py` & `restfy-0.4.0/restfy/router.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,83 @@
-import inspect
-from restfy.http import Request
-
-
-class Handler:
-    def __init__(self, func):
-        self.func = func
-        args = inspect.getfullargspec(func).annotations
-        if 'return' in args:
-            self.return_type = args.pop('return')
-        self.parameters = args
-
-    async def execute(self, properties):
-        args = {}
-        for key, kind in self.parameters.items():
-            value = properties.get(key)
-            if not value:
-                raise Exception(f'Parameter {key}')
-            if kind in [int, float, bool]:
-                try:
-                    value = kind(value)
-                except Exception as e:
-                    raise Exception(f'Error try cast value "{value}" {key} {kind}: {e}')
-            args[key] = value
-        ret = await self.func(**args)
-        return ret
+from restfy.request import Request
+from restfy.handler import Handler
 
 
 class Route:
-    def __init__(self, name='', node='', path=None, handle=None, method='', prepare_data=True):
+    def __init__(self, name='', node='', path=None, handle=None, method='', prepare_data=True, websocket=False):
         self.properties = {}
         self.handlers = {}
         self.routes = {}
         self.variable = None
         self.is_variable = False
         self.variable_type = str
         self.name = name
         self.prepare_data: bool = prepare_data
+        self.is_websocket = websocket
+
+    def __repr__(self):
+        return f'{self.__class__}: {self.name}'
 
-    def add_node(self, path, handle, method='GET'):
+    def add_node(self, path, handle, method='GET', websocket=False):
         node = path.pop(0)
+        if websocket:
+            method = 'GET'
         if node.startswith('{'):
             if self.variable:
                 route = self.variable
             else:
-                route = Route()
+                route = Route(websocket=websocket)
                 route.is_variable = True
                 route.name = node[1:-1]
                 self.variable = route
         else:
-            route = self.routes.get(node, Route())
+            route = self.routes.get(node, Route(websocket=websocket))
             route.name = node
             self.routes[node] = route
         if path:
-            route.add_node(path=path, handle=handle, method=method)
+            route.add_node(path=path, handle=handle, method=method, websocket=websocket)
         else:
-            route.add_handler(Handler(handle), method)
+            route.add_handler(handle, method)
 
-    def add_handler(self, handle, method):
-        self.handlers[method] = handle
+    def add_handler(self, func, method: str):
+        handler = Handler(func)
+        self.handlers[method] = handler
 
     async def exec(self, request: Request):
         handler = self.handlers[request.method]
         if self.prepare_data and request.app.prepare_request_data:
             request.prepare_data()
-        properties = {'request': request, **self.properties}
-        return await handler.execute(properties)
+        for key, value in self.properties.items():
+            request.path_args[key] = value
+        return await handler.execute(self.properties, request)
 
 
 class Router(Route):
     def __init__(self, base_url=''):
         super().__init__()
         self.base_url = base_url
 
-    def add_route(self, path, handle, method='GET'):
+    def add_route(
+            self,
+            path: str,
+            handle: callable,
+            *,
+            method: str = 'GET',
+            websocket: bool = False
+    ):
         path = path[1:].split('/')
         if len(path) == 1 and path[0] == '':
-            self.add_handler(Handler(handle), method)
+            self.add_handler(handle, method)
         else:
-            self.add_node(path=path, handle=handle, method=method)
+            self.add_node(path=path, handle=handle, method=method, websocket=websocket)
 
     def register_router(self, path, router):
         nodes = path[1:].split('/')
         if len(nodes) == 1 and nodes[0] == '':
+            self.handlers = router.handlers
             self.routes = router.routes
             self.variable = router.variable
             self.is_variable = router.is_variable
         else:
             routes = self.routes
             while True:
                 node = nodes.pop(0)
@@ -104,29 +96,31 @@
 
     def match(self, url, method):
         nodes = url[1:].split('/')
         if len(nodes) == 1 and nodes[0] == '':
             return self
         routes = self.routes
         variable = self.variable
-        properties = {}
+        args = {}
+        route = None
         while len(nodes) > 0:
             node = nodes.pop(0)
             route = routes.get(node, None)
             if not route:
                 if variable:
                     route = variable
-                    properties[route.name] = node
+                    args[route.name] = node
                 else:
                     break
-            routes = route.routes
-            variable = route.variable
+            else:
+                routes = route.routes
+                variable = route.variable
         if route:
             if method in route.handlers:
-                route.properties = properties
+                route.properties = args
             else:
                 route = None
         return route
 
     def get(self, path):
         def wrapper(func):
             self.add_route(path, handle=func)
@@ -164,7 +158,13 @@
         return wrapper
 
     def head(self, path):
         def wrapper(func):
             self.add_route(path, handle=func, method='HEAD')
             return func
         return wrapper
+
+    def websocket(self, path):
+        def wrapper(func):
+            self.add_route(path, handle=func, method='GET', websocket=True)
+            return func
+        return wrapper
```

### Comparing `restfy-0.3.2/PKG-INFO` & `restfy-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: restfy
-Version: 0.3.2
+Version: 0.4.0
 Summary: A small rest framework
 Home-page: https://github.com/manasseslima/restfy
 License: MIT
 Author: Manasses Lima
 Author-email: manasseslima@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bike (>=0.3.1,<0.4.0)
+Requires-Dist: httplus (>=0.1.0,<0.2.0)
 Project-URL: Repository, https://github.com/manasseslima/restfy
 Description-Content-Type: text/markdown
 
 # restfy
 A small rest framework.
 
 [![Stable Version](https://img.shields.io/pypi/v/restfy?label=pypi)](https://pypi.org/project/restfy/)
@@ -169,9 +171,38 @@
 
 
 app = Application()
 app.register_middleware(DefaultMiddleware)
 
 ```
 
-
-
+### HTTP client requests
+With http module, you can realize asynchronous requests to other services.
+The most simple request can be seen below.
+```python
+from restfy import http
+...
+res = await http.get('https://someserver.api/endpoint')
+print(res.status)
+# 200
+```
+In addition to the get function, others functions are available like 
+post(), put(), delete() and patch(). 
+If other request method are necessary, we can use request() function passing method param.
+The next example shows a more complex example.
+```python
+from restfy import http
+
+...
+url = 'https://someserver.api/endpoint'
+data = {
+    'name': 'Nick',
+    'surname': 'Lauda'
+}
+headers = {
+    'Content-Type': 'application/json'
+}
+...
+res = await http.post(url=url, data=data, headers=headers)
+print(res.status)
+# 200
+```
```

