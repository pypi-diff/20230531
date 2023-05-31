# Comparing `tmp/starbear-0.0.2.tar.gz` & `tmp/starbear-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbear-0.0.2.tar", max compression
+gzip compressed data, was "starbear-0.0.3.tar", max compression
```

## Comparing `starbear-0.0.2.tar` & `starbear-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      786 2023-01-23 23:55:41.591024 starbear-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       95 2023-01-22 18:07:37.078561 starbear-0.0.2/starbear/__init__.py
--rw-r--r--   0        0        0     5039 2023-01-23 07:22:15.140808 starbear-0.0.2/starbear/base-lib.js
--rw-r--r--   0        0        0      552 2023-01-22 20:51:07.514209 starbear-0.0.2/starbear/base-template.html
--rw-r--r--   0        0        0     4709 2023-01-20 21:19:49.660082 starbear-0.0.2/starbear/page.py
--rw-r--r--   0        0        0     6759 2023-01-22 18:36:53.392128 starbear-0.0.2/starbear/repr.py
--rw-r--r--   0        0        0     8976 2023-01-22 18:16:09.046473 starbear-0.0.2/starbear/serve.py
--rw-r--r--   0        0        0     2525 2023-01-23 07:23:44.113526 starbear-0.0.2/starbear/utils.py
--rw-r--r--   0        0        0       18 2023-01-23 23:55:41.623915 starbear-0.0.2/starbear/version.py
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 starbear-0.0.2/setup.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 starbear-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      786 2023-05-31 17:00:55.345292 starbear-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-01-22 18:07:37.078561 starbear-0.0.3/starbear/__init__.py
+-rw-r--r--   0        0        0     4988 2023-05-31 16:06:31.359436 starbear-0.0.3/starbear/base-lib.js
+-rw-r--r--   0        0        0      552 2023-01-22 20:51:07.514209 starbear-0.0.3/starbear/base-template.html
+-rw-r--r--   0        0        0     5075 2023-05-31 17:00:43.309664 starbear-0.0.3/starbear/page.py
+-rw-r--r--   0        0        0     6759 2023-01-22 18:36:53.392128 starbear-0.0.3/starbear/repr.py
+-rw-r--r--   0        0        0     9683 2023-05-31 17:00:43.309894 starbear-0.0.3/starbear/serve.py
+-rw-r--r--   0        0        0     2525 2023-01-23 07:23:44.113526 starbear-0.0.3/starbear/utils.py
+-rw-r--r--   0        0        0       18 2023-05-31 17:00:55.378845 starbear-0.0.3/starbear/version.py
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 starbear-0.0.3/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 starbear-0.0.3/PKG-INFO
```

### Comparing `starbear-0.0.2/pyproject.toml` & `starbear-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starbear"
-version = "0.0.2"
+version = "0.0.3"
 description = "Framework for easy small local web apps or programs"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 uvicorn = "^0.17.6"
```

### Comparing `starbear-0.0.2/starbear/base-lib.js` & `starbear-0.0.3/starbear/base-lib.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -53,23 +53,25 @@
             },
             body: JSON.stringify(args),
         })
     }
 }
 
 
-async function $$BEAR_CB(selector, method, args, promise, return_result) {
-    let object = window;
+async function $$BEAR_CB(selector, extractor, promise) {
+    let root = window;
+
     if (selector) {
         const element = document.querySelector(selector);
-        object = (await (element.__object));
+        root = (await (element.__object));
     }
+
     try {
-        let result = await object[method](...args);
-        await promise.resolve(return_result ? result : null);
+        let result = await extractor(root);
+        await promise.resolve(result);
     } catch (exc) {
         await promise.reject(exc);
         throw exc;
     }
 }
```

### Comparing `starbear-0.0.2/starbear/base-template.html` & `starbear-0.0.3/starbear/base-template.html`

 * *Files identical despite different names*

### Comparing `starbear-0.0.2/starbear/page.py` & `starbear-0.0.3/starbear/page.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 class Page:
     def __init__(
         self,
         iq,
         oq,
         representer,
         selector=None,
+        query_params={},
         track_history=True,
         sent_resources=None,
     ):
         self.iq = iq
         self.oq = oq
         self.selector = selector
+        self.query_params = query_params
         self.representer = representer
         self.track_history = track_history
         self.sent_resources = sent_resources or ResourceDeduplicator()
         self.tasks = set()
-        self.do = Caller(self, return_result=False)
-        self.call = Caller(self, return_result=True)
+        self.js = JavaScriptOperation(self, [])
 
     def __getitem__(self, selector):
         if isinstance(selector, Tag):
             tid = selector.attributes.get("id", None)
             if not tid:
                 raise Exception("Cannot locate element because it has no id.")
             selector = f"#{tid}"
@@ -118,31 +119,46 @@
     def delete(self):
         self._push(self.put(H.span(), "outerHTML"))
 
     async def recv(self):
         return await self.iq.get()
 
 
-class Caller:
-    def __init__(self, element, return_result):
+call_template = "$$BEAR_CB({selector}, {extractor}, {future});"
+
+
+def _extractor(sequence):
+    result = "x"
+    for entry in sequence:
+        if isinstance(entry, str):
+            result = f"{result}.{entry}"
+        elif isinstance(entry, (list, tuple)):
+            args = ",".join([str(Resource(x)) for x in entry])
+            result = f"{result}({args})"
+        else:
+            raise TypeError()
+    return f"(x => {result})"
+
+
+class JavaScriptOperation:
+    def __init__(self, element, sequence):
         self.__element = element
-        self.__selector = element.selector
-        self.__return_result = return_result
+        self.__sequence = sequence
+        self.__future = aio.Future()
 
     def __getattr__(self, attr):
-        def call(*args):
-            call_template = "$$BEAR_CB('{selector}', '{method}', {args}, {future}, {return_result});"
-            future = aio.Future()
-            self.__element.page_select("body").without_history().print(
-                H.script(
-                    call_template.format(
-                        method=attr,
-                        selector=self.__selector,
-                        future=Resource(future),
-                        args=Resource(args),
-                        return_result=int(self.__return_result),
-                    )
-                ),
-            )
-            return future
+        return type(self)(self.__element, [*self.__sequence, attr])
 
-        return call
+    def __call__(self, *args):
+        return type(self)(self.__element, [*self.__sequence, args])
+
+    def __await__(self):
+        self.__element.page_select("body").without_history().print(
+            H.script(
+                call_template.format(
+                    selector=Resource(self.__element.selector),
+                    extractor=_extractor(self.__sequence),
+                    future=Resource(self.__future),
+                )
+            ),
+        )
+        return iter(self.__future)
```

### Comparing `starbear-0.0.2/starbear/repr.py` & `starbear-0.0.3/starbear/repr.py`

 * *Files identical despite different names*

### Comparing `starbear-0.0.2/starbear/serve.py` & `starbear-0.0.3/starbear/serve.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,28 +47,31 @@
         self._queue.appendleft(entry)
         self._unfinished_tasks += 1
         self._finished.clear()
         self._wakeup_next(self._getters)
 
 
 class Cub:
-    def __init__(self, mother, session):
+    def __init__(self, mother, session, query_params={}):
         self.mother = mother
         self.fn = mother.fn
         self.path = mother.path
         self.session = session
+        self.query_params = query_params
         self.route = f"{self.path}/{self.session}"
         self.methods = {}
         self.representer = Representer(self.route)
         self.iq = aio.Queue()
         self.oq = Queue2()
         self.history = []
         self.reset = False
         self.ws = None
-        self.page = Page(self.iq, self.oq, representer=self.representer)
+        self.page = Page(
+            self.iq, self.oq, representer=self.representer, query_params=query_params
+        )
         self.coro = aio.create_task(self.run())
         self._sd_coro = None
 
     def schedule_selfdestruct(self):
         async def sd():
             await aio.sleep(self.mother.session_timeout)
             del self.mother.cubs[self.session]
@@ -143,15 +146,18 @@
         self.ws = ws
 
         if self.reset:
             for entry in self.history:
                 await ws.send_text(entry)
             self.reset = False
 
-        await aio.wait([recv(), send()], return_when=aio.FIRST_COMPLETED)
+        await aio.wait(
+            [aio.create_task(recv()), aio.create_task(send())],
+            return_when=aio.FIRST_COMPLETED,
+        )
         self.schedule_selfdestruct()
 
     async def route_method(self, request):
         method_id = request.path_params["method"]
         method = self.representer.callback_registry.resolve(method_id)
         try:
             args = await self.json(request)
@@ -184,19 +190,26 @@
         self.representer.queue_registry.put(
             qid=data["reqid"],
             value=data["value"],
         )
         return JSONResponse({"status": "ok"})
 
 
+def get_session_from_request(request):
+    session_base = request.path_params.get("session", None)
+    if session_base is None:
+        session_base = base64.urlsafe_b64encode(uuid().bytes).decode("utf8").strip("=")
+    return session_base
+
+
 def forward_cub(fn):
     @wraps(fn)
     async def fwd(self, request):
-        session = request.path_params["session"]
-        cub = self._get(session)
+        session = get_session_from_request(request)
+        cub = self._get(session, query_params=request.query_params)
         if cub is None:
             print(f"Trying to access missing session: {session}")
             return JSONResponse({"missing": session}, status_code=404)
         else:
             return await fn(self, request, cub)
 
     return fwd
@@ -206,33 +219,40 @@
     def __init__(self, fn, path, session_timeout=60, hide_sessions=True):
         self.fn = fn
         self.path = path.rstrip("/")
         self.session_timeout = session_timeout
         self.hide_sessions = hide_sessions
         self.cubs = {}
 
-    def _get(self, sess, ensure=False):
+    def _get(self, sess, query_params={}, ensure=False):
         if sess not in self.cubs:
             if ensure:
                 print(f"Creating session: {sess}")
-                self.cubs[sess] = Cub(self, sess)
+                self.cubs[sess] = Cub(self, sess, query_params=query_params)
             else:
                 return None
         return self.cubs[sess]
 
     async def route_dispatch(self, request):
-        session = base64.urlsafe_b64encode(uuid().bytes).decode("utf8").strip("=")
+        session = get_session_from_request(request)
         if self.hide_sessions:
-            return await self._get(session, ensure=True).route_main(request)
+            return await self._get(
+                session, query_params=request.query_params, ensure=True
+            ).route_main(request)
         else:
-            return RedirectResponse(url=f"{self.path}/{session}")
+            url = f"{self.path}/{session}"
+            if request.query_params:
+                url = f"{url}?{request.query_params}"
+            return RedirectResponse(url=url)
 
     async def route_main(self, request):
-        session = request.path_params["session"]
-        return await self._get(session, ensure=True).route_main(request)
+        session = get_session_from_request(request)
+        return await self._get(
+            session, query_params=request.query_params, ensure=True
+        ).route_main(request)
 
     @forward_cub
     async def route_socket(self, ws, cub):
         return await cub.route_socket(ws)
 
     @forward_cub
     async def route_method(self, request, cub):
```

### Comparing `starbear-0.0.2/starbear/utils.py` & `starbear-0.0.3/starbear/utils.py`

 * *Files identical despite different names*

### Comparing `starbear-0.0.2/setup.py` & `starbear-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['hrepr>=0.5.0,<0.6.0',
  'starlette>=0.20.3,<0.21.0',
  'uvicorn>=0.17.6,<0.18.0',
  'websockets>=10.3,<11.0']
 
 setup_kwargs = {
     'name': 'starbear',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Framework for easy small local web apps or programs',
     'long_description': 'None',
     'author': 'Olivier Breuleux',
     'author_email': 'breuleux@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `starbear-0.0.2/PKG-INFO` & `starbear-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbear
-Version: 0.0.2
+Version: 0.0.3
 Summary: Framework for easy small local web apps or programs
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

