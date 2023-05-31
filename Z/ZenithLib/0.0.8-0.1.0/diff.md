# Comparing `tmp/zenithlib-0.0.8.tar.gz` & `tmp/zenithlib-0.1.0.tar.gz`

## Comparing `zenithlib-0.0.8.tar` & `zenithlib-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,19 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.0.8/.gitattributes
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 zenithlib-0.0.8/Zenith/Web.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 zenithlib-0.0.8/Zenith/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.0.8/Zenith/src/tests.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 zenithlib-0.0.8/examples/check_vers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.0.8/scripts/bupload.sh
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.0.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.0.8/LICENSE
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zenithlib-0.0.8/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 zenithlib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 zenithlib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.1.0/.gitattributes
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/Builder.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/Stylesheet.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/Web.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/ZenithLang.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/langAST.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/langParser.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/langTranspiler.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/__testing__/out.html
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/src/tests.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 zenithlib-0.1.0/examples/server.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.1.0/scripts/bupload.sh
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 zenithlib-0.1.0/README.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 zenithlib-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 zenithlib-0.1.0/PKG-INFO
```

### Comparing `zenithlib-0.0.8/Zenith/Web.py` & `zenithlib-0.1.0/Zenith/Web.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 import datetime
 from http.server import BaseHTTPRequestHandler, HTTPServer
-import time
 
-class Server(BaseHTTPRequestHandler):
+class CustomServer(BaseHTTPRequestHandler):
     HEADER_VALUE = "text/html"
     HEADER_TYPE = "Content-type"
-    
+    BUILT_ROUTES = {}
+
     def do_GET(self):
         self.send_response(200)
         self.send_header(self.HEADER_TYPE, self.HEADER_VALUE)
         self.end_headers()
-        self.wfile.write(bytes("<h1>Zenith Server</h1>", "utf-8"))
-        
-class WApp(Server):
-    def __init__(self) -> None:
+
+        path = self.path[1:]  # Remove the leading '/' from the path
+        if path in self.BUILT_ROUTES:
+            response = self.BUILT_ROUTES[path]
+            self.wfile.write(response.encode('utf-8'))
+        else:
+            self.send_response(404)
+            self.wfile.write(b"<h1>404 Not Found</h1>")
+
+class WApp:
+    def __init__(self):
         self.port = 3000
         self.host = 'localhost'
         self.devServer = False
         self.static_url_path = "static"
         self.name = "Zenith App"
         self.logging = True
-    
-    class set:
-        def headers(TYPE, VALUE):
-            Server.do_GET()
-            
+        self.webServer = HTTPServer((self.host, self.port), CustomServer)
+
+    @staticmethod
+    def register_route(route, response):
+        CustomServer.BUILT_ROUTES[route] = response
+
     def serve(self):
         current_time = datetime.datetime.now()
         time_stamp = current_time.timestamp()
-
-        webServer = HTTPServer((self.host, self.port), Server)
         print(f"Starting server at http://{self.host}:{self.port}")
         if self.devServer:
             print(f"\t• Running as development server")
         print(f"\t• Started {datetime.datetime.fromtimestamp(time_stamp)}\n")
         try:
-            webServer.serve_forever()
-        except  KeyboardInterrupt:
+            self.webServer.serve_forever()
+        except KeyboardInterrupt:
             pass
-        webServer.server_close()
+        self.webServer.server_close()
         print("Server stopped.")
 
+
```

### Comparing `zenithlib-0.0.8/.gitignore` & `zenithlib-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.8/LICENSE` & `zenithlib-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.8/pyproject.toml` & `zenithlib-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ZenithLib"
-version = "0.0.08"
+version = "0.1.0"
 authors = [
   { name="Ryan Rudd", email="rsrudd@gmail.com" },
 ]
 description = "Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

